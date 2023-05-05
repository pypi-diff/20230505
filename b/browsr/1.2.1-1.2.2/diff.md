# Comparing `tmp/browsr-1.2.1.tar.gz` & `tmp/browsr-1.2.2.tar.gz`

## Comparing `browsr-1.2.1.tar` & `browsr-1.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.2.1/.releaserc.js
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.2.1/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/__main__.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/_base.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/_version.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/code_browser.css
--rw-r--r--   0        0        0    11980 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/code_browser.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.2.1/docs/api_documentation.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.2.1/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.2.1/docs/contributing.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.2.1/docs/index.md
--rw-r--r--   0        0        0   115582 2020-02-02 00:00:00.000000 browsr-1.2.1/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    79896 2020-02-02 00:00:00.000000 browsr-1.2.1/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.2.1/tests/conftest.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 browsr-1.2.1/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.2.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.2.1/README.md
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 browsr-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 browsr-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.2.2/.releaserc.js
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.2.2/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/__main__.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/_base.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/_version.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/code_browser.css
+-rw-r--r--   0        0        0    11980 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/code_browser.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.2.2/docs/api_documentation.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.2.2/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.2.2/docs/contributing.md
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.2.2/docs/index.md
+-rw-r--r--   0        0        0   115617 2020-02-02 00:00:00.000000 browsr-1.2.2/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    79931 2020-02-02 00:00:00.000000 browsr-1.2.2/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.2.2/tests/conftest.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 browsr-1.2.2/tests/test_cli.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.2.2/README.md
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 browsr-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 browsr-1.2.2/PKG-INFO
```

### Comparing `browsr-1.2.1/.pre-commit-config.yaml` & `browsr-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/.releaserc.js` & `browsr-1.2.2/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/mkdocs.yaml` & `browsr-1.2.2/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/.github/semantic_release/package-lock.json` & `browsr-1.2.2/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/.github/semantic_release/release_notes.hbs` & `browsr-1.2.2/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/.github/workflows/lint.yaml` & `browsr-1.2.2/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/.github/workflows/publish.yaml` & `browsr-1.2.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/.github/workflows/release.yaml` & `browsr-1.2.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/.github/workflows/tests.yaml` & `browsr-1.2.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/browsr/_base.py` & `browsr-1.2.2/browsr/_base.py`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/browsr/code_browser.py` & `browsr-1.2.2/browsr/code_browser.py`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/docs/contributing.md` & `browsr-1.2.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/docs/index.md` & `browsr-1.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/requirements/requirements-dev.txt` & `browsr-1.2.2/requirements/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1065,15 +1065,17 @@
     --hash=sha256:d9c206c29b46cfd343ea7cdfe1232443072bbb270d6a46f59c259460db76779a \
     --hash=sha256:e49eb4e95ff6fd7c0c402508894b1ef0e01b99a44320ba7d8ecbabefddcc5569 \
     --hash=sha256:f8286396b351785801a976b1e85ea88e937712ee2c3ac653710a4a57a8da5d9c \
     --hash=sha256:f8fc330c3370a81bbf3f88557097d1ea26cd8b019d6433aa59f71195f5ddebbf \
     --hash=sha256:fbd359831c1657d69bb81f0db962905ee05e5e9451913b18b831febfe0519082 \
     --hash=sha256:fe7e1c262d3392afcf5071df9afa574544f28eac825284596ac6db56e6d11062 \
     --hash=sha256:fed1e1cf6a42577953abbe8e6cf2fe2f566daebde7c34724ec8803c4c0cda579
-    # via rich-pixels
+    # via
+    #   -r requirements.in
+    #   rich-pixels
 pip-tools==6.13.0 \
     --hash=sha256:50943f151d87e752abddec8158622c34ad7f292e193836e90e30d87da60b19d9 \
     --hash=sha256:61d46bd2eb8016ed4a924e196e6e5b0a268cd3babd79e593048720db23522bb1
     # via -r requirements.in
 platformdirs==3.5.0 \
     --hash=sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4 \
     --hash=sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335
```

### Comparing `browsr-1.2.1/requirements/requirements-prod.txt` & `browsr-1.2.2/requirements/requirements-prod.txt`

 * *Files 0% similar despite different names*

```diff
@@ -793,15 +793,17 @@
     --hash=sha256:d9c206c29b46cfd343ea7cdfe1232443072bbb270d6a46f59c259460db76779a \
     --hash=sha256:e49eb4e95ff6fd7c0c402508894b1ef0e01b99a44320ba7d8ecbabefddcc5569 \
     --hash=sha256:f8286396b351785801a976b1e85ea88e937712ee2c3ac653710a4a57a8da5d9c \
     --hash=sha256:f8fc330c3370a81bbf3f88557097d1ea26cd8b019d6433aa59f71195f5ddebbf \
     --hash=sha256:fbd359831c1657d69bb81f0db962905ee05e5e9451913b18b831febfe0519082 \
     --hash=sha256:fe7e1c262d3392afcf5071df9afa574544f28eac825284596ac6db56e6d11062 \
     --hash=sha256:fed1e1cf6a42577953abbe8e6cf2fe2f566daebde7c34724ec8803c4c0cda579
-    # via rich-pixels
+    # via
+    #   -r requirements.in
+    #   rich-pixels
 portalocker==2.7.0 \
     --hash=sha256:032e81d534a88ec1736d03f780ba073f047a06c478b06e2937486f334e955c51 \
     --hash=sha256:a07c5b4f3985c3cf4798369631fb7011adb498e2a46d8440efc75a8f29a0f983
     # via msal-extensions
 protobuf==4.22.3 \
     --hash=sha256:13233ee2b9d3bd9a5f216c1fa2c321cd564b93d8f2e4f521a85b585447747997 \
     --hash=sha256:23452f2fdea754a8251d0fc88c0317735ae47217e0d27bf330a30eec2848811a \
```

### Comparing `browsr-1.2.1/.gitignore` & `browsr-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/LICENSE.txt` & `browsr-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/README.md` & `browsr-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `browsr-1.2.1/pyproject.toml` & `browsr-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
   "click~=8.1.3",
   "fsspec~=2023.1.0",
   "pandas~=1.5.2",
   "rich~=13.3.5",
   "rich-click~=1.5.2",
   "rich-pixels~=2.1.1",
   "textual~=0.22.3",
-  "universal-pathlib~=0.0.21"
+  "universal-pathlib~=0.0.21",
+  "Pillow>=9.1.0"
 ]
 description = "TUI File Browser App"
 dynamic = ["version"]
 keywords = []
 license = "MIT"
 name = "browsr"
 readme = "README.md"
```

### Comparing `browsr-1.2.1/PKG-INFO` & `browsr-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.2.1
+Version: 1.2.2
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4.0,>=3.8
 Requires-Dist: art~=5.7
 Requires-Dist: click~=8.1.3
 Requires-Dist: fsspec~=2023.1.0
 Requires-Dist: pandas~=1.5.2
+Requires-Dist: pillow>=9.1.0
 Requires-Dist: rich-click~=1.5.2
 Requires-Dist: rich-pixels~=2.1.1
 Requires-Dist: rich~=13.3.5
 Requires-Dist: textual~=0.22.3
 Requires-Dist: universal-pathlib~=0.0.21
 Provides-Extra: all
 Requires-Dist: adlfs~=2023.1.0; extra == 'all'
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.2.1 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.2.2 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
 flannery@juftin.com> License-Expression: MIT License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: <4.0,>=3.8 Requires-Dist: art~=5.7 Requires-Dist: click~=8.1.3
 Requires-Dist: fsspec~=2023.1.0 Requires-Dist: pandas~=1.5.2 Requires-Dist:
-rich-click~=1.5.2 Requires-Dist: rich-pixels~=2.1.1 Requires-Dist: rich~=13.3.5
-Requires-Dist: textual~=0.22.3 Requires-Dist: universal-pathlib~=0.0.21
-Provides-Extra: all Requires-Dist: adlfs~=2023.1.0; extra == 'all' Requires-
-Dist: aiohttp~=3.8.3; extra == 'all' Requires-Dist: gcsfs~=2023.1.0; extra ==
-'all' Requires-Dist: pyarrow~=10.0.0; extra == 'all' Requires-Dist:
-requests~=2.28.2; extra == 'all' Requires-Dist: s3fs~=2023.1.0; extra == 'all'
-Provides-Extra: parquet Requires-Dist: pyarrow~=10.0.0; extra == 'parquet'
-Provides-Extra: remote Requires-Dist: adlfs~=2023.1.0; extra == 'remote'
-Requires-Dist: aiohttp~=3.8.3; extra == 'remote' Requires-Dist:
-gcsfs~=2023.1.0; extra == 'remote' Requires-Dist: requests~=2.28.2; extra ==
-'remote' Requires-Dist: s3fs~=2023.1.0; extra == 'remote' Description-Content-
-Type: text/markdown # browsr
+pillow>=9.1.0 Requires-Dist: rich-click~=1.5.2 Requires-Dist: rich-
+pixels~=2.1.1 Requires-Dist: rich~=13.3.5 Requires-Dist: textual~=0.22.3
+Requires-Dist: universal-pathlib~=0.0.21 Provides-Extra: all Requires-Dist:
+adlfs~=2023.1.0; extra == 'all' Requires-Dist: aiohttp~=3.8.3; extra == 'all'
+Requires-Dist: gcsfs~=2023.1.0; extra == 'all' Requires-Dist: pyarrow~=10.0.0;
+extra == 'all' Requires-Dist: requests~=2.28.2; extra == 'all' Requires-Dist:
+s3fs~=2023.1.0; extra == 'all' Provides-Extra: parquet Requires-Dist:
+pyarrow~=10.0.0; extra == 'parquet' Provides-Extra: remote Requires-Dist:
+adlfs~=2023.1.0; extra == 'remote' Requires-Dist: aiohttp~=3.8.3; extra ==
+'remote' Requires-Dist: gcsfs~=2023.1.0; extra == 'remote' Requires-Dist:
+requests~=2.28.2; extra == 'remote' Requires-Dist: s3fs~=2023.1.0; extra ==
+'remote' Description-Content-Type: text/markdown # browsr
                                    [browsr]
 [![browsr Version](https://img.shields.io/pypi/v/
 browsr?color=blue&label=browsr)](https://github.com/juftin/browsr) [![PyPI]
 (https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/
 browsr/) [![Testing Status](https://github.com/juftin/browsr/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
```

