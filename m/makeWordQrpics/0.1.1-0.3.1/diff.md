# Comparing `tmp/MakeWordQrpics-0.1.1.tar.gz` & `tmp/makeWordQrpics-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MakeWordQrpics-0.1.1.tar", last modified: Tue Feb 28 06:59:39 2023, max compression
+gzip compressed data, was "makeWordQrpics-0.3.1.tar", last modified: Fri May  5 12:41:16 2023, max compression
```

## Comparing `MakeWordQrpics-0.1.1.tar` & `makeWordQrpics-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 06:59:39.395508 MakeWordQrpics-0.1.1/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 MakeWordQrpics-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 MakeWordQrpics-0.1.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-02-28 06:59:39.349508 MakeWordQrpics-0.1.1/MakeWordQrpics/
-drwxrwxrwx   0        0        0        0 2023-02-28 06:59:39.380511 MakeWordQrpics-0.1.1/MakeWordQrpics/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 06:42:06.000000 MakeWordQrpics-0.1.1/MakeWordQrpics/Function/__init__.py
--rw-rw-rw-   0        0        0     5573 2022-11-23 09:35:24.000000 MakeWordQrpics-0.1.1/MakeWordQrpics/Function/optionDb.py
-drwxrwxrwx   0        0        0        0 2023-02-28 06:59:39.391509 MakeWordQrpics-0.1.1/MakeWordQrpics/Ui/
--rw-rw-rw-   0        0        0     5422 2023-02-28 06:51:36.000000 MakeWordQrpics-0.1.1/MakeWordQrpics/Ui/TableToWordUi.py
--rw-rw-rw-   0        0        0        0 2023-02-28 06:41:59.000000 MakeWordQrpics-0.1.1/MakeWordQrpics/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 06:54:16.000000 MakeWordQrpics-0.1.1/MakeWordQrpics/__init__.py
--rw-rw-rw-   0        0        0    11319 2023-02-28 06:59:23.000000 MakeWordQrpics-0.1.1/MakeWordQrpics/make_word_qrpics.py
-drwxrwxrwx   0        0        0        0 2023-02-28 06:59:39.369506 MakeWordQrpics-0.1.1/MakeWordQrpics.egg-info/
--rw-rw-rw-   0        0        0      464 2023-02-28 06:59:39.000000 MakeWordQrpics-0.1.1/MakeWordQrpics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-02-28 06:59:39.000000 MakeWordQrpics-0.1.1/MakeWordQrpics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 06:59:39.000000 MakeWordQrpics-0.1.1/MakeWordQrpics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-02-28 06:59:39.000000 MakeWordQrpics-0.1.1/MakeWordQrpics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      464 2023-02-28 06:59:39.395508 MakeWordQrpics-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 MakeWordQrpics-0.1.1/README.md
--rw-rw-rw-   0        0        0      135 2023-02-28 06:59:39.398507 MakeWordQrpics-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-02-28 06:56:52.000000 MakeWordQrpics-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.622435 makeWordQrpics-0.3.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 makeWordQrpics-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 makeWordQrpics-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      424 2023-05-05 12:41:16.622435 makeWordQrpics-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 makeWordQrpics-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.606354 makeWordQrpics-0.3.1/makeWordQrpics/
+drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.615436 makeWordQrpics-0.3.1/makeWordQrpics/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 06:42:06.000000 makeWordQrpics-0.3.1/makeWordQrpics/Function/__init__.py
+-rw-rw-rw-   0        0        0     5573 2022-11-23 09:35:24.000000 makeWordQrpics-0.3.1/makeWordQrpics/Function/optionDb.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.620463 makeWordQrpics-0.3.1/makeWordQrpics/Ui/
+-rw-rw-rw-   0        0        0     5422 2023-02-28 06:51:36.000000 makeWordQrpics-0.3.1/makeWordQrpics/Ui/TableToWordUi.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 06:41:59.000000 makeWordQrpics-0.3.1/makeWordQrpics/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 06:54:16.000000 makeWordQrpics-0.3.1/makeWordQrpics/__init__.py
+-rw-rw-rw-   0        0        0    11319 2023-02-28 06:59:23.000000 makeWordQrpics-0.3.1/makeWordQrpics/make_word_qrpics.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.612438 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/
+-rw-rw-rw-   0        0        0      424 2023-05-05 12:41:16.000000 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-05 12:41:16.000000 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:41:16.000000 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-05 12:41:16.000000 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      135 2023-05-05 12:41:16.623436 makeWordQrpics-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      970 2023-05-05 12:41:04.000000 makeWordQrpics-0.3.1/setup.py
```

### Comparing `MakeWordQrpics-0.1.1/LICENSE.txt` & `makeWordQrpics-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MakeWordQrpics-0.1.1/MakeWordQrpics/Function/optionDb.py` & `makeWordQrpics-0.3.1/makeWordQrpics/Function/optionDb.py`

 * *Files identical despite different names*

### Comparing `MakeWordQrpics-0.1.1/MakeWordQrpics/Ui/TableToWordUi.py` & `makeWordQrpics-0.3.1/makeWordQrpics/Ui/TableToWordUi.py`

 * *Files identical despite different names*

### Comparing `MakeWordQrpics-0.1.1/MakeWordQrpics/make_word_qrpics.py` & `makeWordQrpics-0.3.1/makeWordQrpics/make_word_qrpics.py`

 * *Files identical despite different names*

### Comparing `MakeWordQrpics-0.1.1/setup.py` & `makeWordQrpics-0.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
-MINOR = 1
-PATCH = 1
+MINOR = 3
+PATCH =1
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
-	name = "MakeWordQrpics",
+	name = "makeWordQrpics",
 	version = VERSION,
     author ="wangweidong",
     author_email = "17891967090@163.com",
     description='PDF撕裂者单个功能',
     long_description_content_type="text/markdown",
-	url = 'https://mail.163.com/js6/main.jsp?sid=PAlGWIYldfIQjfQTFYllFVEyKXidwtNk&df=mail163_letter#module=welcome.WelcomeModule%7C%7B%7D',
+	url = 'https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
 	long_description = open('README.md',encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
 
 	packages = find_packages(),
  	# license = 'Apache',
    	classifiers = [
```

