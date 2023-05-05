# Comparing `tmp/robotframework-debug-4.3.2.tar.gz` & `tmp/robotframework-debug-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-debug-4.3.2.tar", last modified: Wed Apr 12 20:00:15 2023, max compression
+gzip compressed data, was "robotframework-debug-4.3.3.tar", last modified: Fri May  5 16:32:41 2023, max compression
```

## Comparing `robotframework-debug-4.3.2.tar` & `robotframework-debug-4.3.3.tar`

### file list

```diff
@@ -1,43 +1,40 @@
-drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-12 20:00:15.017619 robotframework-debug-4.3.2/
--rw-r--r--   0 snooz      (501) staff       (20)      545 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/.coveragerc
--rw-r--r--   0 snooz      (501) staff       (20)      272 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/.gitpod.yml
--rw-r--r--   0 snooz      (501) staff       (20)     5811 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/ChangeLog
--rw-r--r--   0 snooz      (501) staff       (20)      139 2023-03-20 22:34:10.000000 robotframework-debug-4.3.2/CreateWheel.sh
--rw-r--r--   0 snooz      (501) staff       (20)     1471 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/LICENSE
--rw-r--r--   0 snooz      (501) staff       (20)      215 2023-03-15 21:54:14.000000 robotframework-debug-4.3.2/MANIFEST.in
--rw-r--r--   0 snooz      (501) staff       (20)     6027 2023-04-12 20:00:15.017718 robotframework-debug-4.3.2/PKG-INFO
--rw-r--r--   0 snooz      (501) staff       (20)     5047 2023-03-19 19:57:13.000000 robotframework-debug-4.3.2/README.rst
-drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-12 20:00:15.014631 robotframework-debug-4.3.2/RobotDebug/
--rw-r--r--   0 snooz      (501) staff       (20)     5878 2023-03-31 20:37:02.000000 robotframework-debug-4.3.2/RobotDebug/RobotDebug.py
--rw-r--r--   0 snooz      (501) staff       (20)      154 2023-03-31 08:22:53.000000 robotframework-debug-4.3.2/RobotDebug/__init__.py
--rw-r--r--   0 snooz      (501) staff       (20)    12567 2023-04-03 06:49:02.000000 robotframework-debug-4.3.2/RobotDebug/cmdcompleter.py
--rw-r--r--   0 snooz      (501) staff       (20)     9931 2023-04-02 21:41:20.000000 robotframework-debug-4.3.2/RobotDebug/debugcmd.py
--rw-r--r--   0 snooz      (501) staff       (20)      396 2023-03-31 20:37:02.000000 robotframework-debug-4.3.2/RobotDebug/globals.py
--rw-r--r--   0 snooz      (501) staff       (20)     4195 2023-04-07 20:09:22.000000 robotframework-debug-4.3.2/RobotDebug/history_app.py
--rw-r--r--   0 snooz      (501) staff       (20)     9129 2023-04-07 20:09:22.000000 robotframework-debug-4.3.2/RobotDebug/lexer.py
--rw-r--r--   0 snooz      (501) staff       (20)    13309 2023-04-02 21:53:42.000000 robotframework-debug-4.3.2/RobotDebug/prompttoolkitcmd.py
--rw-r--r--   0 snooz      (501) staff       (20)     3330 2023-03-31 08:23:06.000000 robotframework-debug-4.3.2/RobotDebug/robotkeyword.py
--rw-r--r--   0 snooz      (501) staff       (20)     1892 2023-04-01 18:18:08.000000 robotframework-debug-4.3.2/RobotDebug/robotlib.py
--rw-r--r--   0 snooz      (501) staff       (20)     1286 2023-03-31 08:23:06.000000 robotframework-debug-4.3.2/RobotDebug/shell.py
--rw-r--r--   0 snooz      (501) staff       (20)     4279 2023-03-31 08:23:06.000000 robotframework-debug-4.3.2/RobotDebug/sourcelines.py
--rw-r--r--   0 snooz      (501) staff       (20)     2587 2023-03-31 08:23:06.000000 robotframework-debug-4.3.2/RobotDebug/styles.py
--rw-r--r--   0 snooz      (501) staff       (20)       18 2023-04-12 19:58:55.000000 robotframework-debug-4.3.2/RobotDebug/version.py
--rw-r--r--   0 snooz      (501) staff       (20)       26 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/_config.yml
--rw-r--r--   0 snooz      (501) staff       (20)      738 2023-03-31 08:27:09.000000 robotframework-debug-4.3.2/pyproject.toml
-drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-12 20:00:15.016021 robotframework-debug-4.3.2/robotframework_debug.egg-info/
--rw-r--r--   0 snooz      (501) staff       (20)     6027 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/PKG-INFO
--rw-r--r--   0 snooz      (501) staff       (20)      890 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/SOURCES.txt
--rw-r--r--   0 snooz      (501) staff       (20)        1 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/dependency_links.txt
--rw-r--r--   0 snooz      (501) staff       (20)       86 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/entry_points.txt
--rw-r--r--   0 snooz      (501) staff       (20)        1 2023-03-15 17:54:44.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/not-zip-safe
--rw-r--r--   0 snooz      (501) staff       (20)       77 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/requires.txt
--rw-r--r--   0 snooz      (501) staff       (20)       11 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/top_level.txt
--rw-r--r--   0 snooz      (501) staff       (20)      159 2023-04-12 20:00:15.018064 robotframework-debug-4.3.2/setup.cfg
--rwxr-xr-x   0 snooz      (501) staff       (20)     2112 2023-04-07 19:54:01.000000 robotframework-debug-4.3.2/setup.py
-drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-12 20:00:15.017444 robotframework-debug-4.3.2/tests/
--rw-r--r--   0 snooz      (501) staff       (20)        0 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/tests/__init__.py
--rw-r--r--   0 snooz      (501) staff       (20)     1426 2023-04-02 18:53:31.000000 robotframework-debug-4.3.2/tests/demo.py
--rw-r--r--   0 snooz      (501) staff       (20)      609 2023-03-31 08:22:53.000000 robotframework-debug-4.3.2/tests/step.robot
--rw-r--r--   0 snooz      (501) staff       (20)      844 2023-03-31 20:34:46.000000 robotframework-debug-4.3.2/tests/step_listener.robot
--rw-r--r--   0 snooz      (501) staff       (20)     6067 2023-04-01 10:10:07.000000 robotframework-debug-4.3.2/tests/test_debuglibrary.py
--rw-r--r--   0 snooz      (501) staff       (20)     4624 2023-04-01 10:10:07.000000 robotframework-debug-4.3.2/tests/test_lib.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-05 16:32:41.693233 robotframework-debug-4.3.3/
+-rw-r--r--   0 rener      (502) wheel        (0)      545 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/.coveragerc
+-rw-r--r--   0 rener      (502) wheel        (0)      272 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/.gitpod.yml
+-rw-r--r--   0 rener      (502) wheel        (0)     5811 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/ChangeLog
+-rw-r--r--   0 rener      (502) wheel        (0)      139 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/CreateWheel.sh
+-rw-r--r--   0 rener      (502) wheel        (0)     1471 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/LICENSE
+-rw-r--r--   0 rener      (502) wheel        (0)      215 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/MANIFEST.in
+-rw-r--r--   0 rener      (502) wheel        (0)     6027 2023-05-05 16:32:41.693328 robotframework-debug-4.3.3/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)     5047 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/README.rst
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-05 16:32:41.691743 robotframework-debug-4.3.3/RobotDebug/
+-rw-r--r--   0 rener      (502) wheel        (0)     5878 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/RobotDebug.py
+-rw-r--r--   0 rener      (502) wheel        (0)      154 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)    12567 2023-05-05 16:27:48.000000 robotframework-debug-4.3.3/RobotDebug/cmdcompleter.py
+-rw-r--r--   0 rener      (502) wheel        (0)     9931 2023-05-05 16:26:16.000000 robotframework-debug-4.3.3/RobotDebug/debugcmd.py
+-rw-r--r--   0 rener      (502) wheel        (0)      396 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/globals.py
+-rw-r--r--   0 rener      (502) wheel        (0)     4195 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/history_app.py
+-rw-r--r--   0 rener      (502) wheel        (0)     9135 2023-05-05 16:27:39.000000 robotframework-debug-4.3.3/RobotDebug/lexer.py
+-rw-r--r--   0 rener      (502) wheel        (0)    13309 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/prompttoolkitcmd.py
+-rw-r--r--   0 rener      (502) wheel        (0)     3330 2023-05-05 16:18:45.000000 robotframework-debug-4.3.3/RobotDebug/robotkeyword.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1892 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/robotlib.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1286 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/shell.py
+-rw-r--r--   0 rener      (502) wheel        (0)     4279 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/sourcelines.py
+-rw-r--r--   0 rener      (502) wheel        (0)     2587 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/RobotDebug/styles.py
+-rw-r--r--   0 rener      (502) wheel        (0)       18 2023-05-05 16:29:42.000000 robotframework-debug-4.3.3/RobotDebug/version.py
+-rw-r--r--   0 rener      (502) wheel        (0)       26 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/_config.yml
+-rw-r--r--   0 rener      (502) wheel        (0)      738 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/pyproject.toml
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-05 16:32:41.692729 robotframework-debug-4.3.3/robotframework_debug.egg-info/
+-rw-r--r--   0 rener      (502) wheel        (0)     6027 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)      832 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       86 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/entry_points.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2022-09-28 17:59:17.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/not-zip-safe
+-rw-r--r--   0 rener      (502) wheel        (0)       77 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/requires.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       11 2023-05-05 16:32:41.000000 robotframework-debug-4.3.3/robotframework_debug.egg-info/top_level.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      159 2023-05-05 16:32:41.693613 robotframework-debug-4.3.3/setup.cfg
+-rwxr-xr-x   0 rener      (502) wheel        (0)     2112 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/setup.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-05 16:32:41.693112 robotframework-debug-4.3.3/tests/
+-rw-r--r--   0 rener      (502) wheel        (0)        0 2022-09-28 17:53:40.000000 robotframework-debug-4.3.3/tests/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)      609 2023-05-05 15:42:55.000000 robotframework-debug-4.3.3/tests/step.robot
+-rw-r--r--   0 rener      (502) wheel        (0)     6067 2022-09-28 18:50:01.000000 robotframework-debug-4.3.3/tests/test_debuglibrary.py
```

### Comparing `robotframework-debug-4.3.2/.coveragerc` & `robotframework-debug-4.3.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/ChangeLog` & `robotframework-debug-4.3.3/ChangeLog`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/LICENSE` & `robotframework-debug-4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/PKG-INFO` & `robotframework-debug-4.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-debug
-Version: 4.3.2
+Version: 4.3.3
 Summary: RobotFramework debug shell
 Home-page: https://github.com/imbus/robotframework-debug/
 Author: René Rohner
 Author-email: snooz@postoe.de
 License: New BSD
 Keywords: robotframework,debug,shell,repl
 Platform: Linux
```

### Comparing `robotframework-debug-4.3.2/README.rst` & `robotframework-debug-4.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/RobotDebug.py` & `robotframework-debug-4.3.3/RobotDebug/RobotDebug.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/cmdcompleter.py` & `robotframework-debug-4.3.3/RobotDebug/cmdcompleter.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/debugcmd.py` & `robotframework-debug-4.3.3/RobotDebug/debugcmd.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/history_app.py` & `robotframework-debug-4.3.3/RobotDebug/history_app.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/lexer.py` & `robotframework-debug-4.3.3/RobotDebug/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 def get_variable_token(token_list):
     for token in token_list:
         if len(token.value) == 0:
             continue
         try:
-            var_tokens = token.tokenize_variables()
+            var_tokens = list(token.tokenize_variables())
         except Exception:
             var_tokens = [token]
         for v_token in var_tokens:
             yield v_token
 
 
 class RobotFrameworkLocalLexer(Lexer):
```

### Comparing `robotframework-debug-4.3.2/RobotDebug/prompttoolkitcmd.py` & `robotframework-debug-4.3.3/RobotDebug/prompttoolkitcmd.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/robotkeyword.py` & `robotframework-debug-4.3.3/RobotDebug/robotkeyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/robotlib.py` & `robotframework-debug-4.3.3/RobotDebug/robotlib.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/shell.py` & `robotframework-debug-4.3.3/RobotDebug/shell.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/sourcelines.py` & `robotframework-debug-4.3.3/RobotDebug/sourcelines.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/RobotDebug/styles.py` & `robotframework-debug-4.3.3/RobotDebug/styles.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/pyproject.toml` & `robotframework-debug-4.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/robotframework_debug.egg-info/PKG-INFO` & `robotframework-debug-4.3.3/robotframework_debug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-debug
-Version: 4.3.2
+Version: 4.3.3
 Summary: RobotFramework debug shell
 Home-page: https://github.com/imbus/robotframework-debug/
 Author: René Rohner
 Author-email: snooz@postoe.de
 License: New BSD
 Keywords: robotframework,debug,shell,repl
 Platform: Linux
```

### Comparing `robotframework-debug-4.3.2/robotframework_debug.egg-info/SOURCES.txt` & `robotframework-debug-4.3.3/robotframework_debug.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,12 +27,9 @@
 robotframework_debug.egg-info/SOURCES.txt
 robotframework_debug.egg-info/dependency_links.txt
 robotframework_debug.egg-info/entry_points.txt
 robotframework_debug.egg-info/not-zip-safe
 robotframework_debug.egg-info/requires.txt
 robotframework_debug.egg-info/top_level.txt
 tests/__init__.py
-tests/demo.py
 tests/step.robot
-tests/step_listener.robot
-tests/test_debuglibrary.py
-tests/test_lib.py
+tests/test_debuglibrary.py
```

### Comparing `robotframework-debug-4.3.2/setup.py` & `robotframework-debug-4.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/tests/step.robot` & `robotframework-debug-4.3.3/tests/step.robot`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.2/tests/test_debuglibrary.py` & `robotframework-debug-4.3.3/tests/test_debuglibrary.py`

 * *Files identical despite different names*

