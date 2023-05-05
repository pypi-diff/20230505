# Comparing `tmp/pyracf-0.5.9.tar.gz` & `tmp/pyracf-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.5.9.tar", last modified: Fri May  5 10:02:09 2023, max compression
+gzip compressed data, was "pyracf-0.6.0.tar", last modified: Fri May  5 13:32:40 2023, max compression
```

## Comparing `pyracf-0.5.9.tar` & `pyracf-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 10:02:09.927516 pyracf-0.5.9/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.5.9/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.5.9/MANIFEST.in
--rw-rw-r--   0 henri     (1000) henri     (1000)     7873 2023-05-05 10:02:09.927516 pyracf-0.5.9/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)     7348 2023-05-05 10:02:02.000000 pyracf-0.5.9/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-05 10:02:09.927516 pyracf-0.5.9/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-05 10:01:02.000000 pyracf-0.5.9/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 10:02:09.923516 pyracf-0.5.9/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 10:02:09.923516 pyracf-0.5.9/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    33417 2023-05-05 10:00:54.000000 pyracf-0.5.9/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   125683 2023-05-01 20:17:28.000000 pyracf-0.5.9/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 10:02:09.927516 pyracf-0.5.9/src/pyracf.egg-info/
--rw-rw-r--   0 henri     (1000) henri     (1000)     7873 2023-05-05 10:02:09.000000 pyracf-0.5.9/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-05 10:02:09.000000 pyracf-0.5.9/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-05 10:02:09.000000 pyracf-0.5.9/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-05 10:02:09.000000 pyracf-0.5.9/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-05 10:02:09.000000 pyracf-0.5.9/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 13:32:40.627825 pyracf-0.6.0/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.6.0/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.6.0/MANIFEST.in
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7928 2023-05-05 13:32:40.627825 pyracf-0.6.0/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7403 2023-05-05 13:22:15.000000 pyracf-0.6.0/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-05 13:32:40.627825 pyracf-0.6.0/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-05 13:21:36.000000 pyracf-0.6.0/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 13:32:40.627825 pyracf-0.6.0/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 13:32:40.627825 pyracf-0.6.0/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    33417 2023-05-05 10:00:54.000000 pyracf-0.6.0/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   126402 2023-05-05 13:28:47.000000 pyracf-0.6.0/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 13:32:40.627825 pyracf-0.6.0/src/pyracf.egg-info/
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7928 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-05 13:32:40.000000 pyracf-0.6.0/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.5.9/LICENSE` & `pyracf-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.5.9/PKG-INFO` & `pyracf-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.5.9
+Version: 0.6.0
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,19 +26,20 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
-### 0.5.9 (Bugsquashing)
+### 0.6.0 (Bug free?)
 - XLS generation fully functional again (also for z/VM unloads)
 - Oprhan detection working again
 - Conditional Dataset Access Records now parsing correctly
 - Conditional Dataset Access now correctly pickled :)
+- Fixed parsing of GRCACC records (had misparsed AUTH_ID)
 
 ### 0.5.4 (Even more recordtypes!!)
 - new property: genericConditionalAccess. Will show GRCACC records.
 - Fixed some nasty 'default recordtypes' bugs
   
 ### 0.5.0 (Pickle FTW!)
```

### Comparing `pyracf-0.5.9/README.md` & `pyracf-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
-### 0.5.9 (Bugsquashing)
+### 0.6.0 (Bug free?)
 - XLS generation fully functional again (also for z/VM unloads)
 - Oprhan detection working again
 - Conditional Dataset Access Records now parsing correctly
 - Conditional Dataset Access now correctly pickled :)
+- Fixed parsing of GRCACC records (had misparsed AUTH_ID)
 
 ### 0.5.4 (Even more recordtypes!!)
 - new property: genericConditionalAccess. Will show GRCACC records.
 - Fixed some nasty 'default recordtypes' bugs
   
 ### 0.5.0 (Pickle FTW!)
```

### Comparing `pyracf-0.5.9/setup.py` & `pyracf-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.5.9",
+    version="0.6.0",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.5.9/src/pyracf/__init__.py` & `pyracf-0.6.0/src/pyracf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.5.9/src/pyracf/offsets.json` & `pyracf-0.6.0/src/pyracf/offsets.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999829931972789%*

 * *Differences: {"'general-resource-conditional-access-record'": "{'offsets': {6: {'field-name': "*

 * *                                                 "'GRCACC_ACCESS'}}}"}*

```diff
@@ -895,15 +895,15 @@
                 "field-name": "GRCACC_AUTH_ID",
                 "start": "280",
                 "type": "Char"
             },
             {
                 "end": "296",
                 "field-desc": "The authority of the conditional access element/user combination. Valid values are NONE, READ, UPDATE, CONTROL, and ALTER.",
-                "field-name": "GRCACC_AUTH_ID",
+                "field-name": "GRCACC_ACCESS",
                 "start": "289",
                 "type": "Char"
             },
             {
                 "end": "302",
                 "field-desc": "The number of times that the general resource was accessed.",
                 "field-name": "GRCACC_ACCESS_CNT",
```

### Comparing `pyracf-0.5.9/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.6.0/src/pyracf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.5.9
+Version: 0.6.0
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,19 +26,20 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
-### 0.5.9 (Bugsquashing)
+### 0.6.0 (Bug free?)
 - XLS generation fully functional again (also for z/VM unloads)
 - Oprhan detection working again
 - Conditional Dataset Access Records now parsing correctly
 - Conditional Dataset Access now correctly pickled :)
+- Fixed parsing of GRCACC records (had misparsed AUTH_ID)
 
 ### 0.5.4 (Even more recordtypes!!)
 - new property: genericConditionalAccess. Will show GRCACC records.
 - Fixed some nasty 'default recordtypes' bugs
   
 ### 0.5.0 (Pickle FTW!)
```

