# Comparing `tmp/jaaql-monitor-1.2.29.tar.gz` & `tmp/jaaql-monitor-1.2.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.29.tar", last modified: Fri May  5 11:09:57 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.30.tar", last modified: Fri May  5 11:32:31 2023, max compression
```

## Comparing `jaaql-monitor-1.2.29.tar` & `jaaql-monitor-1.2.30.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:09:57.384931 jaaql-monitor-1.2.29/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.29/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-05 11:09:57.383925 jaaql-monitor-1.2.29/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.29/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 11:09:57.379925 jaaql-monitor-1.2.29/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-05 11:09:57.000000 jaaql-monitor-1.2.29/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-05 11:09:57.000000 jaaql-monitor-1.2.29/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:09:57.000000 jaaql-monitor-1.2.29/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-05 11:09:57.000000 jaaql-monitor-1.2.29/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 11:09:57.000000 jaaql-monitor-1.2.29/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 11:09:57.382924 jaaql-monitor-1.2.29/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.29/monitor/__init__.py
--rw-rw-rw-   0        0        0    23833 2023-05-05 11:09:22.000000 jaaql-monitor-1.2.29/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-05 11:09:48.000000 jaaql-monitor-1.2.29/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-05 11:09:57.384931 jaaql-monitor-1.2.29/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.29/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:32:31.816358 jaaql-monitor-1.2.30/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.30/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-05 11:32:31.815358 jaaql-monitor-1.2.30/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.30/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 11:32:31.812362 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 11:32:31.815358 jaaql-monitor-1.2.30/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.30/monitor/__init__.py
+-rw-rw-rw-   0        0        0    23822 2023-05-05 11:32:21.000000 jaaql-monitor-1.2.30/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-05 11:32:22.000000 jaaql-monitor-1.2.30/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 11:32:31.816358 jaaql-monitor-1.2.30/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.30/setup.py
```

### Comparing `jaaql-monitor-1.2.29/LICENSE.txt` & `jaaql-monitor-1.2.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.29/PKG-INFO` & `jaaql-monitor-1.2.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.29
+Version: 1.2.30
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.29/README.md` & `jaaql-monitor-1.2.30/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.29/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.30/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.29
+Version: 1.2.30
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.29/monitor/main.py` & `jaaql-monitor-1.2.30/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,14 +390,16 @@
     if state.database_override is not None:
         send_json["database"] = state.database_override
     if not state.is_transactional:
         send_json["autocommit"] = True
 
     state.request_handler(METHOD__post, ENDPOINT__submit, send_json=send_json)
 
+    state.fetched_query = ""
+
 
 def parse_user_printing_any_errors(state, potential_user, allow_spaces: bool = False):
     if " " in potential_user and not allow_spaces:
         print_error(state, "Expected user without spaces, instead found spaces in user: '" + potential_user + "'")
     if not potential_user.startswith("@"):
         print_error(state, "Malformatted user, expected user to start with @")
 
@@ -437,15 +439,14 @@
         except EOFError:
             break
 
         if fetched_line.startswith(COMMAND__initialiser):
             fetched_line = fetched_line.strip()  # Ignore the line terminator e.g. \r\n
             if fetched_line == COMMAND__go or fetched_line == COMMAND__go_short:
                 on_go(state)
-                state.fetched_query = ""
             elif fetched_line == COMMAND__reset or fetched_line == COMMAND__reset_short:
                 state.fetched_query = ""
             elif fetched_line == COMMAND__print or fetched_line == COMMAND__print_short:
                 dump_buffer(state)
             elif len(state.fetched_query.strip()) != 0:
                 print_error(state, "Tried to execute the command '" + fetched_line + "' but buffer was non empty.")
             elif fetched_line == COMMAND__wipe_dbms:
```

### Comparing `jaaql-monitor-1.2.29/setup.py` & `jaaql-monitor-1.2.30/setup.py`

 * *Files identical despite different names*

