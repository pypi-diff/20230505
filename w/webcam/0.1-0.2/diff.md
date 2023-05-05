# Comparing `tmp/webcam-0.1.tar.gz` & `tmp/webcam-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-0.1.tar", last modified: Fri May  5 08:44:20 2023, max compression
+gzip compressed data, was "webcam-0.2.tar", last modified: Fri May  5 08:51:00 2023, max compression
```

## Comparing `webcam-0.1.tar` & `webcam-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:44:20.744606 webcam-0.1/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.1/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-05-05 08:44:20.744606 webcam-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 08:44:20.744606 webcam-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1318 2023-05-05 08:44:16.000000 webcam-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:44:20.711732 webcam-0.1/webcam/
--rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.1/webcam/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-05-05 08:42:27.000000 webcam-0.1/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    10572 2023-05-05 08:42:27.000000 webcam-0.1/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:44:20.742495 webcam-0.1/webcam.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-05-05 08:44:20.000000 webcam-0.1/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-05 08:44:20.000000 webcam-0.1/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:44:20.000000 webcam-0.1/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-05 08:44:20.000000 webcam-0.1/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 08:44:20.000000 webcam-0.1/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 08:51:00.386967 webcam-0.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.2/LICENSE
+-rw-rw-rw-   0        0        0     1311 2023-05-05 08:51:00.386967 webcam-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:51:00.386967 webcam-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1309 2023-05-05 08:50:48.000000 webcam-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:51:00.362988 webcam-0.2/webcam/
+-rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.2/webcam/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-05-05 08:42:27.000000 webcam-0.2/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    10572 2023-05-05 08:42:27.000000 webcam-0.2/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:51:00.386967 webcam-0.2/webcam.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/top_level.txt
```

### Comparing `webcam-0.1/LICENSE` & `webcam-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-0.1/PKG-INFO` & `webcam-0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.1
+Version: 0.2
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `webcam-0.1/setup.py` & `webcam-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='0.1',
+    version='0.2',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     packages=find_packages(),
     python_requires='>=3.6',
     install_requires=[
         'numpy',
-        'opencv-python-headless',
+        'opencv-python',
         'imutils'
     ],
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
```

### Comparing `webcam-0.1/webcam/_webcam_background.py` & `webcam-0.2/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-0.1/webcam/webcam.py` & `webcam-0.2/webcam/webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-0.1/webcam.egg-info/PKG-INFO` & `webcam-0.2/webcam.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.1
+Version: 0.2
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

