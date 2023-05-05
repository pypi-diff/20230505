# Comparing `tmp/alacorder-80.2.7.tar.gz` & `tmp/alacorder-80.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.2.7.tar", max compression
+gzip compressed data, was "alacorder-80.2.8.tar", max compression
```

## Comparing `alacorder-80.2.7.tar` & `alacorder-80.2.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.7/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.7/README.md
--rw-r--r--   0        0        0      697 2023-05-05 19:33:58.994579 alacorder-80.2.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-05 15:35:05.911439 alacorder-80.2.7/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.7/src/alacorder/__init__.py
--rw-r--r--   0        0        0   219882 2023-05-05 19:33:49.642425 alacorder-80.2.7/src/alacorder/__main__.py
--rw-r--r--   0        0        0   219882 2023-05-05 19:33:46.605189 alacorder-80.2.7/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.8/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.8/README.md
+-rw-r--r--   0        0        0      697 2023-05-05 19:56:30.927112 alacorder-80.2.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-05 19:36:29.887923 alacorder-80.2.8/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.8/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   219919 2023-05-05 19:55:49.707172 alacorder-80.2.8/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   219919 2023-05-05 19:55:34.492224 alacorder-80.2.8/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.8/PKG-INFO
```

### Comparing `alacorder-80.2.7/LICENSE` & `alacorder-80.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.7/README.md` & `alacorder-80.2.8/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.7/pyproject.toml` & `alacorder-80.2.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.2.7"
+version = "80.2.8"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.2.7/src/alacorder/.DS_Store` & `alacorder-80.2.8/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.7/src/alacorder/__main__.py` & `alacorder-80.2.8/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.7"
+version = "80.2.8"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3209,14 +3209,15 @@
             .alias("HabitualOffenderNumber"),
             pl.col("Sentence")
             .str.extract(r"Victim DOB\:\s+(\d?\d?/?\d?\d?/?\d?\d?\d?\d?)")
             .str.to_date("%m/%d/%Y", strict=False)
             .alias("VictimDOB"),
         ]
     )
+    sent = sent.drop_nulls("Number")
     sent = sent.fill_null("")
     return sent
 
 
 #   #   #   #        FETCH (PDF SCRAPER)        #   #   #   #
```

### Comparing `alacorder-80.2.7/src/alacorder/alac.py` & `alacorder-80.2.8/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.7"
+version = "80.2.8"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3209,14 +3209,15 @@
             .alias("HabitualOffenderNumber"),
             pl.col("Sentence")
             .str.extract(r"Victim DOB\:\s+(\d?\d?/?\d?\d?/?\d?\d?\d?\d?)")
             .str.to_date("%m/%d/%Y", strict=False)
             .alias("VictimDOB"),
         ]
     )
+    sent = sent.drop_nulls("Number")
     sent = sent.fill_null("")
     return sent
 
 
 #   #   #   #        FETCH (PDF SCRAPER)        #   #   #   #
```

### Comparing `alacorder-80.2.7/PKG-INFO` & `alacorder-80.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.2.7
+Version: 80.2.8
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

