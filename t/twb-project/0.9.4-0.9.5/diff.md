# Comparing `tmp/twb_project-0.9.4.tar.gz` & `tmp/twb_project-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.9.4.tar", max compression
+gzip compressed data, was "twb_project-0.9.5.tar", max compression
```

## Comparing `twb_project-0.9.4.tar` & `twb_project-0.9.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.4/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.4/README.md
--rw-r--r--   0        0        0      760 2023-05-04 17:46:06.730806 twb_project-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.4/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.4/twb/bip.py
--rw-r--r--   0        0        0    19887 2023-05-04 17:45:23.616437 twb_project-0.9.4/twb/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.4/twb/builder_helpers.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.4/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.4/twb/downloader.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.4/twb/logger.py
--rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-0.9.4/twb/logger_init.py
--rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.4/twb/modifier.py
--rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.4/twb/parallelization.py
--rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.4/twb/reader.py
--rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.4/twb/utils.py
--rw-r--r--   0        0        0     6272 2023-05-04 17:44:00.629468 twb_project-0.9.4/twb/warehouse.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.4/setup.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.5/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.5/README.md
+-rw-r--r--   0        0        0      760 2023-05-05 03:07:54.207803 twb_project-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.5/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.5/twb/bip.py
+-rw-r--r--   0        0        0    20020 2023-05-05 03:07:36.078433 twb_project-0.9.5/twb/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.5/twb/builder_helpers.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.5/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.5/twb/downloader.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.5/twb/logger.py
+-rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-0.9.5/twb/logger_init.py
+-rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.5/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.5/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.5/twb/reader.py
+-rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.5/twb/utils.py
+-rw-r--r--   0        0        0     6272 2023-05-04 17:44:00.629468 twb_project-0.9.5/twb/warehouse.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.5/setup.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.5/PKG-INFO
```

### Comparing `twb_project-0.9.4/LICENSE` & `twb_project-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/README.md` & `twb_project-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/pyproject.toml` & `twb_project-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.9.4"
+version = "0.9.5"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.9.4/twb/bip.py` & `twb_project-0.9.5/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/twb/builder.py` & `twb_project-0.9.5/twb/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,16 @@
 
     def _decompress_executor(self, file_path: str) -> List[str]:
         # Initialize temporary directory.
         temp_dir = os.path.join(self.output_dir, 'temp')
         os.makedirs(temp_dir, exist_ok=True)
 
         archive_filename = os.path.basename(file_path)
-        decompressed_dir_name = '.'.join(archive_filename.split('.')[:-1])
-        decompressed_dir_path = os.path.join(temp_dir, decompressed_dir_name)
+        random_id = uuid.uuid4().hex
+        decompressed_dir_path = os.path.join(temp_dir, random_id)
         os.makedirs(decompressed_dir_path, exist_ok=True)
 
         logging.debug(f'Decompressing [{archive_filename}]...')
 
         with py7zr.SevenZipFile(file_path, mode='r', mp=False) as z:
             start_time = time.time()
             z.extractall(path=decompressed_dir_path)
@@ -99,16 +99,15 @@
     def _process_executor(self, xml_path: str) -> List[str]:
         """
         Process the file.
         :param xml_path: the path of the file to be processed.
         :return: the number of URLs processed
         """
         # Initialize processed directory.
-        processed_dir = os.path.join(self.output_dir, 'temp', 'processed')
-        os.makedirs(processed_dir, exist_ok=True)
+        processed_dir = os.path.dirname(xml_path)
 
         logging.debug(f'Processing {os.path.basename(xml_path)}...')
 
         article_id: Optional[str] = None
         article_title: Optional[str] = None
         article_info: Optional[dict] = None
 
@@ -215,19 +214,14 @@
             logging.critical(f'Error occurred when processing the file [{xml_file}]: {e}')
             processed_files = []
 
         try:
             # Remove XML file.
             os.remove(xml_path)
 
-            # If the parent dir of this XML file is empty, remove it.
-            parent_dir = os.path.dirname(xml_path)
-            if len(os.listdir(parent_dir)) == 0:
-                cleanup_dir(parent_dir)
-
         except:
             logging.error(f'Failed to remove the XML file [{xml_path}].')
 
         logging.debug(f'Processed (OK): count = {len(processed_files)}')
 
         return processed_files
 
@@ -259,14 +253,19 @@
                 with open(warehouse_metadata_path, 'a') as f:
                     f.write(json.dumps(new_metadata) + '\n')
 
                 # Remove the modified file.
                 os.remove(processed_file)
                 os.remove(metadata_file)
 
+                # If the parent dir of this XML file is empty, remove it.
+                parent_dir = os.path.dirname(processed_file)
+                if len(os.listdir(parent_dir)) == 0:
+                    cleanup_dir(parent_dir)
+
             warehouse_file.close()
 
             logging.debug(f'Warehouse delivered (OK): {assigned_warehouse}')
 
         except Exception as e:
             logging.critical(f'Error occurred when moving the file to the warehouse. {e}')
 
@@ -333,15 +332,20 @@
 
         processed_count = 0
         finished_count = 0
 
         def _decompress_callback(decompressed_files: List[str]):
             nonlocal available_process_count
 
-            logging.debug(f'Decompressed (OK): {decompressed_files}')
+            if not decompressed_files:
+                logging.debug(f'Decompressed (EMPTY): {decompressed_files}')
+                return
+
+            decompressed_dir = os.path.dirname(decompressed_files[0])
+            logging.debug(f'Decompressed (OK): {decompressed_dir} ({len(decompressed_files)})')
 
             for decompressed_file in decompressed_files:
                 next_task_type = 'process'
                 next_args = (decompressed_file,)
                 tasks.insert(0, (next_task_type, next_args))
 
             available_process_count += 1
```

### Comparing `twb_project-0.9.4/twb/decompressor.py` & `twb_project-0.9.5/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/twb/downloader.py` & `twb_project-0.9.5/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/twb/logger.py` & `twb_project-0.9.5/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/twb/logger_init.py` & `twb_project-0.9.5/twb/logger_init.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/twb/modifier.py` & `twb_project-0.9.5/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/twb/parallelization.py` & `twb_project-0.9.5/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/twb/reader.py` & `twb_project-0.9.5/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/twb/utils.py` & `twb_project-0.9.5/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/twb/warehouse.py` & `twb_project-0.9.5/twb/warehouse.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.4/setup.py` & `twb_project-0.9.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.9.4/PKG-INFO` & `twb_project-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.9.4
+Version: 0.9.5
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

