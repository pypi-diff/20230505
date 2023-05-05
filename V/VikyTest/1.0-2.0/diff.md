# Comparing `tmp/VikyTest-1.0.tar.gz` & `tmp/VikyTest-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VikyTest-1.0.tar", last modified: Fri May  5 05:52:58 2023, max compression
+gzip compressed data, was "VikyTest-2.0.tar", last modified: Fri May  5 06:06:16 2023, max compression
```

## Comparing `VikyTest-1.0.tar` & `VikyTest-2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 05:52:58.643551 VikyTest-1.0/
--rwx------   0 ec2-user  (1000) ec2-user  (1000)     1061 2023-05-04 05:18:17.000000 VikyTest-1.0/LICENSE.txt
--rw-------   0 ec2-user  (1000) ec2-user  (1000)     8561 2023-05-05 05:52:58.643551 VikyTest-1.0/PKG-INFO
--rwx------   0 ec2-user  (1000) ec2-user  (1000)     8124 2023-05-04 05:18:17.000000 VikyTest-1.0/README.md
--rwx------   0 ec2-user  (1000) ec2-user  (1000)       86 2023-05-04 05:18:17.000000 VikyTest-1.0/pyproject.toml
--rw-------   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-05 05:52:58.643551 VikyTest-1.0/setup.cfg
--rwx------   0 ec2-user  (1000) ec2-user  (1000)      808 2023-05-05 05:49:37.000000 VikyTest-1.0/setup.py
-drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 05:52:58.639551 VikyTest-1.0/src/
-drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 05:52:58.639551 VikyTest-1.0/src/VikyTest/
--rwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-04 05:27:28.000000 VikyTest-1.0/src/VikyTest/__init__.py
--rwx------   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-05 05:46:55.000000 VikyTest-1.0/src/VikyTest/medToolkit.py
-drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 05:52:58.639551 VikyTest-1.0/src/VikyTest.egg-info/
--rw-------   0 ec2-user  (1000) ec2-user  (1000)     8561 2023-05-05 05:52:58.000000 VikyTest-1.0/src/VikyTest.egg-info/PKG-INFO
--rw-------   0 ec2-user  (1000) ec2-user  (1000)      241 2023-05-05 05:52:58.000000 VikyTest-1.0/src/VikyTest.egg-info/SOURCES.txt
--rw-------   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-05 05:52:58.000000 VikyTest-1.0/src/VikyTest.egg-info/dependency_links.txt
--rw-------   0 ec2-user  (1000) ec2-user  (1000)        9 2023-05-05 05:52:58.000000 VikyTest-1.0/src/VikyTest.egg-info/top_level.txt
+drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:06:16.304373 VikyTest-2.0/
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)     1061 2023-05-04 05:18:17.000000 VikyTest-2.0/LICENSE.txt
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)      395 2023-05-05 06:06:16.304373 VikyTest-2.0/PKG-INFO
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)     8124 2023-05-04 05:18:17.000000 VikyTest-2.0/README.md
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)       86 2023-05-04 05:18:17.000000 VikyTest-2.0/pyproject.toml
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-05 06:06:16.304373 VikyTest-2.0/setup.cfg
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)     1193 2023-05-05 06:04:36.000000 VikyTest-2.0/setup.py
+drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:06:16.304373 VikyTest-2.0/src/
+drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:06:16.304373 VikyTest-2.0/src/VikyTest/
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-04 05:27:28.000000 VikyTest-2.0/src/VikyTest/__init__.py
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-05 05:46:55.000000 VikyTest-2.0/src/VikyTest/medToolkit.py
+drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:06:16.304373 VikyTest-2.0/src/VikyTest.egg-info/
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)      395 2023-05-05 06:06:16.000000 VikyTest-2.0/src/VikyTest.egg-info/PKG-INFO
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)      241 2023-05-05 06:06:16.000000 VikyTest-2.0/src/VikyTest.egg-info/SOURCES.txt
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-05 06:06:16.000000 VikyTest-2.0/src/VikyTest.egg-info/dependency_links.txt
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)        9 2023-05-05 06:06:16.000000 VikyTest-2.0/src/VikyTest.egg-info/top_level.txt
```

### Comparing `VikyTest-1.0/LICENSE.txt` & `VikyTest-2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VikyTest-1.0/PKG-INFO` & `VikyTest-2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: VikyTest
-Version: 1.0
-Summary: Medical NLP Toolkit
-Download-URL: https://sample-videos.com/zip/10mb.zip
-Author: VigneshVallavan
-Author-email: vigneshvallavan1999@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # vLife | Virtusa
 
 
 ## Usage
 
 ```
 from vMedNLP import medToolKit
@@ -327,8 +313,8 @@
 
 ### II.II - DICOM redaction:
 
 The function redacts PII from both the image as well as the associated metadata. The dicom images must be passed as pydicom image objects.
 
 > **Syntax:**
 > ` d = Deidentification()
- d.call(file_type,"",filename)`
+ d.call(file_type,"",filename)`
```

