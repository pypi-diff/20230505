# Comparing `tmp/pyracf-0.5.4.tar.gz` & `tmp/pyracf-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.5.4.tar", last modified: Mon May  1 20:21:10 2023, max compression
+gzip compressed data, was "pyracf-0.5.7.tar", last modified: Fri May  5 09:33:30 2023, max compression
```

## Comparing `pyracf-0.5.4.tar` & `pyracf-0.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-01 20:21:10.419753 pyracf-0.5.4/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.5.4/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.5.4/MANIFEST.in
--rw-rw-r--   0 henri     (1000) henri     (1000)     6604 2023-05-01 20:21:10.419753 pyracf-0.5.4/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)     6079 2023-03-26 14:05:05.000000 pyracf-0.5.4/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-01 20:21:10.419753 pyracf-0.5.4/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-01 20:21:04.000000 pyracf-0.5.4/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-01 20:21:10.415753 pyracf-0.5.4/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-01 20:21:10.415753 pyracf-0.5.4/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    33323 2023-05-01 20:17:28.000000 pyracf-0.5.4/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   125683 2023-05-01 20:17:28.000000 pyracf-0.5.4/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-01 20:21:10.419753 pyracf-0.5.4/src/pyracf.egg-info/
--rw-rw-r--   0 henri     (1000) henri     (1000)     6604 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:33:30.663992 pyracf-0.5.7/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.5.7/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.5.7/MANIFEST.in
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7637 2023-05-05 09:33:30.663992 pyracf-0.5.7/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7112 2023-05-01 20:31:25.000000 pyracf-0.5.7/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-05 09:33:30.663992 pyracf-0.5.7/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-05 09:32:23.000000 pyracf-0.5.7/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:33:30.659992 pyracf-0.5.7/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:33:30.659992 pyracf-0.5.7/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    33415 2023-05-05 09:17:24.000000 pyracf-0.5.7/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   125683 2023-05-01 20:17:28.000000 pyracf-0.5.7/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 09:33:30.659992 pyracf-0.5.7/src/pyracf.egg-info/
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7637 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-05 09:33:30.000000 pyracf-0.5.7/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.5.4/LICENSE` & `pyracf-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.5.4/PKG-INFO` & `pyracf-0.5.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.5.4
+Version: 0.5.7
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyracf
 
-PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database. It consumes the IRRDBU00 unload and creates "Panda DataFrames" for every 'recordtype', allowing for easy manipulation and analysis of the data. With the new release, PyRACF now supports saving and loading pickle files, making it easier than ever to work with large RACF datasets. See https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types and https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility for a description of these records. The DataFrames will have the same 'fieldnames' as described in the docs. Install PyRACF with pip install pyracf or check out the source code on GitHub: https://github.com/wizardofzos/pyracf/releases/latest. Get started with PyRACF today and take control of your RACF data like never before!
+## PyRACF: A Python module for analyzing RACF security
+
+PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database, providing an efficient and intuitive way to analyze security setups on IBM Z systems. By consuming the IRRDBU00 unload, PyRACF generates "Panda DataFrames" for each 'recordtype', which allow for seamless manipulation and analysis of the data.
+
+Pandas is a powerful data manipulation library in Python that allows for easy querying of the DataFrames generated by PyRACF. With Pandas, you can perform complex queries on the security data to extract meaningful insights into the security posture of your system.
+
+PyRACF's support for saving and loading pickle files makes it easier than ever to work with large RACF datasets, giving you the ability to perform comprehensive analyses of your security setup.
+
+For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
+
+To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
+
 
 ## Updates
 
+### 0.5.4 (Even more recordtypes!!)
+- new property: genericConditionalAccess. Will show GRCACC records.
+- Fixed some nasty 'default recordtypes' bugs
+  
 ### 0.5.0 (Pickle FTW!)
 
 - new function: save_pickles(path=path, prefix=prefix). Will save all parsed dataframes as pickles (/path/_prefix_*RECORDTYPE*.pickle)
 - Can now initialize RACF object from pickle-folder/prefix. To reuse earlier saves pickle files. See examples below
 - parse_fancycli now has two optional arguments (save_pickles and prefix) to also save pickle files after parsing to the directory as specified in save_pickles. The prefix argument is only useed with save_pickles isn't False
 
 ### 0.4.5 (Fix Community Update Bug, thanks @Martydog)
@@ -75,14 +90,15 @@
 | Function/Property | Explanation | Example |
 |---|---|---|
 | auditors | Returns DataFrame with all user having the auditor bit switched on | mysys.auditors |
 | connects | Returns DataFrame with all user to group connects | mysys.connects |
 | datasetAccess | Returns DataFrame with all Accesslists for all dataset profiles | mysys.datasetsAccess |
 | datasets | Returns DataFrame with all datasetprofiles | mysys.datasets |
 | genericAccess | Returns DataFrame with with all accesslists for generic resource profiles | mysys.genericAccess
+| genericConditionalAccess | Returns DataFrame with with all conditional accesslists for generic resource profiles | mysys.genericConditionalAccess
 | generics | Returns DataFrame with with all generic resource profiles | mysys.generics 
 | group | Returns DataFrame with with one dataset profile only | mysys.group('SYS1') |
 | groupConnect | Returns DataFrame with with user group connection records (0203 recordtype) | mysys.groupConnect |
 | groups | Returns DataFrame with all group data | mysys.groups |
 | installdata | Returns DataFrame with with user installation data (0204 recordtype) | mysys.installdata |
 | operations | Returns a DataFrame  with all operations users | mysys.operations |
 | orphans | Returns 2 DataFrames one with orphans in dataset profile access lists, and one for generic resources | d, g = mysys.orphans |
```

### Comparing `pyracf-0.5.4/README.md` & `pyracf-0.5.7/src/pyracf.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,43 @@
+Metadata-Version: 2.1
+Name: pyracf
+Version: 0.5.7
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
 
-PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database. It consumes the IRRDBU00 unload and creates "Panda DataFrames" for every 'recordtype', allowing for easy manipulation and analysis of the data. With the new release, PyRACF now supports saving and loading pickle files, making it easier than ever to work with large RACF datasets. See https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types and https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility for a description of these records. The DataFrames will have the same 'fieldnames' as described in the docs. Install PyRACF with pip install pyracf or check out the source code on GitHub: https://github.com/wizardofzos/pyracf/releases/latest. Get started with PyRACF today and take control of your RACF data like never before!
+## PyRACF: A Python module for analyzing RACF security
+
+PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database, providing an efficient and intuitive way to analyze security setups on IBM Z systems. By consuming the IRRDBU00 unload, PyRACF generates "Panda DataFrames" for each 'recordtype', which allow for seamless manipulation and analysis of the data.
+
+Pandas is a powerful data manipulation library in Python that allows for easy querying of the DataFrames generated by PyRACF. With Pandas, you can perform complex queries on the security data to extract meaningful insights into the security posture of your system.
+
+PyRACF's support for saving and loading pickle files makes it easier than ever to work with large RACF datasets, giving you the ability to perform comprehensive analyses of your security setup.
+
+For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
+
+To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
+
 
 ## Updates
 
+### 0.5.4 (Even more recordtypes!!)
+- new property: genericConditionalAccess. Will show GRCACC records.
+- Fixed some nasty 'default recordtypes' bugs
+  
 ### 0.5.0 (Pickle FTW!)
 
 - new function: save_pickles(path=path, prefix=prefix). Will save all parsed dataframes as pickles (/path/_prefix_*RECORDTYPE*.pickle)
 - Can now initialize RACF object from pickle-folder/prefix. To reuse earlier saves pickle files. See examples below
 - parse_fancycli now has two optional arguments (save_pickles and prefix) to also save pickle files after parsing to the directory as specified in save_pickles. The prefix argument is only useed with save_pickles isn't False
 
 ### 0.4.5 (Fix Community Update Bug, thanks @Martydog)
@@ -60,14 +90,15 @@
 | Function/Property | Explanation | Example |
 |---|---|---|
 | auditors | Returns DataFrame with all user having the auditor bit switched on | mysys.auditors |
 | connects | Returns DataFrame with all user to group connects | mysys.connects |
 | datasetAccess | Returns DataFrame with all Accesslists for all dataset profiles | mysys.datasetsAccess |
 | datasets | Returns DataFrame with all datasetprofiles | mysys.datasets |
 | genericAccess | Returns DataFrame with with all accesslists for generic resource profiles | mysys.genericAccess
+| genericConditionalAccess | Returns DataFrame with with all conditional accesslists for generic resource profiles | mysys.genericConditionalAccess
 | generics | Returns DataFrame with with all generic resource profiles | mysys.generics 
 | group | Returns DataFrame with with one dataset profile only | mysys.group('SYS1') |
 | groupConnect | Returns DataFrame with with user group connection records (0203 recordtype) | mysys.groupConnect |
 | groups | Returns DataFrame with all group data | mysys.groups |
 | installdata | Returns DataFrame with with user installation data (0204 recordtype) | mysys.installdata |
 | operations | Returns a DataFrame  with all operations users | mysys.operations |
 | orphans | Returns 2 DataFrames one with orphans in dataset profile access lists, and one for generic resources | d, g = mysys.orphans |
```

### Comparing `pyracf-0.5.4/setup.py` & `pyracf-0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.5.4",
+    version="0.5.7",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.5.4/src/pyracf/__init__.py` & `pyracf-0.5.7/src/pyracf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                     'USBD': ['_users','0200'],
                     'USGCON': ['_groupConnect','0203'],
                     'USINSTD': ['_installdata','0204'],
                     'USCON': ['_connectData','0205'],
                     'USTSO': ['_userTSO','0220'],
                     'USOMVS': ['_userOMVS','0270'],
                     'DSBD': ['_datasets','0400'],
-                    'DSCACC': ['_datasetPermit','0402'],
+                    'DSCACC': ['_datasetConditionalAccess','0402'],
                     'DSACC': ['_datasetAccess','0404'],
                     'GRBD': ['_generics','0500'],
                     'GRMEM': ['_genericMembers','0503'],
                     'GRACC': ['_genericAccess','0505'],
                     'GRCACC': ['_genericConditionalAccess','0507']
                 }
                 exec(f'self.{lookup[recordtype][0]} = pd.read_pickle("{pickle}")')
@@ -308,15 +308,15 @@
         if self.USTSO_RECORDTYPE in thingswewant:
             self._userTSO = pd.DataFrame.from_dict(self.USTSO)          
         if self.USOMVS_RECORDTYPE in thingswewant:
             self._userOMVS = pd.DataFrame.from_dict(self.USOMVS)                        
         if self.DSBD_RECORDTYPE in thingswewant:
             self._datasets = pd.DataFrame.from_dict(self.DSBD)
         if self.DSCACC_RECORDTYPE in thingswewant:
-            self._datasetPermit = pd.DataFrame.from_dict(self.DSBD)
+            self._datasetConditionalAccess = pd.DataFrame.from_dict(self.DSCACC)
         if self.DSACC_RECORDTYPE in thingswewant:
             self._datasetAccess = pd.DataFrame.from_dict(self.DSACC)
         if self.GRBD_RECORDTYPE in thingswewant:
             self._generics = pd.DataFrame.from_dict(self.GRBD)
         if self.GRMEM_RECORDTYPE in thingswewant:
             self._genericMembers = pd.DataFrame.from_dict(self.GRMEM)
         if self.GRACC_RECORDTYPE in thingswewant:
@@ -367,15 +367,15 @@
         if len(self.USTSO) > 0:
             self.save_pickle(df=self._userTSO, dfname='USTSO', path=path, prefix=prefix)          
         if len(self.USOMVS) > 0:
             self.save_pickle(df=self._userOMVS, dfname='USOMVS', path=path, prefix=prefix)                        
         if len(self.DSBD) > 0:
             self.save_pickle(df=self._datasets, dfname='DSBD', path=path, prefix=prefix)
         if len(self.DSCACC) > 0:
-            self.save_pickle(df=self._datasetPermit, dfname='DSBD', path=path, prefix=prefix)
+            self.save_pickle(df=self._datasetConditionalAccess, dfname='DSBD', path=path, prefix=prefix)
         if len(self.DSACC) > 0:
             self.save_pickle(df=self._datasetAccess, dfname='DSACC', path=path, prefix=prefix)
         if len(self.GRBD) > 0:
             self.save_pickle(df=self._generics, dfname='GRBD', path=path, prefix=prefix)
         if len(self.GRMEM) > 0:
             self.save_pickle(df=self._genericMembers, dfname='GRMEM', path=path, prefix=prefix)
         if len(self.GRACC) > 0:
@@ -447,18 +447,18 @@
     @property
     def datasets(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._datasets
 
     @property
-    def datasetPermit(self):
+    def datasetConditionalAccess(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
-        return self._datasetPermit
+        return self._datasetConditionalAccess
 
     @property
     def connects(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._connects
 
@@ -519,37 +519,37 @@
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._userTSO    
         
     @property
     def orphans(self):
         
-        if self._records[DSACC_RECORDTYPE]['parsed'] + self._records[GRACC_RECORDTYPE]['parsed'] == 0:
+        if self._records[self.DSACC_RECORDTYPE]['parsed'] + self._records[self.GRACC_RECORDTYPE]['parsed'] == 0:
             raise StoopidException('No dataset/generic access records parsed! (PEBKAM/ID-10T error)')
             
         datasetOrphans = None
         genericOrphans = None
 
-        if self._records[DSACC_RECORDTYPE]['parsed'] > 0:
+        if self._records[self.DSACC_RECORDTYPE]['parsed'] > 0:
             self._datasetAccess = self._datasetAccess.assign(inGroups=self._datasetAccess.DSACC_AUTH_ID.isin(self._groups.GPBD_NAME))
             self._datasetAccess = self._datasetAccess.assign(inUsers=self._datasetAccess.DSACC_AUTH_ID.isin(self._users.USBD_NAME))
             datasetOrphans = self._datasetAccess.loc[(self._datasetAccess['inGroups'] == False) & (self._datasetAccess['inUsers'] == False) & (self._datasetAccess['DSACC_AUTH_ID'] != "*") & (self._datasetAccess['DSACC_AUTH_ID'] != "&RACUID")]
         
-        if self._records[GRACC_RECORDTYPE]['parsed'] > 0:
+        if self._records[self.GRACC_RECORDTYPE]['parsed'] > 0:
                 self._genericAccess = self._genericAccess.assign(inGroups=self._genericAccess.GRACC_AUTH_ID.isin(self._groups.GPBD_NAME))
                 self._genericAccess = self._genericAccess.assign(inUsers=self._genericAccess.GRACC_AUTH_ID.isin(self._users.USBD_NAME))
                 genericOrphans =  self._genericAccess.loc[(self._genericAccess['inGroups'] == False) & (self._genericAccess['inUsers'] == False) & (self._genericAccess['GRACC_AUTH_ID'] != "*") & (self._genericAccess['GRACC_AUTH_ID'] != "&RACUID")]
 
         return datasetOrphans, genericOrphans
 
     def xls(self,fileName='irrdbu00.xlsx'):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
 
-        if self._records[DSACC_RECORDTYPE]['parsed'] + self._records[GRACC_RECORDTYPE]['parsed'] == 0:
+        if self._records[self.DSACC_RECORDTYPE]['parsed'] + self._records[self.GRACC_RECORDTYPE]['parsed'] == 0:
             raise StoopidException('No dataset/generic access records parsed! (PEBKAM/ID-10T error)')
 
         writer = pd.ExcelWriter(f'{fileName}', engine='xlsxwriter')
         accessLevelFormats = {
                     'N': writer.book.add_format({'bg_color': 'silver'}),
                     'E': writer.book.add_format({'bg_color': 'purple'}),
                     'R': writer.book.add_format({'bg_color': 'yellow'}),
@@ -616,15 +616,15 @@
                     if i>0 and j>0:
                         rdict = worksheet.table.get(j,None)
                         centry = rdict.get(i,None)
                         if centry:
                             value = shared_strings[centry.string]
                             worksheet.write(j, i, value, accessLevelFormats[value])
 
-        if self._records[DSBD_RECORDTYPE]['parsed'] > 0:
+        if self._records[self.DSBD_RECORDTYPE]['parsed'] > 0:
             ss = datetime.now()
             profilesInClass = list(self.datasetAccess['DSACC_NAME'].unique())
             authIDsInClass = list(self.datasetAccess['DSACC_AUTH_ID'].unique())
             authids = 0
             longestProfile = 0
             for p in profilesInClass:
                 if len(p) > longestProfile:
```

### Comparing `pyracf-0.5.4/src/pyracf/offsets.json` & `pyracf-0.5.7/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.5.4/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.5.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1
-Name: pyracf
-Version: 0.5.4
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
 
-PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database. It consumes the IRRDBU00 unload and creates "Panda DataFrames" for every 'recordtype', allowing for easy manipulation and analysis of the data. With the new release, PyRACF now supports saving and loading pickle files, making it easier than ever to work with large RACF datasets. See https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types and https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility for a description of these records. The DataFrames will have the same 'fieldnames' as described in the docs. Install PyRACF with pip install pyracf or check out the source code on GitHub: https://github.com/wizardofzos/pyracf/releases/latest. Get started with PyRACF today and take control of your RACF data like never before!
+## PyRACF: A Python module for analyzing RACF security
+
+PyRACF is a powerful Python module that simplifies the parsing and querying of any RACF database, providing an efficient and intuitive way to analyze security setups on IBM Z systems. By consuming the IRRDBU00 unload, PyRACF generates "Panda DataFrames" for each 'recordtype', which allow for seamless manipulation and analysis of the data.
+
+Pandas is a powerful data manipulation library in Python that allows for easy querying of the DataFrames generated by PyRACF. With Pandas, you can perform complex queries on the security data to extract meaningful insights into the security posture of your system.
+
+PyRACF's support for saving and loading pickle files makes it easier than ever to work with large RACF datasets, giving you the ability to perform comprehensive analyses of your security setup.
+
+For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
+
+To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
+
 
 ## Updates
 
+### 0.5.4 (Even more recordtypes!!)
+- new property: genericConditionalAccess. Will show GRCACC records.
+- Fixed some nasty 'default recordtypes' bugs
+  
 ### 0.5.0 (Pickle FTW!)
 
 - new function: save_pickles(path=path, prefix=prefix). Will save all parsed dataframes as pickles (/path/_prefix_*RECORDTYPE*.pickle)
 - Can now initialize RACF object from pickle-folder/prefix. To reuse earlier saves pickle files. See examples below
 - parse_fancycli now has two optional arguments (save_pickles and prefix) to also save pickle files after parsing to the directory as specified in save_pickles. The prefix argument is only useed with save_pickles isn't False
 
 ### 0.4.5 (Fix Community Update Bug, thanks @Martydog)
@@ -75,14 +75,15 @@
 | Function/Property | Explanation | Example |
 |---|---|---|
 | auditors | Returns DataFrame with all user having the auditor bit switched on | mysys.auditors |
 | connects | Returns DataFrame with all user to group connects | mysys.connects |
 | datasetAccess | Returns DataFrame with all Accesslists for all dataset profiles | mysys.datasetsAccess |
 | datasets | Returns DataFrame with all datasetprofiles | mysys.datasets |
 | genericAccess | Returns DataFrame with with all accesslists for generic resource profiles | mysys.genericAccess
+| genericConditionalAccess | Returns DataFrame with with all conditional accesslists for generic resource profiles | mysys.genericConditionalAccess
 | generics | Returns DataFrame with with all generic resource profiles | mysys.generics 
 | group | Returns DataFrame with with one dataset profile only | mysys.group('SYS1') |
 | groupConnect | Returns DataFrame with with user group connection records (0203 recordtype) | mysys.groupConnect |
 | groups | Returns DataFrame with all group data | mysys.groups |
 | installdata | Returns DataFrame with with user installation data (0204 recordtype) | mysys.installdata |
 | operations | Returns a DataFrame  with all operations users | mysys.operations |
 | orphans | Returns 2 DataFrames one with orphans in dataset profile access lists, and one for generic resources | d, g = mysys.orphans |
```

