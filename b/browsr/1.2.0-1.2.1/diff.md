# Comparing `tmp/browsr-1.2.0.tar.gz` & `tmp/browsr-1.2.1.tar.gz`

## Comparing `browsr-1.2.0.tar` & `browsr-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.2.0/.releaserc.js
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.2.0/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.2.0/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.2.0/browsr/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 browsr-1.2.0/browsr/__main__.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 browsr-1.2.0/browsr/_base.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.2.0/browsr/_version.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 browsr-1.2.0/browsr/code_browser.css
--rw-r--r--   0        0        0    11864 2020-02-02 00:00:00.000000 browsr-1.2.0/browsr/code_browser.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.2.0/docs/api_documentation.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.2.0/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.2.0/docs/contributing.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.2.0/docs/index.md
--rw-r--r--   0        0        0   115582 2020-02-02 00:00:00.000000 browsr-1.2.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    79896 2020-02-02 00:00:00.000000 browsr-1.2.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 browsr-1.2.0/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.2.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.2.0/README.md
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 browsr-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 browsr-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.2.1/.releaserc.js
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.2.1/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.2.1/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/__main__.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/_base.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/_version.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/code_browser.css
+-rw-r--r--   0        0        0    11980 2020-02-02 00:00:00.000000 browsr-1.2.1/browsr/code_browser.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.2.1/docs/api_documentation.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.2.1/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.2.1/docs/contributing.md
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.2.1/docs/index.md
+-rw-r--r--   0        0        0   115582 2020-02-02 00:00:00.000000 browsr-1.2.1/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    79896 2020-02-02 00:00:00.000000 browsr-1.2.1/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 browsr-1.2.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.2.1/README.md
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 browsr-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 browsr-1.2.1/PKG-INFO
```

### Comparing `browsr-1.2.0/.pre-commit-config.yaml` & `browsr-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/.releaserc.js` & `browsr-1.2.1/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/mkdocs.yaml` & `browsr-1.2.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/.github/semantic_release/package-lock.json` & `browsr-1.2.1/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/.github/semantic_release/release_notes.hbs` & `browsr-1.2.1/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/.github/workflows/lint.yaml` & `browsr-1.2.1/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/.github/workflows/publish.yaml` & `browsr-1.2.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/.github/workflows/release.yaml` & `browsr-1.2.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/.github/workflows/tests.yaml` & `browsr-1.2.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/browsr/_base.py` & `browsr-1.2.1/browsr/_base.py`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/browsr/code_browser.py` & `browsr-1.2.1/browsr/code_browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-Code browser example.
+Browsr TUI App
 
-Run with:
-    python code_browser.py PATH
+This module contains the code browser app for the browsr package.
+This app was inspired by the CodeBrowser example from textual
 """
 
 import json
 import pathlib
 from os import getenv
 from typing import TYPE_CHECKING, Any, Iterable, List, Optional, Union
 
@@ -154,15 +154,16 @@
             df = pd.read_csv(document, nrows=500)
             return self.df_to_table(pandas_dataframe=df, table=self.table_view)
         elif document.suffix == ".parquet":
             df = pd.read_parquet(document)[:500]
             return self.df_to_table(pandas_dataframe=df, table=self.table_view)
         elif document.suffix.lower() in [".png", ".jpg", ".jpeg"]:
             screen_width = self.app.size.width / 4
-            with Image.open(document) as image:
+            with document.open("rb") as buf:
+                image = Image.open(buf)
                 image_width = image.width
                 image_height = image.height
                 size_ratio = image_width / screen_width
                 new_width = min(int(image_width / size_ratio), image_width)
                 new_height = min(int(image_height / size_ratio), image_height)
                 resized = image.resize((new_width, new_height))
                 content = rich_pixels.Pixels.from_image(resized)
```

### Comparing `browsr-1.2.0/docs/contributing.md` & `browsr-1.2.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/docs/index.md` & `browsr-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/requirements/requirements-dev.txt` & `browsr-1.2.1/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/requirements/requirements-prod.txt` & `browsr-1.2.1/requirements/requirements-prod.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/.gitignore` & `browsr-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/LICENSE.txt` & `browsr-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/README.md` & `browsr-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/pyproject.toml` & `browsr-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.0/PKG-INFO` & `browsr-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.2.0
+Version: 1.2.1
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.2.0 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.2.1 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
 flannery@juftin.com> License-Expression: MIT License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

