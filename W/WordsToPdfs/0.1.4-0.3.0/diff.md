# Comparing `tmp/WordsToPdfs-0.1.4.tar.gz` & `tmp/WordsToPdfs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WordsToPdfs-0.1.4.tar", last modified: Tue Feb 28 03:32:34 2023, max compression
+gzip compressed data, was "WordsToPdfs-0.3.0.tar", last modified: Fri May  5 12:23:35 2023, max compression
```

## Comparing `WordsToPdfs-0.1.4.tar` & `WordsToPdfs-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 03:32:34.024017 WordsToPdfs-0.1.4/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 WordsToPdfs-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 WordsToPdfs-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      481 2023-02-28 03:32:34.025014 WordsToPdfs-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 WordsToPdfs-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 03:32:33.993012 WordsToPdfs-0.1.4/WordsToPdfs/
-drwxrwxrwx   0        0        0        0 2023-02-28 03:32:34.013017 WordsToPdfs-0.1.4/WordsToPdfs/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 02:34:37.000000 WordsToPdfs-0.1.4/WordsToPdfs/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 03:32:34.020017 WordsToPdfs-0.1.4/WordsToPdfs/Ui/
--rw-rw-rw-   0        0        0     3689 2022-11-15 03:34:05.000000 WordsToPdfs-0.1.4/WordsToPdfs/Ui/WordToPdfUi.py
--rw-rw-rw-   0        0        0        0 2023-02-28 02:34:43.000000 WordsToPdfs-0.1.4/WordsToPdfs/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 02:33:27.000000 WordsToPdfs-0.1.4/WordsToPdfs/__init__.py
--rw-rw-rw-   0        0        0    17923 2023-02-28 03:30:03.000000 WordsToPdfs-0.1.4/WordsToPdfs/msg_words_to_pdfs.py
-drwxrwxrwx   0        0        0        0 2023-02-28 03:32:34.009014 WordsToPdfs-0.1.4/WordsToPdfs.egg-info/
--rw-rw-rw-   0        0        0      481 2023-02-28 03:32:33.000000 WordsToPdfs-0.1.4/WordsToPdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-02-28 03:32:33.000000 WordsToPdfs-0.1.4/WordsToPdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 03:32:33.000000 WordsToPdfs-0.1.4/WordsToPdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-28 03:32:33.000000 WordsToPdfs-0.1.4/WordsToPdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2023-02-28 03:32:34.027016 WordsToPdfs-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-02-28 03:32:22.000000 WordsToPdfs-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.568752 WordsToPdfs-0.3.0/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 WordsToPdfs-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 WordsToPdfs-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      421 2023-05-05 12:23:35.568752 WordsToPdfs-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 WordsToPdfs-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.557722 WordsToPdfs-0.3.0/WordsToPdfs/
+drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.566788 WordsToPdfs-0.3.0/WordsToPdfs/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:33:27.000000 WordsToPdfs-0.3.0/WordsToPdfs/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.567746 WordsToPdfs-0.3.0/WordsToPdfs/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:33:27.000000 WordsToPdfs-0.3.0/WordsToPdfs/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:33:27.000000 WordsToPdfs-0.3.0/WordsToPdfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.564714 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/
+-rw-rw-rw-   0        0        0      421 2023-05-05 12:23:35.000000 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-05 12:23:35.000000 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:23:35.000000 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 12:23:35.000000 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      135 2023-05-05 12:23:35.569754 WordsToPdfs-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-05-05 12:23:31.000000 WordsToPdfs-0.3.0/setup.py
```

### Comparing `WordsToPdfs-0.1.4/LICENSE.txt` & `WordsToPdfs-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `WordsToPdfs-0.1.4/setup.py` & `WordsToPdfs-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
-MINOR = 1
-PATCH = 4
+MINOR = 3
+PATCH = 0
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "WordsToPdfs",
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
- 	license = 'Apache',
+ 	# license = 'Apache',
    	classifiers = [
        'Programming Language :: Python',
 
     ],
     #包含的类型
     package_data={'': ['*.csv', '*.txt','.toml', "*.pyd",'*.exe', '*.db']}, #这个很重要
     include_package_data=True #也选上
```

