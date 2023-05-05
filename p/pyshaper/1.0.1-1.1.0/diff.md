# Comparing `tmp/pyshaper-1.0.1.tar.gz` & `tmp/pyshaper-1.1.0.tar.gz`

## Comparing `pyshaper-1.0.1.tar` & `pyshaper-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pyshaper-1.0.1/LICENSE
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 pyshaper-1.0.1/README.md
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pyshaper-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    16804 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/CommonObservables.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/GroundSpace.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/Manifolds.py
--rw-r--r--   0        0        0    10078 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/Observables.py
--rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/Shaper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/utils/__init__.py
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/utils/data_utils.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 pyshaper-1.0.1/src/pyshaper/utils/plot_utils.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 pyshaper-1.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pyshaper-1.0.1/LICENSE
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 pyshaper-1.0.1/README.md
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pyshaper-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 pyshaper-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pyshaper-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 pyshaper-1.1.0/README.md
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pyshaper-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16804 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/CommonObservables.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/GroundSpace.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/Manifolds.py
+-rw-r--r--   0        0        0    10078 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/Observables.py
+-rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/Shaper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/utils/__init__.py
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/utils/data_utils.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 pyshaper-1.1.0/src/pyshaper/utils/plot_utils.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 pyshaper-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pyshaper-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 pyshaper-1.1.0/README.md
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pyshaper-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 pyshaper-1.1.0/PKG-INFO
```

### Comparing `pyshaper-1.0.1/LICENSE` & `pyshaper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshaper-1.0.1/README.md` & `pyshaper-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SHAPER (v1.0.1)
+# SHAPER (v1.1.0)
 
 [![GitHub Project](https://img.shields.io/badge/GitHub--blue?style=social&logo=GitHub)](https://github.com/rikab/shaper)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7689890.svg)](https://doi.org/10.5281/zenodo.7689890)
 
 [![PyPI version](https://img.shields.io/pypi/v/pyshaper.svg)](https://pypi.org/project/pyshaper/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pyshaper.svg)](https://pypi.org/project/pyshaper/)
 
@@ -23,35 +23,32 @@
 ## Installation
 
 ### From PyPI
 
 In your Python environment run
 
 ```
-python -m pip install numpy torch  # c.f. https://github.com/jeanfeydy/geomloss/issues/69
 python -m pip install pyshaper
 # python -m pip install --upgrade 'pyshaper[all]'  # for all extras
 ```
 
 ### From this repository locally
 
 In your Python environment from the top level of this repository run
 
 ```
-python -m pip install numpy torch  # c.f. https://github.com/jeanfeydy/geomloss/issues/69
 python -m pip install .
 # python -m pip install --upgrade '.[all]'  # for all extras
 ```
 
 ### From GitHub
 
 In your Python environment run
 
 ```
-python -m pip install numpy torch  # c.f. https://github.com/jeanfeydy/geomloss/issues/69
 python -m pip install "pyshaper @ git+https://github.com/rikab/shaper.git"
 # python -m pip install --upgrade "pyshaper[all] @ git+https://github.com/rikab/shaper.git"  # for all extras
 ```
 
 ## Example Usage
 
 For an example of how to use `SHAPER`, see the notebook `examples/example.ipynb`. This notebook contains example code for loading data, using pre-built shape observables, defining custom shape observables, running the `SHAPER` algorithm to evaluate these observables, and making plots.
@@ -77,19 +74,19 @@
 
 ## Citation
 
 If you use `SHAPER`, please cite both this code archive and the corresponding paper, "Can You Hear the Shape of a Jet"?:
 
     @software{SHAPER,
       author = {Rikab Gambhir},
-      title = "{pyshaper: v1.0.1}",
-      version = {1.0.1},
+      title = "{pyshaper: v1.1.0}",
+      version = {1.1.0},
       doi = {10.5281/zenodo.7689890},
       url = {doi.org/10.5281/zenodo.7689890},
-      note = {https://github.com/rikab/SHAPER/releases/tag/v1.0.1}
+      note = {https://github.com/rikab/SHAPER/releases/tag/v1.1.0}
     }
 
     @article{Ba:2023hix,
     author = "Ba, Demba and Dogra, Akshunna S. and Gambhir, Rikab and Tasissa, Abiy and Thaler, Jesse",
     title = "{SHAPER: Can You Hear the Shape of a Jet?}",
     eprint = "2302.12266",
     archivePrefix = "arXiv",
@@ -97,14 +94,15 @@
     reportNumber = "MIT-CTP 5535",
     month = "2",
     year = "2023"
     }
 
 ## Changelog
 
+- v1.1.0: 5 May 2023. Updated Geomloss dependency
 - v1.0.1: 10 March 2023. PyPi-installable release. Minor changes to example and optional dependency handling.
 - v1.0.0: 24 February 2023. Official public release.
 
 Based on the work in ["SHAPER: Can You Hear the Shape of a Jet?" (arxiv:2302.12266)](https://arxiv.org/abs/2302.12266)
 
 Bugs, Fixes, Ideas, or Questions? Contact me at rikab@mit.edu
```

### Comparing `pyshaper-1.0.1/pyproject.toml` & `pyshaper-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 dependencies = [
     "torch>=1.10.0",
-    "geomloss>=0.2.3",
+    "geomloss>=0.2.6",
     "pyjet>=1.9.0",  # FIXME: Deprecated
     "scipy>=1.5.1",
     "matplotlib>=3.5.0",
     "numpy",  # compatible versions controlled through scipy
 ]
 
 [project.urls]
```

### Comparing `pyshaper-1.0.1/src/pyshaper/CommonObservables.py` & `pyshaper-1.1.0/src/pyshaper/CommonObservables.py`

 * *Files identical despite different names*

### Comparing `pyshaper-1.0.1/src/pyshaper/Manifolds.py` & `pyshaper-1.1.0/src/pyshaper/Manifolds.py`

 * *Files identical despite different names*

### Comparing `pyshaper-1.0.1/src/pyshaper/Observables.py` & `pyshaper-1.1.0/src/pyshaper/Observables.py`

 * *Files identical despite different names*

### Comparing `pyshaper-1.0.1/src/pyshaper/Shaper.py` & `pyshaper-1.1.0/src/pyshaper/Shaper.py`

 * *Files identical despite different names*

### Comparing `pyshaper-1.0.1/src/pyshaper/utils/data_utils.py` & `pyshaper-1.1.0/src/pyshaper/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `pyshaper-1.0.1/src/pyshaper/utils/plot_utils.py` & `pyshaper-1.1.0/src/pyshaper/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pyshaper-1.0.1/.gitignore` & `pyshaper-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyshaper-1.0.1/PKG-INFO` & `pyshaper-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshaper
-Version: 1.0.1
+Version: 1.1.0
 Summary: framework for defining, building, and evaluating generalized shape observables for collider physics
 Project-URL: Documentation, https://github.com/rikab/SHAPER
 Project-URL: Homepage, https://github.com/rikab/SHAPER
 Project-URL: Issue Tracker, https://github.com/rikab/SHAPER/issues
 Project-URL: Releases, https://github.com/rikab/SHAPER/releases
 Project-URL: Source Code, https://github.com/rikab/SHAPER
 Author-email: Rikab Gambhir <rikab@mit.edu>
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
-Requires-Dist: geomloss>=0.2.3
+Requires-Dist: geomloss>=0.2.6
 Requires-Dist: matplotlib>=3.5.0
 Requires-Dist: numpy
 Requires-Dist: pyjet>=1.9.0
 Requires-Dist: scipy>=1.5.1
 Requires-Dist: torch>=1.10.0
 Provides-Extra: all
 Requires-Dist: pyshaper[energyflow,viz]; extra == 'all'
@@ -37,15 +37,15 @@
 Requires-Dist: scikit-learn>=1.2.0; extra == 'energyflow'
 Requires-Dist: tensorflow-macos>=2.7.0; platform_machine == 'arm64' and platform_system == 'Darwin' and extra == 'energyflow'
 Requires-Dist: tensorflow>=2.7.0; platform_machine != 'arm64' and extra == 'energyflow'
 Provides-Extra: viz
 Requires-Dist: imageio>=2.20.0; extra == 'viz'
 Description-Content-Type: text/markdown
 
-# SHAPER (v1.0.1)
+# SHAPER (v1.1.0)
 
 [![GitHub Project](https://img.shields.io/badge/GitHub--blue?style=social&logo=GitHub)](https://github.com/rikab/shaper)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7689890.svg)](https://doi.org/10.5281/zenodo.7689890)
 
 [![PyPI version](https://img.shields.io/pypi/v/pyshaper.svg)](https://pypi.org/project/pyshaper/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pyshaper.svg)](https://pypi.org/project/pyshaper/)
 
@@ -66,35 +66,32 @@
 ## Installation
 
 ### From PyPI
 
 In your Python environment run
 
 ```
-python -m pip install numpy torch  # c.f. https://github.com/jeanfeydy/geomloss/issues/69
 python -m pip install pyshaper
 # python -m pip install --upgrade 'pyshaper[all]'  # for all extras
 ```
 
 ### From this repository locally
 
 In your Python environment from the top level of this repository run
 
 ```
-python -m pip install numpy torch  # c.f. https://github.com/jeanfeydy/geomloss/issues/69
 python -m pip install .
 # python -m pip install --upgrade '.[all]'  # for all extras
 ```
 
 ### From GitHub
 
 In your Python environment run
 
 ```
-python -m pip install numpy torch  # c.f. https://github.com/jeanfeydy/geomloss/issues/69
 python -m pip install "pyshaper @ git+https://github.com/rikab/shaper.git"
 # python -m pip install --upgrade "pyshaper[all] @ git+https://github.com/rikab/shaper.git"  # for all extras
 ```
 
 ## Example Usage
 
 For an example of how to use `SHAPER`, see the notebook `examples/example.ipynb`. This notebook contains example code for loading data, using pre-built shape observables, defining custom shape observables, running the `SHAPER` algorithm to evaluate these observables, and making plots.
@@ -120,19 +117,19 @@
 
 ## Citation
 
 If you use `SHAPER`, please cite both this code archive and the corresponding paper, "Can You Hear the Shape of a Jet"?:
 
     @software{SHAPER,
       author = {Rikab Gambhir},
-      title = "{pyshaper: v1.0.1}",
-      version = {1.0.1},
+      title = "{pyshaper: v1.1.0}",
+      version = {1.1.0},
       doi = {10.5281/zenodo.7689890},
       url = {doi.org/10.5281/zenodo.7689890},
-      note = {https://github.com/rikab/SHAPER/releases/tag/v1.0.1}
+      note = {https://github.com/rikab/SHAPER/releases/tag/v1.1.0}
     }
 
     @article{Ba:2023hix,
     author = "Ba, Demba and Dogra, Akshunna S. and Gambhir, Rikab and Tasissa, Abiy and Thaler, Jesse",
     title = "{SHAPER: Can You Hear the Shape of a Jet?}",
     eprint = "2302.12266",
     archivePrefix = "arXiv",
@@ -140,14 +137,15 @@
     reportNumber = "MIT-CTP 5535",
     month = "2",
     year = "2023"
     }
 
 ## Changelog
 
+- v1.1.0: 5 May 2023. Updated Geomloss dependency
 - v1.0.1: 10 March 2023. PyPi-installable release. Minor changes to example and optional dependency handling.
 - v1.0.0: 24 February 2023. Official public release.
 
 Based on the work in ["SHAPER: Can You Hear the Shape of a Jet?" (arxiv:2302.12266)](https://arxiv.org/abs/2302.12266)
 
 Bugs, Fixes, Ideas, or Questions? Contact me at rikab@mit.edu
```

