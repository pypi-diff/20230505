# Comparing `tmp/table_builder_io-0.1.tar.gz` & `tmp/table_builder_io-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "table_builder_io-0.1.tar", last modified: Thu Oct  6 03:56:27 2022, max compression
+gzip compressed data, was "table_builder_io-0.1.1.tar", last modified: Thu May  4 23:08:57 2023, max compression
```

## Comparing `table_builder_io-0.1.tar` & `table_builder_io-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3259 2022-08-08 05:08:55.898721 table_builder_io-0.1/.gitignore
--rw-r--r--   0        0        0     1266 2022-10-06 03:55:31.553715 table_builder_io-0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1101 2022-08-08 01:54:14.489125 table_builder_io-0.1/LICENSE
--rw-r--r--   0        0        0     7234 2022-10-06 03:55:31.563715 table_builder_io-0.1/README.md
--rw-r--r--   0        0        0      914 2022-10-06 03:55:31.571715 table_builder_io-0.1/dev_notes.md
--rw-r--r--   0        0        0    39067 2022-03-30 09:36:40.182818 table_builder_io-0.1/examples.ipynb
--rw-r--r--   0        0        0     1145 2022-10-06 03:55:31.584715 table_builder_io-0.1/noxfile.py
--rw-r--r--   0        0        0      750 2022-10-06 03:55:31.594714 table_builder_io-0.1/pyproject.toml
--rw-r--r--   0        0        0      148 2022-08-08 01:54:14.500125 table_builder_io-0.1/setup.py
--rw-r--r--   0        0        0      133 2022-10-06 03:55:46.785443 table_builder_io-0.1/table_builder_io/__init__.py
--rw-r--r--   0        0        0     2397 2022-10-06 03:55:31.614717 table_builder_io-0.1/table_builder_io/parse_metadata.py
--rw-r--r--   0        0        0    15389 2022-10-06 03:55:31.624714 table_builder_io-0.1/table_builder_io/reader.py
--rw-r--r--   0        0        0     3011 2022-10-06 03:55:31.635714 table_builder_io-0.1/table_builder_io/regexes.py
--rw-r--r--   0        0        0    29590 2022-10-06 03:55:31.647714 table_builder_io-0.1/test/csv_test_cases.py
--rw-r--r--   0        0        0     1594 2022-02-27 06:44:30.767609 table_builder_io-0.1/test/mini_testfile.csv
--rw-r--r--   0        0        0     1590 2022-08-08 02:20:01.856156 table_builder_io-0.1/test/mini_testfile_dataset_footer_variant.csv
--rw-r--r--   0        0        0   178224 2022-02-25 16:27:00.000000 table_builder_io-0.1/test/sa2_pow_vs_sa2_ur_bne_bc_worker_total_wafer.csv
--rw-r--r--   0        0        0     1419 2022-10-06 03:55:31.656715 table_builder_io-0.1/test/test_data_filtering.py
--rw-r--r--   0        0        0     2979 2022-10-06 03:55:31.664714 table_builder_io-0.1/test/test_metadata_parsing.py
--rw-r--r--   0        0        0     6462 2022-10-06 03:55:31.674713 table_builder_io-0.1/test/test_tabio.py
--rw-r--r--   0        0        0     7717 1970-01-01 00:00:00.000000 table_builder_io-0.1/PKG-INFO
+-rw-r--r--   0        0        0     3259 2022-08-08 05:08:55.898721 table_builder_io-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1266 2022-10-06 03:55:31.553715 table_builder_io-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1101 2022-08-08 01:54:14.489125 table_builder_io-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7234 2022-10-06 03:55:31.563715 table_builder_io-0.1.1/README.md
+-rw-r--r--   0        0        0      914 2022-10-06 03:55:31.571715 table_builder_io-0.1.1/dev_notes.md
+-rw-r--r--   0        0        0    39067 2022-03-30 09:36:40.182818 table_builder_io-0.1.1/examples.ipynb
+-rw-r--r--   0        0        0     1145 2022-10-06 03:55:31.584715 table_builder_io-0.1.1/noxfile.py
+-rw-r--r--   0        0        0      750 2022-10-06 03:55:31.594714 table_builder_io-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      148 2022-08-08 01:54:14.500125 table_builder_io-0.1.1/setup.py
+-rw-r--r--   0        0        0      135 2023-05-04 23:07:35.780594 table_builder_io-0.1.1/table_builder_io/__init__.py
+-rw-r--r--   0        0        0     2397 2022-10-06 03:55:31.614717 table_builder_io-0.1.1/table_builder_io/parse_metadata.py
+-rw-r--r--   0        0        0    15403 2023-05-04 23:06:49.048643 table_builder_io-0.1.1/table_builder_io/reader.py
+-rw-r--r--   0        0        0     3011 2022-10-06 03:55:31.635714 table_builder_io-0.1.1/table_builder_io/regexes.py
+-rw-r--r--   0        0        0    29590 2022-10-06 03:55:31.647714 table_builder_io-0.1.1/test/csv_test_cases.py
+-rw-r--r--   0        0        0     1594 2022-02-27 06:44:30.767609 table_builder_io-0.1.1/test/mini_testfile.csv
+-rw-r--r--   0        0        0     1590 2022-08-08 02:20:01.856156 table_builder_io-0.1.1/test/mini_testfile_dataset_footer_variant.csv
+-rw-r--r--   0        0        0   178224 2022-02-25 16:27:00.000000 table_builder_io-0.1.1/test/sa2_pow_vs_sa2_ur_bne_bc_worker_total_wafer.csv
+-rw-r--r--   0        0        0     1419 2022-10-06 03:55:31.656715 table_builder_io-0.1.1/test/test_data_filtering.py
+-rw-r--r--   0        0        0     2979 2022-10-06 03:55:31.664714 table_builder_io-0.1.1/test/test_metadata_parsing.py
+-rw-r--r--   0        0        0     6462 2022-10-06 03:55:31.674713 table_builder_io-0.1.1/test/test_tabio.py
+-rw-r--r--   0        0        0     7719 1970-01-01 00:00:00.000000 table_builder_io-0.1.1/PKG-INFO
```

### Comparing `table_builder_io-0.1/.gitignore` & `table_builder_io-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/CHANGELOG.md` & `table_builder_io-0.1.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/LICENSE` & `table_builder_io-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/README.md` & `table_builder_io-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/dev_notes.md` & `table_builder_io-0.1.1/dev_notes.md`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/examples.ipynb` & `table_builder_io-0.1.1/examples.ipynb`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/noxfile.py` & `table_builder_io-0.1.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/pyproject.toml` & `table_builder_io-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/table_builder_io/parse_metadata.py` & `table_builder_io-0.1.1/table_builder_io/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/table_builder_io/reader.py` & `table_builder_io-0.1.1/table_builder_io/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
                     level = 0
                 else:
                     level = None
                 out = out.drop(index="Total", level=level)
             try:
                 # int32 is probably safe, largest index would be meshblock ids?
                 out.index = out.index.astype("int32")
-            except TypeError:
+            except (TypeError, ValueError):
                 pass
 
             if not self._has_multilevel_cols:
                 col_headers = pd.Index(col_headers, name=self.column_dimensions[0])
 
         else:
             if self._has_multilevel_cols:
```

### Comparing `table_builder_io-0.1/table_builder_io/regexes.py` & `table_builder_io-0.1.1/table_builder_io/regexes.py`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/test/csv_test_cases.py` & `table_builder_io-0.1.1/test/csv_test_cases.py`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/test/mini_testfile.csv` & `table_builder_io-0.1.1/test/mini_testfile.csv`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/test/mini_testfile_dataset_footer_variant.csv` & `table_builder_io-0.1.1/test/mini_testfile_dataset_footer_variant.csv`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/test/sa2_pow_vs_sa2_ur_bne_bc_worker_total_wafer.csv` & `table_builder_io-0.1.1/test/sa2_pow_vs_sa2_ur_bne_bc_worker_total_wafer.csv`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/test/test_data_filtering.py` & `table_builder_io-0.1.1/test/test_data_filtering.py`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/test/test_metadata_parsing.py` & `table_builder_io-0.1.1/test/test_metadata_parsing.py`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/test/test_tabio.py` & `table_builder_io-0.1.1/test/test_tabio.py`

 * *Files identical despite different names*

### Comparing `table_builder_io-0.1/PKG-INFO` & `table_builder_io-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: table_builder_io
-Version: 0.1
+Version: 0.1.1
 Summary: Tool for reading ABS TableBuilder datasets easily in Python.
 Author-email: Matt Richards <matt.richards@veitchlister.com>, Veitch Lister Consulting <developers@veitchlister.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

