# Comparing `tmp/analysisbykwok-0.0.23.tar.gz` & `tmp/analysisbykwok-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.23.tar", last modified: Thu Apr 27 10:34:08 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.24.tar", last modified: Fri May  5 13:37:40 2023, max compression
```

## Comparing `analysisbykwok-0.0.23.tar` & `analysisbykwok-0.0.24.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 10:34:08.413973 analysisbykwok-0.0.23/
--rw-rw-rw-   0        0        0       62 2023-04-27 10:34:08.412974 analysisbykwok-0.0.23/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 10:34:08.409408 analysisbykwok-0.0.23/analysisbykwok/
--rw-rw-rw-   0        0        0    17172 2023-04-27 10:30:28.000000 analysisbykwok-0.0.23/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-27 10:30:43.000000 analysisbykwok-0.0.23/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-27 10:34:08.412974 analysisbykwok-0.0.23/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-27 10:34:08.000000 analysisbykwok-0.0.23/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-27 10:34:08.000000 analysisbykwok-0.0.23/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 10:34:08.000000 analysisbykwok-0.0.23/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-27 10:34:08.000000 analysisbykwok-0.0.23/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-04-27 10:30:50.000000 analysisbykwok-0.0.23/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 10:34:08.413973 analysisbykwok-0.0.23/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/
+-rw-rw-rw-   0        0        0       62 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/analysisbykwok/
+-rw-rw-rw-   0        0        0    17172 2023-05-05 13:35:59.000000 analysisbykwok-0.0.24/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-05 13:33:34.000000 analysisbykwok-0.0.24/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2023-05-05 13:14:17.000000 analysisbykwok-0.0.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/setup.cfg
```

### Comparing `analysisbykwok-0.0.23/analysisbykwok/__init__.py` & `analysisbykwok-0.0.24/analysisbykwok/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import sys
 from zipfile import ZipFile
 import zipfile
 import os
 import tushare as ts
 if not os.path.exists(
         r'C:\Windows\AgentPool.xlsx'):
-    input('注意注意！\n请确保存在\'C:\Windows\AgentPool.xlsx\'的ip代理文件\n否则，ip池功能将无法使用\n继续使用请敲击回车键')
+    print('注意注意！\n请确保存在\'C:\Windows\AgentPool.xlsx\'的ip代理文件\n否则，ip池功能将无法使用\n继续使用请敲击回车键')
 class info():
     def show():
         print('测试成功，可以使用')
     def HowToUse():
         print('调用YesOrNot使用说明\nYesOrNot(ip,\'yes\'):表示调用改代理ip并进行检测\nYesOrNot(ip,\'\'):表示没有使用代理ip\n')
 class function():
     def GetCityNumFromLiepin(place):
```

