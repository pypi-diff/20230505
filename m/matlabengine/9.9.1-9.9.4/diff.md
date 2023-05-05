# Comparing `tmp/matlabengine-9.9.1.tar.gz` & `tmp/matlabengine-9.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlabengine-9.9.1.tar", last modified: Mon Sep 12 22:54:23 2022, max compression
+gzip compressed data, was "matlabengine-9.9.4.tar", last modified: Fri May  5 19:18:08 2023, max compression
```

## Comparing `matlabengine-9.9.1.tar` & `matlabengine-9.9.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 22:54:23.525110 matlabengine-9.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-09-12 22:54:14.000000 matlabengine-9.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6007 2022-09-12 22:54:23.525110 matlabengine-9.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-09-12 22:54:14.000000 matlabengine-9.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-12 22:54:14.000000 matlabengine-9.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-12 22:54:23.525110 matlabengine-9.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    14336 2022-09-12 22:54:14.000000 matlabengine-9.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 22:54:23.517109 matlabengine-9.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 22:54:23.521110 matlabengine-9.9.1/src/matlab/
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 22:54:23.521110 matlabengine-9.9.1/src/matlab/_internal/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13093 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/_internal/mlarray_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/_internal/mlarray_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 22:54:23.521110 matlabengine-9.9.1/src/matlab/engine/
--rw-r--r--   0 runner    (1001) docker     (121)     7215 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/engine/basefuture.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/engine/engineerror.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/engine/enginehelper.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/engine/enginesession.py
--rw-r--r--   0 runner    (1001) docker     (121)     4989 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/engine/fevalfuture.py
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/engine/futureresult.py
--rw-r--r--   0 runner    (1001) docker     (121)    10224 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/engine/matlabengine.py
--rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/engine/matlabfuture.py
--rw-r--r--   0 runner    (1001) docker     (121)     9105 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/mlarray.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-09-12 22:54:14.000000 matlabengine-9.9.1/src/matlab/mlexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 22:54:23.521110 matlabengine-9.9.1/src/matlabengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6007 2022-09-12 22:54:23.000000 matlabengine-9.9.1/src/matlabengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-09-12 22:54:23.000000 matlabengine-9.9.1/src/matlabengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 22:54:23.000000 matlabengine-9.9.1/src/matlabengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 22:54:23.000000 matlabengine-9.9.1/src/matlabengine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-12 22:54:23.000000 matlabengine-9.9.1/src/matlabengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:18:08.251824 matlabengine-9.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-05 19:17:56.000000 matlabengine-9.9.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-05 19:18:08.251824 matlabengine-9.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-05 19:17:56.000000 matlabengine-9.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 19:17:56.000000 matlabengine-9.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:18:08.251824 matlabengine-9.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-05 19:17:56.000000 matlabengine-9.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:18:08.247824 matlabengine-9.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:18:08.247824 matlabengine-9.9.4/src/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:18:08.247824 matlabengine-9.9.4/src/matlab/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/_internal/mlarray_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/_internal/mlarray_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:18:08.251824 matlabengine-9.9.4/src/matlab/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/engine/basefuture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/engine/engineerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/engine/enginehelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/engine/enginesession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/engine/fevalfuture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/engine/futureresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/engine/matlabengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/engine/matlabfuture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/mlarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-05 19:17:56.000000 matlabengine-9.9.4/src/matlab/mlexceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:18:08.251824 matlabengine-9.9.4/src/matlabengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-05 19:18:08.000000 matlabengine-9.9.4/src/matlabengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-05 19:18:08.000000 matlabengine-9.9.4/src/matlabengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:18:08.000000 matlabengine-9.9.4/src/matlabengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:18:08.000000 matlabengine-9.9.4/src/matlabengine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 19:18:08.000000 matlabengine-9.9.4/src/matlabengine.egg-info/top_level.txt
```

### Comparing `matlabengine-9.9.1/LICENSE.txt` & `matlabengine-9.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/PKG-INFO` & `matlabengine-9.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: matlabengine
-Version: 9.9.1
+Version: 9.9.4
 Summary: A module to call MATLAB from Python
 Home-page: https://github.com/mathworks/matlab-engine-for-python/
 Author: MathWorks
-License: MathWorks XSLA License
+License: LICENSE.txt, located in this repository
 Project-URL: Documentation, https://www.mathworks.com/help/matlab/matlab-engine-for-python.html
 Project-URL: Source, https://github.com/mathworks/matlab-engine-for-python
 Project-URL: Tracker, https://github.com/mathworks/matlab-engine-for-python/issues
 Keywords: MATLAB,MATLAB Engine for Python
 Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -38,15 +38,15 @@
 
 ## Install
 
 ### Windows
 MATLAB Engine API for Python can be installed directly from the Python Package Index.
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```bash
-$ python -m pip install matlabengine==9.9.1
+$ python -m pip install matlabengine==9.9.4
 ```
 
 
 
 ### Linux&reg; 
 Prior to installation, check the default install location of MATLAB by calling ```matlabroot``` in a MATLAB Command Window. By default, Linux installs MATLAB at:<br>
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
@@ -63,15 +63,15 @@
 # in .tcshrc
 setenv LD_LIBRARY_PATH ${LD_LIBRARY_PATH}:<matlabroot>/bin/glnxa64
 ```
 
 MATLAB Engine API for Python can be installed directly from the Python Package Index.
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```bash
-$ python -m pip install matlabengine==9.9.1
+$ python -m pip install matlabengine==9.9.4
 ```
 
 ### macOS
 Prior to installation, check the default install location of MATLAB by calling ```matlabroot``` in a MATLAB Command Window. By default, macOS installs MATLAB at:<br>
 
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```/Applications/MATLAB_R2020b.app```
@@ -87,15 +87,15 @@
 # in .tcshrc
 setenv DYLD_LIBRARY_PATH ${DYLD_LIBRARY_PATH}:<matlabroot>/bin/maci64
 ```
 
 MATLAB Engine API for Python can be installed directly from the Python Package Index.
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```bash
-$ python -m pip install matlabengine==9.9.1
+$ python -m pip install matlabengine==9.9.4
 ```
 
 ---
 
 ## Getting Started
 * Start Python.
 * Import the ```matlab.engine``` package into the Python session.
@@ -139,15 +139,15 @@
 
 ## Troubleshooting
 See [Troubleshoot MATLAB Errors in Python](https://www.mathworks.com/help/matlab/matlab_external/troubleshoot-matlab-errors-in-python.html) for troubleshooting assistance.
 
 ---
 
 ## License
-This software is licensed under the MathWorks XSLA License, which is available in the LICENSE.txt file within this repository.
+The license is available in the LICENSE.txt file within this repository.
 
 ---
 
 ## Support
 Technical issues or enhancement requests can be submitted [here](https://github.com/mathworks/matlab-engine-for-python/issues). 
 
 ---
```

### Comparing `matlabengine-9.9.1/README.md` & `matlabengine-9.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ## Install
 
 ### Windows
 MATLAB Engine API for Python can be installed directly from the Python Package Index.
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```bash
-$ python -m pip install matlabengine==9.9.1
+$ python -m pip install matlabengine==9.9.4
 ```
 
 
 
 ### Linux&reg; 
 Prior to installation, check the default install location of MATLAB by calling ```matlabroot``` in a MATLAB Command Window. By default, Linux installs MATLAB at:<br>
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
@@ -42,15 +42,15 @@
 # in .tcshrc
 setenv LD_LIBRARY_PATH ${LD_LIBRARY_PATH}:<matlabroot>/bin/glnxa64
 ```
 
 MATLAB Engine API for Python can be installed directly from the Python Package Index.
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```bash
-$ python -m pip install matlabengine==9.9.1
+$ python -m pip install matlabengine==9.9.4
 ```
 
 ### macOS
 Prior to installation, check the default install location of MATLAB by calling ```matlabroot``` in a MATLAB Command Window. By default, macOS installs MATLAB at:<br>
 
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```/Applications/MATLAB_R2020b.app```
@@ -66,15 +66,15 @@
 # in .tcshrc
 setenv DYLD_LIBRARY_PATH ${DYLD_LIBRARY_PATH}:<matlabroot>/bin/maci64
 ```
 
 MATLAB Engine API for Python can be installed directly from the Python Package Index.
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```bash
-$ python -m pip install matlabengine==9.9.1
+$ python -m pip install matlabengine==9.9.4
 ```
 
 ---
 
 ## Getting Started
 * Start Python.
 * Import the ```matlab.engine``` package into the Python session.
@@ -118,15 +118,15 @@
 
 ## Troubleshooting
 See [Troubleshoot MATLAB Errors in Python](https://www.mathworks.com/help/matlab/matlab_external/troubleshoot-matlab-errors-in-python.html) for troubleshooting assistance.
 
 ---
 
 ## License
-This software is licensed under the MathWorks XSLA License, which is available in the LICENSE.txt file within this repository.
+The license is available in the LICENSE.txt file within this repository.
 
 ---
 
 ## Support
 Technical issues or enhancement requests can be submitted [here](https://github.com/mathworks/matlab-engine-for-python/issues). 
 
 ---
```

### Comparing `matlabengine-9.9.1/setup.py` & `matlabengine-9.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         'Darwin': 'DYLD_LIBRARY_PATH'
     }
     
     # MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string)
     MATLAB_REL = 'R2020b'
 
     # MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string)
-    MATLAB_VER = '9.9.1' 
+    MATLAB_VER = '9.9.4' 
 
     # MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string)
     SUPPORTED_PYTHON_VERSIONS = set(['3.6', '3.7', '3.8'])
 
     # MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string)
     VER_TO_REL = {
         "9.9": "R2020b",
@@ -204,16 +204,15 @@
         eng_major_minor = self._get_engine_ver_major_minor()
         matlab_ver_major_minor = (matlab_ver_match.group(1), matlab_ver_match.group(2))
         return (matlab_ver_major_minor == eng_major_minor)
     
     def verify_matlab_release(self, root):
         """
         Parses VersionInfo.xml to verify the MATLAB release matches the supported release
-        for the Python Engine. The major and minor version numbers must match. Everything
-        else will be ignored.
+        for the Python Engine.
         """
         version_info = os.path.join(root, 'VersionInfo.xml')
         if not os.path.isfile(version_info):
             return False
         
         tree = xml.parse(version_info)
         tree_root = tree.getroot()
@@ -304,18 +303,18 @@
 if __name__ == '__main__':
     with open('README.md', 'r', encoding='utf-8') as rm:
         long_description = rm.read()
 
     setup(
         name="matlabengine",
         # MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string)
-        version="9.9.1",
+        version="9.9.4",
         description='A module to call MATLAB from Python',
         author='MathWorks',
-        license="MathWorks XSLA License",
+        license="LICENSE.txt, located in this repository",
         url='https://github.com/mathworks/matlab-engine-for-python/',
         long_description=long_description,
         long_description_content_type="text/markdown",
         package_dir={'': 'src'},
         packages=find_packages(where="src"),
         cmdclass={'build_py': _MatlabFinder},
         package_data={'': ['_arch.txt']},
```

### Comparing `matlabengine-9.9.1/src/matlab/__init__.py` & `matlabengine-9.9.4/src/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/_internal/mlarray_sequence.py` & `matlabengine-9.9.4/src/matlab/_internal/mlarray_sequence.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/_internal/mlarray_utils.py` & `matlabengine-9.9.4/src/matlab/_internal/mlarray_utils.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/engine/__init__.py` & `matlabengine-9.9.4/src/matlab/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/engine/basefuture.py` & `matlabengine-9.9.4/src/matlab/engine/basefuture.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/engine/enginehelper.py` & `matlabengine-9.9.4/src/matlab/engine/enginehelper.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/engine/enginesession.py` & `matlabengine-9.9.4/src/matlab/engine/enginesession.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/engine/fevalfuture.py` & `matlabengine-9.9.4/src/matlab/engine/fevalfuture.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/engine/futureresult.py` & `matlabengine-9.9.4/src/matlab/engine/futureresult.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/engine/matlabengine.py` & `matlabengine-9.9.4/src/matlab/engine/matlabengine.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/engine/matlabfuture.py` & `matlabengine-9.9.4/src/matlab/engine/matlabfuture.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/mlarray.py` & `matlabengine-9.9.4/src/matlab/mlarray.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlab/mlexceptions.py` & `matlabengine-9.9.4/src/matlab/mlexceptions.py`

 * *Files identical despite different names*

### Comparing `matlabengine-9.9.1/src/matlabengine.egg-info/PKG-INFO` & `matlabengine-9.9.4/src/matlabengine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: matlabengine
-Version: 9.9.1
+Version: 9.9.4
 Summary: A module to call MATLAB from Python
 Home-page: https://github.com/mathworks/matlab-engine-for-python/
 Author: MathWorks
-License: MathWorks XSLA License
+License: LICENSE.txt, located in this repository
 Project-URL: Documentation, https://www.mathworks.com/help/matlab/matlab-engine-for-python.html
 Project-URL: Source, https://github.com/mathworks/matlab-engine-for-python
 Project-URL: Tracker, https://github.com/mathworks/matlab-engine-for-python/issues
 Keywords: MATLAB,MATLAB Engine for Python
 Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -38,15 +38,15 @@
 
 ## Install
 
 ### Windows
 MATLAB Engine API for Python can be installed directly from the Python Package Index.
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```bash
-$ python -m pip install matlabengine==9.9.1
+$ python -m pip install matlabengine==9.9.4
 ```
 
 
 
 ### Linux&reg; 
 Prior to installation, check the default install location of MATLAB by calling ```matlabroot``` in a MATLAB Command Window. By default, Linux installs MATLAB at:<br>
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
@@ -63,15 +63,15 @@
 # in .tcshrc
 setenv LD_LIBRARY_PATH ${LD_LIBRARY_PATH}:<matlabroot>/bin/glnxa64
 ```
 
 MATLAB Engine API for Python can be installed directly from the Python Package Index.
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```bash
-$ python -m pip install matlabengine==9.9.1
+$ python -m pip install matlabengine==9.9.4
 ```
 
 ### macOS
 Prior to installation, check the default install location of MATLAB by calling ```matlabroot``` in a MATLAB Command Window. By default, macOS installs MATLAB at:<br>
 
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```/Applications/MATLAB_R2020b.app```
@@ -87,15 +87,15 @@
 # in .tcshrc
 setenv DYLD_LIBRARY_PATH ${DYLD_LIBRARY_PATH}:<matlabroot>/bin/maci64
 ```
 
 MATLAB Engine API for Python can be installed directly from the Python Package Index.
 <!-- MUST_BE_UPDATED_EACH_RELEASE (Search repo for this string) -->
 ```bash
-$ python -m pip install matlabengine==9.9.1
+$ python -m pip install matlabengine==9.9.4
 ```
 
 ---
 
 ## Getting Started
 * Start Python.
 * Import the ```matlab.engine``` package into the Python session.
@@ -139,15 +139,15 @@
 
 ## Troubleshooting
 See [Troubleshoot MATLAB Errors in Python](https://www.mathworks.com/help/matlab/matlab_external/troubleshoot-matlab-errors-in-python.html) for troubleshooting assistance.
 
 ---
 
 ## License
-This software is licensed under the MathWorks XSLA License, which is available in the LICENSE.txt file within this repository.
+The license is available in the LICENSE.txt file within this repository.
 
 ---
 
 ## Support
 Technical issues or enhancement requests can be submitted [here](https://github.com/mathworks/matlab-engine-for-python/issues). 
 
 ---
```

### Comparing `matlabengine-9.9.1/src/matlabengine.egg-info/SOURCES.txt` & `matlabengine-9.9.4/src/matlabengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

