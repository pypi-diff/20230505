# Comparing `tmp/pokerlib-2.2.1.tar.gz` & `tmp/pokerlib-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerlib-2.2.1.tar", max compression
+gzip compressed data, was "pokerlib-2.2.2.tar", max compression
```

## Comparing `pokerlib-2.2.1.tar` & `pokerlib-2.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.1/LICENSE
--rw-r--r--   0        0        0     6276 2023-05-02 19:42:40.871493 pokerlib-2.2.1/README.md
--rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.1/pokerlib/__init__.py
--rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/_handparser.py
--rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/_player.py
--rw-r--r--   0        0        0    17719 2023-05-02 19:48:34.711495 pokerlib-2.2.1/pokerlib/_round.py
--rw-r--r--   0        0        0     6936 2023-04-07 09:33:14.596230 pokerlib-2.2.1/pokerlib/_table.py
--rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/enums.py
--rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/implementations/__init__.py
--rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/implementations/_no_muck_showdown_table.py
--rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.1/pokerlib/implementations/_no_muck_table.py
--rw-r--r--   0        0        0      663 2023-05-02 20:03:26.111499 pokerlib-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     7001 1970-01-01 00:00:00.000000 pokerlib-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.2/LICENSE
+-rw-r--r--   0        0        0     6276 2023-05-02 19:42:40.871493 pokerlib-2.2.2/README.md
+-rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.2/pokerlib/__init__.py
+-rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/_handparser.py
+-rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/_player.py
+-rw-r--r--   0        0        0    17675 2023-05-05 19:27:14.959085 pokerlib-2.2.2/pokerlib/_round.py
+-rw-r--r--   0        0        0     6936 2023-04-07 09:33:14.596230 pokerlib-2.2.2/pokerlib/_table.py
+-rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/enums.py
+-rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/implementations/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/implementations/_no_muck_showdown_table.py
+-rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/implementations/_no_muck_table.py
+-rw-r--r--   0        0        0      663 2023-05-05 19:32:10.249004 pokerlib-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7001 1970-01-01 00:00:00.000000 pokerlib-2.2.2/PKG-INFO
```

### Comparing `pokerlib-2.2.1/LICENSE` & `pokerlib-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.1/README.md` & `pokerlib-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.1/pokerlib/_handparser.py` & `pokerlib-2.2.2/pokerlib/_handparser.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.1/pokerlib/_player.py` & `pokerlib-2.2.2/pokerlib/_player.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.1/pokerlib/_round.py` & `pokerlib-2.2.2/pokerlib/_round.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,18 @@
         return self.players.nextUnfoldedIndex(self.button)
     @property
     def last_aggressor_index(self):
         return self.players.previousUnfoldedIndex(
             self.current_index)
     @property
     def small_blind_player_index(self):
-        return self.button - 2 if len(self.players) > 2 else self.button - 1
+        return (self.button - 1) % len(self.players)
     @property
     def big_blind_player_index(self):
-        return self.button - 1 if len(self.players) > 2 else self.button
+        return (self.button - 2) % len(self.players)
 
     @property
     def current_player(self):
         return self.players[self.current_index]
 
     @property
     def turn_stake(self):
```

### Comparing `pokerlib-2.2.1/pokerlib/_table.py` & `pokerlib-2.2.2/pokerlib/_table.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.1/pokerlib/enums.py` & `pokerlib-2.2.2/pokerlib/enums.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.1/pyproject.toml` & `pokerlib-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokerlib"
-version = "2.2.1"
+version = "2.2.2"
 description = "Python poker library"
 repository = "https://github.com/kuco23/pokerlib/"
 authors = ["kuco23 <nseverkar@gmail.com>"]
 keywords = ['python', 'poker', 'library']
 readme = "README.md"
 classifiers=  [
     'Development Status :: 3 - Alpha',
```

### Comparing `pokerlib-2.2.1/PKG-INFO` & `pokerlib-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerlib
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python poker library
 Home-page: https://github.com/kuco23/pokerlib/
 Keywords: python,poker,library
 Author: kuco23
 Author-email: nseverkar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

