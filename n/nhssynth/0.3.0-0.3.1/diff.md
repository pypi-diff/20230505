# Comparing `tmp/nhssynth-0.3.0.tar.gz` & `tmp/nhssynth-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhssynth-0.3.0.tar", max compression
+gzip compressed data, was "nhssynth-0.3.1.tar", max compression
```

## Comparing `nhssynth-0.3.0.tar` & `nhssynth-0.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.3.0/LICENSE
--rw-r--r--   0        0        0     7937 2023-04-26 19:31:33.655713 nhssynth-0.3.0/README.md
--rw-r--r--   0        0        0     1473 2023-04-26 19:31:59.711829 nhssynth-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.3.0/src/nhssynth/cli/__init__.py
--rw-r--r--   0        0        0     3437 2023-04-26 19:31:33.656962 nhssynth-0.3.0/src/nhssynth/cli/common_arguments.py
--rw-r--r--   0        0        0     8878 2023-04-26 19:31:33.657342 nhssynth-0.3.0/src/nhssynth/cli/config.py
--rw-r--r--   0        0        0     1826 2023-04-26 19:31:33.657526 nhssynth-0.3.0/src/nhssynth/cli/model_arguments.py
--rw-r--r--   0        0        0     6768 2023-04-26 19:31:33.657824 nhssynth-0.3.0/src/nhssynth/cli/module_arguments.py
--rw-r--r--   0        0        0     7416 2023-04-26 19:31:33.658068 nhssynth-0.3.0/src/nhssynth/cli/module_setup.py
--rw-r--r--   0        0        0     1396 2023-04-26 19:31:33.658300 nhssynth-0.3.0/src/nhssynth/cli/run.py
--rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.3.0/src/nhssynth/common/__init__.py
--rw-r--r--   0        0        0      354 2023-04-26 19:31:33.658538 nhssynth-0.3.0/src/nhssynth/common/common.py
--rw-r--r--   0        0        0     3613 2023-04-26 19:31:33.658743 nhssynth-0.3.0/src/nhssynth/common/constants.py
--rw-r--r--   0        0        0      376 2023-04-26 19:31:33.658992 nhssynth-0.3.0/src/nhssynth/common/debugging.py
--rw-r--r--   0        0        0     2132 2023-04-18 15:14:18.123813 nhssynth-0.3.0/src/nhssynth/common/dicts.py
--rw-r--r--   0        0        0     3119 2023-04-26 19:31:33.659233 nhssynth-0.3.0/src/nhssynth/common/io.py
--rw-r--r--   0        0        0      582 2023-04-26 19:31:33.659388 nhssynth-0.3.0/src/nhssynth/common/strings.py
--rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.3.0/src/nhssynth/modules/__init__.py
--rw-r--r--   0        0        0       20 2023-03-06 16:05:17.363712 nhssynth-0.3.0/src/nhssynth/modules/dataloader/__init__.py
--rw-r--r--   0        0        0     4082 2023-04-12 15:32:23.986086 nhssynth-0.3.0/src/nhssynth/modules/dataloader/io.py
--rw-r--r--   0        0        0     5253 2023-04-12 15:46:13.535858 nhssynth-0.3.0/src/nhssynth/modules/dataloader/metadata.py
--rw-r--r--   0        0        0    16743 2023-04-26 19:31:33.659686 nhssynth-0.3.0/src/nhssynth/modules/dataloader/metatransformer.py
--rw-r--r--   0        0        0     1347 2023-04-26 19:31:33.659921 nhssynth-0.3.0/src/nhssynth/modules/dataloader/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.3.0/src/nhssynth/modules/evaluation/__init__.py
--rw-r--r--   0        0        0    14071 2023-04-26 19:31:33.660200 nhssynth-0.3.0/src/nhssynth/modules/evaluation/full_report.py
--rw-r--r--   0        0        0     2644 2023-04-13 10:57:28.285918 nhssynth-0.3.0/src/nhssynth/modules/evaluation/io.py
--rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.3.0/src/nhssynth/modules/evaluation/metrics.py
--rw-r--r--   0        0        0     1835 2023-04-26 19:31:33.660620 nhssynth-0.3.0/src/nhssynth/modules/evaluation/run.py
--rw-r--r--   0        0        0       48 2023-04-26 19:31:33.660900 nhssynth-0.3.0/src/nhssynth/modules/model/__init__.py
--rw-r--r--   0        0        0     4379 2023-04-26 19:31:33.661089 nhssynth-0.3.0/src/nhssynth/modules/model/common/DPMixin.py
--rw-r--r--   0        0        0     6407 2023-04-26 19:31:33.661275 nhssynth-0.3.0/src/nhssynth/modules/model/common/Model.py
--rw-r--r--   0        0        0     3447 2023-04-26 19:31:33.661529 nhssynth-0.3.0/src/nhssynth/modules/model/io.py
--rw-r--r--   0        0        0     1648 2023-04-26 19:31:33.661707 nhssynth-0.3.0/src/nhssynth/modules/model/models/DPVAE.py
--rw-r--r--   0        0        0     9881 2023-04-26 19:31:33.661896 nhssynth-0.3.0/src/nhssynth/modules/model/models/VAE.py
--rw-r--r--   0        0        0      129 2023-04-26 19:31:33.662043 nhssynth-0.3.0/src/nhssynth/modules/model/models/__init__.py
--rw-r--r--   0        0        0     2221 2023-04-26 19:31:33.662267 nhssynth-0.3.0/src/nhssynth/modules/model/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.3.0/src/nhssynth/modules/plotting/__init__.py
--rw-r--r--   0        0        0     2611 2023-04-13 11:19:38.014249 nhssynth-0.3.0/src/nhssynth/modules/plotting/io.py
--rw-r--r--   0        0        0     6421 2023-04-13 19:24:58.843577 nhssynth-0.3.0/src/nhssynth/modules/plotting/plots.py
--rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.3.0/src/nhssynth/modules/plotting/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.3.0/src/nhssynth/modules/structure/__init__.py
--rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.3.0/src/nhssynth/modules/structure/run.py
--rw-r--r--   0        0        0     9241 1970-01-01 00:00:00.000000 nhssynth-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.3.1/LICENSE
+-rw-r--r--   0        0        0     8859 2023-05-04 19:45:30.956684 nhssynth-0.3.1/README.md
+-rw-r--r--   0        0        0     1867 2023-05-05 15:52:55.455154 nhssynth-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.3.1/src/nhssynth/cli/__init__.py
+-rw-r--r--   0        0        0     3437 2023-04-26 19:31:33.656962 nhssynth-0.3.1/src/nhssynth/cli/common_arguments.py
+-rw-r--r--   0        0        0     8854 2023-04-27 13:25:22.472512 nhssynth-0.3.1/src/nhssynth/cli/config.py
+-rw-r--r--   0        0        0     1826 2023-04-26 19:31:33.657526 nhssynth-0.3.1/src/nhssynth/cli/model_arguments.py
+-rw-r--r--   0        0        0     6768 2023-04-26 19:31:33.657824 nhssynth-0.3.1/src/nhssynth/cli/module_arguments.py
+-rw-r--r--   0        0        0     7421 2023-05-05 14:21:02.300157 nhssynth-0.3.1/src/nhssynth/cli/module_setup.py
+-rw-r--r--   0        0        0     1396 2023-04-26 19:31:33.658300 nhssynth-0.3.1/src/nhssynth/cli/run.py
+-rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.3.1/src/nhssynth/common/__init__.py
+-rw-r--r--   0        0        0      385 2023-04-27 13:22:15.158073 nhssynth-0.3.1/src/nhssynth/common/common.py
+-rw-r--r--   0        0        0     3613 2023-04-26 19:31:33.658743 nhssynth-0.3.1/src/nhssynth/common/constants.py
+-rw-r--r--   0        0        0      376 2023-04-26 19:31:33.658992 nhssynth-0.3.1/src/nhssynth/common/debugging.py
+-rw-r--r--   0        0        0     2369 2023-04-27 13:23:24.877565 nhssynth-0.3.1/src/nhssynth/common/dicts.py
+-rw-r--r--   0        0        0     3149 2023-04-27 13:23:45.952265 nhssynth-0.3.1/src/nhssynth/common/io.py
+-rw-r--r--   0        0        0      582 2023-04-26 19:31:33.659388 nhssynth-0.3.1/src/nhssynth/common/strings.py
+-rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.3.1/src/nhssynth/modules/__init__.py
+-rw-r--r--   0        0        0       20 2023-03-06 16:05:17.363712 nhssynth-0.3.1/src/nhssynth/modules/dataloader/__init__.py
+-rw-r--r--   0        0        0     4082 2023-04-12 15:32:23.986086 nhssynth-0.3.1/src/nhssynth/modules/dataloader/io.py
+-rw-r--r--   0        0        0     5253 2023-04-12 15:46:13.535858 nhssynth-0.3.1/src/nhssynth/modules/dataloader/metadata.py
+-rw-r--r--   0        0        0    17033 2023-05-05 14:21:02.300580 nhssynth-0.3.1/src/nhssynth/modules/dataloader/metatransformer.py
+-rw-r--r--   0        0        0     1328 2023-05-05 14:21:02.301252 nhssynth-0.3.1/src/nhssynth/modules/dataloader/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.3.1/src/nhssynth/modules/evaluation/__init__.py
+-rw-r--r--   0        0        0    14071 2023-04-26 19:31:33.660200 nhssynth-0.3.1/src/nhssynth/modules/evaluation/full_report.py
+-rw-r--r--   0        0        0     2622 2023-05-05 14:21:02.301903 nhssynth-0.3.1/src/nhssynth/modules/evaluation/io.py
+-rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.3.1/src/nhssynth/modules/evaluation/metrics.py
+-rw-r--r--   0        0        0     1835 2023-04-26 19:31:33.660620 nhssynth-0.3.1/src/nhssynth/modules/evaluation/run.py
+-rw-r--r--   0        0        0       48 2023-04-26 19:31:33.660900 nhssynth-0.3.1/src/nhssynth/modules/model/__init__.py
+-rw-r--r--   0        0        0     4345 2023-04-28 11:01:27.969421 nhssynth-0.3.1/src/nhssynth/modules/model/common/DPMixin.py
+-rw-r--r--   0        0        0     6391 2023-05-05 15:47:58.057779 nhssynth-0.3.1/src/nhssynth/modules/model/common/Model.py
+-rw-r--r--   0        0        0     3425 2023-05-05 14:21:02.302352 nhssynth-0.3.1/src/nhssynth/modules/model/io.py
+-rw-r--r--   0        0        0     1648 2023-04-26 19:31:33.661707 nhssynth-0.3.1/src/nhssynth/modules/model/models/DPVAE.py
+-rw-r--r--   0        0        0     9945 2023-05-05 15:52:45.345428 nhssynth-0.3.1/src/nhssynth/modules/model/models/VAE.py
+-rw-r--r--   0        0        0      129 2023-04-26 19:31:33.662043 nhssynth-0.3.1/src/nhssynth/modules/model/models/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-05 14:21:02.302796 nhssynth-0.3.1/src/nhssynth/modules/model/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.3.1/src/nhssynth/modules/plotting/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-05 14:21:02.303228 nhssynth-0.3.1/src/nhssynth/modules/plotting/io.py
+-rw-r--r--   0        0        0     6421 2023-04-13 19:24:58.843577 nhssynth-0.3.1/src/nhssynth/modules/plotting/plots.py
+-rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.3.1/src/nhssynth/modules/plotting/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.3.1/src/nhssynth/modules/structure/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.3.1/src/nhssynth/modules/structure/run.py
+-rw-r--r--   0        0        0    10163 1970-01-01 00:00:00.000000 nhssynth-0.3.1/PKG-INFO
```

### Comparing `nhssynth-0.3.0/LICENSE` & `nhssynth-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/README.md` & `nhssynth-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 <!-- PROJECT SHIELDS -->
 <div align="center">
 
-[![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth?style=flat-square)](https://pypi.org/project/nhssynth/)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/nhssynth?style=flat-square)](https://pypi.org/project/nhssynth/)
-[![PyPI - Package Status](https://img.shields.io/pypi/status/nhssynth?style=flat-square)](https://pypi.org/project/nhssynth/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth?style=flat-square)](https://www.python.org/downloads/release/python-3100/)
-[![PyPI - License](https://img.shields.io/pypi/l/nhssynth?style=flat-square)](https://github.com/nhsx/nhssynth/blob/main/LICENSE)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000?style=flat-square)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square)](https://pycqa.github.io/isort/)
+![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/coverage.json)
+![Tests Passing](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/tests.json)
+![Lines of Code](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/loc.json)
+![Percentage Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/comments.json)
+[![Snyk Package Health](https://snyk.io/advisor/python/nhssynth/badge.svg)](https://snyk.io/advisor/python/nhssynth)
 
 </div>
+<div align="center">
+
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)](https://www.python.org/downloads/release/python-3100/)
+[![PyPI - Package Status](https://img.shields.io/pypi/status/nhssynth)](https://pypi.org/project/nhssynth/)
+[![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth)](https://pypi.org/project/nhssynth/)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/nhssynth)](https://pypi.org/project/nhssynth/)
+[![PyPI - License](https://img.shields.io/pypi/l/nhssynth)](https://github.com/nhsx/nhssynth/blob/main/LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)
 
+</div>
 
 <!-- PROJECT LOGO -->
 <div align="center">
   <a href="https://nhsx.github.io/NHSSynth">
     <img src="docs/assets/NHS.svg" alt="Logo" width="200" height="100">
   </a>
   <p align="center">
     <a href="https://nhsx.github.io/NHSSynth"><strong>Explore the docs »</strong></a>
-    <br /><br /><br />
+    <br /><br />
   </p>
 </div>
 
 # NHS Synth
 
 ## About
 
@@ -90,17 +98,19 @@
 
 To ensure reproducibility, you should always specify a `--seed` value and provide the `--save-config` flag to dump the exact configuration specified / inferred for the run. This configuration file can then be used in the future to reproduce the exact same run or shared with others to run the same configuration on their dataset, etc.
 
 The figure below shows the structure and workflow of the package and its modules.
 
 ![](docs/modules.png)
 
+View a visualisation of the codebase [here](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=nhsx%2Fnhssynth)!
+
 ### Roadmap
 
-See the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed features (and known issues).
+See the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed features (and known bugs). Our [milestones](https://github.com/nhsx/NHSSynth/milestones) represent longer term goals for the project.
 
 ### Contributing
 
 Any contributions you wish to make are **greatly appreciated**, we encourage you to first raise an issue to discuss with the maintainers. If you are interested in contributing, please follow these steps:
 
 1. Fork the project
 2. Create your branch (`git checkout -b <yourusername>/<featurename>`)
@@ -122,12 +132,12 @@
 
 ### License
 
 Distributed under the MIT License. _See [LICENSE](./LICENSE) for more information._
 
 ### Contact
 
-This project is under active development by [@HarrisonWilde](https://github.com/HarrisonWilde), for any questions or security concerns [contact him](mailto:h.wilde@warwick.ac.uk) or [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose). Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net).
+This project is under active development by [@HarrisonWilde](https://github.com/HarrisonWilde). For feature requests and bugs, please [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose); for security concerns, please open a [draft security advisory](https://github.com/nhsx/NHSSynth/security/advisories/new). Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net).
 
 To find out more about the [Analytics Unit](https://www.nhsx.nhs.uk/key-tools-and-info/nhsx-analytics-unit/) visit our [project website](https://nhsx.github.io/AnalyticsUnit/projects.html) or get in touch at [england.tdau@nhs.net](mailto:england.tdau@nhs.net).
 
 <!-- ### Acknowledgements -->
```

#### html2text {}

```diff
@@ -1,23 +1,31 @@
- [![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth?style=flat-
-    square)](https://pypi.org/project/nhssynth/) [![PyPI - Wheel](https://
-   img.shields.io/pypi/wheel/nhssynth?style=flat-square)](https://pypi.org/
-   project/nhssynth/) [![PyPI - Package Status](https://img.shields.io/pypi/
-status/nhssynth?style=flat-square)](https://pypi.org/project/nhssynth/) [![PyPI
- - Python Version](https://img.shields.io/pypi/pyversions/nhssynth?style=flat-
-   square)](https://www.python.org/downloads/release/python-3100/) [![PyPI -
- License](https://img.shields.io/pypi/l/nhssynth?style=flat-square)](https://
-  github.com/nhsx/nhssynth/blob/main/LICENSE) [![Code style: black](https://
-  img.shields.io/badge/code%20style-black-000000?style=flat-square)](https://
-    github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/
-%20imports-isort-%231674b1?style=flat-square)](https://pycqa.github.io/isort/)
+           ![Coverage](https://img.shields.io/endpoint?url=https://
+gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
+ coverage.json) ![Tests Passing](https://img.shields.io/endpoint?url=https://
+gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
+   tests.json) ![Lines of Code](https://img.shields.io/endpoint?url=https://
+gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
+ loc.json) ![Percentage Comments](https://img.shields.io/endpoint?url=https://
+gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
+comments.json) [![Snyk Package Health](https://snyk.io/advisor/python/nhssynth/
+             badge.svg)](https://snyk.io/advisor/python/nhssynth)
+  [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)]
+   (https://www.python.org/downloads/release/python-3100/) [![PyPI - Package
+Status](https://img.shields.io/pypi/status/nhssynth)](https://pypi.org/project/
+ nhssynth/) [![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth)]
+ (https://pypi.org/project/nhssynth/) [![PyPI - Wheel](https://img.shields.io/
+ pypi/wheel/nhssynth)](https://pypi.org/project/nhssynth/) [![PyPI - License]
+  (https://img.shields.io/pypi/l/nhssynth)](https://github.com/nhsx/nhssynth/
+    blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/
+ code%20style-black-000000)](https://github.com/psf/black) [![Imports: isort]
+      (https://img.shields.io/badge/%20imports-isort-%231674b1)](https://
+                            pycqa.github.io/isort/)
                                     [Logo]
                              Explore_the_docs_Â»
 
-
 # NHS Synth ## About This repository currently consists of a Python package
 alongside research and investigative materials covering the effectiveness of
 the package and synthetic data more generally when applied to NHS use cases.
 See the internal [project description](https://nhsx.github.io/nhsx-internship-
 projects/synthetic-data-exploration-vae/) for more information. _**Note:** No
 data, public or private are shared in this repository._ ## Getting Started ###
 Project Structure - The main package and codebase is found in [`src/nhssynth`]
@@ -71,31 +79,35 @@
 override any of the arguments provided in the configuration file by passing
 them as arguments in the command line. To ensure reproducibility, you should
 always specify a `--seed` value and provide the `--save-config` flag to dump
 the exact configuration specified / inferred for the run. This configuration
 file can then be used in the future to reproduce the exact same run or shared
 with others to run the same configuration on their dataset, etc. The figure
 below shows the structure and workflow of the package and its modules. ![]
-(docs/modules.png) ### Roadmap See the [open issues](https://github.com/nhsx/
-NHSSynth/issues) for a list of proposed features (and known issues). ###
+(docs/modules.png) View a visualisation of the codebase [here](https://mango-
+dune-07a8b7110.1.azurestaticapps.net/?repo=nhsx%2Fnhssynth)! ### Roadmap See
+the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of
+proposed features (and known bugs). Our [milestones](https://github.com/nhsx/
+NHSSynth/milestones) represent longer term goals for the project. ###
 Contributing Any contributions you wish to make are **greatly appreciated**, we
 encourage you to first raise an issue to discuss with the maintainers. If you
 are interested in contributing, please follow these steps: 1. Fork the project
 2. Create your branch (`git checkout -b /`) 3. Commit your changes (`git commit
 -m 'Add some amazing feature'`) 4. Push to the branch (`git push origin /`) 5.
 Open a PR and we will try to get it merged! _See [CONTRIBUTING.md](./
 CONTRIBUTING.md) for detailed guidance._ Thanks to everyone that has
 contributed so far!
                [https://contrib.rocks/image?repo=nhsx/nhssynth]
 This codebase builds on previous NHSX Analytics Unit PhD internships
 contextualising and investigating the potential use of Variational Auto
 Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic
 Danks and David Brind. ### License Distributed under the MIT License. _See
 [LICENSE](./LICENSE) for more information._ ### Contact This project is under
-active development by [@HarrisonWilde](https://github.com/HarrisonWilde), for
-any questions or security concerns [contact him](mailto:h.wilde@warwick.ac.uk)
-or [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose).
+active development by [@HarrisonWilde](https://github.com/HarrisonWilde). For
+feature requests and bugs, please [raise an issue](https://github.com/nhsx/
+NHSSynth/issues/new/choose); for security concerns, please open a [draft
+security advisory](https://github.com/nhsx/NHSSynth/security/advisories/new).
 Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net). To find
 out more about the [Analytics Unit](https://www.nhsx.nhs.uk/key-tools-and-info/
 nhsx-analytics-unit/) visit our [project website](https://nhsx.github.io/
 AnalyticsUnit/projects.html) or get in touch at [england.tdau@nhs.net](mailto:
 england.tdau@nhs.net).
```

### Comparing `nhssynth-0.3.0/pyproject.toml` & `nhssynth-0.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhssynth"
-version = "0.3.0"
+version = "0.3.1"
 description = "Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics"
 authors = ["HarrisonWilde <harrisondwilde@outlook.com>"]
 maintainers = ["NHSE TDAU <england.tdau@nhs.net>"]
 license = "MIT"
 readme = ["README.md"]
 repository = "https://github.com/nhsx/NHSSynth"
 keywords = ["synthetic data", "privacy", "fairness", "machine learning"]
@@ -40,17 +40,35 @@
 mkdocs-material = "^9.1.4"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 pymdown-extensions = "^9.10"
 
-[tool.poetry.group.dev]
+[tool.poetry.group.aux]
 optional = true
 
-[tool.poetry.group.dev.dependencies]
+[tool.poetry.group.aux.dependencies]
 jupyter = "^1.0.0"
 notebook = "^6.5.4"
 
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+tox = "^4.0.0"
+
+[tool.pytest.ini_options]
+testpaths = "tests"
+filterwarnings = ["ignore::DeprecationWarning:pkg_resources"]
+
+[tool.coverage.run]
+source = ["src/nhssynth/cli", "src/nhssynth/common", "src/nhssynth/modules"]
+omit = [
+    "src/nhssynth/common/debugging.py",
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nhssynth-0.3.0/src/nhssynth/cli/common_arguments.py` & `nhssynth-0.3.1/src/nhssynth/cli/common_arguments.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/cli/config.py` & `nhssynth-0.3.1/src/nhssynth/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,15 @@
         module_parsers: The dict of module-level parsers mapped to their names.
 
     Returns:
         A tuple containing two elements:
             - A dictionary containing all arguments and their default values.
             - A list of kvps of the required arguments and their associated module.
     """
-    all_actions = {
-        "top-level": top_parser._actions,
-        **{m: p._actions for m, p in module_parsers.items()},
-    }
+    all_actions = {"top-level": top_parser._actions} | {m: p._actions for m, p in module_parsers.items()}
     defaults = {}
     required_args = []
     for module, actions in all_actions.items():
         for action in actions:
             if action.dest not in ["help", "==SUPPRESS=="]:
                 defaults[action.dest] = action.default
                 if action.required:
```

### Comparing `nhssynth-0.3.0/src/nhssynth/cli/model_arguments.py` & `nhssynth-0.3.1/src/nhssynth/cli/model_arguments.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/cli/module_arguments.py` & `nhssynth-0.3.1/src/nhssynth/cli/module_arguments.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/cli/module_setup.py` & `nhssynth-0.3.1/src/nhssynth/cli/module_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from nhssynth.modules import dataloader, evaluation, model, plotting, structure
 
 
 class ModuleConfig:
     """
     Represents a module's configuration, containing the following attributes:
 
-    Properties:
+    Attributes:
         func: A callable that executes the module's functionality.
         add_args: A callable that populates the module's sub-parser arguments.
         description: A description of the module's functionality.
         help: A help message for the module's command-line interface.
         common_parsers: A list of common parsers to add to the module's sub-parser, appending the 'dataset' and 'core' parsers to those passed.
     """
 
@@ -39,16 +39,16 @@
             assert (
                 "core" not in common_parsers
             ), "The 'core' parser is automatically added to all modules, remove it from the ModuleConfig."
             self.common_parsers = ["dataset", "core"] + common_parsers
         else:
             self.common_parsers = ["dataset", "core"]
 
-    def __call__(self, *args, **kwargs) -> argparse.Namespace:
-        self.func(*args, **kwargs)
+    def __call__(self, args: argparse.Namespace) -> argparse.Namespace:
+        return self.func(args)
 
 
 def run_pipeline(args: argparse.Namespace) -> None:
     """Runs the specified pipeline of modules with the passed configuration `args`."""
     print("Running full pipeline...")
     args.modules_to_run = PIPELINE
     for module_name in PIPELINE:
```

### Comparing `nhssynth-0.3.0/src/nhssynth/cli/run.py` & `nhssynth-0.3.1/src/nhssynth/cli/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/common/constants.py` & `nhssynth-0.3.1/src/nhssynth/common/constants.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/common/dicts.py` & `nhssynth-0.3.1/src/nhssynth/common/dicts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Common functions for working with dictionaries."""
-from typing import Any
+from typing import Any, Union
 
 
-def filter_dict(d: dict, filter_keys: set | list, include: bool = False) -> dict:
+def filter_dict(d: dict, filter_keys: Union[set, list], include: bool = False) -> dict:
     """
     Given a dictionary, return a new dictionary either including or excluding keys in a given `filter` set.
 
     Args:
         d: A dictionary to filter.
         filter_keys: A list or set of keys to either include or exclude.
         include: Determine whether to return a dictionary including or excluding keys in `filter`.
@@ -24,15 +24,15 @@
     if include:
         filtered_keys = set(filter_keys) & set(d.keys())
     else:
         filtered_keys = set(d.keys()) - set(filter_keys)
     return {k: v for k, v in d.items() if k in filtered_keys}
 
 
-def get_key_by_value(d: dict, value) -> Any | None:
+def get_key_by_value(d: dict, value) -> Union[Any, None]:
     """
     Find the first key in a dictionary with a given value.
 
     Args:
         d: A dictionary to search through.
         value: The value to search for.
 
@@ -59,19 +59,24 @@
 
     Args:
         d: A dictionary with possibly nested keys.
 
     Returns:
         A flattened dictionary.
 
+    Raises:
+        ValueError: If duplicate keys are found in the flattened dictionary.
+
     Examples:
         >>> d = {'a': 1, 'b': {'c': 2, 'd': {'e': 3}}}
         >>> flatten_dict(d)
         {'a': 1, 'c': 2, 'e': 3}
     """
     items = []
     for k, v in d.items():
         if isinstance(v, dict):
             items.extend(flatten_dict(v).items())
         else:
             items.append((k, v))
+    if len(set([p[0] for p in items])) != len(items):
+        raise ValueError(f"Duplicate keys found in flattened dictionary")
     return dict(items)
```

### Comparing `nhssynth-0.3.0/src/nhssynth/common/io.py` & `nhssynth-0.3.1/src/nhssynth/common/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Common building-block functions for handling module input and output."""
 import warnings
 from pathlib import Path
+from typing import Union
 
 
 def experiment_io(experiment_name: str, dir_experiments: str = "experiments") -> str:
     """
     Create an experiment's directory and return the path.
 
     Args:
@@ -31,15 +32,15 @@
     Returns:
         The filename with the correct ending and potentially an inserted suffix.
     """
     path_fn = Path(fn)
     return str(path_fn.parent / path_fn.stem) + suffix + ending
 
 
-def consistent_endings(args: list[str | tuple[str, str] | tuple[str, str, str]]) -> list[str]:
+def consistent_endings(args: list[Union[str, tuple[str, str], tuple[str, str, str]]]) -> list[str]:
     return list(consistent_ending(arg) if isinstance(arg, str) else consistent_ending(*arg) for arg in args)
 
 
 def potential_suffix(fn: str, fn_base: str) -> str:
     """
     Checks if `fn` is a suffix (starts with an underscore) to append to `fn_base`, or a filename in its own right.
```

### Comparing `nhssynth-0.3.0/src/nhssynth/common/strings.py` & `nhssynth-0.3.1/src/nhssynth/common/strings.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/dataloader/io.py` & `nhssynth-0.3.1/src/nhssynth/modules/dataloader/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/dataloader/metadata.py` & `nhssynth-0.3.1/src/nhssynth/modules/dataloader/metadata.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/dataloader/metatransformer.py` & `nhssynth-0.3.1/src/nhssynth/modules/dataloader/metatransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import warnings
-from typing import Any
+from typing import Any, Union
 
 import numpy as np
 import pandas as pd
 from nhssynth.common.constants import SDV_SYNTHESIZERS
 from nhssynth.common.dicts import filter_dict
 from nhssynth.modules.dataloader.metadata import get_sdtypes
 from rdt.transformers import *
 from sdv.metadata import SingleTableMetadata
 from sdv.single_table.base import BaseSingleTableSynthesizer
 
 
 # TODO should this be an @classmethod?
-def get_transformer(d: dict) -> BaseTransformer | None:
+def get_transformer(d: dict) -> Union[BaseTransformer, None]:
     """
     Return a callable transformer object constructed from data in the given dictionary.
 
     Args:
         d: A dictionary containing the transformer data.
 
     Returns:
@@ -91,22 +91,29 @@
     - `inverse_apply(synthetic_data)`: Apply the inverse of the MetaTransformer to the given data.
 
     Note that `mt.apply` is a helper function that runs `mt.apply_dtypes`, `mt.instaniate`, `mt.assemble`, `mt.prepare` and finally
     `mt.count_onehots_and_singles` in sequence on a given raw dataset. Along the way it assigns the attributes listed above. *This workflow is highly
     encouraged to ensure that the MetaTransformer is properly instantiated for use with the model module.*
     """
 
-    def __init__(self, metadata, allow_null_transformers, synthesizer) -> None:
+    def __init__(
+        self,
+        metadata,
+        allow_null_transformers=False,
+        synthesizer="TVAE",
+    ) -> None:
         self.allow_null_transformers: bool = allow_null_transformers
         self.Synthesizer: BaseSingleTableSynthesizer = SDV_SYNTHESIZERS[synthesizer]
         self.dtypes: dict[str, dict[str, Any]] = {cn: cd.get("dtype", {}) for cn, cd in metadata.items()}
         self.sdtypes: dict[str, dict[str, Any]] = {
             cn: filter_dict(cd, {"dtype", "transformer"}) for cn, cd in metadata.items()
         }
-        self.transformers: dict[str, BaseTransformer | None] = {cn: get_transformer(cd) for cn, cd in metadata.items()}
+        self.transformers: dict[str, Union[BaseTransformer, None]] = {
+            cn: get_transformer(cd) for cn, cd in metadata.items()
+        }
 
     def apply_dtypes(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Applies dtypes from the metadata to `data` and infers missing dtypes by reading pandas defaults.
 
         Args:
             data: The raw input DataFrame.
@@ -119,29 +126,29 @@
                 f"Incomplete metadata, detecting missing `dtype`s for column(s): {[k for k, v in self.dtypes.items() if not v]} automatically...",
                 UserWarning,
             )
             self.dtypes.update({cn: data[cn].dtype for cn, cv in self.dtypes.items() if not cv})
         return data.astype(self.dtypes)
 
     def _instantiate_ohe_component_transformers(
-        self, transformers: dict[str, BaseTransformer | None]
+        self, transformers: dict[str, Union[BaseTransformer, None]]
     ) -> dict[str, BaseTransformer]:
         """
         Instantiates a OneHotEncoder for each resulting `*.component` column that arises from a ClusterBasedNormalizer.
 
         Args:
             transformers: A dictionary mapping column names to their assigned transformers.
 
         Returns:
             A dictionary mapping each `*.component` column to a OneHotEncoder.
         """
         return {
             f"{cn}.component": OneHotEncoder()
             for cn, transformer in transformers.items()
-            if transformer.get_name() == "ClusterBasedNormalizer"
+            if transformer and transformer.get_name() == "ClusterBasedNormalizer"
         }
 
     def instantiate(self, data: pd.DataFrame) -> BaseSingleTableSynthesizer:
         """
         Instantiates a `self.Synthesizer` object from the given metadata and data. Infers missing metadata (sdtypes and transformers).
 
         Args:
@@ -169,23 +176,23 @@
             warnings.warn(
                 f"Incomplete metadata, detecting missing `transformers`s for column(s): {[k for k, v in self.transformers.items() if not v]} automatically...",
                 UserWarning,
             )
         synthesizer = self.Synthesizer(metadata)
         synthesizer.auto_assign_transformers(data)
         with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
+            warnings.filterwarnings("ignore", message="Replacing the default transformer for column")
             synthesizer.update_transformers(
                 self.transformers if self.allow_null_transformers else {k: v for k, v in self.transformers.items() if v}
             )
         # TODO this is a hacky way to get the component columns we want to apply OneHotEncoder to
         component_transformer = self._instantiate_ohe_component_transformers(synthesizer.get_transformers())
         return synthesizer, component_transformer
 
-    def _get_dtype(self, cn: str) -> str | np.dtype:
+    def _get_dtype(self, cn: str) -> Union[str, np.dtype]:
         """Returns the dtype for the given column name `cn`."""
         return self.dtypes[cn].name if not isinstance(self.dtypes[cn], str) else self.dtypes[cn]
 
     def assemble(self) -> dict[str, dict[str, Any]]:
         """
         Rearranges the dtype, sdtype and transformer metadata into a consistent format ready for output.
 
@@ -251,20 +258,22 @@
                 - Non-one-hotted column indices
         """
         if not self.assembled_metadata:
             self.assembled_metadata = self.assemble()
         onehot_idxs = []
         single_idxs = []
         for cn, cd in self.assembled_metadata.items():
-            if cd["transformer"].get("name") == "OneHotEncoder":
-                onehot_idxs.append(data.columns.get_indexer(data.filter(like=cn + ".value").columns).tolist())
-            elif cd["transformer"].get("name") == "ClusterBasedNormalizer":
-                onehot_idxs.append(data.columns.get_indexer(data.filter(like=cn + ".component.value").columns).tolist())
+            if cd["transformer"] and cd["transformer"].get("name") == "OneHotEncoder":
+                onehot_idxs.append(data.columns.get_indexer(data.filter(regex=f"^{cn}.value").columns).tolist())
+            elif cd["transformer"] and cd["transformer"].get("name") == "ClusterBasedNormalizer":
+                onehot_idxs.append(
+                    data.columns.get_indexer(data.filter(regex=f"^{cn}.component.value").columns).tolist()
+                )
                 single_idxs.append(data.columns.get_loc(cn + ".normalized"))
-            elif cd["transformer"].get("name") != "RegexGenerator":
+            elif not cd["transformer"] or cd["transformer"].get("name") != "RegexGenerator":
                 single_idxs.append(data.columns.get_loc(cn))
         if not onehot_idxs:
             onehot_idxs.append([])
         return onehot_idxs, single_idxs
 
     def apply(self, data: pd.DataFrame) -> pd.DataFrame:
         """
```

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/dataloader/run.py` & `nhssynth-0.3.1/src/nhssynth/modules/dataloader/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     typed_dataset, prepared_dataset = mt.apply(dataset)
 
     write_data_outputs(typed_dataset, prepared_dataset, mt, fn_dataset, fn_metadata, dir_experiment, args)
 
     if "model" in args.modules_to_run:
         args.module_handover.update(
             {
-                "fn_dataset": fn_dataset,
-                "prepared_dataset": prepared_dataset,
+                "dataset": fn_dataset,
+                "prepared": prepared_dataset,
                 "metatransformer": mt,
             }
         )
     if "evaluation" in args.modules_to_run:
-        args.module_handover.update({"typed_dataset": typed_dataset, "sdtypes": mt.get_sdtypes()})
+        args.module_handover.update({"typed": typed_dataset, "sdtypes": mt.get_sdtypes()})
 
     print("")
 
     return args
```

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/evaluation/full_report.py` & `nhssynth-0.3.1/src/nhssynth/modules/evaluation/full_report.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/evaluation/io.py` & `nhssynth-0.3.1/src/nhssynth/modules/evaluation/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     Args:
         args: The arguments passed to the module, in this case potentially carrying the outputs of the dataloader module.
         dir_experiment: The path to the experiment directory.
 
     Returns:
         The data, metadata and metatransformer.
     """
-    if all(x in args.module_handover for x in ["fn_dataset", "typed_dataset", "synthetic", "sdtypes"]):
+    if all(x in args.module_handover for x in ["dataset", "typed", "synthetic", "sdtypes"]):
         return (
-            args.module_handover["fn_dataset"],
-            args.module_handover["typed_dataset"],
+            args.module_handover["dataset"],
+            args.module_handover["typed"],
             args.module_handover["synthetic"],
             args.module_handover["sdtypes"],
         )
     else:
         fn_dataset, fn_typed, fn_synthetic, fn_metadata = check_input_paths(
             args.dataset, args.typed, args.synthetic, args.metadata, dir_experiment
         )
```

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/evaluation/metrics.py` & `nhssynth-0.3.1/src/nhssynth/modules/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/evaluation/run.py` & `nhssynth-0.3.1/src/nhssynth/modules/evaluation/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/model/common/DPMixin.py` & `nhssynth-0.3.1/src/nhssynth/modules/model/common/DPMixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         max_grad_norm: float = 5.0,
         secure_mode: bool = False,
         **kwargs,
     ):
         if not isinstance(self, Model):
             raise TypeError("DPMixin can only be used with Model classes")
         super(DPMixin, self).__init__(*args, **kwargs)
-        self.private: bool = True
         self.target_epsilon: float = target_epsilon
         self.target_delta: float = target_delta or 1 / self.nrows
         self.max_grad_norm: float = max_grad_norm
         self.secure_mode: bool = secure_mode
 
     def make_private(self, num_epochs: int, module: Optional[nn.Module] = None) -> GradSampleModule:
         """
```

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/model/common/Model.py` & `nhssynth-0.3.1/src/nhssynth/modules/model/common/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         assert len(singles) + sum([len(x) for x in onehots]) == self.ncols
         self.data_loader: DataLoader = DataLoader(
             # Should the data also all be turned into floats?
             TensorDataset(torch.Tensor(data.to_numpy())),
             pin_memory=True,
             batch_size=batch_size,
         )
-        self.private: bool = False
         self.setup_device(use_gpu)
 
     def setup_device(self, use_gpu: bool) -> None:
         """Sets up the device to use for training (CPU or GPU) depending on `use_gpu` and device availability."""
         if use_gpu:
             if torch.cuda.is_available():
                 self.device: torch.device = torch.device("cuda:0")
@@ -97,15 +96,15 @@
             **{k: getattr(args, k) for k in ["batch_size", "use_gpu"] + cls._get_args() if getattr(args, k)},
         )
 
     def _start_training(self, num_epochs: int, patience: int, tracked_metrics: list[str]) -> None:
         """Initialises the training process."""
         self.num_epochs = num_epochs
         self.patience = patience
-        if not self.private and "Privacy" in tracked_metrics:
+        if not hasattr(self, "target_epsilon") and "Privacy" in tracked_metrics:
             tracked_metrics.remove("Privacy")
         self.metrics = {metric: np.empty(0, dtype=float) for metric in tracked_metrics}
         self.stats_bars = {
             metric: tqdm(total=0, desc="", position=i, bar_format="{desc}", leave=True)
             for i, metric in enumerate(tracked_metrics)
         }
         self.max_length = max([len(add_spaces_before_caps(s)) + 5 for s in tracked_metrics] + [20])
```

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/model/io.py` & `nhssynth-0.3.1/src/nhssynth/modules/model/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,18 @@
     Args:
         args: The arguments passed to the module, in this case potentially carrying the outputs of the dataloader module.
         dir_experiment: The path to the experiment directory.
 
     Returns:
         The data, metadata and metatransformer.
     """
-    if all(x in args.module_handover for x in ["fn_dataset", "prepared_dataset", "metatransformer"]):
+    if all(x in args.module_handover for x in ["dataset", "prepared", "metatransformer"]):
         return (
-            args.module_handover["fn_dataset"],
-            args.module_handover["prepared_dataset"],
+            args.module_handover["dataset"],
+            args.module_handover["prepared"],
             args.module_handover["metatransformer"],
         )
     else:
         fn_dataset, fn_prepared, fn_metatransformer = check_input_paths(
             args.dataset, args.prepared, args.metatransformer, dir_experiment
         )
```

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/model/models/DPVAE.py` & `nhssynth-0.3.1/src/nhssynth/modules/model/models/DPVAE.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/model/models/VAE.py` & `nhssynth-0.3.1/src/nhssynth/modules/model/models/VAE.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,26 +167,27 @@
         ]
 
     def reconstruct(self, X):
         mu_z, logsigma_z = self.encoder(X)
         x_recon = self.decoder(mu_z)
         return x_recon
 
-    def generate(self, N: Optional[int] = None):
+    def generate(self, N: Optional[int] = None) -> pd.DataFrame:
         N = N or self.nrows
         z_samples = torch.randn_like(torch.ones((N, self.encoder.latent_dim)), device=self.device)
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", message="Using a non-full backward hook")
             x_gen = self.decoder(z_samples)
         x_gen_ = torch.ones_like(x_gen, device=self.device)
 
-        for cat_idxs in self.onehots:
-            x_gen_[:, cat_idxs] = torch.distributions.one_hot_categorical.OneHotCategorical(
-                logits=x_gen[:, cat_idxs]
-            ).sample()
+        if self.onehots != [[]]:
+            for cat_idxs in self.onehots:
+                x_gen_[:, cat_idxs] = torch.distributions.one_hot_categorical.OneHotCategorical(
+                    logits=x_gen[:, cat_idxs]
+                ).sample()
 
         x_gen_[:, self.singles] = x_gen[:, self.singles] + torch.exp(
             self.noiser(x_gen[:, self.singles])
         ) * torch.randn_like(x_gen[:, self.singles])
         if torch.cuda.is_available():
             x_gen_ = x_gen_.cpu()
         return pd.DataFrame(x_gen_.detach(), columns=self.columns)
@@ -201,23 +202,24 @@
 
         s = torch.randn_like(mu_z)
         z_samples = mu_z + s * torch.exp(logsigma_z)
 
         x_recon = self.decoder(z_samples)
 
         categoric_loglik = 0
-        if len(self.onehots):
+
+        if self.onehots != [[]]:
             for cat_idxs in self.onehots:
                 categoric_loglik += -torch.nn.functional.cross_entropy(
                     x_recon[:, cat_idxs],
                     torch.max(X[:, cat_idxs], 1)[1],
                 ).sum()
 
         gauss_loglik = 0
-        if len(self.singles):
+        if self.singles:
             gauss_loglik = (
                 Normal(
                     loc=x_recon[:, self.singles],
                     scale=torch.exp(self.noiser(x_recon[:, self.singles])),
                 )
                 .log_prob(X[:, self.singles])
                 .sum()
```

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/model/run.py` & `nhssynth-0.3.1/src/nhssynth/modules/model/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 
 def run(args: argparse.Namespace) -> argparse.Namespace:
     print("Running model architecture module...")
 
     set_seed(args.seed)
     dir_experiment = experiment_io(args.experiment_name)
+
     synthetic_list = []
     results_list = []
     num_epochs_list = []
     for architecture in args.architecture:
         for i in range(args.repeats):
             print(f"\nModel architecture: {architecture}\nRepeat: {i + 1} of {args.repeats}")
 
-            set_seed((args.seed or 1) + i)
+            set_seed(args.seed + i if args.seed else None)
 
             fn_dataset, prepared_dataset, mt = load_required_data(args, dir_experiment)
             onehots, singles = mt.get_onehots_and_singles()
 
             model = MODELS[architecture].from_args(
                 args=args,
                 data=prepared_dataset,
```

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/plotting/io.py` & `nhssynth-0.3.1/src/nhssynth/modules/plotting/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     Args:
         args: The arguments passed to the module, in this case potentially carrying the outputs of the dataloader module.
         dir_experiment: The path to the experiment directory.
 
     Returns:
         The data, metadata and metatransformer.
     """
-    if all(x in args.module_handover for x in ["fn_dataset", "typed_dataset", "synthetic", "report"]):
+    if all(x in args.module_handover for x in ["dataset", "typed", "synthetic", "report"]):
         return (
-            args.module_handover["fn_dataset"],
-            args.module_handover["typed_dataset"],
+            args.module_handover["dataset"],
+            args.module_handover["typed"],
             args.module_handover["synthetic"],
             args.module_handover["report"],
         )
     else:
         fn_dataset, fn_typed, fn_synthetic, fn_report = check_input_paths(
             args.dataset, args.typed, args.synthetic, args.report, dir_experiment
         )
```

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/plotting/plots.py` & `nhssynth-0.3.1/src/nhssynth/modules/plotting/plots.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/src/nhssynth/modules/plotting/run.py` & `nhssynth-0.3.1/src/nhssynth/modules/plotting/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.3.0/PKG-INFO` & `nhssynth-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhssynth
-Version: 0.3.0
+Version: 0.3.1
 Summary: Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics
 Home-page: https://github.com/nhsx/NHSSynth
 License: MIT
 Keywords: synthetic data,privacy,fairness,machine learning
 Author: HarrisonWilde
 Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU
@@ -29,33 +29,41 @@
 Project-URL: Docs, https://nhsx.github.io/NHSSynth
 Project-URL: Repository, https://github.com/nhsx/NHSSynth
 Description-Content-Type: text/markdown
 
 <!-- PROJECT SHIELDS -->
 <div align="center">
 
-[![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth?style=flat-square)](https://pypi.org/project/nhssynth/)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/nhssynth?style=flat-square)](https://pypi.org/project/nhssynth/)
-[![PyPI - Package Status](https://img.shields.io/pypi/status/nhssynth?style=flat-square)](https://pypi.org/project/nhssynth/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth?style=flat-square)](https://www.python.org/downloads/release/python-3100/)
-[![PyPI - License](https://img.shields.io/pypi/l/nhssynth?style=flat-square)](https://github.com/nhsx/nhssynth/blob/main/LICENSE)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000?style=flat-square)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square)](https://pycqa.github.io/isort/)
+![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/coverage.json)
+![Tests Passing](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/tests.json)
+![Lines of Code](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/loc.json)
+![Percentage Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/comments.json)
+[![Snyk Package Health](https://snyk.io/advisor/python/nhssynth/badge.svg)](https://snyk.io/advisor/python/nhssynth)
 
 </div>
+<div align="center">
+
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)](https://www.python.org/downloads/release/python-3100/)
+[![PyPI - Package Status](https://img.shields.io/pypi/status/nhssynth)](https://pypi.org/project/nhssynth/)
+[![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth)](https://pypi.org/project/nhssynth/)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/nhssynth)](https://pypi.org/project/nhssynth/)
+[![PyPI - License](https://img.shields.io/pypi/l/nhssynth)](https://github.com/nhsx/nhssynth/blob/main/LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1)](https://pycqa.github.io/isort/)
 
+</div>
 
 <!-- PROJECT LOGO -->
 <div align="center">
   <a href="https://nhsx.github.io/NHSSynth">
     <img src="docs/assets/NHS.svg" alt="Logo" width="200" height="100">
   </a>
   <p align="center">
     <a href="https://nhsx.github.io/NHSSynth"><strong>Explore the docs »</strong></a>
-    <br /><br /><br />
+    <br /><br />
   </p>
 </div>
 
 # NHS Synth
 
 ## About
 
@@ -122,17 +130,19 @@
 
 To ensure reproducibility, you should always specify a `--seed` value and provide the `--save-config` flag to dump the exact configuration specified / inferred for the run. This configuration file can then be used in the future to reproduce the exact same run or shared with others to run the same configuration on their dataset, etc.
 
 The figure below shows the structure and workflow of the package and its modules.
 
 ![](docs/modules.png)
 
+View a visualisation of the codebase [here](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=nhsx%2Fnhssynth)!
+
 ### Roadmap
 
-See the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed features (and known issues).
+See the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed features (and known bugs). Our [milestones](https://github.com/nhsx/NHSSynth/milestones) represent longer term goals for the project.
 
 ### Contributing
 
 Any contributions you wish to make are **greatly appreciated**, we encourage you to first raise an issue to discuss with the maintainers. If you are interested in contributing, please follow these steps:
 
 1. Fork the project
 2. Create your branch (`git checkout -b <yourusername>/<featurename>`)
@@ -154,13 +164,13 @@
 
 ### License
 
 Distributed under the MIT License. _See [LICENSE](./LICENSE) for more information._
 
 ### Contact
 
-This project is under active development by [@HarrisonWilde](https://github.com/HarrisonWilde), for any questions or security concerns [contact him](mailto:h.wilde@warwick.ac.uk) or [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose). Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net).
+This project is under active development by [@HarrisonWilde](https://github.com/HarrisonWilde). For feature requests and bugs, please [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose); for security concerns, please open a [draft security advisory](https://github.com/nhsx/NHSSynth/security/advisories/new). Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net).
 
 To find out more about the [Analytics Unit](https://www.nhsx.nhs.uk/key-tools-and-info/nhsx-analytics-unit/) visit our [project website](https://nhsx.github.io/AnalyticsUnit/projects.html) or get in touch at [england.tdau@nhs.net](mailto:england.tdau@nhs.net).
 
 <!-- ### Acknowledgements -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nhssynth Version: 0.3.0 Summary: Synthetic data
+Metadata-Version: 2.1 Name: nhssynth Version: 0.3.1 Summary: Synthetic data
 generation pipeline leveraging a Differentially Private Variational Auto
 Encoder assessed using a variety of metrics Home-page: https://github.com/nhsx/
 NHSSynth License: MIT Keywords: synthetic data,privacy,fairness,machine
 learning Author: HarrisonWilde Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU Maintainer-email: england.tdau@nhs.net Requires-Python:
 >=3.9,<3.11 Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
@@ -12,30 +12,38 @@
 pyyaml (>=6.0,<7.0) Requires-Dist: rdt (>=1.4.0,<2.0.0) Requires-Dist:
 sdmetrics (>=0.9.3,<0.10.0) Requires-Dist: sdv (>=1.0.0,<2.0.0) Requires-Dist:
 setuptools (>=67.6.1,<68.0.0) Requires-Dist: torch (==1.13.1) Requires-Dist:
 tqdm (>=4.65.0,<5.0.0) Project-URL: Bug Tracker, https://github.com/nhsx/
 NHSSynth/issues Project-URL: Docs, https://nhsx.github.io/NHSSynth Project-URL:
 Repository, https://github.com/nhsx/NHSSynth Description-Content-Type: text/
 markdown
- [![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth?style=flat-
-    square)](https://pypi.org/project/nhssynth/) [![PyPI - Wheel](https://
-   img.shields.io/pypi/wheel/nhssynth?style=flat-square)](https://pypi.org/
-   project/nhssynth/) [![PyPI - Package Status](https://img.shields.io/pypi/
-status/nhssynth?style=flat-square)](https://pypi.org/project/nhssynth/) [![PyPI
- - Python Version](https://img.shields.io/pypi/pyversions/nhssynth?style=flat-
-   square)](https://www.python.org/downloads/release/python-3100/) [![PyPI -
- License](https://img.shields.io/pypi/l/nhssynth?style=flat-square)](https://
-  github.com/nhsx/nhssynth/blob/main/LICENSE) [![Code style: black](https://
-  img.shields.io/badge/code%20style-black-000000?style=flat-square)](https://
-    github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/
-%20imports-isort-%231674b1?style=flat-square)](https://pycqa.github.io/isort/)
+           ![Coverage](https://img.shields.io/endpoint?url=https://
+gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
+ coverage.json) ![Tests Passing](https://img.shields.io/endpoint?url=https://
+gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
+   tests.json) ![Lines of Code](https://img.shields.io/endpoint?url=https://
+gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
+ loc.json) ![Percentage Comments](https://img.shields.io/endpoint?url=https://
+gist.githubusercontent.com/HarrisonWilde/1ab4eefed81ec381e29f7d4feb9856bc/raw/
+comments.json) [![Snyk Package Health](https://snyk.io/advisor/python/nhssynth/
+             badge.svg)](https://snyk.io/advisor/python/nhssynth)
+  [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nhssynth)]
+   (https://www.python.org/downloads/release/python-3100/) [![PyPI - Package
+Status](https://img.shields.io/pypi/status/nhssynth)](https://pypi.org/project/
+ nhssynth/) [![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth)]
+ (https://pypi.org/project/nhssynth/) [![PyPI - Wheel](https://img.shields.io/
+ pypi/wheel/nhssynth)](https://pypi.org/project/nhssynth/) [![PyPI - License]
+  (https://img.shields.io/pypi/l/nhssynth)](https://github.com/nhsx/nhssynth/
+    blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/
+ code%20style-black-000000)](https://github.com/psf/black) [![Imports: isort]
+      (https://img.shields.io/badge/%20imports-isort-%231674b1)](https://
+                            pycqa.github.io/isort/)
                                     [Logo]
                              Explore_the_docs_Â»
 
-
 # NHS Synth ## About This repository currently consists of a Python package
 alongside research and investigative materials covering the effectiveness of
 the package and synthetic data more generally when applied to NHS use cases.
 See the internal [project description](https://nhsx.github.io/nhsx-internship-
 projects/synthetic-data-exploration-vae/) for more information. _**Note:** No
 data, public or private are shared in this repository._ ## Getting Started ###
 Project Structure - The main package and codebase is found in [`src/nhssynth`]
@@ -89,31 +97,35 @@
 override any of the arguments provided in the configuration file by passing
 them as arguments in the command line. To ensure reproducibility, you should
 always specify a `--seed` value and provide the `--save-config` flag to dump
 the exact configuration specified / inferred for the run. This configuration
 file can then be used in the future to reproduce the exact same run or shared
 with others to run the same configuration on their dataset, etc. The figure
 below shows the structure and workflow of the package and its modules. ![]
-(docs/modules.png) ### Roadmap See the [open issues](https://github.com/nhsx/
-NHSSynth/issues) for a list of proposed features (and known issues). ###
+(docs/modules.png) View a visualisation of the codebase [here](https://mango-
+dune-07a8b7110.1.azurestaticapps.net/?repo=nhsx%2Fnhssynth)! ### Roadmap See
+the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of
+proposed features (and known bugs). Our [milestones](https://github.com/nhsx/
+NHSSynth/milestones) represent longer term goals for the project. ###
 Contributing Any contributions you wish to make are **greatly appreciated**, we
 encourage you to first raise an issue to discuss with the maintainers. If you
 are interested in contributing, please follow these steps: 1. Fork the project
 2. Create your branch (`git checkout -b /`) 3. Commit your changes (`git commit
 -m 'Add some amazing feature'`) 4. Push to the branch (`git push origin /`) 5.
 Open a PR and we will try to get it merged! _See [CONTRIBUTING.md](./
 CONTRIBUTING.md) for detailed guidance._ Thanks to everyone that has
 contributed so far!
                [https://contrib.rocks/image?repo=nhsx/nhssynth]
 This codebase builds on previous NHSX Analytics Unit PhD internships
 contextualising and investigating the potential use of Variational Auto
 Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic
 Danks and David Brind. ### License Distributed under the MIT License. _See
 [LICENSE](./LICENSE) for more information._ ### Contact This project is under
-active development by [@HarrisonWilde](https://github.com/HarrisonWilde), for
-any questions or security concerns [contact him](mailto:h.wilde@warwick.ac.uk)
-or [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose).
+active development by [@HarrisonWilde](https://github.com/HarrisonWilde). For
+feature requests and bugs, please [raise an issue](https://github.com/nhsx/
+NHSSynth/issues/new/choose); for security concerns, please open a [draft
+security advisory](https://github.com/nhsx/NHSSynth/security/advisories/new).
 Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net). To find
 out more about the [Analytics Unit](https://www.nhsx.nhs.uk/key-tools-and-info/
 nhsx-analytics-unit/) visit our [project website](https://nhsx.github.io/
 AnalyticsUnit/projects.html) or get in touch at [england.tdau@nhs.net](mailto:
 england.tdau@nhs.net).
```

