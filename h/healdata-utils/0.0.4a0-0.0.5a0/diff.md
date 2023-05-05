# Comparing `tmp/healdata_utils-0.0.4a0.tar.gz` & `tmp/healdata_utils-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healdata_utils-0.0.4a0.tar", last modified: Mon May  1 21:24:53 2023, max compression
+gzip compressed data, was "healdata_utils-0.0.5a0.tar", last modified: Fri May  5 16:41:59 2023, max compression
```

## Comparing `healdata_utils-0.0.4a0.tar` & `healdata_utils-0.0.5a0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/healdata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvdata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/frictionless/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/frictionless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/frictionless/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/readstat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/readstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/readstat/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/src/healdata_utils/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/validators/frictionless.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/validators/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/src/healdata_utils/validators/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.786627 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 21:24:53.000000 healdata_utils-0.0.4a0/src/healdata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:24:53.790627 healdata_utils-0.0.4a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-01 21:24:36.000000 healdata_utils-0.0.4a0/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvdata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/frictionless/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/frictionless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/frictionless/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/readstat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/readstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/readstat/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/src/healdata_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/validators/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/validators/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/src/healdata_utils/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.146480 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 16:41:59.000000 healdata_utils-0.0.5a0/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:41:59.150480 healdata_utils-0.0.5a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 16:41:48.000000 healdata_utils-0.0.5a0/tests/test_utils.py
```

### Comparing `healdata_utils-0.0.4a0/PKG-INFO` & `healdata_utils-0.0.5a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata_utils
-Version: 0.0.4a0
+Version: 0.0.5a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 # HEAL Data Utilities
@@ -85,18 +85,19 @@
 
 ### Output
 
 Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with 
 the validation reports in the `errors` folder. See below:
 
 - `input/input/my-redcap-data-dictionary-export.csv` : your input file
-- `output/errors/heal-csv-errors-summary.txt`: validation summary for your CSV data dictionary. Modeled after the fricitonless validation report summary.
 
-- `output/errors/heal-csv-errors.json`: 
+- `output/errors/heal-csv-errors.json`: outputted validation report for table in csv file against frictionless schema
+    - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json)
 - `output/errors/heal-json-errors.json`:  outputted jsonschema validation report.
+    - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/jsonschema/data-dictionary.json)
 
 - `output/heal-csvtemplate-data-dictionary.csv`: This is the CSV data dictionary
 - `output/heal-jsontemplate-data-dictionary.json`: This is the JSON version of the data dictionary
 
 > Note, only the JSON version will have the user-specified `title` and `description`
```

### Comparing `healdata_utils-0.0.4a0/README.md` & `healdata_utils-0.0.5a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -76,18 +76,19 @@
 
 ### Output
 
 Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with 
 the validation reports in the `errors` folder. See below:
 
 - `input/input/my-redcap-data-dictionary-export.csv` : your input file
-- `output/errors/heal-csv-errors-summary.txt`: validation summary for your CSV data dictionary. Modeled after the fricitonless validation report summary.
 
-- `output/errors/heal-csv-errors.json`: 
+- `output/errors/heal-csv-errors.json`: outputted validation report for table in csv file against frictionless schema
+    - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json)
 - `output/errors/heal-json-errors.json`:  outputted jsonschema validation report.
+    - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/jsonschema/data-dictionary.json)
 
 - `output/heal-csvtemplate-data-dictionary.csv`: This is the CSV data dictionary
 - `output/heal-jsontemplate-data-dictionary.json`: This is the JSON version of the data dictionary
 
 > Note, only the JSON version will have the user-specified `title` and `description`
```

### Comparing `healdata_utils-0.0.4a0/setup.py` & `healdata_utils-0.0.5a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def generate_long_description():
     return Path("README.md").read_text()
 
 
 setup(
     name='healdata_utils',
-    version='0.0.4-alpha',
+    version='0.0.5-alpha',
     author='Michael Kranz',
     author_email='kranz-michael@norc.org',
     long_description=generate_long_description(),
     long_description_content_type="text/markdown",    
     description='Data packaging tools for the HEAL data ecosystem',
     #TODO: change url to HEAL once migrated.
     url='https://github.com/norc-heal/healdata-utils',
```

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/cli.py` & `healdata_utils-0.0.5a0/src/healdata_utils/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from healdata_utils.transforms.jsontemplate.conversion import convert_templatejson
 from healdata_utils.transforms.readstat.conversion import convert_readstat
 from healdata_utils.transforms.redcapcsv.conversion import convert_redcapcsv
 from healdata_utils.transforms.csvdata.conversion import convert_datacsv
 from healdata_utils.validators.validate import validate_vlmd_json,validate_vlmd_csv
 import json
 from pathlib import Path
-import pandas as pd
 import petl as etl
+import csv
 from collections import deque
 
 from healdata_utils.utils import find_docstring_desc
 
 choice_fxn = {
     'data.csv':convert_datacsv,
     'template.csv':convert_templatecsv,
@@ -93,19 +93,26 @@
     ## add dd title
     if not data_dictionary_props.get('title'):
         data_dictionary_props['title'] = filepath.stem
 
     # get data dictionary package based on the input type
     data_dictionary_package = choice_fxn[inputtype](filepath,data_dictionary_props)
 
-    templatecsv = data_dictionary_package['templatecsv']['data_dictionary'] #TODO: currently only validates tabular but no reason this needs to be case
-    templatejson = data_dictionary_package['templatejson']
+    #TODO: currently only validates fields (ie table) but no reason it cant validate entire data package
+    package_csv = validate_vlmd_csv(data_dictionary_package['templatecsv']['data_dictionary'],to_sync_fields=True)
+    package_json = validate_vlmd_json(data_dictionary_package['templatejson'])
+
+    # TODO: in future just return the packages (eg reports nested within package and not out of)
+    # for now, keep same (report_xxx and templatexxx)
+
+    report_csv = package_csv["report"]
+    report_json = package_json["report"]
+    templatecsv = package_csv["data"]
+    templatejson = package_json["data"]
 
-    report_csv = validate_vlmd_csv(templatecsv)
-    report_json = validate_vlmd_json(templatejson)
     # write to file
     if outputdir!=None:
         outputdir = Path(outputdir)
         if outputdir.is_dir():
             jsontemplate_path = outputdir/"heal-jsontemplate-data-dictionary.json"
             csvtemplate_path = outputdir/"heal-csvtemplate-data-dictionary.csv"
         elif outputdir.parent.is_dir():
@@ -114,15 +121,21 @@
             outputdir = outputdir.parent
         else:
             raise Exception("outputdir must be an existing directory where files can be saved")
         
         # print data dictionaries
         jsontemplate_path.write_text(json.dumps(templatejson,indent=4))
 
-        etl.fromdicts(templatecsv).tocsv(csvtemplate_path)
+        # NOTE: quoting non-numeric to allow special characters for nested delimiters within string columns (ie "=")
+        (
+            etl.fromdicts(templatecsv)
+            .tocsv(csvtemplate_path,
+                quoting=csv.QUOTE_NONNUMERIC)
+
+        )
 
         # print errors
 
         if not report_json['valid']:
             print("JSON data dictionary not valid, see heal-json-errors.json")
  
         if not report_csv['valid']:
```

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/io.py` & `healdata_utils-0.0.5a0/src/healdata_utils/io.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/schemas.py` & `healdata_utils-0.0.5a0/src/healdata_utils/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import requests
 
 jsonschema_url = (
 "https://raw.githubusercontent.com/norc-heal/"
-"heal-metadata-schemas/mbkranz/variable-lvl-csvs/"
+"heal-metadata-schemas/mbkranz/variable-lvl-dev/"
 "variable-level-metadata-schema/schemas/jsonschema/fields.json"
 )
 csvschema_url = (
         "https://raw.githubusercontent.com/norc-heal/heal-metadata-schemas/"
-        "mbkranz/variable-lvl-csvs/"
+        "mbkranz/variable-lvl-dev/"
         "variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json"
     )
 
 # TODO: currently using fields.json and hardcoding -- use data_dictionaries.json 
 healjsonschema = {
     'type':'object',
     'required':[
```

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvdata/conversion.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvdata/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/conversion.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/csvtemplate/mappings.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/csvtemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/frictionless/conversion.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/frictionless/conversion.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,23 @@
     
     frictionless_fields = list(frictionless_schema.get("fields"))
     assert frictionless_fields,"A frictionless schema MUST have a set of fields"
 
 
     # schema level properties
 
-    ## jsonschema
-    required = []
     # frictionless
-    missing_values = frictionless_schema.get("missingValues",None)
+    missing_values = frictionless_schema.get("missingValues",[None,""])
     primary_keys = frictionless_schema.get("primaryKeys",[])
 
     # frictionless --> jsonschema per field
     jsonschema_properties = {}
+    fieldnames = []
     for field in frictionless_fields:
-
+        fieldnames.append(field["name"])
         jsonschema_properties[field["name"]] = prop = {}
 
         #base props
         if "description" in field:
             prop["description"] = field["description"]
         if "title" in field:
             prop["title"] = field["title"]
@@ -58,26 +57,27 @@
         if "minimum" in constraints:
             prop["minimum"] = constraints["minimum"]
 
         if "maximum" in constraints:
             prop["maximum"] = constraints["maximum"]
 
 
-        # missing-ness and required
-        if "required" in constraints or field["name"] in primary_keys:
-            required.append(field["name"])
-        elif missing_values:
-            prop_with_missing = {"oneOf":[
-                prop,{"enum":missing_values}
+        # all fields are required - missing-ness vs. required in tabular perspective is tacked on to property
+        is_required = "required" in constraints or field["name"] in primary_keys
+        if not is_required:
+            prop_with_missing = {
+                "anyOf":[
+                    prop,{"enum":missing_values}
             ]}
             jsonschema_properties[field["name"]] = prop_with_missing
 
+    
     jsonschema_schema = {
         "type":"object",
-        "required":required,
+        "required":fieldnames, 
         "properties":jsonschema_properties
     }
 
     schema = frictionless_schema
     for jsonprop in ["description","title","name"]:
         if schema.get(jsonprop):
             jsonschema_schema[jsonprop] = schema[jsonprop]
```

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/conversion.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/jsontemplate/mappings.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/jsontemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/readstat/conversion.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/readstat/conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,16 @@
         Values are a list of character values (A to Z and _ for SAS, a to z for SATA) 
         representing user defined missing values in SAS and STATA. 
         This appears when using user_missing=True in read_sas7bdat or read_dta 
         if user defined missing values are present.
 
     """
     
-    df,meta = read_pyreadstat(file_path,user_missing=True)
+    _,meta = read_pyreadstat(file_path,user_missing=True) # get user missing values (for stata/sas will make string so need sep call to infer types)
+    df,_ = read_pyreadstat(file_path) # dont fill user defined missing vals (to get correct types)
     df = df.convert_dtypes() #TODO: use visions package for inference (from pandas profile project)
     fields = pd.io.json.build_table_schema(df,index=False)['fields'] #converts to frictionless Table Schema
 
 
     for field in fields:
         field.pop('extDtype',None)
         fieldname = field['name']
```

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/conversion.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/headers.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/headers.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/mappings.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/transforms/redcapcsv/schema.py` & `healdata_utils-0.0.5a0/src/healdata_utils/transforms/redcapcsv/schema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/utils.py` & `healdata_utils-0.0.5a0/src/healdata_utils/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,145 @@
-''' General utilities/helper functions'''
+""" General utilities/helper functions"""
 import re
 from collections.abc import MutableMapping
 
+
 # individual cell utilities
 def strip_html(html_string):
     if html_string:
-        return re.sub(r'<[^>]+>', '', html_string)
+        return re.sub(r"<[^>]+>", "", html_string)
     else:
         return html_string
 
 
 def to_int_if_base10(val):
-    """ 
-    converts value to a string and if 
-    float (or a string rep of a float) of base10 
+    """
+    converts value to a string and if
+    float (or a string rep of a float) of base10
     to an integer string representation.
 
-    NOTE: 
-    """ 
+    NOTE:
+    """
     string = str(val)
 
-    if '.' in string:
-        parts = string.split('.')
-        if len(parts) == 2 and parts[1] == '0':
+    if "." in string:
+        parts = string.split(".")
+        if len(parts) == 2 and parts[1] == "0":
             return parts[0]
-    
+
     return string
 
 
-def parse_dictionary_str(string,item_sep,keyval_sep):
-    """ 
+def parse_dictionary_str(string, item_sep, keyval_sep):
+    """
     parses a stringified dictionary into a dictionary
-    based on item separator 
+    based on item separator
 
     """
     stritems = string.strip().split(item_sep)
     items = {}
     for stritem in stritems:
-        item = stritem.split(keyval_sep,1)
+        item = stritem.split(keyval_sep, 1)
         items[item[0]] = item[1].strip()
-    
-    return items 
+
+    return items
 
 
-def parse_list_str(string,list_sep):
+def parse_list_str(string, list_sep):
     return string.strip().split(list_sep)
 
 
 # dictionary utilities
-def flatten_except_if(dictionary, parent_key=False, sep=".",except_keys=['encodings']):
+def flatten_except_if(dictionary, parent_key=False, sep=".", except_keys=["encodings"]):
     """
-    Turn a nested dictionary into a flattened dictionary. Taken from gen3 
+    Turn a nested dictionary into a flattened dictionary. Taken from gen3
     mds.agg_mds.adapter.flatten
     but added except keys and fixed a bug where parent is always False in MutableMapping
 
     :param dictionary: The dictionary to flatten
     :param parent_key: The string to prepend to dictionary's keys
     :param sep: The string used to separate flattened keys
     :param except_keys: keys to not flatten. Note, can be nested if using notation specified in sep
     :return: A flattened dictionary
     """
 
     items = []
     for key, value in dictionary.items():
         new_key = str(parent_key) + sep + key if parent_key else key
-        if isinstance(value,MutableMapping) and not new_key in except_keys:
+        if isinstance(value, MutableMapping) and not new_key in except_keys:
             items.extend(flatten_except_if(value, new_key, sep).items())
         else:
             items.append((new_key, value))
     return dict(items)
 
 
 def convert_rec_to_json(field):
-    ''' 
+    """
     converts a flattened dictionary to a nested dictionary
     based on JSON path dot notation indicating nesting
-    '''
+    """
     field_json = {}
-    for prop_path,prop in field.items():
-        
-        if str(prop) and str(prop)!="<NA>" and str(prop)!="nan":
+    for prop_path, prop in field.items():
+        if str(prop) and str(prop) != "<NA>" and str(prop) != "nan":
             # initiate the prop to be added with the entire
-            # field 
+            # field
             prop_json = field_json
             # get the inner most dictionary item of the jsonpath
-            nested_names = prop_path.split('.')
-            for i,prop_name in enumerate(nested_names):
-                is_last_nested = i+1==len(nested_names)
+            nested_names = prop_path.split(".")
+            for i, prop_name in enumerate(nested_names):
+                is_last_nested = i + 1 == len(nested_names)
                 if prop_json.get(prop_name) and not is_last_nested:
                     prop_json = prop_json[prop_name]
-                # if no object currently 
+                # if no object currently
                 elif not is_last_nested:
                     prop_json[prop_name] = {}
                     prop_json = prop_json[prop_name]
-                #assign property to inner most item
+                # assign property to inner most item
                 else:
                     prop_json[prop_name] = prop
 
     return field_json
 
 
 # documentation building utilities
 def find_docstring_desc(fxn):
-    """ 
+    """
     return the description part of a docstring
     (ie text before Parameters)
-    """ 
+    """
     exp = "^(.*)Parameters\\n"
     docstring = fxn.__doc__.strip()
     try:
-        return re.search(exp,docstring,re.DOTALL).group(1)
+        return re.search(exp, docstring, re.DOTALL).group(1)
     except AttributeError:
         return docstring
 
 
+# add missing values and order according to the order of a list
+
+
+def sync_fields(data, field_list,missing_value=None):
+    """
+    Sorts fields and adds missing fields (with None value).
+    If extra fields exist in a record that are not in field_list, then tacks on at 
+    end of record.
+
+
+    Parameters
+    --------------
+    data [list]: json array of values
+    fields [list]: the list of all fields (e.g., from a schema)
+
+    Returns
+    -------------
+    list: json array with fields added if missing
+    """
+    data_with_missing = []
 
+    for record in data:
+        extra_fields = list(set(list(record)).difference(field_list))
+        new_record = {field:record.get(field, missing_value) 
+            for field in field_list+extra_fields}
+        data_with_missing.append(new_record)
+
+    
+    return data_with_missing
```

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/validators/jsonschema.py` & `healdata_utils-0.0.5a0/src/healdata_utils/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils/validators/validate.py` & `healdata_utils-0.0.5a0/src/healdata_utils/validators/validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import pandas as pd
 import json
 
 from healdata_utils.schemas import healjsonschema,healcsvschema
 from healdata_utils.io import read_table
 from healdata_utils.transforms.frictionless.conversion import convert_frictionless_to_jsonschema
 from .jsonschema import validate_against_jsonschema
+from healdata_utils import utils
 
 class Validator:
     """ 
-    input a tablular-like data object or pointer
-    to tabular-like data object with a given schema
+    input a data object or pointer/path
+    to data object with a given schema
     and corresponding type of schema. 
     validate against the said schema of a certain type.
     if the validation schema type is different than the 
     input schema type, will convert to that type (eg jsonschema to
     frictionless.)
     """ 
     @classmethod
@@ -79,64 +80,59 @@
         The schema to compare data_or_path to (default: HEAL frictionless template)
 
     Returns
     -------
     dict[bool,dict]
         the returned `validate` function object 
     """
-    validator_params = {
-        "data":data_or_path,
-        "schema":schema,
-        "schema_type":"jsonschema"
-    }
     if isinstance(data_or_path, (str, os.PathLike)):
         validator = Validator.from_jsonfile(
             path=data_or_path,
             schema=schema,
             schema_type="jsonschema"
         )
     else:
-        validator_params
         validator = Validator.from_jsonarray(
             data=data_or_path,
             schema=schema,
             schema_type="jsonschema"
         )
-    
+
     package = validator.validate(validation_schema_type)
     report = package["report"]
     # report_summary = []
     errors_list = []
     for error in report["errors"]:
         errors_list.append({"json_path":error["json_path"],
             "message":error["message"]})
         # report_summary.append([error["json_path"],error["message"]])
 
-
+    package["report"] = {"valid":report["valid"],"errors":errors_list}
     # report_summary_str += "Validation summary for {data_name}"
     # report_summary_str += "\n\n"
     # report_summary_str += "VALID" if report["valid"] else "INVALID"
 
     # report_summary_str += "## Errors "
     # report_summary_str += "\n\n"
 
     # report_summary_str+=str(tabulate(
     #     report_summary,
     #     headers=["JsonPath", "Message"],
     #     tablefmt="grid",
     #     maxcolwidths=[5, 5, 90]
     # ))
 
-    return {"valid":report["valid"],"errors":errors_list}
+    return package
     
 def validate_vlmd_csv(
     data_or_path,
     schema=healcsvschema,
     input_schema_type="frictionless",
-    validation_schema_type="jsonschema"
+    validation_schema_type="jsonschema",
+    to_sync_fields=True
 ):
     """
     Validates a json array against the heal variable level metadata
     schema catered for a CSV tabular data dictionary file.
 
     As there are many options to validate a tabular data file, 
     this function provides options for different different specification
@@ -148,52 +144,59 @@
     Parameters
     ----------
     data_or_path : Path-like object indicating a path to a tabular data source (eg CSV or TSV) or a json array of records (see validate fxn)
     schema : dict, optional
         The schema to compare data_or_path to (default: HEAL frictionless template)
     input_schema_type: str, optional : the type of schema ["jsonschema","frictionless"]
     validation_schema_type: str, optional : the type of schema to use for validation (will convert if input does not eq validation schema types)
+    to_sync_fields : bool, optional[default=True]:whether to add missing fields (ie null) in schema before validation. 
+        Note, this is different than missing values. Missing values do not equal missing fields (think tabular dataset)
+        This also syncs the order of the fields to order of properties in schema.
     Returns
     -------
     dict[bool,dict]
         the returned `validate` function object 
         (eg., `{"valid":False,"errors":[...]}`)
     """
-    #TODO: refactor into multiple functions/classes
 
+    # instantiate validator object with correct class method depending on input
     if isinstance(data_or_path, (str, os.PathLike)):
         validator = Validator.from_csv_file(path=data_or_path,schema=schema,schema_type=input_schema_type)
 
     else:
         validator = Validator.from_jsonarray(data=data_or_path,schema=schema,schema_type=input_schema_type)
 
+    # sync fields
+    if input_schema_type=="frictionless":
+        field_list = [field["name"] for field in schema["fields"]]
+    elif input_schema_type=="jsonschema":
+        field_list = [fieldname for fieldname in list(schema["items"]["properties"])]
+    validator.data = utils.sync_fields(validator.data, field_list,missing_value="")
 
     package = validator.validate(validation_schema_type)
     report = package["report"]
 
-    if input_schema_type=="frictionless":
-        columns = [field["name"] for field in schema["fields"]]
-
+    # get most relevant report properties specific to tabular data
     error_list = []
     # report_summary = []
-
     for error in report["errors"]:
         if error["validator"]=="required":
             row = error["relative_path"][0]
             column = error["validator_value"][-1]
         else:
             row,column = error["relative_path"]
 
         error_list.append(
             {"row":row,
             "column":column,
             "message":error["message"]}
         )
         # report_summary.append([row,column,error["message"]])
 
+    package["report"] = {"valid":report["valid"],"errors":error_list}
 
     # report_summary_str += "Validation summary for {data_name}"
     # report_summary_str += "\n\n"
     # report_summary_str += "VALID" if report["valid"] else "INVALID"
 
     # report_summary_str += "## Errors "
     # report_summary_str += "\n\n"
@@ -203,14 +206,14 @@
     #     headers=["Row", "Column", "Message"],
     #     tablefmt="grid",
     #     maxcolwidths=[5, 5, 90]
     # ))
 
 
 
-    return {"valid":report["valid"],"errors":error_list}
+    return package
```

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils.egg-info/PKG-INFO` & `healdata_utils-0.0.5a0/src/healdata_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata-utils
-Version: 0.0.4a0
+Version: 0.0.5a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 # HEAL Data Utilities
@@ -85,18 +85,19 @@
 
 ### Output
 
 Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with 
 the validation reports in the `errors` folder. See below:
 
 - `input/input/my-redcap-data-dictionary-export.csv` : your input file
-- `output/errors/heal-csv-errors-summary.txt`: validation summary for your CSV data dictionary. Modeled after the fricitonless validation report summary.
 
-- `output/errors/heal-csv-errors.json`: 
+- `output/errors/heal-csv-errors.json`: outputted validation report for table in csv file against frictionless schema
+    - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json)
 - `output/errors/heal-json-errors.json`:  outputted jsonschema validation report.
+    - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/jsonschema/data-dictionary.json)
 
 - `output/heal-csvtemplate-data-dictionary.csv`: This is the CSV data dictionary
 - `output/heal-jsontemplate-data-dictionary.json`: This is the JSON version of the data dictionary
 
 > Note, only the JSON version will have the user-specified `title` and `description`
```

### Comparing `healdata_utils-0.0.4a0/src/healdata_utils.egg-info/SOURCES.txt` & `healdata_utils-0.0.5a0/src/healdata_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 src/healdata_utils/transforms/redcapcsv/mappings.py
 src/healdata_utils/transforms/redcapcsv/schema.py
 src/healdata_utils/validators/__init__.py
 src/healdata_utils/validators/frictionless.py
 src/healdata_utils/validators/jsonschema.py
 src/healdata_utils/validators/validate.py
 tests/test_cli.py
-tests/test_schemas.py
+tests/test_schemas.py
+tests/test_utils.py
```

### Comparing `healdata_utils-0.0.4a0/tests/test_schemas.py` & `healdata_utils-0.0.5a0/tests/test_schemas.py`

 * *Files identical despite different names*

