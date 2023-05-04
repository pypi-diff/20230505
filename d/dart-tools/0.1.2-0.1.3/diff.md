# Comparing `tmp/dart-tools-0.1.2.tar.gz` & `tmp/dart-tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.1.2.tar", last modified: Thu Apr 13 20:39:45 2023, max compression
+gzip compressed data, was "dart-tools-0.1.3.tar", last modified: Thu May  4 23:32:41 2023, max compression
```

## Comparing `dart-tools-0.1.2.tar` & `dart-tools-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-04-13 20:39:45.249085 dart-tools-0.1.2/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.1.2/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     4408 2023-04-13 20:39:45.248750 dart-tools-0.1.2/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.1.2/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-04-13 20:39:45.245988 dart-tools-0.1.2/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.1.2/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    11087 2023-04-13 20:37:15.000000 dart-tools-0.1.2/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.1.2/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-04-13 20:39:45.248256 dart-tools-0.1.2/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     4408 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      290 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/dependency_links.txt
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       14 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1789 2023-04-13 20:34:41.000000 dart-tools-0.1.2/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-04-13 20:39:45.249195 dart-tools-0.1.2/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-04 23:32:41.277038 dart-tools-0.1.3/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.1.3/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4408 2023-05-04 23:32:41.276565 dart-tools-0.1.3/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.1.3/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-04 23:32:41.273026 dart-tools-0.1.3/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.1.3/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    11532 2023-05-04 23:26:01.000000 dart-tools-0.1.3/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.1.3/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-04 23:32:41.276058 dart-tools-0.1.3/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4408 2023-05-04 23:32:41.000000 dart-tools-0.1.3/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      290 2023-05-04 23:32:41.000000 dart-tools-0.1.3/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-05-04 23:32:41.000000 dart-tools-0.1.3/dart_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-05-04 23:32:41.000000 dart-tools-0.1.3/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       14 2023-05-04 23:32:41.000000 dart-tools-0.1.3/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-05-04 23:32:41.000000 dart-tools-0.1.3/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1789 2023-05-04 23:26:24.000000 dart-tools-0.1.3/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-05-04 23:32:41.277150 dart-tools-0.1.3/setup.cfg
```

### Comparing `dart-tools-0.1.2/LICENSE` & `dart-tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.1.2/PKG-INFO` & `dart-tools-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.1.2 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.1.3 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.1.2/README.md` & `dart-tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.1.2/dart/dart.py` & `dart-tools-0.1.3/dart/dart.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,34 @@
 _CLIENT_DUID_KEY = "clientDuid"
 _HOST_KEY = "host"
 _HOSTS_KEY = "hosts"
 _CSRF_TOKEN_KEY = "csrfToken"
 _SESSION_ID_KEY = "sessionId"
 
 _DUID_CHARS = string.ascii_lowercase + string.ascii_uppercase + string.digits + "-_"
-_TERM_STATUS_KINDS = {"Finished", "Canceled"}
+_COMPLETED_STATUS_KINDS = {"Finished", "Canceled"}
+_DEFAULT_DESCRIPTION = {
+    "root": {
+        "direction": None,
+        "format": "",
+        "indent": 0,
+        "type": "root",
+        "version": 1,
+        "children": [
+            {
+                "direction": None,
+                "format": "",
+                "indent": 0,
+                "type": "paragraph",
+                "version": 1,
+                "children": [],
+            }
+        ],
+    }
+}
 
 
 # TODO dedupe these functions with other usages elsewhere
 def _make_duid():
     return "".join(random.choices(_DUID_CHARS, k=12))
 
 
@@ -264,15 +283,15 @@
     user_email = user_bundle["user"]["email"]
     active_duid = next(
         e["duid"] for e in user_bundle["dartboards"] if e["kind"] == "Active"
     )
     unterm_status_duids = {
         e["duid"]
         for e in user_bundle["statuses"]
-        if e["kind"] not in _TERM_STATUS_KINDS
+        if e["kind"] not in _COMPLETED_STATUS_KINDS
     }
     filtered_tasks = [
         e
         for e in user_bundle["tasks"]
         if not e["inTrash"]
         and e["dartboardDuid"] == active_duid
         and user_email in e["assigneeEmails"]
@@ -321,15 +340,15 @@
     task = {
         "duid": _make_duid(),
         "uuid": str(uuid4()),
         "drafterEmail": None,
         "dartboardUuid": active_uuid,
         "order": order,
         "title": title,
-        "description": "",
+        "description": _DEFAULT_DESCRIPTION,
         "statusDuid": status_duid,
         "assigneeEmails": [user_email],
         "subscriberEmails": [user_email],
         "tagDuids": [],
         "priority": None,
         "size": None,
         "dueAt": None,
```

### Comparing `dart-tools-0.1.2/dart/order_manager.py` & `dart-tools-0.1.3/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.1.2/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.1.3/dart_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.1.2 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.1.3 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.1.2/pyproject.toml` & `dart-tools-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.1.2"
+version = "0.1.3"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.7"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

