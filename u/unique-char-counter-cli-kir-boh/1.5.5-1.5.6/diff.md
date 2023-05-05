# Comparing `tmp/unique_char_counter_cli_kir_boh-1.5.5.tar.gz` & `tmp/unique_char_counter_cli_kir_boh-1.5.6.tar.gz`

## Comparing `unique_char_counter_cli_kir_boh-1.5.5.tar` & `unique_char_counter_cli_kir_boh-1.5.6.tar`

### file list

```diff
@@ -1,21 +1,15 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/Task 5 Package.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/misc.xml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/modules.xml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/vcs.xml
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/__init__.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/tests/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/LICENSE
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/pyproject.toml
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/__init__.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/tests/__init__.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/LICENSE
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.6/PKG-INFO
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.5/.pytest_cache/v/cache/nodeids` & `unique_char_counter_cli_kir_boh-1.5.6/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.5/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-1.5.6/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,11 +30,7 @@
         mock_get_obj_from_cli.return_value = Namespace(string=True, file=False, hashable_obj='some file')
         self.assertEqual(unique_char_counter_cli.main(), 7)
 
 
     @patch('builtins.open', new_callable=mock_open, read_data='dat\nafff')
     def test_read_file_in_chunks(self, mock_open):
         self.assertEqual(unique_char_counter_cli.read_file_in_chunks('file.txt', chunk_size=3), 'dat\nafff')
-
-
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.5/LICENSE` & `unique_char_counter_cli_kir_boh-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.5/README.md` & `unique_char_counter_cli_kir_boh-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.5/pyproject.toml` & `unique_char_counter_cli_kir_boh-1.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "unique_char_counter_cli_kir_boh"
-version = "1.5.5"
+version = "1.5.6"
 authors = [
   { name="Kiril Bogatiuk", email="kirillbogatu2005@gmail.com" },
 ]
 maintainers = [
     {name ="Stanislav Hrytsyshyn", email="kirillbogatu2005@gmail.com"},
 ]
 description = "Project gets hashable obj from cli an returns uniqe items amount, other funcs desribed in README.md"
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.5/PKG-INFO` & `unique_char_counter_cli_kir_boh-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unique_char_counter_cli_kir_boh
-Version: 1.5.5
+Version: 1.5.6
 Summary: Project gets hashable obj from cli an returns uniqe items amount, other funcs desribed in README.md
 Author-email: Kiril Bogatiuk <kirillbogatu2005@gmail.com>
 Maintainer-email: Stanislav Hrytsyshyn <kirillbogatu2005@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

