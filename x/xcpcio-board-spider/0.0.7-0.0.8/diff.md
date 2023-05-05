# Comparing `tmp/xcpcio_board_spider-0.0.7.tar.gz` & `tmp/xcpcio_board_spider-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcpcio_board_spider-0.0.7.tar", max compression
+gzip compressed data, was "xcpcio_board_spider-0.0.8.tar", max compression
```

## Comparing `xcpcio_board_spider-0.0.7.tar` & `xcpcio_board_spider-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-05-02 16:10:27.416997 xcpcio_board_spider-0.0.7/LICENSE
--rw-r--r--   0        0        0      538 2023-05-02 16:10:27.416997 xcpcio_board_spider-0.0.7/README.md
--rw-r--r--   0        0        0     1004 2023-05-02 16:10:27.420997 xcpcio_board_spider-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       40 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/__init__.py
--rw-r--r--   0        0        0       34 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/__init__.py
--rw-r--r--   0        0        0      377 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/logger.py
--rw-r--r--   0        0        0     1074 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/logo.py
--rw-r--r--   0        0        0     1863 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/spider/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/spider/domjudge/__init__.py
--rw-r--r--   0        0        0       24 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/spider/domjudge/v2/__init__.py
--rw-r--r--   0        0        0     5319 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/spider/domjudge/v2/domjudge.py
--rw-r--r--   0        0        0      113 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/__init__.py
--rw-r--r--   0        0        0      303 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/constants.py
--rw-r--r--   0        0        0     2492 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/contest.py
--rw-r--r--   0        0        0     1041 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/submission.py
--rw-r--r--   0        0        0     1585 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/team.py
--rw-r--r--   0        0        0      262 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/type.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-05 16:17:38.797640 xcpcio_board_spider-0.0.8/LICENSE
+-rw-r--r--   0        0        0      538 2023-05-05 16:17:38.797640 xcpcio_board_spider-0.0.8/README.md
+-rw-r--r--   0        0        0     1004 2023-05-05 16:17:38.801640 xcpcio_board_spider-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/__init__.py
+-rw-r--r--   0        0        0      377 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/logger.py
+-rw-r--r--   0        0        0     1074 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/logo.py
+-rw-r--r--   0        0        0     1863 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/domjudge/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/domjudge/v2/__init__.py
+-rw-r--r--   0        0        0     5319 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/domjudge/v2/domjudge.py
+-rw-r--r--   0        0        0      113 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/__init__.py
+-rw-r--r--   0        0        0      303 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/constants.py
+-rw-r--r--   0        0        0     3288 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/contest.py
+-rw-r--r--   0        0        0     1020 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/submission.py
+-rw-r--r--   0        0        0     1555 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/team.py
+-rw-r--r--   0        0        0      262 2023-05-05 16:17:38.837640 xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/type.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.8/PKG-INFO
```

### Comparing `xcpcio_board_spider-0.0.7/LICENSE` & `xcpcio_board_spider-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.7/README.md` & `xcpcio_board_spider-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.7/pyproject.toml` & `xcpcio_board_spider-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcpcio-board-spider"
-version = "0.0.7"
+version = "0.0.8"
 description = "XCPCIO Board Spider"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/logo.py` & `xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/logo.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/utils.py` & `xcpcio_board_spider-0.0.8/xcpcio_board_spider/core/utils.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.7/xcpcio_board_spider/spider/domjudge/v2/domjudge.py` & `xcpcio_board_spider-0.0.8/xcpcio_board_spider/spider/domjudge/v2/domjudge.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/contest.py` & `xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/contest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import typing
+import json
+
 from .type import *
 
 
 class Contest:
     def __init__(self,
                  contest_name: str = "",
                  start_time: int = 0,
@@ -28,14 +30,16 @@
         self.organization = organization
         self.status_time_display = status_time_display
         self.medal = medal
         self.balloon_color = [Color(**item) for item in balloon_color]
 
         if logo is not None:
             self.logo = Image(**logo)
+        else:
+            self.logo = None
 
     def fill_problem_id(self):
         self.problem_id = [chr(ord('A') + i)
                            for i in range(self.problem_quantity)]
 
     def fill_balloon_color(self):
         default_balloon_color_list = [
@@ -51,7 +55,27 @@
             Color(background_color='rgba(159, 19, 236, 0.7)', color='#fff'),
             Color(background_color='rgba(42, 197, 202, 0.7)', color='#fff'),
             Color(background_color='rgba(142, 56, 54, 0.7)', color='#fff'),
             Color(background_color='rgba(0, 0, 0, 0.7)', color='#fff'),
         ]
 
         self.balloon_color = default_balloon_color_list[:self.problem_quantity]
+
+    @property
+    def __json__(self):
+        json_obj = {}
+
+        json_obj["contest_name"] = self.contest_name
+        json_obj["start_time"] = self.start_time
+        json_obj["end_time"] = self.end_time
+        json_obj["frozen_time"] = self.frozen_time
+        json_obj["penalty"] = self.penalty
+        json_obj["problem_quantity"] = self.problem_quantity
+        json_obj["problem_id"] = self.problem_id
+        json_obj["group"] = self.group
+        json_obj["organization"] = self.organization
+        json_obj["status_time_display"] = self.status_time_display
+        json_obj["medal"] = self.medal
+        json_obj["balloon_color"] = self.balloon_color
+        json_obj["logo"] = self.logo
+
+        return json.dumps(json_obj)
```

### Comparing `xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/submission.py` & `xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/submission.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,25 +14,25 @@
         self.timestamp = timestamp
         self.status = status
 
         self.submission_id = submission_id
 
     @property
     def __json__(self):
-        json_string = {}
+        json_obj = {}
 
-        json_string["team_id"] = self.team_id
-        json_string["problem_id"] = self.problem_id
-        json_string["timestamp"] = self.timestamp
-        json_string["status"] = self.status
+        json_obj["team_id"] = self.team_id
+        json_obj["problem_id"] = self.problem_id
+        json_obj["timestamp"] = self.timestamp
+        json_obj["status"] = self.status
 
         if self.submission_id is not None:
-            json_string["submission_id"] = self.submission_id
+            json_obj["submission_id"] = self.submission_id
 
-        return json_string
+        return json_obj
 
 
 ISubmissions = typing.List[Submission]
 
 
 class Submissions(ISubmissions):
     def __init__(self):
```

### Comparing `xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/team.py` & `xcpcio_board_spider-0.0.8/xcpcio_board_spider/type/team.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,33 +24,33 @@
         self.unofficial = unofficial
         self.girl = girl
 
         self.extra = extra
 
     @property
     def __json__(self):
-        json_string = {}
+        json_obj = {}
 
-        json_string["team_id"] = self.team_id
-        json_string["name"] = self.name
-        json_string["organization"] = self.organization
+        json_obj["team_id"] = self.team_id
+        json_obj["name"] = self.name
+        json_obj["organization"] = self.organization
 
         if self.members is not None:
-            json_string["members"] = self.members
+            json_obj["members"] = self.members
         if self.coach is not None:
-            json_string["coach"] = self.coach
+            json_obj["coach"] = self.coach
 
         if self.official is not None:
-            json_string["official"] = self.official
+            json_obj["official"] = self.official
         if self.unofficial is not None:
-            json_string["unofficial"] = self.unofficial
+            json_obj["unofficial"] = self.unofficial
         if self.girl is not None:
-            json_string["girl"] = self.girl
+            json_obj["girl"] = self.girl
 
-        return json_string
+        return json_obj
 
 
 ITeams = typing.Dict[str, Team]
 
 
 class Teams(ITeams):
     def __init__(self):
```

### Comparing `xcpcio_board_spider-0.0.7/PKG-INFO` & `xcpcio_board_spider-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcpcio-board-spider
-Version: 0.0.7
+Version: 0.0.8
 Summary: XCPCIO Board Spider
 License: MIT
 Author: Dup4
 Author-email: lyuzhi.pan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

