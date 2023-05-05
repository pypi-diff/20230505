# Comparing `tmp/twb_project-0.9.5.tar.gz` & `tmp/twb_project-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.9.5.tar", max compression
+gzip compressed data, was "twb_project-0.9.6.tar", max compression
```

## Comparing `twb_project-0.9.5.tar` & `twb_project-0.9.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.5/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.5/README.md
--rw-r--r--   0        0        0      760 2023-05-05 03:07:54.207803 twb_project-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.5/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.5/twb/bip.py
--rw-r--r--   0        0        0    20020 2023-05-05 03:07:36.078433 twb_project-0.9.5/twb/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.5/twb/builder_helpers.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.5/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.5/twb/downloader.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.5/twb/logger.py
--rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-0.9.5/twb/logger_init.py
--rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.5/twb/modifier.py
--rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.5/twb/parallelization.py
--rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.5/twb/reader.py
--rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.5/twb/utils.py
--rw-r--r--   0        0        0     6272 2023-05-04 17:44:00.629468 twb_project-0.9.5/twb/warehouse.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.5/setup.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.6/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.6/README.md
+-rw-r--r--   0        0        0      760 2023-05-05 14:20:12.789097 twb_project-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.6/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.6/twb/bip.py
+-rw-r--r--   0        0        0    20020 2023-05-05 03:07:36.078433 twb_project-0.9.6/twb/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.6/twb/builder_helpers.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.6/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.6/twb/downloader.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.6/twb/logger.py
+-rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-0.9.6/twb/logger_init.py
+-rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.6/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.6/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.6/twb/reader.py
+-rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.6/twb/utils.py
+-rw-r--r--   0        0        0     5877 2023-05-05 14:17:57.836997 twb_project-0.9.6/twb/warehouse.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.6/setup.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.6/PKG-INFO
```

### Comparing `twb_project-0.9.5/LICENSE` & `twb_project-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/README.md` & `twb_project-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/pyproject.toml` & `twb_project-0.9.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.9.5"
+version = "0.9.6"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.9.5/twb/bip.py` & `twb_project-0.9.6/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/builder.py` & `twb_project-0.9.6/twb/builder.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/decompressor.py` & `twb_project-0.9.6/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/downloader.py` & `twb_project-0.9.6/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/logger.py` & `twb_project-0.9.6/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/logger_init.py` & `twb_project-0.9.6/twb/logger_init.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/modifier.py` & `twb_project-0.9.6/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/parallelization.py` & `twb_project-0.9.6/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/reader.py` & `twb_project-0.9.6/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/utils.py` & `twb_project-0.9.6/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.5/twb/warehouse.py` & `twb_project-0.9.6/twb/warehouse.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,21 +29,22 @@
             new_filename, new_metadata_filename = get_warehouse_filenames(new_filename_basename)
             new_filepath = os.path.join(self.output_dir, new_filename)
             new_metadata_filepath = os.path.join(self.output_dir, new_metadata_filename)
             with open(new_filepath, 'w') as f:
                 f.truncate(0)
             with open(new_metadata_filepath, 'w') as f:
                 f.truncate(0)
-            logging.debug(f'New warehouse created: {new_filename_basename}.')
             self.available_warehouses.append(new_filename_basename)
-            self.warehouse_indexer += 1
+            logging.debug(f'New warehouse created: {new_filename_basename}.')
 
         except:
             logging.error(f'Failed to create new warehouse: {new_filename_basename}.')
 
+        self.warehouse_indexer += 1
+
     def assign_warehouse(self) -> str:
         """
         This function is intended to be called in main process (no parallelism).
         """
         free_warehouses = [w for w in self.available_warehouses if w not in self.occupied_warehouses]
         if len(free_warehouses) == 0:
             self.create_warehouse()
@@ -66,54 +67,45 @@
 
         return min_size_warehouse
 
     def bulk_assign(self, files: List[str]) -> Dict[str, List[str]]:
         """
         This function is intended to be called in main process (no parallelism).
         """
-        free_warehouses = [w for w in self.available_warehouses if w not in self.occupied_warehouses]
+        free_warehouses: List[str] = [w for w in self.available_warehouses if w not in self.occupied_warehouses]
         remaining_sizes = {
             w: self.max_size - get_file_size(os.path.join(self.output_dir, get_warehouse_filenames(w)[0]))
             for w in free_warehouses
         }
+        acceptable_warehouses: List[Tuple[str, int]] = []
         warehouse_assignments = dict()
 
         def _sync_warehouses():
-            nonlocal free_warehouses, remaining_sizes
+            nonlocal free_warehouses, remaining_sizes, acceptable_warehouses
             free_warehouses = [w for w in self.available_warehouses if w not in self.occupied_warehouses]
-            for w in free_warehouses:
-                if w not in remaining_sizes:
-                    remaining_sizes[w] = self.max_size
-
-        def _get_acceptable_warehouses(needed_size):
-            nonlocal free_warehouses, remaining_sizes
             acceptable_warehouses = []
             for w in free_warehouses:
                 if w not in remaining_sizes:
                     remaining_sizes[w] = self.max_size
-                if remaining_sizes[w] >= needed_size:
+                if remaining_sizes[w] > 0:
                     acceptable_warehouses.append((w, remaining_sizes[w]))
-            return acceptable_warehouses
+            acceptable_warehouses = sorted(acceptable_warehouses, key=lambda x: x[1], reverse=True)
 
         for file in files:
-            file_size = get_file_size(file)
             _sync_warehouses()
-            acceptable_warehouses = _get_acceptable_warehouses(needed_size=file_size)
             while not acceptable_warehouses:
                 self.create_warehouse()
                 _sync_warehouses()
-                acceptable_warehouses = _get_acceptable_warehouses(needed_size=file_size)
                 if not acceptable_warehouses:
                     logging.critical(f'Failed to create new warehouse for file: {file}.')
-            min_size_warehouses = min(acceptable_warehouses, key=lambda x: x[1])
-            min_size_warehouse = min_size_warehouses[0]
+            min_size_warehouse, _ = acceptable_warehouses[0]
             if min_size_warehouse not in warehouse_assignments:
                 warehouse_assignments[min_size_warehouse] = []
             warehouse_assignments[min_size_warehouse].append(file)
-            remaining_sizes[min_size_warehouse] -= file_size
+            remaining_sizes[min_size_warehouse] -= get_file_size(file)
 
         for warehouse in warehouse_assignments.keys():
             logging.debug(f'Bulk assigning warehouse: {warehouse}.')
             self.occupied_warehouses.append(warehouse)
 
         return warehouse_assignments
```

### Comparing `twb_project-0.9.5/setup.py` & `twb_project-0.9.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.9.5',
+    'version': '0.9.6',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.9.5/PKG-INFO` & `twb_project-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.9.5
+Version: 0.9.6
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

