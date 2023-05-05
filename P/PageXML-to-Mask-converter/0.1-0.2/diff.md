# Comparing `tmp/PageXML_to_Mask_converter-0.1.tar.gz` & `tmp/PageXML_to_Mask_converter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PageXML_to_Mask_converter-0.1.tar", last modified: Wed Jul  1 14:34:00 2020, max compression
+gzip compressed data, was "PageXML_to_Mask_converter-0.2.tar", last modified: Fri May  5 12:43:06 2023, max compression
```

## Comparing `PageXML_to_Mask_converter-0.1.tar` & `PageXML_to_Mask_converter-0.2.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 alexanderh  (1000) alexanderh  (1000)        0 2020-07-01 14:34:00.979882 PageXML_to_Mask_converter-0.1/
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)      691 2020-07-01 14:34:00.979882 PageXML_to_Mask_converter-0.1/PKG-INFO
-drwxr-xr-x   0 alexanderh  (1000) alexanderh  (1000)        0 2020-07-01 14:34:00.979882 PageXML_to_Mask_converter-0.1/PageXML_to_Mask_converter.egg-info/
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)      691 2020-07-01 14:34:00.000000 PageXML_to_Mask_converter-0.1/PageXML_to_Mask_converter.egg-info/PKG-INFO
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)      408 2020-07-01 14:34:00.000000 PageXML_to_Mask_converter-0.1/PageXML_to_Mask_converter.egg-info/SOURCES.txt
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)        1 2020-07-01 14:34:00.000000 PageXML_to_Mask_converter-0.1/PageXML_to_Mask_converter.egg-info/dependency_links.txt
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       64 2020-07-01 14:34:00.000000 PageXML_to_Mask_converter-0.1/PageXML_to_Mask_converter.egg-info/entry_points.txt
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       13 2020-07-01 14:34:00.000000 PageXML_to_Mask_converter-0.1/PageXML_to_Mask_converter.egg-info/requires.txt
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       23 2020-07-01 14:34:00.000000 PageXML_to_Mask_converter-0.1/PageXML_to_Mask_converter.egg-info/top_level.txt
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       46 2020-07-01 14:31:07.000000 PageXML_to_Mask_converter-0.1/README.md
-drwxr-xr-x   0 alexanderh  (1000) alexanderh  (1000)        0 2020-07-01 14:34:00.979882 PageXML_to_Mask_converter-0.1/pagexml_mask_converter/
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)        0 2020-07-01 14:31:07.000000 PageXML_to_Mask_converter-0.1/pagexml_mask_converter/__init__.py
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)    12340 2020-07-01 14:31:07.000000 PageXML_to_Mask_converter-0.1/pagexml_mask_converter/pagexml_to_mask.py
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       12 2020-07-01 14:31:07.000000 PageXML_to_Mask_converter-0.1/requirements.txt
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       38 2020-07-01 14:34:00.979882 PageXML_to_Mask_converter-0.1/setup.cfg
--rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)     1074 2020-07-01 14:31:07.000000 PageXML_to_Mask_converter-0.1/setup.py
+drwxr-xr-x   0 alexanderh  (1000) alexanderh  (1000)        0 2023-05-05 12:43:06.374592 PageXML_to_Mask_converter-0.2/
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)    35149 2021-02-16 13:30:03.000000 PageXML_to_Mask_converter-0.2/LICENSE.md
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)      652 2023-05-05 12:43:06.374592 PageXML_to_Mask_converter-0.2/PKG-INFO
+drwxr-xr-x   0 alexanderh  (1000) alexanderh  (1000)        0 2023-05-05 12:43:06.371259 PageXML_to_Mask_converter-0.2/PageXML_to_Mask_converter.egg-info/
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)      652 2023-05-05 12:43:06.000000 PageXML_to_Mask_converter-0.2/PageXML_to_Mask_converter.egg-info/PKG-INFO
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)      520 2023-05-05 12:43:06.000000 PageXML_to_Mask_converter-0.2/PageXML_to_Mask_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)        1 2023-05-05 12:43:06.000000 PageXML_to_Mask_converter-0.2/PageXML_to_Mask_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       63 2023-05-05 12:43:06.000000 PageXML_to_Mask_converter-0.2/PageXML_to_Mask_converter.egg-info/entry_points.txt
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       13 2023-05-05 12:43:06.000000 PageXML_to_Mask_converter-0.2/PageXML_to_Mask_converter.egg-info/requires.txt
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       23 2023-05-05 12:43:06.000000 PageXML_to_Mask_converter-0.2/PageXML_to_Mask_converter.egg-info/top_level.txt
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       46 2021-02-16 13:30:03.000000 PageXML_to_Mask_converter-0.2/README.md
+drwxr-xr-x   0 alexanderh  (1000) alexanderh  (1000)        0 2023-05-05 12:43:06.371259 PageXML_to_Mask_converter-0.2/pagexml_mask_converter/
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)        0 2021-02-16 13:30:03.000000 PageXML_to_Mask_converter-0.2/pagexml_mask_converter/__init__.py
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)     2373 2021-02-16 13:30:03.000000 PageXML_to_Mask_converter-0.2/pagexml_mask_converter/color_legend.py
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)     6659 2021-02-16 13:30:03.000000 PageXML_to_Mask_converter-0.2/pagexml_mask_converter/data.py
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)    14890 2023-05-05 12:26:25.000000 PageXML_to_Mask_converter-0.2/pagexml_mask_converter/pagexml_to_mask.py
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)      448 2023-05-05 12:31:33.000000 PageXML_to_Mask_converter-0.2/pagexml_mask_converter/test.py
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       12 2021-02-16 13:30:03.000000 PageXML_to_Mask_converter-0.2/requirements.txt
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)       38 2023-05-05 12:43:06.374592 PageXML_to_Mask_converter-0.2/setup.cfg
+-rw-r--r--   0 alexanderh  (1000) alexanderh  (1000)     1074 2023-05-05 12:39:02.000000 PageXML_to_Mask_converter-0.2/setup.py
```

### Comparing `PageXML_to_Mask_converter-0.1/PKG-INFO` & `PageXML_to_Mask_converter-0.2/PageXML_to_Mask_converter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: PageXML_to_Mask_converter
-Version: 0.1
-Summary: UNKNOWN
+Name: PageXML-to-Mask-converter
+Version: 0.2
 Home-page: https://github.com/Gawajn/pagexml_to_mask
 Author: Alexander Hartelt
 Author-email: alexander.hartelt@informatik.uni-wuerzburg.de
-License: UNKNOWN
-Description: Simple Script to convert PageXML to Imagemasks
 Keywords: XML; Mask
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+Simple Script to convert PageXML to Imagemasks
```

### Comparing `PageXML_to_Mask_converter-0.1/PageXML_to_Mask_converter.egg-info/PKG-INFO` & `PageXML_to_Mask_converter-0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: PageXML-to-Mask-converter
-Version: 0.1
-Summary: UNKNOWN
+Name: PageXML_to_Mask_converter
+Version: 0.2
 Home-page: https://github.com/Gawajn/pagexml_to_mask
 Author: Alexander Hartelt
 Author-email: alexander.hartelt@informatik.uni-wuerzburg.de
-License: UNKNOWN
-Description: Simple Script to convert PageXML to Imagemasks
 Keywords: XML; Mask
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+Simple Script to convert PageXML to Imagemasks
```

### Comparing `PageXML_to_Mask_converter-0.1/setup.py` & `PageXML_to_Mask_converter-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='PageXML_to_Mask_converter',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     long_description=long_description,
 
     long_description_content_type="text/markdown",
     include_package_data=True,
     author="Alexander Hartelt",
     author_email="alexander.hartelt@informatik.uni-wuerzburg.de",
```

