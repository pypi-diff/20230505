# Comparing `tmp/alacorder-80.2.2.tar.gz` & `tmp/alacorder-80.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.2.2.tar", max compression
+gzip compressed data, was "alacorder-80.2.3.tar", max compression
```

## Comparing `alacorder-80.2.2.tar` & `alacorder-80.2.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.2/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.2/README.md
--rw-r--r--   0        0        0      697 2023-05-04 17:45:17.811797 alacorder-80.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.2/src/alacorder/__init__.py
--rw-r--r--   0        0        0   213003 2023-05-04 17:44:09.990203 alacorder-80.2.2/src/alacorder/__main__.py
--rw-r--r--   0        0        0   213003 2023-05-04 17:44:03.464820 alacorder-80.2.2/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.3/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.3/README.md
+-rw-r--r--   0        0        0      697 2023-05-04 23:08:10.123900 alacorder-80.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-04 23:08:09.337520 alacorder-80.2.3/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.3/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   213039 2023-05-04 23:08:21.143224 alacorder-80.2.3/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   213039 2023-05-04 23:08:25.187008 alacorder-80.2.3/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.3/PKG-INFO
```

### Comparing `alacorder-80.2.2/LICENSE` & `alacorder-80.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.2/README.md` & `alacorder-80.2.3/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.2/pyproject.toml` & `alacorder-80.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.2.2"
+version = "80.2.3"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.2.2/src/alacorder/__main__.py` & `alacorder-80.2.3/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.2"
+version = "80.2.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -26,15 +26,15 @@
 
 
 #   #   #   #                LOGS                #   #   #   #
 
 
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
-pl.Config.set_tbl_width_chars(90)
+pl.Config.set_tbl_width_chars(100)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_dataframe_shape_below(True)
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 FNAME = f"{name} {version}"
 FSHORT_NAME = f"{name} {'.'.join(version.split('.')[0:-1])}"
 
@@ -3061,14 +3061,15 @@
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
             .alias("HabitualOffender"),
             pl.col("Sentence")
             .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume") 
             .str.replace_all(r"[X\s0-9]", "")
+            .str.replace(r'\.','')
             .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
             .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
             .cast(pl.Float64, strict=False)
             .alias("DrugVolume"),
             pl.col("Sentence")
             .str.extract(r"Drug Code\: (.+?)Habitual Offender Number")
```

### Comparing `alacorder-80.2.2/src/alacorder/alac.py` & `alacorder-80.2.3/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.2"
+version = "80.2.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -26,15 +26,15 @@
 
 
 #   #   #   #                LOGS                #   #   #   #
 
 
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
-pl.Config.set_tbl_width_chars(90)
+pl.Config.set_tbl_width_chars(100)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_dataframe_shape_below(True)
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 FNAME = f"{name} {version}"
 FSHORT_NAME = f"{name} {'.'.join(version.split('.')[0:-1])}"
 
@@ -3061,14 +3061,15 @@
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
             .alias("HabitualOffender"),
             pl.col("Sentence")
             .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume") 
             .str.replace_all(r"[X\s0-9]", "")
+            .str.replace(r'\.','')
             .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
             .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
             .cast(pl.Float64, strict=False)
             .alias("DrugVolume"),
             pl.col("Sentence")
             .str.extract(r"Drug Code\: (.+?)Habitual Offender Number")
```

### Comparing `alacorder-80.2.2/PKG-INFO` & `alacorder-80.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.2.2
+Version: 80.2.3
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

