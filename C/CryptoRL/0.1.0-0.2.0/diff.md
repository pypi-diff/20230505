# Comparing `tmp/CryptoRL-0.1.0.tar.gz` & `tmp/CryptoRL-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CryptoRL-0.1.0.tar", last modified: Wed Mar 22 23:57:49 2023, max compression
+gzip compressed data, was "CryptoRL-0.2.0.tar", last modified: Fri May  5 01:50:42 2023, max compression
```

## Comparing `CryptoRL-0.1.0.tar` & `CryptoRL-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,46 @@
-drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-03-22 23:57:49.119371 CryptoRL-0.1.0/
-drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-03-22 23:57:49.107495 CryptoRL-0.1.0/.github/
-drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-03-22 23:57:49.112232 CryptoRL-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 joey       (501) staff       (20)      834 2023-03-11 18:54:23.000000 CryptoRL-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 joey       (501) staff       (20)      126 2023-03-11 18:54:23.000000 CryptoRL-0.1.0/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 joey       (501) staff       (20)      595 2023-03-11 18:54:23.000000 CryptoRL-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-03-22 23:57:49.112635 CryptoRL-0.1.0/.github/workflows/
--rw-r--r--   0 joey       (501) staff       (20)     1154 2023-03-11 18:59:14.000000 CryptoRL-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 joey       (501) staff       (20)     1799 2023-03-11 17:46:11.000000 CryptoRL-0.1.0/.gitignore
--rw-r--r--   0 joey       (501) staff       (20)      639 2023-03-22 23:47:49.000000 CryptoRL-0.1.0/CONTRIBUTING.md
-drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-03-22 23:57:49.115257 CryptoRL-0.1.0/CryptoRL.egg-info/
--rw-r--r--   0 joey       (501) staff       (20)     2998 2023-03-22 23:57:49.000000 CryptoRL-0.1.0/CryptoRL.egg-info/PKG-INFO
--rw-r--r--   0 joey       (501) staff       (20)      500 2023-03-22 23:57:49.000000 CryptoRL-0.1.0/CryptoRL.egg-info/SOURCES.txt
--rw-r--r--   0 joey       (501) staff       (20)        1 2023-03-22 23:57:49.000000 CryptoRL-0.1.0/CryptoRL.egg-info/dependency_links.txt
--rw-r--r--   0 joey       (501) staff       (20)      189 2023-03-22 23:57:49.000000 CryptoRL-0.1.0/CryptoRL.egg-info/requires.txt
--rw-r--r--   0 joey       (501) staff       (20)        9 2023-03-22 23:57:49.000000 CryptoRL-0.1.0/CryptoRL.egg-info/top_level.txt
--rw-r--r--   0 joey       (501) staff       (20)     1065 2023-02-19 02:51:31.000000 CryptoRL-0.1.0/LICENSE
--rw-r--r--   0 joey       (501) staff       (20)     2230 2023-03-11 18:54:23.000000 CryptoRL-0.1.0/Makefile
--rw-r--r--   0 joey       (501) staff       (20)     2998 2023-03-22 23:57:49.119021 CryptoRL-0.1.0/PKG-INFO
--rw-r--r--   0 joey       (501) staff       (20)      892 2023-03-22 23:47:49.000000 CryptoRL-0.1.0/README.md
-drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-03-22 23:57:49.117223 CryptoRL-0.1.0/cryptorl/
--rw-r--r--   0 joey       (501) staff       (20)       91 2023-03-22 23:47:49.000000 CryptoRL-0.1.0/cryptorl/__init__.py
--rw-r--r--   0 joey       (501) staff       (20)     2808 2023-03-22 23:47:49.000000 CryptoRL-0.1.0/cryptorl/data.py
--rw-r--r--   0 joey       (501) staff       (20)      310 2023-03-22 23:47:49.000000 CryptoRL-0.1.0/cryptorl/env_crypto.py
-drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-03-22 23:57:49.118302 CryptoRL-0.1.0/cryptorl/tests/
--rw-r--r--   0 joey       (501) staff       (20)      369 2023-03-11 18:59:14.000000 CryptoRL-0.1.0/cryptorl/tests/integration_test.py
--rw-r--r--   0 joey       (501) staff       (20)     1199 2023-03-11 18:59:14.000000 CryptoRL-0.1.0/cryptorl/tests/unit_test.py
--rw-r--r--   0 joey       (501) staff       (20)     2312 2023-03-22 23:47:49.000000 CryptoRL-0.1.0/pyproject.toml
--rw-r--r--   0 joey       (501) staff       (20)       38 2023-03-22 23:57:49.119837 CryptoRL-0.1.0/setup.cfg
--rw-rw-r--   0 joey       (501) staff       (20)       39 2023-02-16 17:05:04.000000 CryptoRL-0.1.0/setup.py
+drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-05-05 01:50:42.798951 CryptoRL-0.2.0/
+drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-05-05 01:50:42.786726 CryptoRL-0.2.0/.github/
+drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-05-05 01:50:42.788565 CryptoRL-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 joey       (501) staff       (20)      834 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 joey       (501) staff       (20)      126 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 joey       (501) staff       (20)      595 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 joey       (501) staff       (20)      118 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-05-05 01:50:42.789133 CryptoRL-0.2.0/.github/workflows/
+-rw-r--r--   0 joey       (501) staff       (20)     1154 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 joey       (501) staff       (20)     1885 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/.gitignore
+-rw-r--r--   0 joey       (501) staff       (20)      255 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 joey       (501) staff       (20)      639 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/CONTRIBUTING.md
+drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-05-05 01:50:42.791290 CryptoRL-0.2.0/CryptoRL.egg-info/
+-rw-r--r--   0 joey       (501) staff       (20)     3501 2023-05-05 01:50:42.000000 CryptoRL-0.2.0/CryptoRL.egg-info/PKG-INFO
+-rw-r--r--   0 joey       (501) staff       (20)      779 2023-05-05 01:50:42.000000 CryptoRL-0.2.0/CryptoRL.egg-info/SOURCES.txt
+-rw-r--r--   0 joey       (501) staff       (20)        1 2023-05-05 01:50:42.000000 CryptoRL-0.2.0/CryptoRL.egg-info/dependency_links.txt
+-rw-r--r--   0 joey       (501) staff       (20)      236 2023-05-05 01:50:42.000000 CryptoRL-0.2.0/CryptoRL.egg-info/requires.txt
+-rw-r--r--   0 joey       (501) staff       (20)        9 2023-05-05 01:50:42.000000 CryptoRL-0.2.0/CryptoRL.egg-info/top_level.txt
+-rw-r--r--   0 joey       (501) staff       (20)     1065 2023-02-19 02:51:31.000000 CryptoRL-0.2.0/LICENSE
+-rw-r--r--   0 joey       (501) staff       (20)     2230 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/Makefile
+-rw-r--r--   0 joey       (501) staff       (20)     3501 2023-05-05 01:50:42.798687 CryptoRL-0.2.0/PKG-INFO
+-rw-r--r--   0 joey       (501) staff       (20)     1396 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/README.md
+drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-05-05 01:50:42.794107 CryptoRL-0.2.0/cryptorl/
+-rw-r--r--   0 joey       (501) staff       (20)      305 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/cryptorl/__init__.py
+-rw-r--r--   0 joey       (501) staff       (20)     5330 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/cryptorl/data.py
+-rw-r--r--   0 joey       (501) staff       (20)      612 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/cryptorl/env_crypto.py
+-rw-r--r--   0 joey       (501) staff       (20)     2434 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/cryptorl/predict_DT.py
+-rw-r--r--   0 joey       (501) staff       (20)     1817 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/cryptorl/predict_LR.py
+-rw-r--r--   0 joey       (501) staff       (20)     1491 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/cryptorl/predict_NN.py
+drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-05-05 01:50:42.794921 CryptoRL-0.2.0/cryptorl/tests/
+-rw-r--r--   0 joey       (501) staff       (20)      369 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/cryptorl/tests/integration_test.py
+-rw-r--r--   0 joey       (501) staff       (20)     3043 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/cryptorl/tests/unit_test.py
+-rw-r--r--   0 joey       (501) staff       (20)     1489 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/cryptorl/utils.py
+drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-05-05 01:50:42.797386 CryptoRL-0.2.0/docs/
+-rw-r--r--   0 joey       (501) staff       (20)      634 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/docs/Makefile
+-rw-r--r--   0 joey       (501) staff       (20)     2156 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/docs/conf.py
+-rw-r--r--   0 joey       (501) staff       (20)      959 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/docs/index.rst
+-rw-r--r--   0 joey       (501) staff       (20)      800 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/docs/make.bat
+-rw-r--r--   0 joey       (501) staff       (20)       70 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 joey       (501) staff       (20)        0 2023-05-05 01:50:42.798316 CryptoRL-0.2.0/docs/source/
+-rw-r--r--   0 joey       (501) staff       (20)     1022 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/docs/source/cryptorl.rst
+-rw-r--r--   0 joey       (501) staff       (20)     1405 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/docs/source/example.rst
+-rw-r--r--   0 joey       (501) staff       (20)       61 2023-05-04 21:23:43.000000 CryptoRL-0.2.0/docs/source/modules.rst
+-rw-r--r--   0 joey       (501) staff       (20)     2454 2023-05-05 01:45:25.000000 CryptoRL-0.2.0/pyproject.toml
+-rw-r--r--   0 joey       (501) staff       (20)       38 2023-05-05 01:50:42.799030 CryptoRL-0.2.0/setup.cfg
+-rw-rw-r--   0 joey       (501) staff       (20)       39 2023-02-16 17:05:04.000000 CryptoRL-0.2.0/setup.py
```

### Comparing `CryptoRL-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `CryptoRL-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `CryptoRL-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `CryptoRL-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `CryptoRL-0.1.0/.github/workflows/build.yml` & `CryptoRL-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `CryptoRL-0.1.0/.gitignore` & `CryptoRL-0.2.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -123,7 +123,16 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# Docs generated files
+docs/_build
+docs/_static
+docs/_templates
+
+# 
+.DS_Store
+.vscode
```

### Comparing `CryptoRL-0.1.0/CONTRIBUTING.md` & `CryptoRL-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `CryptoRL-0.1.0/CryptoRL.egg-info/PKG-INFO` & `CryptoRL-0.2.0/CryptoRL.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CryptoRL
-Version: 0.1.0
+Version: 0.2.0
 Summary: Fetching time series data of cryptocurrencies and using ML and RL to do cryptocurrency trading.
 Author-email: Ziyi Xia <zx2325@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Ziyi Xia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,24 +39,40 @@
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # CryptoRL
 Fetching time series data of cryptocurrencies and using ML and RL to do cryptocurrency trading.
 
-<img src="https://img.shields.io/github/license/ZiyiXia/CryptoRL" alt="CryptoRL MIT License"/>
-<img src="https://img.shields.io/github/issues/ZiyiXia/CryptoRL" alt="Issue"/>
-<img src="https://img.shields.io/github/actions/workflow/status/ZiyiXia/CryptoRL/build.yml?label=build%20status&logo=github" alt="built status">
-<img src="https://img.shields.io/codecov/c/github/ZiyiXia/CryptoRL?logo=codecov" alt="codecov">
+[![License: MIT](https://img.shields.io/github/license/ZiyiXia/CryptoRL)](https://opensource.org/licenses/MIT)
+
+[![GitHub Issue](https://img.shields.io/github/issues/ZiyiXia/CryptoRL)](https://github.com/ZiyiXia/CryptoRL/issues)
+
+[![PyPI](https://img.shields.io/pypi/v/CryptoRL)](https://pypi.org/project/CryptoRL/)
+
+![](https://img.shields.io/github/actions/workflow/status/ZiyiXia/CryptoRL/build.yml?label=build%20status&logo=github)
+
+[![codecov](https://img.shields.io/codecov/c/github/ZiyiXia/CryptoRL?logo=codecov)](https://app.codecov.io/gh/ZiyiXia/CryptoRL)
+
+[![docs](https://img.shields.io/readthedocs/cryptorl)](https://cryptorl.readthedocs.io)
+
 
 ## Overview
 CryptoRL will use popular deep reinforcement learning algorithms and machine learning algorithms to do cryptocurrency trading.
 
 ## Installation
 
 Run ```pip install cryptorl``` to install CryptoRL.
 
-## Usage
+## Getting started
 
 To fetch data, please use the functions in *data.py*.
 
+For example:
+
+```fetch_single('2020-01-01', '2022-01-01', 'aapl')```
+
+will return a DataFrame object that containing the cleaned data with required ticker and range of dates.
+
 With well processed data, you can use *env_crypto.py* to construct crypto market environment.
+
+Read the [documentation](https://cryptorl.readthedocs.io) for more details.
```

### Comparing `CryptoRL-0.1.0/LICENSE` & `CryptoRL-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CryptoRL-0.1.0/Makefile` & `CryptoRL-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `CryptoRL-0.1.0/PKG-INFO` & `CryptoRL-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CryptoRL
-Version: 0.1.0
+Version: 0.2.0
 Summary: Fetching time series data of cryptocurrencies and using ML and RL to do cryptocurrency trading.
 Author-email: Ziyi Xia <zx2325@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Ziyi Xia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,24 +39,40 @@
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # CryptoRL
 Fetching time series data of cryptocurrencies and using ML and RL to do cryptocurrency trading.
 
-<img src="https://img.shields.io/github/license/ZiyiXia/CryptoRL" alt="CryptoRL MIT License"/>
-<img src="https://img.shields.io/github/issues/ZiyiXia/CryptoRL" alt="Issue"/>
-<img src="https://img.shields.io/github/actions/workflow/status/ZiyiXia/CryptoRL/build.yml?label=build%20status&logo=github" alt="built status">
-<img src="https://img.shields.io/codecov/c/github/ZiyiXia/CryptoRL?logo=codecov" alt="codecov">
+[![License: MIT](https://img.shields.io/github/license/ZiyiXia/CryptoRL)](https://opensource.org/licenses/MIT)
+
+[![GitHub Issue](https://img.shields.io/github/issues/ZiyiXia/CryptoRL)](https://github.com/ZiyiXia/CryptoRL/issues)
+
+[![PyPI](https://img.shields.io/pypi/v/CryptoRL)](https://pypi.org/project/CryptoRL/)
+
+![](https://img.shields.io/github/actions/workflow/status/ZiyiXia/CryptoRL/build.yml?label=build%20status&logo=github)
+
+[![codecov](https://img.shields.io/codecov/c/github/ZiyiXia/CryptoRL?logo=codecov)](https://app.codecov.io/gh/ZiyiXia/CryptoRL)
+
+[![docs](https://img.shields.io/readthedocs/cryptorl)](https://cryptorl.readthedocs.io)
+
 
 ## Overview
 CryptoRL will use popular deep reinforcement learning algorithms and machine learning algorithms to do cryptocurrency trading.
 
 ## Installation
 
 Run ```pip install cryptorl``` to install CryptoRL.
 
-## Usage
+## Getting started
 
 To fetch data, please use the functions in *data.py*.
 
+For example:
+
+```fetch_single('2020-01-01', '2022-01-01', 'aapl')```
+
+will return a DataFrame object that containing the cleaned data with required ticker and range of dates.
+
 With well processed data, you can use *env_crypto.py* to construct crypto market environment.
+
+Read the [documentation](https://cryptorl.readthedocs.io) for more details.
```

### Comparing `CryptoRL-0.1.0/pyproject.toml` & `CryptoRL-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "CryptoRL"
 authors = [{name = "Ziyi Xia", email = "zx2325@columbia.edu"}]
 description="Fetching time series data of cryptocurrencies and using ML and RL to do cryptocurrency trading."
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -47,27 +47,35 @@
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "twine",
     "wheel",
     "numpy",
     "pandas",
     "gym",
+    "tensorflow",
+    "scikit-learn",
+    "matplotlib",
+    "yfinance",
+    "ta",
     "Historic-Crypto",
 ]
 
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
 
 [tool.check-manifest]
 ignore = [
     "Makefile",
-    "CONTRIBUTING.md"
+    "CONTRIBUTING.md",
+    "docs/*",
+    "docs/source/*",
+    ".readthedocs.yaml"
 ]
 
 [tool.flake8]
 ignore = ['E203', 'W503']
 max-line-length=120
 exclude=[
     'cryptorl/tests/*',
```

