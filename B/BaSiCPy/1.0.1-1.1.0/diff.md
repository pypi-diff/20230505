# Comparing `tmp/BaSiCPy-1.0.1.tar.gz` & `tmp/BaSiCPy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BaSiCPy-1.0.1.tar", last modified: Thu Dec  1 13:47:57 2022, max compression
+gzip compressed data, was "BaSiCPy-1.1.0.tar", last modified: Fri May  5 11:39:36 2023, max compression
```

## Comparing `BaSiCPy-1.0.1.tar` & `BaSiCPy-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 13:47:57.550941 BaSiCPy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2022-12-01 13:47:36.000000 BaSiCPy-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-12-01 13:47:36.000000 BaSiCPy-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11154 2022-12-01 13:47:57.550941 BaSiCPy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10003 2022-12-01 13:47:36.000000 BaSiCPy-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-01 13:47:36.000000 BaSiCPy-1.0.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1897 2022-12-01 13:47:57.550941 BaSiCPy-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 13:47:57.546941 BaSiCPy-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 13:47:57.546941 BaSiCPy-1.0.1/src/BaSiCPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11154 2022-12-01 13:47:57.000000 BaSiCPy-1.0.1/src/BaSiCPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      511 2022-12-01 13:47:57.000000 BaSiCPy-1.0.1/src/BaSiCPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 13:47:57.000000 BaSiCPy-1.0.1/src/BaSiCPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2022-12-01 13:47:57.000000 BaSiCPy-1.0.1/src/BaSiCPy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      389 2022-12-01 13:47:57.000000 BaSiCPy-1.0.1/src/BaSiCPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-12-01 13:47:57.000000 BaSiCPy-1.0.1/src/BaSiCPy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 13:47:57.550941 BaSiCPy-1.0.1/src/basicpy/
--rw-r--r--   0 runner    (1001) docker     (122)      402 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/src/basicpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3343 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/src/basicpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16365 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/src/basicpy/_jax_routines.py
--rw-r--r--   0 runner    (1001) docker     (122)    23420 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/src/basicpy/basicpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     4827 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/src/basicpy/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 13:47:57.550941 BaSiCPy-1.0.1/src/basicpy/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/src/basicpy/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1886 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/src/basicpy/tools/_jax_idct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2744 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/src/basicpy/tools/dct_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2022-12-01 13:47:38.000000 BaSiCPy-1.0.1/src/basicpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:36.835169 BaSiCPy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 11:39:20.000000 BaSiCPy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 11:39:20.000000 BaSiCPy-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-05-05 11:39:36.835169 BaSiCPy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-05-05 11:39:20.000000 BaSiCPy-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 11:39:20.000000 BaSiCPy-1.1.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-05 11:39:36.835169 BaSiCPy-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:36.831169 BaSiCPy-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:36.831169 BaSiCPy-1.1.0/src/BaSiCPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-05-05 11:39:36.000000 BaSiCPy-1.1.0/src/BaSiCPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-05 11:39:36.000000 BaSiCPy-1.1.0/src/BaSiCPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:39:36.000000 BaSiCPy-1.1.0/src/BaSiCPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 11:39:36.000000 BaSiCPy-1.1.0/src/BaSiCPy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-05 11:39:36.000000 BaSiCPy-1.1.0/src/BaSiCPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 11:39:36.000000 BaSiCPy-1.1.0/src/BaSiCPy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:36.831169 BaSiCPy-1.1.0/src/basicpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16365 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/_jax_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29557 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/basicpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:36.835169 BaSiCPy-1.1.0/src/basicpy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/tools/_jax_idct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/tools/dct_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/src/basicpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:36.835169 BaSiCPy-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/tests/test_jax_idct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-05 11:39:22.000000 BaSiCPy-1.1.0/tests/test_tools_dct2D.py
```

### Comparing `BaSiCPy-1.0.1/LICENSE` & `BaSiCPy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BaSiCPy-1.0.1/PKG-INFO` & `BaSiCPy-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BaSiCPy
-Version: 1.0.1
+Version: 1.1.0
 Summary: A python package for background and shading correction of optical microscopy images
 Home-page: https://github.com/peng-lab/BaSiCPy
 Author: Nicholas Schaub, Tim Morello, Tingying Peng, Yohsuke T. Fukai
 Author-email: nick.schaub@nih.gov, timothy.morello@downstate.edu, tingying.peng@helmholtz-muenchen.de, ysk@yfukai.net
 License: MIT
 Project-URL: Bug Tracker, https://github.com/peng-lab/BaSiCPy/issues
 Keywords: background shading flatfield darkfield biology optical microscopy image illumination
@@ -61,15 +61,15 @@
 ---
 ## Usage
 
 See [Read the Docs](https://basicpy.readthedocs.io/en/latest/) for the detailed usage.
 
 ## Installation
 
-### For Mac, Linux or WSL2 users
+### For Mac (Intel chip), Linux or WSL2 users
 
  Install from PyPI
 
 ```console
 pip install basicpy
 ```
 
@@ -77,20 +77,33 @@
 
 ```console
 git clone https://github.com/peng-lab/BaSiCPy.git
 cd BaSiCPy
 pip install .
 ```
 
-### For windows users
+### For Mac users with M1 chip
+
+BaSiCPy requires [`jax`](https://github.com/google/jax/),
+which has potential build issue with M1 chips.
+One easiest solution is using [Miniforge](https://github.com/conda-forge/miniforge)
+as explained [here](https://github.com/google/jax/issues/5501).
+In the Miniforge environment, please try the following:
+```bash
+pip install "jax[cpu]==0.3.22" jaxlib
+pip install basicpy
+```
+
+### For Windows users
 
 BaSiCPy requires [`jax`](https://github.com/google/jax/) which does not support Windows officially.
 However, thanks to [cloudhan/jax-windows-builder](https://github.com/cloudhan/jax-windows-builder), we can install BaSiCPy as follows:
-```
-pip install "jax[cpu]===0.3.14" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
+
+```bash
+pip install "jax[cpu]==0.3.14" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
 pip install basicpy
 ```
 For details and latest updates, see [this issue](https://github.com/google/jax/issues/438).
 
 ### Install with dev dependencies
 
 ```console
```

### Comparing `BaSiCPy-1.0.1/README.md` & `BaSiCPy-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ---
 ## Usage
 
 See [Read the Docs](https://basicpy.readthedocs.io/en/latest/) for the detailed usage.
 
 ## Installation
 
-### For Mac, Linux or WSL2 users
+### For Mac (Intel chip), Linux or WSL2 users
 
  Install from PyPI
 
 ```console
 pip install basicpy
 ```
 
@@ -51,20 +51,33 @@
 
 ```console
 git clone https://github.com/peng-lab/BaSiCPy.git
 cd BaSiCPy
 pip install .
 ```
 
-### For windows users
+### For Mac users with M1 chip
+
+BaSiCPy requires [`jax`](https://github.com/google/jax/),
+which has potential build issue with M1 chips.
+One easiest solution is using [Miniforge](https://github.com/conda-forge/miniforge)
+as explained [here](https://github.com/google/jax/issues/5501).
+In the Miniforge environment, please try the following:
+```bash
+pip install "jax[cpu]==0.3.22" jaxlib
+pip install basicpy
+```
+
+### For Windows users
 
 BaSiCPy requires [`jax`](https://github.com/google/jax/) which does not support Windows officially.
 However, thanks to [cloudhan/jax-windows-builder](https://github.com/cloudhan/jax-windows-builder), we can install BaSiCPy as follows:
-```
-pip install "jax[cpu]===0.3.14" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
+
+```bash
+pip install "jax[cpu]==0.3.14" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
 pip install basicpy
 ```
 For details and latest updates, see [this issue](https://github.com/google/jax/issues/438).
 
 ### Install with dev dependencies
 
 ```console
```

### Comparing `BaSiCPy-1.0.1/setup.cfg` & `BaSiCPy-1.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 keywords = background shading flatfield darkfield biology optical microscopy image illumination
 project_urls = 
 	Bug Tracker = https://github.com/peng-lab/BaSiCPy/issues
 
 [options]
 packages = find:
 install_requires = 
-	jax>=0.3.10,<=0.3.23
-	jaxlib>=0.3.10,<=0.3.23 # to import jaxlib.xla_extension.XlaRuntimeError
+	hyperactive>=4.4.0
+	jax>=0.3.10 #,<=0.3.23
+	jaxlib>=0.3.10 #,<=0.3.23 # to import jaxlib.xla_extension.XlaRuntimeError
 	numpy
 	pooch
 	pydantic>=1.9.1
 	scikit-image
 	scipy
 python_requires = >=3.7
 package_dir =
```

### Comparing `BaSiCPy-1.0.1/src/BaSiCPy.egg-info/PKG-INFO` & `BaSiCPy-1.1.0/src/BaSiCPy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BaSiCPy
-Version: 1.0.1
+Version: 1.1.0
 Summary: A python package for background and shading correction of optical microscopy images
 Home-page: https://github.com/peng-lab/BaSiCPy
 Author: Nicholas Schaub, Tim Morello, Tingying Peng, Yohsuke T. Fukai
 Author-email: nick.schaub@nih.gov, timothy.morello@downstate.edu, tingying.peng@helmholtz-muenchen.de, ysk@yfukai.net
 License: MIT
 Project-URL: Bug Tracker, https://github.com/peng-lab/BaSiCPy/issues
 Keywords: background shading flatfield darkfield biology optical microscopy image illumination
@@ -61,15 +61,15 @@
 ---
 ## Usage
 
 See [Read the Docs](https://basicpy.readthedocs.io/en/latest/) for the detailed usage.
 
 ## Installation
 
-### For Mac, Linux or WSL2 users
+### For Mac (Intel chip), Linux or WSL2 users
 
  Install from PyPI
 
 ```console
 pip install basicpy
 ```
 
@@ -77,20 +77,33 @@
 
 ```console
 git clone https://github.com/peng-lab/BaSiCPy.git
 cd BaSiCPy
 pip install .
 ```
 
-### For windows users
+### For Mac users with M1 chip
+
+BaSiCPy requires [`jax`](https://github.com/google/jax/),
+which has potential build issue with M1 chips.
+One easiest solution is using [Miniforge](https://github.com/conda-forge/miniforge)
+as explained [here](https://github.com/google/jax/issues/5501).
+In the Miniforge environment, please try the following:
+```bash
+pip install "jax[cpu]==0.3.22" jaxlib
+pip install basicpy
+```
+
+### For Windows users
 
 BaSiCPy requires [`jax`](https://github.com/google/jax/) which does not support Windows officially.
 However, thanks to [cloudhan/jax-windows-builder](https://github.com/cloudhan/jax-windows-builder), we can install BaSiCPy as follows:
-```
-pip install "jax[cpu]===0.3.14" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
+
+```bash
+pip install "jax[cpu]==0.3.14" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
 pip install basicpy
 ```
 For details and latest updates, see [this issue](https://github.com/google/jax/issues/438).
 
 ### Install with dev dependencies
 
 ```console
```

### Comparing `BaSiCPy-1.0.1/src/basicpy/__main__.py` & `BaSiCPy-1.1.0/src/basicpy/__main__.py`

 * *Files identical despite different names*

### Comparing `BaSiCPy-1.0.1/src/basicpy/_jax_routines.py` & `BaSiCPy-1.1.0/src/basicpy/_jax_routines.py`

 * *Files identical despite different names*

### Comparing `BaSiCPy-1.0.1/src/basicpy/basicpy.py` & `BaSiCPy-1.1.0/src/basicpy/basicpy.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import jax.numpy as jnp
 
 # 3rd party modules
 import numpy as np
+from hyperactive import Hyperactive
+from hyperactive.optimizers import HillClimbingOptimizer
 from jax import device_put
 from jax.image import ResizeMethod
 from jax.image import resize as jax_resize
 from pydantic import BaseModel, Field, PrivateAttr, root_validator
 from skimage.transform import resize as skimage_resize
 
 from basicpy._jax_routines import ApproximateFit, LadmapFit
+from basicpy.metrics import entropy
 from basicpy.tools.dct_tools import JaxDCT
 
 # Package modules
 from basicpy.types import ArrayLike, PathLike
 
 newax = jnp.newaxis
 
@@ -244,26 +247,33 @@
                     working_shape = self.working_size
             target_shape = [*Im.shape[:2], *working_shape]
             Im = self._resize(Im, target_shape)
 
         return Im
 
     def fit(
-        self, images: np.ndarray, fitting_weight: Optional[np.ndarray] = None
+        self,
+        images: np.ndarray,
+        fitting_weight: Optional[np.ndarray] = None,
+        skip_shape_warning=False,
     ) -> None:
         """Generate illumination correction profiles from images.
 
         Args:
             images: Input images to fit shading model.
                     Must be 3-dimensional or 4-dimensional array
                     with dimension of (T,Y,X) or (T,Z,Y,X).
                     T can be either of time or mosaic position.
-            fitting_weight: relative fitting weight for each pixel.
+                    Multichannel images should be
+                    independently corrected for each channel.
+            fitting_weight: Relative fitting weight for each pixel.
                     Higher value means more contribution to fitting.
                     Must has the same shape as images.
+            skip_shape_warning: if True, warning for last dimension
+                    less than 10 is suppressed.
 
         Example:
             >>> from basicpy import BaSiC
             >>> from basicpy import datasets as bdata
             >>> images = bdata.wsi_brain()
             >>> basic = BaSiC()  # use default settings
             >>> basic.fit(images)
@@ -276,15 +286,26 @@
                 fitting_weight = fitting_weight[:, np.newaxis, ...]
         elif images.ndim == 4:
             if self.fitting_mode == FittingMode.approximate:
                 raise ValueError(
                     "Only 3-dimensional images are accepted for the approximate mode."
                 )
         else:
-            raise ValueError("images must be 3 or 4-dimensional array")
+            raise ValueError(
+                "Images must be 3 or 4-dimensional array, "
+                + "with dimension of (T,Y,X) or (T,Z,Y,X)."
+            )
+
+        if images.shape[-1] < 10 and not skip_shape_warning:
+            logger.warning(
+                "Image last dimension is less than 10. "
+                + "Are you supplying images with the channel dimension?"
+                + "Multichannel images should be "
+                + "independently corrected for each channel."
+            )
 
         if fitting_weight is not None and fitting_weight.shape != images.shape:
             raise ValueError("fitting_weight must have the same shape as images.")
 
         logger.info("=== BaSiC fit started ===")
         start_time = time.monotonic()
 
@@ -441,15 +462,18 @@
                     break
             if i == self.max_reweight_iterations - 1:
                 logger.warning("Reweighting did not converge.")
             last_S = S
             last_D = D
 
         if not converged:
-            logger.warning("Single-step optimization did not converge at the last reweighting step.")
+            logger.warning(
+                "Single-step optimization did not converge "
+                + "at the last reweighting step."
+            )
 
         assert S is not None
         assert D is not None
         assert B is not None
 
         if self.sort_intensity:
             for i in range(self.max_reweight_iterations_baseline):
@@ -558,15 +582,15 @@
             f"=== BaSiC transform finished in {time.monotonic()-start_time} seconds ==="
         )
         return output
 
     # REFACTOR large datasets will probably prefer saving corrected images to
     # files directly, a generator may be handy
     def fit_transform(
-        self, images: ArrayLike, timelapse: bool = True
+        self, images: ArrayLike, timelapse: bool = False
     ) -> Union[Tuple[np.ndarray, np.ndarray], np.ndarray]:
         """Fit and transform on data.
 
         Args:
             images: input images to fit and correct. See `fit`.
 
         Returns:
@@ -576,14 +600,154 @@
             >>> corrected = basic.fit_transform(images)
         """
         self.fit(images)
         corrected = self.transform(images, timelapse)
 
         return corrected
 
+    def autotune(
+        self,
+        images: np.ndarray,
+        fitting_weight: Optional[np.ndarray] = None,
+        skip_shape_warning: bool = False,
+        *,
+        optmizer=None,
+        n_iter=100,
+        search_space=None,
+        init_params=None,
+        timelapse: bool = False,
+        histogram_qmin: float = 0.01,
+        histogram_qmax: float = 0.99,
+        histogram_bins: int = 100,
+        histogram_use_fitting_weight: bool = True,
+        early_stop: bool = True,
+        early_stop_n_iter_no_change: int = 10,
+        early_stop_torelance: float = 1e-6,
+        random_state: Optional[int] = None,
+    ) -> None:
+        """Automatically tune the parameters of the model.
+
+        Args:
+            images: input images to fit and correct. See `fit`.
+            fitting_weight: Relative fitting weight for each pixel. See `fit`.
+            skip_shape_warning: if True, warning for last dimension
+                    less than 10 is suppressed.
+            optimizer: optimizer to use. Defaults to
+                    `hyperactive.optimizers.HillClimbingOptimizer`.
+            n_iter: number of iterations for the optimizer. Defaults to 100.
+            search_space: search space for the optimizer.
+                    Defaults to a reasonable range for each parameter.
+            init_params: initial parameters for the optimizer.
+                    Defaults to a reasonable initial value for each parameter.
+            timelapse: if True, corrects the timelapse/photobleaching offsets.
+            histogram_qmin: the minimum quantile to use for the histogram.
+                    Defaults to 0.01.
+            histogram_qmax: the maximum quantile to use for the histogram.
+                    Defaults to 0.99.
+            histogram_bins: the number of bins to use for the histogram.
+                    Defaults to 100.
+            early_stop: if True, stops the optimization when the change in
+                    entropy is less than `early_stop_torelance`.
+                    Defaults to True.
+            early_stop_n_iter_no_change: the number of iterations for early
+                    stopping. Defaults to 10.
+            early_stop_torelance: the absolute value torelance
+                    for early stopping.
+            random_state: random state for the optimizer.
+
+        """
+
+        if search_space is None:
+            search_space = {
+                "smoothness_flatfield": list(np.logspace(-3, 1, 20)),
+                "smoothness_darkfield": [0] + list(np.logspace(-3, 1, 20)),
+                "sparse_cost_darkfield": [0] + list(np.logspace(-3, 1, 20)),
+            }
+        if init_params is None:
+            init_params = {
+                "smoothness_flatfield": 0.1,
+                "smoothness_darkfield": 1e-3,
+                "sparse_cost_darkfield": 1e-3,
+            }
+
+        # calculate the histogram range
+        basic = self.copy(update=init_params)
+        basic.fit(
+            images,
+            fitting_weight=fitting_weight,
+            skip_shape_warning=skip_shape_warning,
+        )
+        transformed = basic.transform(images, timelapse=timelapse)
+        vmin, vmax = np.quantile(transformed, [histogram_qmin, histogram_qmax])
+        val_range = vmax - vmin  # fix the value range for histogram
+
+        if fitting_weight is None or not histogram_use_fitting_weight:
+            weights = None
+        else:
+            weights = fitting_weight
+
+        def fit_and_calc_entropy(params):
+            try:
+                basic = self.copy(update=params)
+                basic.fit(
+                    images,
+                    fitting_weight=fitting_weight,
+                    skip_shape_warning=skip_shape_warning,
+                )
+                transformed = basic.transform(images, timelapse=timelapse)
+                vmin_new = np.quantile(transformed, histogram_qmin)
+
+                entropy_value = entropy(
+                    transformed,
+                    vmin=vmin_new,
+                    vmax=vmin_new + val_range,
+                    bins=histogram_bins,
+                    weights=weights,
+                    clip=True,
+                )
+                return -entropy_value
+            except RuntimeError:
+                return -np.inf
+
+        if optmizer is None:
+            optimizer = HillClimbingOptimizer(
+                epsilon=0.1,
+                distribution="laplace",
+                n_neighbours=4,
+                rand_rest_p=0.1,
+            )
+
+        hyper = Hyperactive()
+
+        params = dict(
+            optimizer=optimizer,
+            n_iter=n_iter,
+            initialize=dict(warm_start=[init_params]),
+            random_state=random_state,
+        )
+
+        if early_stop:
+            params.update(
+                dict(
+                    early_stopping=dict(
+                        n_iter_no_change=early_stop_n_iter_no_change,
+                        tol_abs=early_stop_torelance,
+                    )
+                )
+            )
+
+        hyper.add_search(
+            fit_and_calc_entropy,
+            search_space,
+            **params,
+        )
+        hyper.run()
+        best_params = hyper.best_para(fit_and_calc_entropy)
+        self.__dict__.update(best_params)
+
     @property
     def score(self):
         """The BaSiC fit final score."""
         return self._score
 
     @property
     def reweight_score(self):
```

### Comparing `BaSiCPy-1.0.1/src/basicpy/datasets.py` & `BaSiCPy-1.1.0/src/basicpy/datasets.py`

 * *Files identical despite different names*

### Comparing `BaSiCPy-1.0.1/src/basicpy/tools/_jax_idct.py` & `BaSiCPy-1.1.0/src/basicpy/tools/_jax_idct.py`

 * *Files identical despite different names*

### Comparing `BaSiCPy-1.0.1/src/basicpy/tools/dct_tools.py` & `BaSiCPy-1.1.0/src/basicpy/tools/dct_tools.py`

 * *Files identical despite different names*

