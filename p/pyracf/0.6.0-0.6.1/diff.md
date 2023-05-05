# Comparing `tmp/pyracf-0.6.0.tar.gz` & `tmp/pyracf-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.6.0.tar", last modified: Fri May  5 13:32:40 2023, max compression
+gzip compressed data, was "pyracf-0.6.1.tar", last modified: Fri May  5 19:34:07 2023, max compression
```

## Comparing `pyracf-0.6.0.tar` & `pyracf-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 13:32:40.627825 pyracf-0.6.0/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.6.0/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.6.0/MANIFEST.in
--rw-rw-r--   0 henri     (1000) henri     (1000)     7928 2023-05-05 13:32:40.627825 pyracf-0.6.0/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)     7403 2023-05-05 13:22:15.000000 pyracf-0.6.0/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-05 13:32:40.627825 pyracf-0.6.0/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-05 13:21:36.000000 pyracf-0.6.0/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 13:32:40.627825 pyracf-0.6.0/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 13:32:40.627825 pyracf-0.6.0/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    33417 2023-05-05 10:00:54.000000 pyracf-0.6.0/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   126402 2023-05-05 13:28:47.000000 pyracf-0.6.0/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 13:32:40.627825 pyracf-0.6.0/src/pyracf.egg-info/
--rw-rw-r--   0 henri     (1000) henri     (1000)     7928 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 19:34:07.114300 pyracf-0.6.1/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.6.1/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.6.1/MANIFEST.in
+-rw-rw-r--   0 henri     (1000) henri     (1000)     8019 2023-05-05 19:34:07.114300 pyracf-0.6.1/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7494 2023-05-05 19:33:48.000000 pyracf-0.6.1/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-05 19:34:07.114300 pyracf-0.6.1/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-05 19:33:03.000000 pyracf-0.6.1/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 19:34:07.114300 pyracf-0.6.1/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 19:34:07.114300 pyracf-0.6.1/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    33417 2023-05-05 10:00:54.000000 pyracf-0.6.1/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   126403 2023-05-05 19:32:44.000000 pyracf-0.6.1/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 19:34:07.114300 pyracf-0.6.1/src/pyracf.egg-info/
+-rw-rw-r--   0 henri     (1000) henri     (1000)     8019 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.6.0/LICENSE` & `pyracf-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.6.0/PKG-INFO` & `pyracf-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.6.0
+Version: 0.6.1
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,21 +26,22 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
-### 0.6.0 (Bug free?)
+### 0.6.1 (Bug free?)
 - XLS generation fully functional again (also for z/VM unloads)
 - Oprhan detection working again
 - Conditional Dataset Access Records now parsing correctly
 - Conditional Dataset Access now correctly pickled :)
 - Fixed parsing of GRCACC records (had misparsed AUTH_ID)
-
+- Conditional Generic (General) Records now with correct column name (GRCACC_CLASS_NAME)
+  
 ### 0.5.4 (Even more recordtypes!!)
 - new property: genericConditionalAccess. Will show GRCACC records.
 - Fixed some nasty 'default recordtypes' bugs
   
 ### 0.5.0 (Pickle FTW!)
 
 - new function: save_pickles(path=path, prefix=prefix). Will save all parsed dataframes as pickles (/path/_prefix_*RECORDTYPE*.pickle)
```

### Comparing `pyracf-0.6.0/README.md` & `pyracf-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
-### 0.6.0 (Bug free?)
+### 0.6.1 (Bug free?)
 - XLS generation fully functional again (also for z/VM unloads)
 - Oprhan detection working again
 - Conditional Dataset Access Records now parsing correctly
 - Conditional Dataset Access now correctly pickled :)
 - Fixed parsing of GRCACC records (had misparsed AUTH_ID)
-
+- Conditional Generic (General) Records now with correct column name (GRCACC_CLASS_NAME)
+  
 ### 0.5.4 (Even more recordtypes!!)
 - new property: genericConditionalAccess. Will show GRCACC records.
 - Fixed some nasty 'default recordtypes' bugs
   
 ### 0.5.0 (Pickle FTW!)
 
 - new function: save_pickles(path=path, prefix=prefix). Will save all parsed dataframes as pickles (/path/_prefix_*RECORDTYPE*.pickle)
```

### Comparing `pyracf-0.6.0/setup.py` & `pyracf-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.6.0",
+    version="0.6.1",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.6.0/src/pyracf/__init__.py` & `pyracf-0.6.1/src/pyracf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.6.0/src/pyracf/offsets.json` & `pyracf-0.6.1/src/pyracf/offsets.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999829931972789%*

 * *Differences: {"'general-resource-conditional-access-record'": "{'offsets': {2: {'field-name': "*

 * *                                                 "'GRCACC_CLASS_NAME'}}}"}*

```diff
@@ -867,15 +867,15 @@
                 "field-name": "GRCACC_NAME",
                 "start": "6",
                 "type": "Char"
             },
             {
                 "end": "260",
                 "field-desc": "Name of the class to which the general resource profile belongs.",
-                "field-name": "GRACC_CLASS_NAME",
+                "field-name": "GRCACC_CLASS_NAME",
                 "start": "253",
                 "type": "Char"
             },
             {
                 "end": "269",
                 "field-desc": "The type of conditional access checking that is being performed. Valid values are CONSOLE, TERMINAL, JESINPUT, SYSID, APPCPORT, SERVAUTH, PROGRAM, and CRITERIA.",
                 "field-name": "GRCACC_CATYPE",
```

### Comparing `pyracf-0.6.0/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.6.1/src/pyracf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.6.0
+Version: 0.6.1
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,21 +26,22 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
-### 0.6.0 (Bug free?)
+### 0.6.1 (Bug free?)
 - XLS generation fully functional again (also for z/VM unloads)
 - Oprhan detection working again
 - Conditional Dataset Access Records now parsing correctly
 - Conditional Dataset Access now correctly pickled :)
 - Fixed parsing of GRCACC records (had misparsed AUTH_ID)
-
+- Conditional Generic (General) Records now with correct column name (GRCACC_CLASS_NAME)
+  
 ### 0.5.4 (Even more recordtypes!!)
 - new property: genericConditionalAccess. Will show GRCACC records.
 - Fixed some nasty 'default recordtypes' bugs
   
 ### 0.5.0 (Pickle FTW!)
 
 - new function: save_pickles(path=path, prefix=prefix). Will save all parsed dataframes as pickles (/path/_prefix_*RECORDTYPE*.pickle)
```

