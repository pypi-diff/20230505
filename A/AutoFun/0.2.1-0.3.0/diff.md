# Comparing `tmp/AutoFun-0.2.1.tar.gz` & `tmp/AutoFun-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoFun-0.2.1.tar", last modified: Tue Feb 28 08:24:46 2023, max compression
+gzip compressed data, was "dist\AutoFun-0.3.0.tar", last modified: Fri May  5 11:19:28 2023, max compression
```

## Comparing `AutoFun-0.2.1.tar` & `AutoFun-0.3.0.tar`

### file list

```diff
@@ -1,69 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.781231 AutoFun-0.2.1/
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.600989 AutoFun-0.2.1/AutoFun/
--rw-rw-rw-   0        0        0     7306 2023-02-28 08:21:39.000000 AutoFun-0.2.1/AutoFun/AutoPy.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.623983 AutoFun-0.2.1/AutoFun/CutPdf/
--rw-rw-rw-   0        0        0    30220 2023-02-28 07:18:28.000000 AutoFun-0.2.1/AutoFun/CutPdf/CutPdf.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.631986 AutoFun-0.2.1/AutoFun/CutPdf/Function/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:41:50.000000 AutoFun-0.2.1/AutoFun/CutPdf/Function/__init__.py
--rw-rw-rw-   0        0        0     5617 2023-02-24 08:23:45.000000 AutoFun-0.2.1/AutoFun/CutPdf/Function/optionDb.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.639991 AutoFun-0.2.1/AutoFun/CutPdf/Ui/
--rw-rw-rw-   0        0        0     7890 2023-02-24 08:23:45.000000 AutoFun-0.2.1/AutoFun/CutPdf/Ui/CutPdfPicUi.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:41:43.000000 AutoFun-0.2.1/AutoFun/CutPdf/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:33:19.000000 AutoFun-0.2.1/AutoFun/CutPdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.646989 AutoFun-0.2.1/AutoFun/OcrFinish/
--rw-rw-rw-   0        0        0    21604 2023-02-27 07:28:12.000000 AutoFun-0.2.1/AutoFun/OcrFinish/OcrFinish.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.653982 AutoFun-0.2.1/AutoFun/OcrFinish/Ui/
--rw-rw-rw-   0        0        0     3241 2023-02-24 08:28:20.000000 AutoFun-0.2.1/AutoFun/OcrFinish/Ui/OcrfinishUi.py
--rw-rw-rw-   0        0        0        0 2023-02-24 08:08:08.000000 AutoFun-0.2.1/AutoFun/OcrFinish/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 08:03:15.000000 AutoFun-0.2.1/AutoFun/OcrFinish/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.668036 AutoFun-0.2.1/AutoFun/OcrPicFun/
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.680233 AutoFun-0.2.1/AutoFun/OcrPicFun/Function/
--rw-rw-rw-   0        0        0        0 2023-02-23 07:30:55.000000 AutoFun-0.2.1/AutoFun/OcrPicFun/Function/__init__.py
--rw-rw-rw-   0        0        0   332380 2022-04-11 02:44:10.000000 AutoFun-0.2.1/AutoFun/OcrPicFun/Function/dict_to_json.py
--rw-rw-rw-   0        0        0     5648 2023-02-24 02:24:41.000000 AutoFun-0.2.1/AutoFun/OcrPicFun/Function/get_json.py
--rw-rw-rw-   0        0        0    31309 2023-02-27 07:00:35.000000 AutoFun-0.2.1/AutoFun/OcrPicFun/OcrPicFun.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.689243 AutoFun-0.2.1/AutoFun/OcrPicFun/Ui/
--rw-rw-rw-   0        0        0     4781 2023-02-24 08:31:54.000000 AutoFun-0.2.1/AutoFun/OcrPicFun/Ui/OcrparameterUi.py
--rw-rw-rw-   0        0        0        0 2023-02-23 07:39:04.000000 AutoFun-0.2.1/AutoFun/OcrPicFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 07:28:02.000000 AutoFun-0.2.1/AutoFun/OcrPicFun/__init__.py
--rw-rw-rw-   0        0        0       78 2023-02-24 08:31:54.000000 AutoFun-0.2.1/AutoFun/OcrPicFun/settings.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.697236 AutoFun-0.2.1/AutoFun/OcrTableFun/
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.712233 AutoFun-0.2.1/AutoFun/OcrTableFun/Function/
--rw-rw-rw-   0        0        0     2460 2022-04-14 09:12:52.000000 AutoFun-0.2.1/AutoFun/OcrTableFun/Function/DB_in_sqlite.py
--rw-rw-rw-   0        0        0        0 2023-02-23 09:00:55.000000 AutoFun-0.2.1/AutoFun/OcrTableFun/Function/__init__.py
--rw-rw-rw-   0        0        0     5573 2022-11-23 09:35:24.000000 AutoFun-0.2.1/AutoFun/OcrTableFun/Function/optionDb.py
--rw-rw-rw-   0        0        0    43028 2023-02-23 09:13:25.000000 AutoFun-0.2.1/AutoFun/OcrTableFun/Function/sqlite_to_excel.py
--rw-rw-rw-   0        0        0    16222 2023-02-28 07:35:35.000000 AutoFun-0.2.1/AutoFun/OcrTableFun/OcrTableFun.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.722232 AutoFun-0.2.1/AutoFun/OcrTableFun/Ui/
--rw-rw-rw-   0        0        0     6585 2023-02-24 08:34:54.000000 AutoFun-0.2.1/AutoFun/OcrTableFun/Ui/OcrTableUi.py
--rw-rw-rw-   0        0        0        0 2023-02-23 09:01:01.000000 AutoFun-0.2.1/AutoFun/OcrTableFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 09:00:01.000000 AutoFun-0.2.1/AutoFun/OcrTableFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.730239 AutoFun-0.2.1/AutoFun/SplitPdfFun/
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.759248 AutoFun-0.2.1/AutoFun/SplitPdfFun/Function/
--rw-rw-rw-   0        0        0     2460 2022-04-14 09:12:52.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/Function/DB_in_sqlite.py
--rw-rw-rw-   0        0        0        0 2023-02-24 08:06:17.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/Function/__init__.py
--rw-rw-rw-   0        0        0     5573 2022-11-23 09:35:24.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/Function/optionDb.py
--rw-rw-rw-   0        0        0     6190 2022-03-30 09:32:28.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/Function/pdf_utils.py
--rw-rw-rw-   0        0        0    19999 2023-02-27 09:38:02.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/Function/splite_pdf.py
--rw-rw-rw-   0        0        0    41721 2023-02-23 09:51:21.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/Function/sqlite_to_excel.py
--rw-rw-rw-   0        0        0    17573 2023-02-28 07:53:13.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/SplitPdfFun.py
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.770240 AutoFun-0.2.1/AutoFun/SplitPdfFun/Ui/
--rw-rw-rw-   0        0        0     4719 2023-02-24 08:40:22.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/Ui/SplitPdfUi.py
--rw-rw-rw-   0        0        0        0 2023-02-24 08:07:46.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 09:28:19.000000 AutoFun-0.2.1/AutoFun/SplitPdfFun/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-24 08:18:18.000000 AutoFun-0.2.1/AutoFun/__init__.py
--rw-rw-rw-   0        0        0       85 2023-02-24 01:07:50.000000 AutoFun-0.2.1/AutoFun/td.txt
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.615982 AutoFun-0.2.1/AutoFun.egg-info/
--rw-rw-rw-   0        0        0      496 2023-02-28 08:24:45.000000 AutoFun-0.2.1/AutoFun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1575 2023-02-28 08:24:46.000000 AutoFun-0.2.1/AutoFun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 08:24:45.000000 AutoFun-0.2.1/AutoFun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-02-28 08:24:46.000000 AutoFun-0.2.1/AutoFun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      496 2023-02-28 08:24:46.782235 AutoFun-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 08:24:46.777290 AutoFun-0.2.1/clazz/
--rw-rw-rw-   0        0        0      750 2023-02-14 08:23:37.000000 AutoFun-0.2.1/clazz/__init__.py
--rw-rw-rw-   0        0        0      185 2023-02-22 10:01:05.000000 AutoFun-0.2.1/clazz/demo.py
--rw-rw-rw-   0        0        0      135 2023-02-28 08:24:46.785233 AutoFun-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1019 2023-02-28 08:21:39.000000 AutoFun-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:19:28.202097 AutoFun-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-05-05 11:19:28.201096 AutoFun-0.3.0/AutoFun.egg-info/
+-rw-rw-rw-   0        0        0      429 2023-05-05 11:19:28.000000 AutoFun-0.3.0/AutoFun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-05-05 11:19:28.000000 AutoFun-0.3.0/AutoFun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:19:28.000000 AutoFun-0.3.0/AutoFun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:19:28.000000 AutoFun-0.3.0/AutoFun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      429 2023-05-05 11:19:28.202097 AutoFun-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.0/README.md
+-rw-rw-rw-   0        0        0      135 2023-05-05 11:19:28.203097 AutoFun-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-05-05 11:18:43.000000 AutoFun-0.3.0/setup.py
```

### Comparing `AutoFun-0.2.1/LICENSE.txt` & `AutoFun-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AutoFun-0.2.1/setup.py` & `AutoFun-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
-MINOR = 2
-PATCH = 1
+MINOR = 3
+PATCH = 0
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "AutoFun",
 	version = VERSION,
     author ="wangweidong",
     author_email = "17891967090@163.com",
-    description='PDF撕裂者单个功能',
+    description='Due Diligence Toolkit Python project',
     long_description_content_type="text/markdown",
-	url = 'https://mail.163.com/js6/main.jsp?sid=PAlGWIYldfIQjfQTFYllFVEyKXidwtNk&df=mail163_letter#module=welcome.WelcomeModule%7C%7B%7D',
+	url = 'https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
 	long_description = open('README.md',encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
-
+    # package_dir = {"":"aaa"},
+    # packages = find_packages(where="aaa"),
 	packages = find_packages(),
- 	# license = '',
+ 	# license = 'Apache',
    	classifiers = [
        'Programming Language :: Python',
 
     ],
     #包含的类型
     package_data={'': ['*.csv', '*.txt','.toml', "*.pyd",'*.exe', '*.db']}, #这个很重要
     include_package_data=True #也选上
```

