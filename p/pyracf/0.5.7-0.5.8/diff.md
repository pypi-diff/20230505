# Comparing `tmp/pyracf-0.5.7.tar.gz` & `tmp/pyracf-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.5.7.tar", last modified: Fri May  5 09:33:30 2023, max compression
+gzip compressed data, was "pyracf-0.5.8.tar", last modified: Fri May  5 09:36:57 2023, max compression
```

## Comparing `pyracf-0.5.7.tar` & `pyracf-0.5.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:33:30.663992 pyracf-0.5.7/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.5.7/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.5.7/MANIFEST.in
--rw-rw-r--   0 henri     (1000) henri     (1000)     7637 2023-05-05 09:33:30.663992 pyracf-0.5.7/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)     7112 2023-05-01 20:31:25.000000 pyracf-0.5.7/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-05 09:33:30.663992 pyracf-0.5.7/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-05 09:32:23.000000 pyracf-0.5.7/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:33:30.659992 pyracf-0.5.7/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:33:30.659992 pyracf-0.5.7/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    33415 2023-05-05 09:17:24.000000 pyracf-0.5.7/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   125683 2023-05-01 20:17:28.000000 pyracf-0.5.7/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:33:30.659992 pyracf-0.5.7/src/pyracf.egg-info/
--rw-rw-r--   0 henri     (1000) henri     (1000)     7637 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:36:57.813152 pyracf-0.5.8/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.5.8/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.5.8/MANIFEST.in
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7819 2023-05-05 09:36:57.813152 pyracf-0.5.8/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7294 2023-05-05 09:36:47.000000 pyracf-0.5.8/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-05 09:36:57.813152 pyracf-0.5.8/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-05 09:34:54.000000 pyracf-0.5.8/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:36:57.813152 pyracf-0.5.8/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:36:57.813152 pyracf-0.5.8/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    33415 2023-05-05 09:17:24.000000 pyracf-0.5.8/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   125683 2023-05-01 20:17:28.000000 pyracf-0.5.8/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:36:57.813152 pyracf-0.5.8/src/pyracf.egg-info/
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7819 2023-05-05 09:36:57.000000 pyracf-0.5.8/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-05 09:36:57.000000 pyracf-0.5.8/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-05 09:36:57.000000 pyracf-0.5.8/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-05 09:36:57.000000 pyracf-0.5.8/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-05 09:36:57.000000 pyracf-0.5.8/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.5.7/LICENSE` & `pyracf-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.5.7/PKG-INFO` & `pyracf-0.5.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pyracf
-Version: 0.5.7
-Summary: Parsing IRRDBU00 unloads in panda dataframes.
-Home-page: https://github.com/wizardofzos/pyracf
-Author: Wizard of z/OS
-Author-email: wizard@zdevops.com
-Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyracf
 
 ## PyRACF: A Python module for analyzing RACF security
 
 PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database, providing an efficient and intuitive way to analyze security setups on IBM Z systems. By consuming the IRRDBU00 unload, PyRACF generates "Panda DataFrames" for each 'recordtype', which allow for seamless manipulation and analysis of the data.
 
 Pandas is a powerful data manipulation library in Python that allows for easy querying of the DataFrames generated by PyRACF. With Pandas, you can perform complex queries on the security data to extract meaningful insights into the security posture of your system.
@@ -26,14 +11,19 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.5.8 (Bugsquashing)
+- XLS generation fully functional again (also for z/VM unloads)
+- Oprhan detection working again
+- Conditional Dataset Access Records now parsing correctly
+
 ### 0.5.4 (Even more recordtypes!!)
 - new property: genericConditionalAccess. Will show GRCACC records.
 - Fixed some nasty 'default recordtypes' bugs
   
 ### 0.5.0 (Pickle FTW!)
 
 - new function: save_pickles(path=path, prefix=prefix). Will save all parsed dataframes as pickles (/path/_prefix_*RECORDTYPE*.pickle)
```

### Comparing `pyracf-0.5.7/README.md` & `pyracf-0.5.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pyracf
+Version: 0.5.8
+Summary: Parsing IRRDBU00 unloads in panda dataframes.
+Home-page: https://github.com/wizardofzos/pyracf
+Author: Wizard of z/OS
+Author-email: wizard@zdevops.com
+Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyracf
 
 ## PyRACF: A Python module for analyzing RACF security
 
 PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database, providing an efficient and intuitive way to analyze security setups on IBM Z systems. By consuming the IRRDBU00 unload, PyRACF generates "Panda DataFrames" for each 'recordtype', which allow for seamless manipulation and analysis of the data.
 
 Pandas is a powerful data manipulation library in Python that allows for easy querying of the DataFrames generated by PyRACF. With Pandas, you can perform complex queries on the security data to extract meaningful insights into the security posture of your system.
@@ -11,14 +26,19 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.5.8 (Bugsquashing)
+- XLS generation fully functional again (also for z/VM unloads)
+- Oprhan detection working again
+- Conditional Dataset Access Records now parsing correctly
+
 ### 0.5.4 (Even more recordtypes!!)
 - new property: genericConditionalAccess. Will show GRCACC records.
 - Fixed some nasty 'default recordtypes' bugs
   
 ### 0.5.0 (Pickle FTW!)
 
 - new function: save_pickles(path=path, prefix=prefix). Will save all parsed dataframes as pickles (/path/_prefix_*RECORDTYPE*.pickle)
```

### Comparing `pyracf-0.5.7/setup.py` & `pyracf-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.5.7",
+    version="0.5.8",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.5.7/src/pyracf/__init__.py` & `pyracf-0.5.8/src/pyracf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.5.7/src/pyracf/offsets.json` & `pyracf-0.5.8/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.5.7/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.5.8/src/pyracf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.5.7
+Version: 0.5.8
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,14 +26,19 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.5.8 (Bugsquashing)
+- XLS generation fully functional again (also for z/VM unloads)
+- Oprhan detection working again
+- Conditional Dataset Access Records now parsing correctly
+
 ### 0.5.4 (Even more recordtypes!!)
 - new property: genericConditionalAccess. Will show GRCACC records.
 - Fixed some nasty 'default recordtypes' bugs
   
 ### 0.5.0 (Pickle FTW!)
 
 - new function: save_pickles(path=path, prefix=prefix). Will save all parsed dataframes as pickles (/path/_prefix_*RECORDTYPE*.pickle)
```

