# Comparing `tmp/jaaql-monitor-1.2.27.tar.gz` & `tmp/jaaql-monitor-1.2.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.27.tar", last modified: Fri May  5 11:03:03 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.28.tar", last modified: Fri May  5 11:05:33 2023, max compression
```

## Comparing `jaaql-monitor-1.2.27.tar` & `jaaql-monitor-1.2.28.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:03:03.472135 jaaql-monitor-1.2.27/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.27/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-05 11:03:03.472135 jaaql-monitor-1.2.27/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.27/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 11:03:03.468162 jaaql-monitor-1.2.27/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-05 11:03:03.000000 jaaql-monitor-1.2.27/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-05 11:03:03.000000 jaaql-monitor-1.2.27/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:03:03.000000 jaaql-monitor-1.2.27/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-05 11:03:03.000000 jaaql-monitor-1.2.27/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 11:03:03.000000 jaaql-monitor-1.2.27/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 11:03:03.471135 jaaql-monitor-1.2.27/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.27/monitor/__init__.py
--rw-rw-rw-   0        0        0    23819 2023-05-05 11:01:24.000000 jaaql-monitor-1.2.27/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-05 11:02:53.000000 jaaql-monitor-1.2.27/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-05 11:03:03.472135 jaaql-monitor-1.2.27/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:05:33.342371 jaaql-monitor-1.2.28/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.28/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-05 11:05:33.341384 jaaql-monitor-1.2.28/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.28/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 11:05:33.337369 jaaql-monitor-1.2.28/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-05 11:05:33.000000 jaaql-monitor-1.2.28/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-05 11:05:33.000000 jaaql-monitor-1.2.28/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:05:33.000000 jaaql-monitor-1.2.28/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-05 11:05:33.000000 jaaql-monitor-1.2.28/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 11:05:33.000000 jaaql-monitor-1.2.28/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 11:05:33.340381 jaaql-monitor-1.2.28/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.28/monitor/__init__.py
+-rw-rw-rw-   0        0        0    23821 2023-05-05 11:05:16.000000 jaaql-monitor-1.2.28/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-05 11:05:24.000000 jaaql-monitor-1.2.28/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 11:05:33.342371 jaaql-monitor-1.2.28/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.28/setup.py
```

### Comparing `jaaql-monitor-1.2.27/LICENSE.txt` & `jaaql-monitor-1.2.28/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.27/PKG-INFO` & `jaaql-monitor-1.2.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.27
+Version: 1.2.28
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.27/README.md` & `jaaql-monitor-1.2.28/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.27/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.28/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.27
+Version: 1.2.28
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.27/monitor/main.py` & `jaaql-monitor-1.2.28/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
             else:
                 print_error(state, "Unrecognised command '" + fetched_line + "'")
         else:
             if len(state.fetched_query.strip()) != 0 or len(fetched_line.strip()) != 0:
                 state.fetched_query += fetched_line  # Do not pre-append things with empty lines
 
             if fetched_line.strip().endswith(COMMAND__go):
-                state.fetched_query = state.fetched_query[:-len(COMMAND__go) + 1]
+                state.fetched_query = state.fetched_query[:-(len(COMMAND__go) + 1)]
                 on_go(state)
 
     if len(state.fetched_query) != 0:
         if state.single_query:
             on_go(state)
         else:
             print_error(state, "Attempting to quit with non-empty buffer. Please submit with \\g or clear with \\r")
```

### Comparing `jaaql-monitor-1.2.27/setup.py` & `jaaql-monitor-1.2.28/setup.py`

 * *Files identical despite different names*

