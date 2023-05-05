# Comparing `tmp/lms_synergy_library-0.1.2.tar.gz` & `tmp/lms_synergy_library-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lms_synergy_library-0.1.2.tar", last modified: Tue Jan 31 13:30:46 2023, max compression
+gzip compressed data, was "lms_synergy_library-0.2.0.tar", last modified: Fri May  5 10:29:28 2023, max compression
```

## Comparing `lms_synergy_library-0.1.2.tar` & `lms_synergy_library-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 kotorkovsciy  (1000) kotorkovsciy  (1000)        0 2023-01-31 13:30:46.422728 lms_synergy_library-0.1.2/
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)     1073 2023-01-30 11:34:43.000000 lms_synergy_library-0.1.2/LICENSE
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)     1413 2023-01-31 13:30:46.414728 lms_synergy_library-0.1.2/PKG-INFO
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)      799 2023-01-31 10:19:16.000000 lms_synergy_library-0.1.2/README.md
-drwxrwxr-x   0 kotorkovsciy  (1000) kotorkovsciy  (1000)        0 2023-01-31 13:30:46.398728 lms_synergy_library-0.1.2/lms_synergy_library/
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)       36 2023-01-31 13:13:34.000000 lms_synergy_library-0.1.2/lms_synergy_library/__init__.py
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)     8861 2023-01-31 10:03:40.000000 lms_synergy_library-0.1.2/lms_synergy_library/lms_synergy_library.py
-drwxrwxr-x   0 kotorkovsciy  (1000) kotorkovsciy  (1000)        0 2023-01-31 13:30:46.414728 lms_synergy_library-0.1.2/lms_synergy_library.egg-info/
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)     1413 2023-01-31 13:30:46.000000 lms_synergy_library-0.1.2/lms_synergy_library.egg-info/PKG-INFO
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)      321 2023-01-31 13:30:46.000000 lms_synergy_library-0.1.2/lms_synergy_library.egg-info/SOURCES.txt
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)        1 2023-01-31 13:30:46.000000 lms_synergy_library-0.1.2/lms_synergy_library.egg-info/dependency_links.txt
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)       39 2023-01-31 13:30:46.000000 lms_synergy_library-0.1.2/lms_synergy_library.egg-info/requires.txt
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)       20 2023-01-31 13:30:46.000000 lms_synergy_library-0.1.2/lms_synergy_library.egg-info/top_level.txt
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)      760 2023-01-31 13:30:09.000000 lms_synergy_library-0.1.2/pyproject.toml
--rw-rw-r--   0 kotorkovsciy  (1000) kotorkovsciy  (1000)       38 2023-01-31 13:30:46.422728 lms_synergy_library-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:28.439326 lms_synergy_library-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 10:28:56.000000 lms_synergy_library-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-05 10:29:28.439326 lms_synergy_library-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-05 10:28:56.000000 lms_synergy_library-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:28.439326 lms_synergy_library-0.2.0/lms_synergy_library/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 10:28:56.000000 lms_synergy_library-0.2.0/lms_synergy_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-05 10:28:56.000000 lms_synergy_library-0.2.0/lms_synergy_library/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 10:28:56.000000 lms_synergy_library-0.2.0/lms_synergy_library/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27586 2023-05-05 10:28:56.000000 lms_synergy_library-0.2.0/lms_synergy_library/lms_synergy_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-05 10:28:56.000000 lms_synergy_library-0.2.0/lms_synergy_library/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:28.439326 lms_synergy_library-0.2.0/lms_synergy_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-05 10:29:28.000000 lms_synergy_library-0.2.0/lms_synergy_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-05 10:29:28.000000 lms_synergy_library-0.2.0/lms_synergy_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:29:28.000000 lms_synergy_library-0.2.0/lms_synergy_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 10:29:28.000000 lms_synergy_library-0.2.0/lms_synergy_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 10:29:28.000000 lms_synergy_library-0.2.0/lms_synergy_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-05 10:28:56.000000 lms_synergy_library-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:29:28.439326 lms_synergy_library-0.2.0/setup.cfg
```

### Comparing `lms_synergy_library-0.1.2/LICENSE` & `lms_synergy_library-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lms_synergy_library-0.1.2/PKG-INFO` & `lms_synergy_library-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lms_synergy_library
-Version: 0.1.2
+Version: 0.2.0
 Summary: A library that allows you to work with LMS
 Author-email: Nikita Kovinjko <kotorkovsciy@gmail.com>
 Project-URL: Homepage, https://github.com/kotorkovsciy/lms-synergy-library
 Project-URL: Bug Tracker, https://github.com/kotorkovsciy/lms-synergy-library/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,38 @@
 
 # get information about user
 lms.get_info()
 
 # get shedule
 lms.get_schedule()
 
+# get news
+lms.get_news()
+
+# get disciplines
+lms.get_disciplines()
+
+# get amount unverified work
+lms.get_amount_unverified_work()
+
+# get pesonal curators
+lms.get_pesonal_curators()
+
+# get tutors
+lms.get_tutors()
+
+# get notifications
+lms.get_notify()
+
+# get notifications archive
+lms.get_notify_archive()
+
+# get unread messages
+lms.get_unread_messages()
+
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `lms_synergy_library-0.1.2/lms_synergy_library.egg-info/PKG-INFO` & `lms_synergy_library-0.2.0/lms_synergy_library.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lms-synergy-library
-Version: 0.1.2
+Version: 0.2.0
 Summary: A library that allows you to work with LMS
 Author-email: Nikita Kovinjko <kotorkovsciy@gmail.com>
 Project-URL: Homepage, https://github.com/kotorkovsciy/lms-synergy-library
 Project-URL: Bug Tracker, https://github.com/kotorkovsciy/lms-synergy-library/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,38 @@
 
 # get information about user
 lms.get_info()
 
 # get shedule
 lms.get_schedule()
 
+# get news
+lms.get_news()
+
+# get disciplines
+lms.get_disciplines()
+
+# get amount unverified work
+lms.get_amount_unverified_work()
+
+# get pesonal curators
+lms.get_pesonal_curators()
+
+# get tutors
+lms.get_tutors()
+
+# get notifications
+lms.get_notify()
+
+# get notifications archive
+lms.get_notify_archive()
+
+# get unread messages
+lms.get_unread_messages()
+
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `lms_synergy_library-0.1.2/pyproject.toml` & `lms_synergy_library-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lms_synergy_library"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
     {name = "Nikita Kovinjko", email = "kotorkovsciy@gmail.com"},
 ]
 description = "A library that allows you to work with LMS"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

