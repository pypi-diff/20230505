# Comparing `tmp/neptune_pytorch-0.1.0.tar.gz` & `tmp/neptune_pytorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_pytorch-0.1.0.tar", max compression
+gzip compressed data, was "neptune_pytorch-0.2.0.tar", max compression
```

## Comparing `neptune_pytorch-0.1.0.tar` & `neptune_pytorch-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      158 2023-05-04 09:22:15.879660 neptune_pytorch-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-03-15 07:40:40.000000 neptune_pytorch-0.1.0/LICENSE
--rw-r--r--   0        0        0      132 2023-05-04 09:22:15.883660 neptune_pytorch-0.1.0/README.md
--rw-r--r--   0        0        0     2565 2023-05-04 09:28:49.777204 neptune_pytorch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      724 2023-03-15 07:45:26.000000 neptune_pytorch-0.1.0/src/neptune_pytorch/__init__.py
--rw-r--r--   0        0        0     7826 2023-05-04 09:22:15.883660 neptune_pytorch-0.1.0/src/neptune_pytorch/impl/__init__.py
--rw-r--r--   0        0        0      738 2023-03-15 07:48:21.000000 neptune_pytorch-0.1.0/src/neptune_pytorch/impl/version.py
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 neptune_pytorch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      580 2023-05-05 19:12:40.043735 neptune_pytorch-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-05-05 19:12:40.043735 neptune_pytorch-0.2.0/LICENSE
+-rw-r--r--   0        0        0      132 2023-05-05 19:12:40.043735 neptune_pytorch-0.2.0/README.md
+-rw-r--r--   0        0        0     2565 2023-05-05 19:12:55.616240 neptune_pytorch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      724 2023-05-05 19:12:40.043735 neptune_pytorch-0.2.0/src/neptune_pytorch/__init__.py
+-rw-r--r--   0        0        0     8984 2023-05-05 19:12:40.043735 neptune_pytorch-0.2.0/src/neptune_pytorch/impl/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-05 19:12:40.043735 neptune_pytorch-0.2.0/src/neptune_pytorch/impl/version.py
+-rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 neptune_pytorch-0.2.0/PKG-INFO
```

### Comparing `neptune_pytorch-0.1.0/LICENSE` & `neptune_pytorch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_pytorch-0.1.0/pyproject.toml` & `neptune_pytorch-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 repository = "https://github.com/neptune-ai/neptune-pytorch"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations-and-supported-tools/model-training/pytorch"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-pytorch"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_pytorch-0.1.0/src/neptune_pytorch/__init__.py` & `neptune_pytorch-0.2.0/src/neptune_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_pytorch-0.1.0/src/neptune_pytorch/impl/__init__.py` & `neptune_pytorch-0.2.0/src/neptune_pytorch/impl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["__version__", "NeptuneLogger"]
 
 import os
+import uuid
 import warnings
 import weakref
 from typing import (
     Optional,
     Union,
 )
 
@@ -38,14 +39,15 @@
     from neptune.new.handler import Handler
     from neptune.new.integrations.utils import verify_type
     from neptune.new.types import File
 
 IS_TORCHVIZ_AVAILABLE = True
 try:
     import torchviz
+    from graphviz import ExecutableNotFound
 except ImportError:
     IS_TORCHVIZ_AVAILABLE = False
 
 INTEGRATION_VERSION_KEY = "source_code/integrations/neptune-pytorch"
 
 
 class NeptuneLogger:
@@ -148,18 +150,26 @@
             msg = "Skipping model visualization because no torchviz installation was found."
             warnings.warn(msg)
             return
 
         def hook(module, input, output):
             if not self._is_viz_saved:
                 dot = torchviz.make_dot(output, params=dict(module.named_parameters()))
-                # Use tempfile correctly.
                 dot.format = "png"
-                dot.render(outfile="torch-viz.png")
-                self._namespace_handler["model"]["visualization"].upload("torch-viz.png")
+                # generate unique name so that multiple concurrent runs
+                # don't over-write each other.
+                viz_name = str(uuid.uuid4()) + ".png"
+                try:
+                    dot.render(outfile=viz_name)
+                    safe_upload_visualization(self._namespace_handler["model"], "visualization", viz_name)
+                except ExecutableNotFound:
+                    # This errors because `dot` renderer is not found even
+                    # if python binding of `graphviz` are available.
+                    warnings.warn("Skipping model visualization because no dot (graphviz) installation was found.")
+
                 self._is_viz_saved = True
 
         self._vis_hook_handler = self.model.register_forward_hook(hook)
 
     def add_hooks_for_params(self):
         def hook(module, inp, output):
             self._params_iter_tracker += 1
@@ -177,41 +187,57 @@
         if model_name is None:
             # Default model name
             model_name = "model.pt"
         else:
             # User is not expected to add extension
             model_name = model_name + ".pt"
 
-        safe_upload(self._namespace_handler["model"], model_name, self.model)
+        safe_upload_model(self._namespace_handler["model"], model_name, self.model)
 
     def save_checkpoint(self, checkpoint_name: Optional[str] = None):
         if checkpoint_name is None:
             # Default checkpoint name
             checkpoint_name = f"checkpoint_{self.ckpt_number}.pt"
             self.ckpt_number += 1
         else:
             # User is not expected to add extension
             checkpoint_name = checkpoint_name + ".pt"
 
-        safe_upload(self._namespace_handler["model"], checkpoint_name, self.model)
+        safe_upload_model(self._namespace_handler["model"]["checkpoints"], checkpoint_name, self.model)
 
     def __del__(self):
         # Remove hooks
         if self._params_hook_handler is not None:
             self._params_hook_handler.remove()
 
         for name, handler in self._gradients_hook_handler.items():
             if handler is not None:
                 handler.remove()
 
         if self._vis_hook_handler is not None:
             self._vis_hook_handler.remove()
 
 
-def safe_upload(run, name, model):
+def safe_upload_visualization(run: Run, name: str, file_name: str):
+    # Function to safely upload a file and
+    # delete the file on completion of upload.
+    # We utilise the weakref.finalize to remove
+    # the file once the stream object goes out-of-scope.
+
+    def remove(file_name):
+        os.remove(file_name)
+        # Also remove graphviz intermediate file.
+        os.remove(file_name.replace(".png", ".gv"))
+
+    with open(file_name, "rb") as f:
+        weakref.finalize(f, remove, file_name)
+        run[name].upload(File.from_stream(f, extension="png"))
+
+
+def safe_upload_model(run: Run, name: str, model: torch.nn.Module):
     # Function to safely upload a file and
     # delete the file on completion of upload.
     # We utilise the weakref.finalize to remove
     # the file once the stream object goes out-of-scope.
 
     torch.save(model.state_dict(), name)
```

### Comparing `neptune_pytorch-0.1.0/src/neptune_pytorch/impl/version.py` & `neptune_pytorch-0.2.0/src/neptune_pytorch/impl/version.py`

 * *Files identical despite different names*

### Comparing `neptune_pytorch-0.1.0/PKG-INFO` & `neptune_pytorch-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-pytorch
-Version: 0.1.0
+Version: 0.2.0
 Summary: Neptune.ai pytorch integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
```

