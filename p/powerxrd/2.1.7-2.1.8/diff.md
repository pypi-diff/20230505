# Comparing `tmp/powerxrd-2.1.7.tar.gz` & `tmp/powerxrd-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/powerxrd-2.1.7.tar", last modified: Wed Nov 30 16:51:53 2022, max compression
+gzip compressed data, was "dist/powerxrd-2.1.8.tar", last modified: Wed Nov 30 17:33:28 2022, max compression
```

## Comparing `powerxrd-2.1.7.tar` & `powerxrd-2.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-30 16:51:53.730609 powerxrd-2.1.7/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1077 2022-05-27 17:32:21.000000 powerxrd-2.1.7/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1735 2022-11-30 16:51:53.730609 powerxrd-2.1.7/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1017 2022-11-22 18:57:11.000000 powerxrd-2.1.7/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-30 16:51:53.726609 powerxrd-2.1.7/powerxrd/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       28 2022-11-18 17:25:26.000000 powerxrd-2.1.7/powerxrd/__init__.py
--rwxrwxr-x   0 andrew    (1000) andrew    (1000)    11773 2022-11-30 16:50:57.000000 powerxrd-2.1.7/powerxrd/main.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-30 16:51:53.730609 powerxrd-2.1.7/powerxrd.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1735 2022-11-30 16:51:53.000000 powerxrd-2.1.7/powerxrd.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      223 2022-11-30 16:51:53.000000 powerxrd-2.1.7/powerxrd.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2022-11-30 16:51:53.000000 powerxrd-2.1.7/powerxrd.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2022-11-30 16:51:53.000000 powerxrd-2.1.7/powerxrd.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2022-11-30 16:51:53.000000 powerxrd-2.1.7/powerxrd.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2022-11-30 16:51:53.730609 powerxrd-2.1.7/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1417 2022-11-30 16:51:24.000000 powerxrd-2.1.7/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-30 17:33:28.839047 powerxrd-2.1.8/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1077 2022-05-27 17:32:21.000000 powerxrd-2.1.8/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1735 2022-11-30 17:33:28.839047 powerxrd-2.1.8/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1017 2022-11-22 18:57:11.000000 powerxrd-2.1.8/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-30 17:33:28.839047 powerxrd-2.1.8/powerxrd/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       28 2022-11-18 17:25:26.000000 powerxrd-2.1.8/powerxrd/__init__.py
+-rwxrwxr-x   0 andrew    (1000) andrew    (1000)    11809 2022-11-30 17:31:15.000000 powerxrd-2.1.8/powerxrd/main.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2022-11-30 17:33:28.839047 powerxrd-2.1.8/powerxrd.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1735 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      223 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2022-11-30 17:33:28.000000 powerxrd-2.1.8/powerxrd.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2022-11-30 17:33:28.839047 powerxrd-2.1.8/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1417 2022-11-30 17:32:31.000000 powerxrd-2.1.8/setup.py
```

### Comparing `powerxrd-2.1.7/LICENSE` & `powerxrd-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `powerxrd-2.1.7/PKG-INFO` & `powerxrd-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerxrd
-Version: 2.1.7
+Version: 2.1.8
 Summary: Simple tools to handle powder XRD (and XRD) data with Python.
 Home-page: https://github.com/andrewrgarcia/powerxrd
 Author: Andrew Garcia, PhD
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powerxrd Version: 2.1.7 Summary: Simple tools to
+Metadata-Version: 2.1 Name: powerxrd Version: 2.1.8 Summary: Simple tools to
 handle powder XRD (and XRD) data with Python. Home-page: https://github.com/
 andrewrgarcia/powerxrd Author: Andrew Garcia, PhD License: MIT Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `powerxrd-2.1.7/README.md` & `powerxrd-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `powerxrd-2.1.7/powerxrd/main.py` & `powerxrd-2.1.8/powerxrd/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,24 +59,25 @@
         ----------
         file : str
             file name and/or path for XRD file in .xy format
         '''
         self.file = file
 
     
-    def importfile(self,format='xy'):
+    def importfile(self):
 
-        if format=='xy':
+        if self.file.split(".")[1]=='xy':
             df = pandas.read_csv(self.file, sep='\t', header=None)   #'https://www.statology.org/pandas-read-text-file/'
-        else:
+
+        if self.file.split(".")[1]=='csv':
             df = pandas.read_csv(self.file, header=None)   
 
-        x,y = np.array(df).T
 
-        return x,y
+        x,y = np.array(df).T
+        return x,y 
 
 class Chart:
 
     def __init__(self,x,y):
         '''Chart structure. Constructs x-y XRD data to manipulate and analyze. 
 
         Parameters
```

### Comparing `powerxrd-2.1.7/powerxrd.egg-info/PKG-INFO` & `powerxrd-2.1.8/powerxrd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerxrd
-Version: 2.1.7
+Version: 2.1.8
 Summary: Simple tools to handle powder XRD (and XRD) data with Python.
 Home-page: https://github.com/andrewrgarcia/powerxrd
 Author: Andrew Garcia, PhD
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powerxrd Version: 2.1.7 Summary: Simple tools to
+Metadata-Version: 2.1 Name: powerxrd Version: 2.1.8 Summary: Simple tools to
 handle powder XRD (and XRD) data with Python. Home-page: https://github.com/
 andrewrgarcia/powerxrd Author: Andrew Garcia, PhD License: MIT Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `powerxrd-2.1.7/setup.py` & `powerxrd-2.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="powerxrd",
-    version="2.1.7",
+    version="2.1.8",
     description="Simple tools to handle powder XRD (and XRD) data with Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andrewrgarcia/powerxrd",
     author="Andrew Garcia, PhD",
     license="MIT",
     classifiers=[
```

