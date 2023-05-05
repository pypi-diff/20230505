# Comparing `tmp/ltbfiles-2.3.1.tar.gz` & `tmp/ltbfiles-2.3.1rc82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltbfiles-2.3.1.tar", last modified: Fri May  5 13:33:53 2023, max compression
+gzip compressed data, was "ltbfiles-2.3.1rc82.tar", last modified: Fri May  5 13:30:05 2023, max compression
```

## Comparing `ltbfiles-2.3.1.tar` & `ltbfiles-2.3.1rc82.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:33:53.250104 ltbfiles-2.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-05-05 13:33:39.000000 ltbfiles-2.3.1/LICENSE_GPL_v3.txt
--rw-r--r--   0 root         (0) root         (0)     1115 2023-05-05 13:33:53.250104 ltbfiles-2.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      548 2023-05-05 13:33:39.000000 ltbfiles-2.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:33:53.247104 ltbfiles-2.3.1/ltbfiles/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-05 13:33:39.000000 ltbfiles-2.3.1/ltbfiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15777 2023-05-05 13:33:39.000000 ltbfiles-2.3.1/ltbfiles/ltbfiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:33:53.249104 ltbfiles-2.3.1/ltbfiles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1115 2023-05-05 13:33:53.000000 ltbfiles-2.3.1/ltbfiles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-05 13:33:53.000000 ltbfiles-2.3.1/ltbfiles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 13:33:53.000000 ltbfiles-2.3.1/ltbfiles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-05 13:33:53.000000 ltbfiles-2.3.1/ltbfiles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 13:33:53.000000 ltbfiles-2.3.1/ltbfiles.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-05-05 13:33:39.000000 ltbfiles-2.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 13:33:53.250104 ltbfiles-2.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:33:53.249104 ltbfiles-2.3.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4776 2023-05-05 13:33:39.000000 ltbfiles-2.3.1/tests/test_load_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.861968 ltbfiles-2.3.1rc82/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/LICENSE_GPL_v3.txt
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-05 13:30:05.861968 ltbfiles-2.3.1rc82/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.858968 ltbfiles-2.3.1rc82/ltbfiles/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/ltbfiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15777 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/ltbfiles/ltbfiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.860968 ltbfiles-2.3.1rc82/ltbfiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-05 13:30:05.861968 ltbfiles-2.3.1rc82/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.860968 ltbfiles-2.3.1rc82/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4776 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/tests/test_load_files.py
```

### Comparing `ltbfiles-2.3.1/LICENSE_GPL_v3.txt` & `ltbfiles-2.3.1rc82/LICENSE_GPL_v3.txt`

 * *Files identical despite different names*

### Comparing `ltbfiles-2.3.1/PKG-INFO` & `ltbfiles-2.3.1rc82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 2.3.1
+Version: 2.3.1rc82
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ltbfiles-2.3.1/README.md` & `ltbfiles-2.3.1rc82/README.md`

 * *Files identical despite different names*

### Comparing `ltbfiles-2.3.1/ltbfiles/ltbfiles.py` & `ltbfiles-2.3.1rc82/ltbfiles/ltbfiles.py`

 * *Files identical despite different names*

### Comparing `ltbfiles-2.3.1/ltbfiles.egg-info/PKG-INFO` & `ltbfiles-2.3.1rc82/ltbfiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 2.3.1
+Version: 2.3.1rc82
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ltbfiles-2.3.1/pyproject.toml` & `ltbfiles-2.3.1rc82/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ltbfiles-2.3.1/tests/test_load_files.py` & `ltbfiles-2.3.1rc82/tests/test_load_files.py`

 * *Files identical despite different names*

