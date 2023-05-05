# Comparing `tmp/timewise-0.3.8.tar.gz` & `tmp/timewise-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timewise-0.3.8.tar", max compression
+gzip compressed data, was "timewise-0.3.9.tar", max compression
```

## Comparing `timewise-0.3.8.tar` & `timewise-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-03-24 11:58:29.162557 timewise-0.3.8/LICENSE
--rw-r--r--   0        0        0     1865 2023-03-24 11:58:29.162557 timewise-0.3.8/README.md
--rw-r--r--   0        0        0      997 2023-03-24 11:58:29.162557 timewise-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      203 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/__init__.py
--rw-r--r--   0        0        0     3480 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/big_parent_sample.py
--rw-r--r--   0        0        0     1380 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/general.py
--rw-r--r--   0        0        0     3298 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/parent_sample_base.py
--rw-r--r--   0        0        0     2171 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/point_source_utils.py
--rw-r--r--   0        0        0    13486 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/utils.py
--rw-r--r--   0        0        0    53939 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/wise_bigdata_desy_cluster.py
--rw-r--r--   0        0        0    71143 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/wise_data_base.py
--rw-r--r--   0        0        0    24601 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/wise_data_by_visit.py
--rw-r--r--   0        0        0     1095 2023-03-24 11:58:29.166557 timewise-0.3.8/timewise/wise_flux_conversion_correction.dat
--rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 timewise-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-28 08:01:21.367310 timewise-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1865 2023-03-28 08:01:21.367310 timewise-0.3.9/README.md
+-rw-r--r--   0        0        0      997 2023-03-28 08:01:21.367310 timewise-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-03-28 08:01:21.367310 timewise-0.3.9/timewise/__init__.py
+-rw-r--r--   0        0        0     3480 2023-03-28 08:01:21.367310 timewise-0.3.9/timewise/big_parent_sample.py
+-rw-r--r--   0        0        0     1380 2023-03-28 08:01:21.367310 timewise-0.3.9/timewise/general.py
+-rw-r--r--   0        0        0     3298 2023-03-28 08:01:21.367310 timewise-0.3.9/timewise/parent_sample_base.py
+-rw-r--r--   0        0        0     2171 2023-03-28 08:01:21.367310 timewise-0.3.9/timewise/point_source_utils.py
+-rw-r--r--   0        0        0    13486 2023-03-28 08:01:21.367310 timewise-0.3.9/timewise/utils.py
+-rw-r--r--   0        0        0    53940 2023-03-28 08:01:21.367310 timewise-0.3.9/timewise/wise_bigdata_desy_cluster.py
+-rw-r--r--   0        0        0    71143 2023-03-28 08:01:21.371310 timewise-0.3.9/timewise/wise_data_base.py
+-rw-r--r--   0        0        0    24601 2023-03-28 08:01:21.371310 timewise-0.3.9/timewise/wise_data_by_visit.py
+-rw-r--r--   0        0        0     1095 2023-03-28 08:01:21.371310 timewise-0.3.9/timewise/wise_flux_conversion_correction.dat
+-rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 timewise-0.3.9/PKG-INFO
```

### Comparing `timewise-0.3.8/LICENSE` & `timewise-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/README.md` & `timewise-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/pyproject.toml` & `timewise-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timewise"
-version = "0.3.8"
+version = "0.3.9"
 description = "A small package to download infrared data from the WISE satellite"
 authors = ["Jannis Necker <jannis.necker@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://timewise.readthedocs.io/en/latest"
 repository = "https://github.com/JannisNe/timewise"
```

### Comparing `timewise-0.3.8/timewise/big_parent_sample.py` & `timewise-0.3.9/timewise/big_parent_sample.py`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/timewise/general.py` & `timewise-0.3.9/timewise/general.py`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/timewise/parent_sample_base.py` & `timewise-0.3.9/timewise/parent_sample_base.py`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/timewise/point_source_utils.py` & `timewise-0.3.9/timewise/point_source_utils.py`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/timewise/utils.py` & `timewise-0.3.9/timewise/utils.py`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/timewise/wise_bigdata_desy_cluster.py` & `timewise-0.3.9/timewise/wise_bigdata_desy_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
         txt = (
             f'{sys.executable} {script_fn} '
             f'--logging_level {logging_level} '
             f'--base_name {self.base_name} '
             f'--min_sep_arcsec {self.min_sep.to("arcsec").value} '
             f'--n_chunks {self._n_chunks} '
             f'--job_id $1 '
-            f'--mak_by_position $2'
+            f'--mask_by_position $2'
         )
 
         logger.debug("writing executable to " + self.executable_filename)
         with open(self.executable_filename, "w") as f:
             f.write(txt)
 
     def get_submit_file_filename(self, ids):
```

### Comparing `timewise-0.3.8/timewise/wise_data_base.py` & `timewise-0.3.9/timewise/wise_data_base.py`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/timewise/wise_data_by_visit.py` & `timewise-0.3.9/timewise/wise_data_by_visit.py`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/timewise/wise_flux_conversion_correction.dat` & `timewise-0.3.9/timewise/wise_flux_conversion_correction.dat`

 * *Files identical despite different names*

### Comparing `timewise-0.3.8/PKG-INFO` & `timewise-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timewise
-Version: 0.3.8
+Version: 0.3.9
 Summary: A small package to download infrared data from the WISE satellite
 Home-page: https://github.com/JannisNe/timewise
 License: MIT
 Author: Jannis Necker
 Author-email: jannis.necker@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

