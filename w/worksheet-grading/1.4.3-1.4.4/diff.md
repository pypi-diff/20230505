# Comparing `tmp/worksheet_grading-1.4.3.tar.gz` & `tmp/worksheet_grading-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worksheet_grading-1.4.3.tar", last modified: Thu Apr 20 23:35:06 2023, max compression
+gzip compressed data, was "worksheet_grading-1.4.4.tar", last modified: Fri May  5 14:27:03 2023, max compression
```

## Comparing `worksheet_grading-1.4.3.tar` & `worksheet_grading-1.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-04-20 23:35:06.573657 worksheet_grading-1.4.3/
--rw-r--r--   0 klaus     (1000) users      (100)     1074 2022-12-02 02:11:23.000000 worksheet_grading-1.4.3/LICENSE
--rw-r--r--   0 klaus     (1000) users      (100)     9783 2023-04-20 23:35:06.574657 worksheet_grading-1.4.3/PKG-INFO
--rwxr-xr-x   0 klaus     (1000) users      (100)     9368 2023-01-20 19:39:13.000000 worksheet_grading-1.4.3/README.md
--rw-r--r--   0 klaus     (1000) users      (100)      781 2023-04-20 23:35:06.574657 worksheet_grading-1.4.3/setup.cfg
--rw-r--r--   0 klaus     (1000) users      (100)       37 2022-12-02 02:11:23.000000 worksheet_grading-1.4.3/setup.py
-drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-04-20 23:35:06.573657 worksheet_grading-1.4.3/worksheet_grading/
--rw-r--r--   0 klaus     (1000) users      (100)      322 2023-04-20 21:47:46.000000 worksheet_grading-1.4.3/worksheet_grading/__init__.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     2156 2023-01-20 05:17:20.000000 worksheet_grading-1.4.3/worksheet_grading/config.py
--rwxr-xr-x   0 klaus     (1000) users      (100)    28101 2023-04-20 21:47:00.000000 worksheet_grading-1.4.3/worksheet_grading/grade.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     3913 2023-01-20 02:01:10.000000 worksheet_grading-1.4.3/worksheet_grading/grade_export.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     6040 2023-01-20 04:02:29.000000 worksheet_grading-1.4.3/worksheet_grading/grade_import.py
--rwxr-xr-x   0 klaus     (1000) users      (100)    24260 2023-01-20 06:32:52.000000 worksheet_grading-1.4.3/worksheet_grading/gradelib.py
--rw-r--r--   0 klaus     (1000) users      (100)      473 2023-01-20 02:00:29.000000 worksheet_grading-1.4.3/worksheet_grading/moodle_util.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     2984 2022-12-04 01:35:57.000000 worksheet_grading-1.4.3/worksheet_grading/split.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     2943 2023-01-19 03:56:33.000000 worksheet_grading-1.4.3/worksheet_grading/util.py
-drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-04-20 23:35:06.573657 worksheet_grading-1.4.3/worksheet_grading.egg-info/
--rw-r--r--   0 klaus     (1000) users      (100)     9783 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/PKG-INFO
--rw-r--r--   0 klaus     (1000) users      (100)      553 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/SOURCES.txt
--rw-r--r--   0 klaus     (1000) users      (100)        1 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/dependency_links.txt
--rw-r--r--   0 klaus     (1000) users      (100)      194 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/entry_points.txt
--rw-r--r--   0 klaus     (1000) users      (100)       25 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/requires.txt
--rw-r--r--   0 klaus     (1000) users      (100)       18 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/top_level.txt
+drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-05-05 14:27:03.121107 worksheet_grading-1.4.4/
+-rw-r--r--   0 klaus     (1000) users      (100)     1074 2022-12-02 02:11:23.000000 worksheet_grading-1.4.4/LICENSE
+-rw-r--r--   0 klaus     (1000) users      (100)     9783 2023-05-05 14:27:03.121107 worksheet_grading-1.4.4/PKG-INFO
+-rwxr-xr-x   0 klaus     (1000) users      (100)     9368 2023-01-20 19:39:13.000000 worksheet_grading-1.4.4/README.md
+-rw-r--r--   0 klaus     (1000) users      (100)      781 2023-05-05 14:27:03.122107 worksheet_grading-1.4.4/setup.cfg
+-rw-r--r--   0 klaus     (1000) users      (100)       37 2022-12-02 02:11:23.000000 worksheet_grading-1.4.4/setup.py
+drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-05-05 14:27:03.120107 worksheet_grading-1.4.4/worksheet_grading/
+-rw-r--r--   0 klaus     (1000) users      (100)      322 2023-05-05 14:19:08.000000 worksheet_grading-1.4.4/worksheet_grading/__init__.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     2156 2023-01-20 05:17:20.000000 worksheet_grading-1.4.4/worksheet_grading/config.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)    29054 2023-05-05 14:18:42.000000 worksheet_grading-1.4.4/worksheet_grading/grade.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     3913 2023-01-20 02:01:10.000000 worksheet_grading-1.4.4/worksheet_grading/grade_export.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     6040 2023-01-20 04:02:29.000000 worksheet_grading-1.4.4/worksheet_grading/grade_import.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)    24260 2023-01-20 06:32:52.000000 worksheet_grading-1.4.4/worksheet_grading/gradelib.py
+-rw-r--r--   0 klaus     (1000) users      (100)      473 2023-01-20 02:00:29.000000 worksheet_grading-1.4.4/worksheet_grading/moodle_util.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     2984 2022-12-04 01:35:57.000000 worksheet_grading-1.4.4/worksheet_grading/split.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     2943 2023-01-19 03:56:33.000000 worksheet_grading-1.4.4/worksheet_grading/util.py
+drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-05-05 14:27:03.121107 worksheet_grading-1.4.4/worksheet_grading.egg-info/
+-rw-r--r--   0 klaus     (1000) users      (100)     9783 2023-05-05 14:27:03.000000 worksheet_grading-1.4.4/worksheet_grading.egg-info/PKG-INFO
+-rw-r--r--   0 klaus     (1000) users      (100)      553 2023-05-05 14:27:03.000000 worksheet_grading-1.4.4/worksheet_grading.egg-info/SOURCES.txt
+-rw-r--r--   0 klaus     (1000) users      (100)        1 2023-05-05 14:27:03.000000 worksheet_grading-1.4.4/worksheet_grading.egg-info/dependency_links.txt
+-rw-r--r--   0 klaus     (1000) users      (100)      194 2023-05-05 14:27:03.000000 worksheet_grading-1.4.4/worksheet_grading.egg-info/entry_points.txt
+-rw-r--r--   0 klaus     (1000) users      (100)       25 2023-05-05 14:27:03.000000 worksheet_grading-1.4.4/worksheet_grading.egg-info/requires.txt
+-rw-r--r--   0 klaus     (1000) users      (100)       18 2023-05-05 14:27:03.000000 worksheet_grading-1.4.4/worksheet_grading.egg-info/top_level.txt
```

### Comparing `worksheet_grading-1.4.3/LICENSE` & `worksheet_grading-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.3/PKG-INFO` & `worksheet_grading-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worksheet_grading
-Version: 1.4.3
+Version: 1.4.4
 Summary: Exercise sheet grading utility with Moodle support
 Home-page: https://gitlab.com/kdvkrs/worksheet_grading
 Author: Klaus Kraßnitzer
 Author-email: klaus@krss.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `worksheet_grading-1.4.3/README.md` & `worksheet_grading-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.3/setup.cfg` & `worksheet_grading-1.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.3/worksheet_grading/config.py` & `worksheet_grading-1.4.4/worksheet_grading/config.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.3/worksheet_grading/grade.py` & `worksheet_grading-1.4.4/worksheet_grading/grade.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 # stdlib imports
 import argparse
 import webbrowser
 import subprocess
 import statistics
+from collections import defaultdict
 
 # external imports
 import readchar
 import readline # overwrite input() for arrow key support
 
 # local imports
 from worksheet_grading.util import *
@@ -110,15 +111,28 @@
             c = None
 
     return c
 
 
 def menu(frame: Frame):
     while True:
-        message = "\n" + bright(light_blue("{} V{}".format(__program__, __version__))) + "\n\n"
+        message = ""
+        # partially graded exercises
+        pg_exc = partially_graded_exercises(frame)
+        # show partially graded exercises
+        if len(pg_exc) > 0:
+            warn = lambda t: bright(red(t))
+            num_pg = sum(len(e) for e in pg_exc.values())
+            message += warn(f"There {'are' if num_pg > 1 else 'is'} {num_pg} partially graded {'exercises' if num_pg > 1 else 'exercise'} the grading state of which will be lost if not graded before exit!\n")
+            message += warn("Partially graded exercises:\n")
+            for e in pg_exc:
+                message += red(f"\t{e}: {pg_exc[e]}\n")
+
+
+        message += "\n" + bright(light_blue("{} V{}".format(__program__, __version__))) + "\n\n"
         message += group_overview(frame)
         actions = [
             ("g", "Quick Grade", act_quick_grade),
             ("s", "Search a group", act_search_group),
             ("a", "Show all groups", act_all_groups),
             ("w", "Write to CSV files", act_write_output),
             ("c", "Check deductions", act_sanity_check),
@@ -741,25 +755,25 @@
 
 def act_sanity_check(state: State):
     points = sc_points()
     sane = True
     for e in state.frame.data.values():
         for ex in e.sheet.exercises.values():
             for a in ex.answers:
-                if a.deductions.deducted_points() < -1 * points[ex.number - 1][a.num - 1]:
+                if a.deductions.deducted_points() < -1 * points[ex.number][a.num-1]:
                     print(red("Invalid deduction found for group \"{}\" exercise {}.{}").format(e.group,
                                                                                                 ex.number, a.num))
                     sane = False
 
     if not sane:
         print()
         print(red("Invalid deductions found, see above output"))
     else:
         print(green("No invalid deductions found"))
-    
+
 
 def act_statistics(state: State):
     stat_frame = state.frame.csv_df
     groups = state.frame.data.keys()
     stat_pts = []
     for g in groups:
         if state.frame.data[g].sheet.grade_status() == GradeStatus.GRADED:
@@ -789,21 +803,30 @@
 def reset_max_lens():
     config.MAX_GROUP_LEN = 0
     config.MAX_NAMES_LEN = 0
 
 
 # Points for sanity check
 def sc_points():
-    points = []
+    points = {}
     for i in config.DEFAULT_MASK:
         exc = config.EXERCISES.get(str(i))
         if exc is not None:
-            points.append(exc)
+            points[i] = exc
     return points
 
+
+def partially_graded_exercises(frame: Frame):
+    pg_exc = defaultdict(list)
+    for e in frame.data.values():
+        for ex in e.sheet.exercises.values():
+            if ex.grade_status == GradeStatus.PARTIALLY_GRADED:
+                pg_exc[e.group].append(ex.number)
+    return pg_exc
+
 # ========== MAIN ========== #
 
 def main():
     # Parse arguments
     parser = argparse.ArgumentParser(__program__, description="Interactive exercise grading tool", formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('-e', '--exercises', default="{}-{}".format(config.DEFAULT_FIRSTEX, config.DEFAULT_LASTEX),
                         help="Exercises that should be considered, must either be a range (e.g., 1-5), comma-separated list (1,4,6) or single exercise (e.g., 3)")
```

### Comparing `worksheet_grading-1.4.3/worksheet_grading/grade_export.py` & `worksheet_grading-1.4.4/worksheet_grading/grade_export.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.3/worksheet_grading/grade_import.py` & `worksheet_grading-1.4.4/worksheet_grading/grade_import.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.3/worksheet_grading/gradelib.py` & `worksheet_grading-1.4.4/worksheet_grading/gradelib.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.3/worksheet_grading/split.py` & `worksheet_grading-1.4.4/worksheet_grading/split.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.3/worksheet_grading/util.py` & `worksheet_grading-1.4.4/worksheet_grading/util.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.3/worksheet_grading.egg-info/PKG-INFO` & `worksheet_grading-1.4.4/worksheet_grading.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worksheet-grading
-Version: 1.4.3
+Version: 1.4.4
 Summary: Exercise sheet grading utility with Moodle support
 Home-page: https://gitlab.com/kdvkrs/worksheet_grading
 Author: Klaus Kraßnitzer
 Author-email: klaus@krss.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `worksheet_grading-1.4.3/worksheet_grading.egg-info/SOURCES.txt` & `worksheet_grading-1.4.4/worksheet_grading.egg-info/SOURCES.txt`

 * *Files identical despite different names*

