# Comparing `tmp/MoveFile-0.1.5.tar.gz` & `tmp/moveFile-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MoveFile-0.1.5.tar", last modified: Wed Feb 22 09:09:19 2023, max compression
+gzip compressed data, was "moveFile-0.3.0.tar", last modified: Fri May  5 12:11:06 2023, max compression
```

## Comparing `MoveFile-0.1.5.tar` & `moveFile-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 09:09:19.320102 MoveFile-0.1.5/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 MoveFile-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 MoveFile-0.1.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-02-22 09:09:19.291093 MoveFile-0.1.5/MoveFile.egg-info/
--rw-rw-rw-   0        0        0      490 2023-02-22 09:09:19.000000 MoveFile-0.1.5/MoveFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-02-22 09:09:19.000000 MoveFile-0.1.5/MoveFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 09:09:19.000000 MoveFile-0.1.5/MoveFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-22 09:09:19.000000 MoveFile-0.1.5/MoveFile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      490 2023-02-22 09:09:19.320102 MoveFile-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-22 07:19:14.000000 MoveFile-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-02-22 09:09:19.309092 MoveFile-0.1.5/moveFile/
-drwxrwxrwx   0        0        0        0 2023-02-22 09:09:19.316094 MoveFile-0.1.5/moveFile/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 MoveFile-0.1.5/moveFile/Ui/__init__.py
--rw-rw-rw-   0        0        0     5125 2022-11-25 03:09:45.000000 MoveFile-0.1.5/moveFile/Ui/moveFileUi.py
--rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 MoveFile-0.1.5/moveFile/__init__.py
--rw-rw-rw-   0        0        0      983 2022-03-30 09:32:28.000000 MoveFile-0.1.5/moveFile/find_file_return_path_m1.py
--rw-rw-rw-   0        0        0     5125 2022-11-25 03:09:45.000000 MoveFile-0.1.5/moveFile/moveFileUi.py
--rw-rw-rw-   0        0        0    27613 2023-02-22 09:06:43.000000 MoveFile-0.1.5/moveFile/msg_yidongwenjian.py
--rw-rw-rw-   0        0        0     5573 2022-11-23 09:35:24.000000 MoveFile-0.1.5/moveFile/optionDb.py
--rw-rw-rw-   0        0        0      135 2023-02-22 09:09:19.322098 MoveFile-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1116 2023-02-22 09:06:43.000000 MoveFile-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:11:06.802070 moveFile-0.3.0/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 moveFile-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 moveFile-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      344 2023-05-05 12:11:06.802070 moveFile-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-22 07:19:14.000000 moveFile-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 12:11:06.791069 moveFile-0.3.0/moveFile/
+drwxrwxrwx   0        0        0        0 2023-05-05 12:11:06.800071 moveFile-0.3.0/moveFile/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 moveFile-0.3.0/moveFile/Ui/__init__.py
+-rw-rw-rw-   0        0        0    71168 2023-04-28 06:15:40.000000 moveFile-0.3.0/moveFile/Ui/moveFileUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 moveFile-0.3.0/moveFile/__init__.py
+-rw-rw-rw-   0        0        0    35840 2023-04-28 06:14:13.000000 moveFile-0.3.0/moveFile/find_file_return_path_m1.pyd
+-rw-rw-rw-   0        0        0   221696 2023-05-05 06:58:51.000000 moveFile-0.3.0/moveFile/moveFile.pyd
+-rw-rw-rw-   0        0        0    68608 2023-04-28 06:14:21.000000 moveFile-0.3.0/moveFile/moveFileUi.pyd
+-rw-rw-rw-   0        0        0    69632 2023-04-28 06:14:45.000000 moveFile-0.3.0/moveFile/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-05-05 12:11:06.797073 moveFile-0.3.0/moveFile.egg-info/
+-rw-rw-rw-   0        0        0      344 2023-05-05 12:11:06.000000 moveFile-0.3.0/moveFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-05-05 12:11:06.000000 moveFile-0.3.0/moveFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:11:06.000000 moveFile-0.3.0/moveFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 12:11:06.000000 moveFile-0.3.0/moveFile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      135 2023-05-05 12:11:06.803069 moveFile-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      989 2023-05-05 12:10:57.000000 moveFile-0.3.0/setup.py
```

### Comparing `MoveFile-0.1.5/LICENSE.txt` & `moveFile-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MoveFile-0.1.5/setup.py` & `moveFile-0.3.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
-MINOR = 1
-PATCH = 5
+MINOR = 3
+PATCH = 0
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
-	name = "MoveFile",
+	name = "moveFile",
 	version = VERSION,
     author ="wangweidong",
     author_email = "17891967090@163.com",
-    description='Dynamsoft Barcode Reader Python project',
+    description='Due Diligence Toolkit Python project',
     long_description_content_type="text/markdown",
-	url = 'https://mail.163.com/js6/main.jsp?sid=PAlGWIYldfIQjfQTFYllFVEyKXidwtNk&df=mail163_letter#module=welcome.WelcomeModule%7C%7B%7D',
+	url = '',
 	long_description = open('README.md',encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
     # package_dir = {"":"aaa"},
     # packages = find_packages(where="aaa"),
 	packages = find_packages(),
- 	license = 'Apache',
+ 	# license = 'Apache',
    	classifiers = [
        'Programming Language :: Python',
 
     ],
     #包含的类型
     package_data={'': ['*.csv', '*.txt','.toml', "*.pyd",'*.exe', '*.db']}, #这个很重要
     include_package_data=True #也选上
```

