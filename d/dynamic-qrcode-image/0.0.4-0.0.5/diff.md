# Comparing `tmp/dynamic_qrcode_image-0.0.4.tar.gz` & `tmp/dynamic_qrcode_image-0.0.5.tar.gz`

## Comparing `dynamic_qrcode_image-0.0.4.tar` & `dynamic_qrcode_image-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/__main__.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/config.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/form.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/qr2.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/qrc.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/w2.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/docs/generate.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/docs/index.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/templates/submit.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/LICENSE
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/__main__.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/config.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/form.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/qr2.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/qrc.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/w2.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/docs/generate.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/docs/index.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/templates/submit.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/LICENSE
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.5/PKG-INFO
```

### Comparing `dynamic_qrcode_image-0.0.4/.github/workflows/python-publish.yml` & `dynamic_qrcode_image-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/qr2.py` & `dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/qr2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿# 生成带logo的二维码图片
 from openpyxl import load_workbook
 from time import strftime,localtime,time
-from qrc import QRC        
+from .qrc import QRC        
 import config
 
 # 根据配置生成文件名
 def generate_uri(row,s='',char='-'):
     for k in config.name:
         n=ord(config.name[k])-ord("A")
         s+=f'{row[n].value}{char}'
```

### Comparing `dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/qrc.py` & `dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/qrc.py`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.4/src/dynamic_qrcode_image/w2.py` & `dynamic_qrcode_image-0.0.5/src/dynamic_qrcode_image/w2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from flask import Flask, escape, request,make_response,redirect,render_template
 from io import BytesIO
 from PIL import Image
-from qrc import QRC
+from .qrc import QRC
 ###############################
 # from flask_wtf import FlaskForm
 # from wtforms import StringField
 # from wtforms.validators import DataRequired
 
 # class MyForm(FlaskForm):
 #     name = StringField('name', validators=[DataRequired()])
```

### Comparing `dynamic_qrcode_image-0.0.4/.gitignore` & `dynamic_qrcode_image-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.4/LICENSE` & `dynamic_qrcode_image-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.4/pyproject.toml` & `dynamic_qrcode_image-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dynamic_qrcode_image"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Duke Bode", email="DukeBode@hotmail.com"},
 ]
 description = "dynamic_qrcode_image"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dynamic_qrcode_image-0.0.4/PKG-INFO` & `dynamic_qrcode_image-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_qrcode_image
-Version: 0.0.4
+Version: 0.0.5
 Summary: dynamic_qrcode_image
 Project-URL: Homepage, https://github.com/DukeBode/dynamic-qrcode-image
 Project-URL: Bug Tracker, https://github.com/DukeBode/dynamic-qrcode-image/issues
 Author-email: Duke Bode <DukeBode@hotmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

