# Comparing `tmp/easierfile-2.1.0.tar.gz` & `tmp/easierfile-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierfile-2.1.0.tar", max compression
+gzip compressed data, was "easierfile-2.2.0.tar", max compression
```

## Comparing `easierfile-2.1.0.tar` & `easierfile-2.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       62 2023-04-21 13:34:36.835394 easierfile-2.1.0/easierfile/__init__.py
--rw-r--r--   0        0        0     4903 2023-05-01 13:07:38.204733 easierfile-2.1.0/easierfile/file.py
--rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-2.1.0/LICENSE
--rw-r--r--   0        0        0      588 2023-05-01 12:41:45.401879 easierfile-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1676 2023-05-01 13:21:24.795756 easierfile-2.1.0/README.md
--rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 easierfile-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-04-21 13:34:36.835394 easierfile-2.2.0/easierfile/__init__.py
+-rw-r--r--   0        0        0     4898 2023-05-05 14:27:07.021333 easierfile-2.2.0/easierfile/file.py
+-rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-2.2.0/LICENSE
+-rw-r--r--   0        0        0      588 2023-05-05 14:29:41.381108 easierfile-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1676 2023-05-01 13:21:24.795756 easierfile-2.2.0/README.md
+-rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 easierfile-2.2.0/PKG-INFO
```

### Comparing `easierfile-2.1.0/easierfile/file.py` & `easierfile-2.2.0/easierfile/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 self.__lock(False)
             except FileNotFoundError:  # Indicates that the file lock does not exist and no further exception handling is required.
                 pass
 
     def __lock(self, is_lock):
         if self.status["exist"]:
             if is_lock:
-                self.__m_file = open(self.__m_info["path"], "w")
+                self.__m_file = open(self.__m_info["path"])
                 _lock_file(self.__m_file)
                 self.__m_is_lock = is_lock
             else:
                 _unlock_file(self.__m_file)
                 self.__m_file.close()
                 self.__m_is_lock = is_lock
         else:
```

### Comparing `easierfile-2.1.0/LICENSE` & `easierfile-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easierfile-2.1.0/pyproject.toml` & `easierfile-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easierfile"
-version = "2.1.0"
+version = "2.2.0"
 description = "An easier-to-use Python package that object-oriented encapsulates Python traditional built-in file operations."
 license = "MIT"
 authors = ["leoweyr <leoweyr@foxmail.com>"]
 readme = "README.md"
 repository = "https://github.com/leoweyr/Python-Easierfile"
 classifiers = [
     "Development Status :: 4 - Beta"
```

### Comparing `easierfile-2.1.0/README.md` & `easierfile-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `easierfile-2.1.0/PKG-INFO` & `easierfile-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierfile
-Version: 2.1.0
+Version: 2.2.0
 Summary: An easier-to-use Python package that object-oriented encapsulates Python traditional built-in file operations.
 Home-page: https://github.com/leoweyr/Python-Easierfile
 License: MIT
 Author: leoweyr
 Author-email: leoweyr@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

