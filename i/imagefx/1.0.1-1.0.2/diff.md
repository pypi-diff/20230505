# Comparing `tmp/imagefx-1.0.1.tar.gz` & `tmp/imagefx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imagefx-1.0.1.tar", last modified: Fri May  5 19:34:28 2023, max compression
+gzip compressed data, was "dist\imagefx-1.0.2.tar", last modified: Fri May  5 19:49:15 2023, max compression
```

## Comparing `imagefx-1.0.1.tar` & `imagefx-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:34:28.000000 imagefx-1.0.1/
--rw-rw-rw-   0        0        0      627 2023-05-05 19:34:28.000000 imagefx-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2234 2023-05-05 19:09:27.000000 imagefx-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 19:34:28.000000 imagefx-1.0.1/imagefx/
--rw-rw-rw-   0        0        0       71 2023-05-05 19:24:13.000000 imagefx-1.0.1/imagefx/__init__.py
--rw-rw-rw-   0        0        0     4498 2023-05-05 19:19:00.000000 imagefx-1.0.1/imagefx/main.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:34:28.000000 imagefx-1.0.1/imagefx.egg-info/
--rw-rw-rw-   0        0        0      627 2023-05-05 19:34:28.000000 imagefx-1.0.1/imagefx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-05-05 19:34:28.000000 imagefx-1.0.1/imagefx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:34:28.000000 imagefx-1.0.1/imagefx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-05 19:34:28.000000 imagefx-1.0.1/imagefx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2023-05-05 19:34:28.000000 imagefx-1.0.1/imagefx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 19:34:28.000000 imagefx-1.0.1/imagefx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 19:34:28.000000 imagefx-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-05-05 19:34:23.000000 imagefx-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:34:28.000000 imagefx-1.0.1/tests/
--rw-rw-rw-   0        0        0      107 2023-05-05 19:25:14.000000 imagefx-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1973 2023-05-05 19:19:10.000000 imagefx-1.0.1/tests/tests_imagefx.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:49:15.000000 imagefx-1.0.2/
+-rw-rw-rw-   0        0        0      627 2023-05-05 19:49:15.000000 imagefx-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2234 2023-05-05 19:09:27.000000 imagefx-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 19:49:15.000000 imagefx-1.0.2/imagefx/
+-rw-rw-rw-   0        0        0       71 2023-05-05 19:24:13.000000 imagefx-1.0.2/imagefx/__init__.py
+-rw-rw-rw-   0        0        0     4478 2023-05-05 19:48:20.000000 imagefx-1.0.2/imagefx/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:49:15.000000 imagefx-1.0.2/imagefx.egg-info/
+-rw-rw-rw-   0        0        0      627 2023-05-05 19:49:15.000000 imagefx-1.0.2/imagefx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-05-05 19:49:15.000000 imagefx-1.0.2/imagefx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:49:15.000000 imagefx-1.0.2/imagefx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-05 19:49:15.000000 imagefx-1.0.2/imagefx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      102 2023-05-05 19:49:15.000000 imagefx-1.0.2/imagefx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 19:49:15.000000 imagefx-1.0.2/imagefx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 19:49:15.000000 imagefx-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-05-05 19:48:30.000000 imagefx-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:49:15.000000 imagefx-1.0.2/tests/
+-rw-rw-rw-   0        0        0      107 2023-05-05 19:25:14.000000 imagefx-1.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1973 2023-05-05 19:19:10.000000 imagefx-1.0.2/tests/tests_imagefx.py
```

### Comparing `imagefx-1.0.1/PKG-INFO` & `imagefx-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagefx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for performing image processing operations
 Home-page: UNKNOWN
 Author: Photon
 Author-email: electrify0608@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `imagefx-1.0.1/README.md` & `imagefx-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `imagefx-1.0.1/imagefx/main.py` & `imagefx-1.0.2/imagefx/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         image_path_or_url (str): Path to the image or to url of it
         scale (float) : Scaling factor for kernel size (default =1.0).
 
         Returns:
             numpy.ndarray: The blurred image"""
 
     # Load the image from file or URL
-    if image_path_or_url.startswith('http' or 'https'):
+    if image_path_or_url.startswith('https'):
         response = requests.get(image_path_or_url)
         img = np.array(Image.open(BytesIO(response.content)))
     else:
         img = cv2.imread(image_path_or_url)
 
     # Apply the Gaussian Blur
     kernel_size = int(2*round(scale) + 1)
@@ -34,15 +34,15 @@
         image_path_or_url (str): Path to the image or to url of it
         factor : Scaling factor to increase or decrease image resolution (default=1.0)
 
     Returns:
         numpy.ndarray: The high resolution image
 
     """
-    if image_path_or_url.startswith('https' or 'http'):
+    if image_path_or_url.startswith('https'):
         response = requests.get(image_path_or_url)
         img = np.array(Image.open(BytesIO(response.content)))
 
     else:
         img = cv2.imread(image_path_or_url)
 
     # Determine the output size
```

### Comparing `imagefx-1.0.1/imagefx.egg-info/PKG-INFO` & `imagefx-1.0.2/imagefx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagefx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for performing image processing operations
 Home-page: UNKNOWN
 Author: Photon
 Author-email: electrify0608@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `imagefx-1.0.1/setup.py` & `imagefx-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 
     name='imagefx',
-    version='1.0.1',
+    version='1.0.2',
     description='Python library for performing image processing operations',
     author='Photon',
     author_email='electrify0608@gmail.com',
     packages=find_packages(),
     install_requires=[
         'requests',
         'Pillow>=8.2.0',
```

### Comparing `imagefx-1.0.1/tests/tests_imagefx.py` & `imagefx-1.0.2/tests/tests_imagefx.py`

 * *Files identical despite different names*

