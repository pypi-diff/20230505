# Comparing `tmp/eurodb-1.0.0.tar.gz` & `tmp/eurodb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurodb-1.0.0.tar", last modified: Fri May  5 10:32:03 2023, max compression
+gzip compressed data, was "eurodb-1.0.1.tar", last modified: Fri May  5 12:19:30 2023, max compression
```

## Comparing `eurodb-1.0.0.tar` & `eurodb-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 10:32:03.260424 eurodb-1.0.0/
--rw-rw-rw-   0        0        0     3089 2023-05-05 10:32:03.259421 eurodb-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2615 2023-05-05 10:25:34.000000 eurodb-1.0.0/README.md
--rw-rw-rw-   0        0        0      746 2023-05-05 10:30:59.000000 eurodb-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 10:32:03.260424 eurodb-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 10:32:03.253311 eurodb-1.0.0/src/
--rw-rw-rw-   0        0        0        0 2023-05-05 10:10:23.000000 eurodb-1.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:32:03.257417 eurodb-1.0.0/src/eurodb.egg-info/
--rw-rw-rw-   0        0        0     3089 2023-05-05 10:32:03.000000 eurodb-1.0.0/src/eurodb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-05-05 10:32:03.000000 eurodb-1.0.0/src/eurodb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 10:32:03.000000 eurodb-1.0.0/src/eurodb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-05 10:32:03.000000 eurodb-1.0.0/src/eurodb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4869 2023-05-05 10:24:20.000000 eurodb-1.0.0/src/eurodb.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:19:30.389925 eurodb-1.0.1/
+-rw-rw-rw-   0        0        0     2955 2023-05-05 12:19:30.388891 eurodb-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2487 2023-05-05 10:40:26.000000 eurodb-1.0.1/README.md
+-rw-rw-rw-   0        0        0      769 2023-05-05 12:18:46.000000 eurodb-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 12:19:30.389925 eurodb-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 12:19:30.380873 eurodb-1.0.1/src/
+-rw-rw-rw-   0        0        0        0 2023-05-05 10:10:23.000000 eurodb-1.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:19:30.386839 eurodb-1.0.1/src/eurodb.egg-info/
+-rw-rw-rw-   0        0        0     2955 2023-05-05 12:19:30.000000 eurodb-1.0.1/src/eurodb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-05-05 12:19:30.000000 eurodb-1.0.1/src/eurodb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:19:30.000000 eurodb-1.0.1/src/eurodb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-05 12:19:30.000000 eurodb-1.0.1/src/eurodb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4869 2023-05-05 10:24:20.000000 eurodb-1.0.1/src/eurodb.py
```

### Comparing `eurodb-1.0.0/PKG-INFO` & `eurodb-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: eurodb
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple PYODBC/SQLAlchemy wrapper for connection handling
-Author-email: Ratouney - Maxime de la Fouchardière <maxime.de-la-fouchardiere@eurodw.eu>
+Author-email: Ratouney - Maxime de la Fouchardière <maxime.fouchardiere@eurodw.eu>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 # EuroDB Lib
 
-## Disclaimer
+## TLDR
 ___
-This is a wrapper for the PYODBC library, that allow multiple connections to be specified in a config file.
+Generate/Fill your config file and use :
 
-## Setup
+```python
+import eurodb
+import pandas as pd
+
+db = connect()
 
-If it's not done, open a terminal in this folder and build the library with :
-> python -m build
+data : pandas.Dataframe = db.query("select stuff from somewhere")
+```
+
+## Setup
 
-Install it with (check the appropriate version number from the generated file above) :
-> pip install dist/eurodb-VERSION-NUMBER.tar.gz
+Install it with :
+> pip install eurodb
 
 Input your credentials into a JSON file of your choosing with the given format (default name is `dblogs.json`) : 
 ```json
 > dblogs.json
 [{
     "name": "Thefirstone",
     "server": "tcp:somefunnyurl.windows.net",
```

### Comparing `eurodb-1.0.0/README.md` & `eurodb-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # EuroDB Lib
 
-## Disclaimer
+## TLDR
 ___
-This is a wrapper for the PYODBC library, that allow multiple connections to be specified in a config file.
+Generate/Fill your config file and use :
 
-## Setup
+```python
+import eurodb
+import pandas as pd
+
+db = connect()
 
-If it's not done, open a terminal in this folder and build the library with :
-> python -m build
+data : pandas.Dataframe = db.query("select stuff from somewhere")
+```
+
+## Setup
 
-Install it with (check the appropriate version number from the generated file above) :
-> pip install dist/eurodb-VERSION-NUMBER.tar.gz
+Install it with :
+> pip install eurodb
 
 Input your credentials into a JSON file of your choosing with the given format (default name is `dblogs.json`) : 
 ```json
 > dblogs.json
 [{
     "name": "Thefirstone",
     "server": "tcp:somefunnyurl.windows.net",
```

### Comparing `eurodb-1.0.0/pyproject.toml` & `eurodb-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
-requires = ["setuptools>=61.0", "pyodbc"]
+requires = ["setuptools", "pyodbc", "SQLAlchemy", "pandas", "typing"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eurodb"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
-  { name="Ratouney - Maxime de la Fouchardière", email="maxime.de-la-fouchardiere@eurodw.eu" },
+  { name="Ratouney - Maxime de la Fouchardière", email="maxime.fouchardiere@eurodw.eu"},
 ]
 description = "A simple PYODBC/SQLAlchemy wrapper for connection handling"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.5"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 #"Homepage" = "https://github.com/pypa/sampleproject"
-#"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+#"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `eurodb-1.0.0/src/eurodb.egg-info/PKG-INFO` & `eurodb-1.0.1/src/eurodb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: eurodb
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple PYODBC/SQLAlchemy wrapper for connection handling
-Author-email: Ratouney - Maxime de la Fouchardière <maxime.de-la-fouchardiere@eurodw.eu>
+Author-email: Ratouney - Maxime de la Fouchardière <maxime.fouchardiere@eurodw.eu>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 # EuroDB Lib
 
-## Disclaimer
+## TLDR
 ___
-This is a wrapper for the PYODBC library, that allow multiple connections to be specified in a config file.
+Generate/Fill your config file and use :
 
-## Setup
+```python
+import eurodb
+import pandas as pd
+
+db = connect()
 
-If it's not done, open a terminal in this folder and build the library with :
-> python -m build
+data : pandas.Dataframe = db.query("select stuff from somewhere")
+```
+
+## Setup
 
-Install it with (check the appropriate version number from the generated file above) :
-> pip install dist/eurodb-VERSION-NUMBER.tar.gz
+Install it with :
+> pip install eurodb
 
 Input your credentials into a JSON file of your choosing with the given format (default name is `dblogs.json`) : 
 ```json
 > dblogs.json
 [{
     "name": "Thefirstone",
     "server": "tcp:somefunnyurl.windows.net",
```

### Comparing `eurodb-1.0.0/src/eurodb.py` & `eurodb-1.0.1/src/eurodb.py`

 * *Files identical despite different names*

