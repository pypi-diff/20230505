# Comparing `tmp/pymrt_client-1.0.3.tar.gz` & `tmp/pymrt_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymrt_client-1.0.3.tar", last modified: Fri May  5 03:09:48 2023, max compression
+gzip compressed data, was "pymrt_client-1.0.4.tar", last modified: Fri May  5 05:43:48 2023, max compression
```

## Comparing `pymrt_client-1.0.3.tar` & `pymrt_client-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 03:09:48.967005 pymrt_client-1.0.3/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 pymrt_client-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2640 2023-05-05 03:09:48.967005 pymrt_client-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 pymrt_client-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 03:09:48.958001 pymrt_client-1.0.3/pymrt_client/
--rw-rw-rw-   0        0        0     5869 2023-04-26 08:02:47.000000 pymrt_client-1.0.3/pymrt_client/Enums.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 pymrt_client-1.0.3/pymrt_client/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 pymrt_client-1.0.3/pymrt_client/drt_structures.py
--rw-rw-rw-   0        0        0     3447 2023-04-26 08:02:47.000000 pymrt_client-1.0.3/pymrt_client/kunyi_ma.py
--rw-rw-rw-   0        0        0    48162 2023-05-05 02:47:27.000000 pymrt_client-1.0.3/pymrt_client/kunyi_mrt.py
--rw-rw-rw-   0        0        0    11497 2023-04-26 08:57:24.000000 pymrt_client-1.0.3/pymrt_client/kunyi_project.py
--rw-rw-rw-   0        0        0    11804 2023-04-26 08:46:57.000000 pymrt_client-1.0.3/pymrt_client/kunyi_util.py
--rw-rw-rw-   0        0        0     3371 2023-04-26 08:59:18.000000 pymrt_client-1.0.3/pymrt_client/minio_handld.py
--rw-rw-rw-   0        0        0     1999 2023-04-26 08:48:42.000000 pymrt_client-1.0.3/pymrt_client/mrt_strunctures.py
--rw-rw-rw-   0        0        0     5421 2023-04-26 08:57:24.000000 pymrt_client-1.0.3/pymrt_client/signal_daq.py
-drwxrwxrwx   0        0        0        0 2023-05-05 03:09:48.965013 pymrt_client-1.0.3/pymrt_client.egg-info/
--rw-rw-rw-   0        0        0     2640 2023-05-05 03:09:48.000000 pymrt_client-1.0.3/pymrt_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-05-05 03:09:48.000000 pymrt_client-1.0.3/pymrt_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 03:09:48.000000 pymrt_client-1.0.3/pymrt_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 03:09:48.000000 pymrt_client-1.0.3/pymrt_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-05 03:09:48.968015 pymrt_client-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-05-05 03:09:33.000000 pymrt_client-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 05:43:48.427668 pymrt_client-1.0.4/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 pymrt_client-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2640 2023-05-05 05:43:48.428681 pymrt_client-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 pymrt_client-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 05:43:48.419106 pymrt_client-1.0.4/pymrt_client/
+-rw-rw-rw-   0        0        0     5869 2023-04-26 08:02:47.000000 pymrt_client-1.0.4/pymrt_client/Enums.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 pymrt_client-1.0.4/pymrt_client/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 pymrt_client-1.0.4/pymrt_client/drt_structures.py
+-rw-rw-rw-   0        0        0     3447 2023-04-26 08:02:47.000000 pymrt_client-1.0.4/pymrt_client/kunyi_ma.py
+-rw-rw-rw-   0        0        0    48162 2023-05-05 02:47:27.000000 pymrt_client-1.0.4/pymrt_client/kunyi_mrt.py
+-rw-rw-rw-   0        0        0    11497 2023-04-26 08:57:24.000000 pymrt_client-1.0.4/pymrt_client/kunyi_project.py
+-rw-rw-rw-   0        0        0    11804 2023-04-26 08:46:57.000000 pymrt_client-1.0.4/pymrt_client/kunyi_util.py
+-rw-rw-rw-   0        0        0     3371 2023-04-26 08:59:18.000000 pymrt_client-1.0.4/pymrt_client/minio_handld.py
+-rw-rw-rw-   0        0        0     1999 2023-04-26 08:48:42.000000 pymrt_client-1.0.4/pymrt_client/mrt_strunctures.py
+-rw-rw-rw-   0        0        0     5421 2023-04-26 08:57:24.000000 pymrt_client-1.0.4/pymrt_client/signal_daq.py
+drwxrwxrwx   0        0        0        0 2023-05-05 05:43:48.426117 pymrt_client-1.0.4/pymrt_client.egg-info/
+-rw-rw-rw-   0        0        0     2640 2023-05-05 05:43:48.000000 pymrt_client-1.0.4/pymrt_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-05-05 05:43:48.000000 pymrt_client-1.0.4/pymrt_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 05:43:48.000000 pymrt_client-1.0.4/pymrt_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-05 05:43:48.000000 pymrt_client-1.0.4/pymrt_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 05:43:48.000000 pymrt_client-1.0.4/pymrt_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-05 05:43:48.428681 pymrt_client-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-05-05 05:43:44.000000 pymrt_client-1.0.4/setup.py
```

### Comparing `pymrt_client-1.0.3/LICENSE` & `pymrt_client-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/PKG-INFO` & `pymrt_client-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymrt_client
-Version: 1.0.3
+Version: 1.0.4
 Summary: pymrt_client
 Home-page: UNKNOWN
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymrt_client-1.0.3/README.md` & `pymrt_client-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/pymrt_client/Enums.py` & `pymrt_client-1.0.4/pymrt_client/Enums.py`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/pymrt_client/kunyi_ma.py` & `pymrt_client-1.0.4/pymrt_client/kunyi_ma.py`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/pymrt_client/kunyi_mrt.py` & `pymrt_client-1.0.4/pymrt_client/kunyi_mrt.py`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/pymrt_client/kunyi_project.py` & `pymrt_client-1.0.4/pymrt_client/kunyi_project.py`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/pymrt_client/kunyi_util.py` & `pymrt_client-1.0.4/pymrt_client/kunyi_util.py`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/pymrt_client/minio_handld.py` & `pymrt_client-1.0.4/pymrt_client/minio_handld.py`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/pymrt_client/mrt_strunctures.py` & `pymrt_client-1.0.4/pymrt_client/mrt_strunctures.py`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/pymrt_client/signal_daq.py` & `pymrt_client-1.0.4/pymrt_client/signal_daq.py`

 * *Files identical despite different names*

### Comparing `pymrt_client-1.0.3/pymrt_client.egg-info/PKG-INFO` & `pymrt_client-1.0.4/pymrt_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymrt-client
-Version: 1.0.3
+Version: 1.0.4
 Summary: pymrt_client
 Home-page: UNKNOWN
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymrt_client-1.0.3/setup.py` & `pymrt_client-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymrt_client",  # 包名
-    version="1.0.3",
+    version="1.0.4",
     author="vcarsystem",
     author_email="service@vcarsystem.com",
     description="pymrt_client",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
+    install_requires = ["pytest","minio==7.1.13"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

