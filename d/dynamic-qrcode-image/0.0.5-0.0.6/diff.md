# Comparing `tmp/dynamic_qrcode_image-0.0.5.tar.gz` & `tmp/dynamic_qrcode_image-0.0.6.tar.gz`

## Comparing `dynamic_qrcode_image-0.0.5.tar` & `dynamic_qrcode_image-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/__main__.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/config.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/form.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/qr2.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/qrc.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/w2.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/docs/generate.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/docs/index.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/templates/submit.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/LICENSE
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/__main__.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/config.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/form.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/qr2.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/qrc.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/w2.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/docs/generate.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/docs/index.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/templates/submit.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/LICENSE
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/PKG-INFO
```

### Comparing `dynamic_qrcode_image-0.0.5/.github/workflows/python-publish.yml` & `dynamic_qrcode_image-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/qr2.py` & `dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/qr2.py`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/qrc.py` & `dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/qrc.py`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/w2.py` & `dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/w2.py`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.5/.gitignore` & `dynamic_qrcode_image-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.5/LICENSE` & `dynamic_qrcode_image-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.5/pyproject.toml` & `dynamic_qrcode_image-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dynamic_qrcode_image"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="Duke Bode", email="DukeBode@hotmail.com"},
 ]
 description = "dynamic_qrcode_image"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dynamic_qrcode_image-0.0.5/PKG-INFO` & `dynamic_qrcode_image-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_qrcode_image
-Version: 0.0.5
+Version: 0.0.6
 Summary: dynamic_qrcode_image
 Project-URL: Homepage, https://github.com/DukeBode/dynamic-qrcode-image
 Project-URL: Bug Tracker, https://github.com/DukeBode/dynamic-qrcode-image/issues
 Author-email: Duke Bode <DukeBode@hotmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

