# Comparing `tmp/aeppl-nightly-0.1.3.dev20230503.tar.gz` & `tmp/aeppl-nightly-0.1.3.dev20230504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl-nightly-0.1.3.dev20230503.tar", last modified: Wed May  3 00:30:08 2023, max compression
+gzip compressed data, was "aeppl-nightly-0.1.3.dev20230504.tar", last modified: Thu May  4 00:29:58 2023, max compression
```

## Comparing `aeppl-nightly-0.1.3.dev20230503.tar` & `aeppl-nightly-0.1.3.dev20230504.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:30:08.651263 aeppl-nightly-0.1.3.dev20230503/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 00:30:08.651263 aeppl-nightly-0.1.3.dev20230503/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:30:08.651263 aeppl-nightly-0.1.3.dev20230503/aeppl/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 00:30:08.651263 aeppl-nightly-0.1.3.dev20230503/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:30:08.647263 aeppl-nightly-0.1.3.dev20230503/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 00:30:08.000000 aeppl-nightly-0.1.3.dev20230503/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-03 00:30:08.000000 aeppl-nightly-0.1.3.dev20230503/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:30:08.000000 aeppl-nightly-0.1.3.dev20230503/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:30:08.000000 aeppl-nightly-0.1.3.dev20230503/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 00:30:08.000000 aeppl-nightly-0.1.3.dev20230503/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 00:30:08.000000 aeppl-nightly-0.1.3.dev20230503/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-03 00:30:08.651263 aeppl-nightly-0.1.3.dev20230503/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:30:08.651263 aeppl-nightly-0.1.3.dev20230503/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-03 00:29:55.000000 aeppl-nightly-0.1.3.dev20230503/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:29:58.134491 aeppl-nightly-0.1.3.dev20230504/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 00:29:58.134491 aeppl-nightly-0.1.3.dev20230504/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:29:58.134491 aeppl-nightly-0.1.3.dev20230504/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 00:29:58.134491 aeppl-nightly-0.1.3.dev20230504/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:29:58.130490 aeppl-nightly-0.1.3.dev20230504/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 00:29:58.000000 aeppl-nightly-0.1.3.dev20230504/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-04 00:29:58.000000 aeppl-nightly-0.1.3.dev20230504/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:29:58.000000 aeppl-nightly-0.1.3.dev20230504/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:29:57.000000 aeppl-nightly-0.1.3.dev20230504/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 00:29:58.000000 aeppl-nightly-0.1.3.dev20230504/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 00:29:58.000000 aeppl-nightly-0.1.3.dev20230504/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 00:29:58.134491 aeppl-nightly-0.1.3.dev20230504/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:29:58.134491 aeppl-nightly-0.1.3.dev20230504/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-04 00:29:46.000000 aeppl-nightly-0.1.3.dev20230504/versioneer.py
```

### Comparing `aeppl-nightly-0.1.3.dev20230503/LICENSE` & `aeppl-nightly-0.1.3.dev20230504/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/PKG-INFO` & `aeppl-nightly-0.1.3.dev20230504/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.3.dev20230503
+Version: 0.1.3.dev20230504
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.3.dev20230503/README.md` & `aeppl-nightly-0.1.3.dev20230504/README.md`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/abstract.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/censoring.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/convolutions.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/convolutions.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,56 +3,52 @@
 from aesara.tensor.random.basic import NormalRV, normal
 
 from aeppl.rewriting import measurable_ir_rewrites_db
 
 
 @node_rewriter((at.sub, at.add))
 def add_independent_normals(fgraph, node):
-    """Replace a sum of two un-valued independent normal RVs with a single normal RV."""
+    """Replace a sum of un-valued independent normal RVs with a single normal RV."""
+
+    if len(node.inputs) < 2:
+        return None
 
     if node.op == at.add:
         sub = False
     else:
         sub = True
 
-    X_rv, Y_rv = node.inputs
-
-    if not (X_rv.owner and Y_rv.owner) or not (
-        # This also checks that the RVs are un-valued (i.e. they're not
-        # `ValuedVariable`s)
-        isinstance(X_rv.owner.op, NormalRV)
-        and isinstance(Y_rv.owner.op, NormalRV)
-    ):
+    # This also implicitly checks that the RVs are un-valued (i.e. they're not
+    # `ValuedVariable`s)
+    if not all(inp.owner and isinstance(inp.owner.op, NormalRV) for inp in node.inputs):
         return None
 
-    old_rv = node.outputs[0]
-
-    mu_x, sigma_x, mu_y, sigma_y, _ = at.broadcast_arrays(
-        *(X_rv.owner.inputs[-2:] + Y_rv.owner.inputs[-2:] + [old_rv])
+    new_size = at.broadcast_shape(
+        *(tuple(inp.owner.inputs[1]) for inp in node.inputs), arrays_are_shapes=True
     )
 
-    new_rng = X_rv.owner.inputs[0].clone()
+    means = [inp.owner.inputs[-2] for inp in node.inputs]
+    covs = [inp.owner.inputs[-1] ** 2 for inp in node.inputs]
+
+    new_rng = node.inputs[0].owner.inputs[0].clone()
 
     new_node = normal.make_node(
         new_rng,
-        old_rv.shape,
-        old_rv.dtype,
-        mu_x + mu_y if not sub else mu_x - mu_y,
-        at.sqrt(sigma_x**2 + sigma_y**2),
+        new_size,
+        node.outputs[0].dtype,
+        at.add(*means) if not sub else at.sub(*means),
+        at.sqrt(at.add(*covs)),
     )
 
     fgraph.add_input(new_rng)
 
     # new_rng must be updated with values of the RNGs output by `new_node
     new_rng.default_update = new_node.outputs[0]
     new_normal_rv = new_node.default_output()
 
-    if old_rv.name:
-        new_normal_rv.name = old_rv.name
-
     return [new_normal_rv]
 
 
 measurable_ir_rewrites_db.register(
     "add_independent_normals",
     add_independent_normals,
     "basic",
```

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/cumsum.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/dists.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/joint_logprob.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/logprob.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/mixture.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/printing.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/rewriting.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/scan.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/tensor.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/transforms.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl/utils.py` & `aeppl-nightly-0.1.3.dev20230504/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl_nightly.egg-info/PKG-INFO` & `aeppl-nightly-0.1.3.dev20230504/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.3.dev20230503
+Version: 0.1.3.dev20230504
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.3.dev20230503/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl-nightly-0.1.3.dev20230504/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/setup.cfg` & `aeppl-nightly-0.1.3.dev20230504/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/setup.py` & `aeppl-nightly-0.1.3.dev20230504/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_abstract.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_censoring.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_composite_logprob.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_composite_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_convolutions.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_convolutions.py`

 * *Files 18% similar despite different names*

```diff
@@ -91,15 +91,14 @@
 
     new_rv_mu = np.broadcast_to(new_rv_mu, new_rv_shape)
     new_rv_sigma = np.broadcast_to(new_rv_sigma, new_rv_shape)
 
     assert isinstance(new_rv.owner.op, NormalRV)
     assert np.allclose(new_rv.owner.inputs[3].eval(), new_rv_mu)
     assert np.allclose(new_rv.owner.inputs[4].eval(), new_rv_sigma)
-    assert new_rv.name == "Z"
 
 
 def test_normal_add_input_valued():
     """Test the case when one of the normal inputs to the add `Op` is a `ValuedVariable`."""
     srng = at.random.RandomStream(0)
 
     X_rv = srng.normal(1.0, name="X")
@@ -113,7 +112,32 @@
 
     valued_var_out_node = fgraph.outputs[0].owner
     # We should not expect the convolution to be applied; instead, the
     # transform should be (for now)
     assert isinstance(
         valued_var_out_node.inputs[0].owner.op, MeasurableElemwiseTransform
     )
+
+
+def test_normal_add_three_inputs():
+    """Test the case when there are more than two inputs in the sum."""
+    srng = at.random.RandomStream(0)
+
+    mu_x = at.vector("mu_x")
+    sigma_x = at.vector("sigma_x")
+    X_rv = srng.normal(mu_x, sigma_x, name="X")
+    mu_y = at.vector("mu_y")
+    sigma_y = at.vector("sigma_y")
+    Y_rv = srng.normal(mu_y, sigma_y, size=(2, 1), name="Y")
+    mu_w = at.vector("mu_w")
+    sigma_w = at.vector("sigma_w")
+    W_rv = srng.normal(mu_w, sigma_w, name="W")
+
+    Z_rv = X_rv + Y_rv + W_rv
+    Z_rv.name = "Z"
+    z_vv = Z_rv.clone()
+
+    fgraph, _, _ = construct_ir_fgraph({Z_rv: z_vv})
+
+    valued_var_out_node = fgraph.outputs[0].owner
+    # The convolution should be applied, and not the transform
+    assert isinstance(valued_var_out_node.inputs[0].owner.op, NormalRV)
```

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_cumsum.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_dist.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_joint_logprob.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_logprob.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_mixture.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_printing.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_rewriting.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_scan.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_tensor.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_transforms.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/tests/test_utils.py` & `aeppl-nightly-0.1.3.dev20230504/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230503/versioneer.py` & `aeppl-nightly-0.1.3.dev20230504/versioneer.py`

 * *Files identical despite different names*

