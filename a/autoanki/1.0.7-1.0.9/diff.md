# Comparing `tmp/autoanki-1.0.7.tar.gz` & `tmp/autoanki-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.0.7.tar", last modified: Fri May  5 19:11:43 2023, max compression
+gzip compressed data, was "autoanki-1.0.9.tar", last modified: Fri May  5 21:40:56 2023, max compression
```

## Comparing `autoanki-1.0.7.tar` & `autoanki-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 19:11:43.302972 autoanki-1.0.7/
--rw-r--r--   0 owner      (501) staff       (20)     1061 2023-04-17 18:57:35.000000 autoanki-1.0.7/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.0.7/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     4335 2023-05-05 19:11:43.303058 autoanki-1.0.7/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     3802 2023-04-19 00:15:21.000000 autoanki-1.0.7/README.md
--rw-r--r--   0 owner      (501) staff       (20)      103 2023-05-05 19:00:34.000000 autoanki-1.0.7/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      939 2023-05-05 19:11:43.303297 autoanki-1.0.7/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 19:11:43.297495 autoanki-1.0.7/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 19:11:43.299225 autoanki-1.0.7/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)     5171 2023-04-27 16:28:13.000000 autoanki-1.0.7/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 19:11:43.300482 autoanki-1.0.7/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     7268 2023-04-17 17:53:21.000000 autoanki-1.0.7/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.0.7/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 19:11:43.301709 autoanki-1.0.7/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    13282 2023-05-05 17:57:22.000000 autoanki-1.0.7/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.0.7/src/autoanki/DatabaseManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.0.7/src/autoanki/DatabaseManager/book_table.sql
--rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.0.7/src/autoanki/DatabaseManager/book_table_view.sql
--rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.0.7/src/autoanki/DatabaseManager/databases_init.sql
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 19:11:43.301921 autoanki-1.0.7/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     6413 2023-04-17 18:46:28.000000 autoanki-1.0.7/src/autoanki/DeckManager/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 19:11:43.302734 autoanki-1.0.7/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)      122 2023-04-17 18:22:48.000000 autoanki-1.0.7/src/autoanki/Dictionary/CC-CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      232 2023-04-17 16:36:34.000000 autoanki-1.0.7/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)     5580 2023-04-17 17:53:21.000000 autoanki-1.0.7/src/autoanki/Dictionary/YellowBridgeDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       58 2023-04-17 18:23:02.000000 autoanki-1.0.7/src/autoanki/Dictionary/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.0.7/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 19:11:43.300033 autoanki-1.0.7/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     4335 2023-05-05 19:11:43.000000 autoanki-1.0.7/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)      798 2023-05-05 19:11:43.000000 autoanki-1.0.7/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 19:11:43.000000 autoanki-1.0.7/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)      244 2023-05-05 19:11:43.000000 autoanki-1.0.7/src/autoanki.egg-info/requires.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 19:11:43.000000 autoanki-1.0.7/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.483939 autoanki-1.0.9/
+-rw-r--r--   0 owner      (501) staff       (20)     1061 2023-04-17 18:57:35.000000 autoanki-1.0.9/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.0.9/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     4335 2023-05-05 21:40:56.484000 autoanki-1.0.9/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     3802 2023-04-19 00:15:21.000000 autoanki-1.0.9/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.0.9/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      662 2023-05-05 21:40:56.484219 autoanki-1.0.9/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.478092 autoanki-1.0.9/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.479828 autoanki-1.0.9/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)     5171 2023-04-27 16:28:13.000000 autoanki-1.0.9/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.481406 autoanki-1.0.9/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     7268 2023-04-17 17:53:21.000000 autoanki-1.0.9/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.482600 autoanki-1.0.9/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    13282 2023-05-05 17:57:22.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/book_table.sql
+-rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/book_table_view.sql
+-rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/databases_init.sql
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.482838 autoanki-1.0.9/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     6413 2023-04-17 18:46:28.000000 autoanki-1.0.9/src/autoanki/DeckManager/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.483694 autoanki-1.0.9/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)      122 2023-04-17 18:22:48.000000 autoanki-1.0.9/src/autoanki/Dictionary/CC-CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      232 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)     5580 2023-04-17 17:53:21.000000 autoanki-1.0.9/src/autoanki/Dictionary/YellowBridgeDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       58 2023-04-17 18:23:02.000000 autoanki-1.0.9/src/autoanki/Dictionary/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.0.9/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.480956 autoanki-1.0.9/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     4335 2023-05-05 21:40:56.000000 autoanki-1.0.9/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)      798 2023-05-05 21:40:56.000000 autoanki-1.0.9/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:40:56.000000 autoanki-1.0.9/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.0.9/src/autoanki.egg-info/not-zip-safe
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:40:56.000000 autoanki-1.0.9/src/autoanki.egg-info/top_level.txt
```

### Comparing `autoanki-1.0.7/LICENSE.txt` & `autoanki-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.7/PKG-INFO` & `autoanki-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.0.7
+Version: 1.0.9
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autoanki-1.0.7/README.md` & `autoanki-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.7/src/autoanki/AutoAnki.py` & `autoanki-1.0.9/src/autoanki/AutoAnki.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.7/src/autoanki/BookCleaner/BookCleaner.py` & `autoanki-1.0.9/src/autoanki/BookCleaner/BookCleaner.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.7/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.0.9/src/autoanki/DatabaseManager/DatabaseManager.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.7/src/autoanki/DatabaseManager/databases_init.sql` & `autoanki-1.0.9/src/autoanki/DatabaseManager/databases_init.sql`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.7/src/autoanki/DeckManager/__init__.py` & `autoanki-1.0.9/src/autoanki/DeckManager/__init__.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.7/src/autoanki/Dictionary/YellowBridgeDictionary.py` & `autoanki-1.0.9/src/autoanki/Dictionary/YellowBridgeDictionary.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.7/src/autoanki.egg-info/PKG-INFO` & `autoanki-1.0.9/src/autoanki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.0.7
+Version: 1.0.9
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autoanki-1.0.7/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.0.9/src/autoanki.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pyproject.toml
 setup.cfg
 src/autoanki/AutoAnki.py
 src/autoanki/__init__.py
 src/autoanki.egg-info/PKG-INFO
 src/autoanki.egg-info/SOURCES.txt
 src/autoanki.egg-info/dependency_links.txt
-src/autoanki.egg-info/requires.txt
+src/autoanki.egg-info/not-zip-safe
 src/autoanki.egg-info/top_level.txt
 src/autoanki/BookCleaner/BookCleaner.py
 src/autoanki/BookCleaner/__init__.py
 src/autoanki/DatabaseManager/DatabaseManager.py
 src/autoanki/DatabaseManager/__init__.py
 src/autoanki/DatabaseManager/book_table.sql
 src/autoanki/DatabaseManager/book_table_view.sql
```

