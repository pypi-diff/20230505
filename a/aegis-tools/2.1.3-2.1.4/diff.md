# Comparing `tmp/aegis-tools-2.1.3.tar.gz` & `tmp/aegis-tools-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.1.3.tar", last modified: Mon Apr 24 22:50:27 2023, max compression
+gzip compressed data, was "aegis-tools-2.1.4.tar", last modified: Fri May  5 18:35:21 2023, max compression
```

## Comparing `aegis-tools-2.1.3.tar` & `aegis-tools-2.1.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.198832 aegis-tools-2.1.3/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.3/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18100 2022-11-21 04:55:50.000000 aegis-tools-2.1.3/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.3/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.3/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-04-04 22:56:26.000000 aegis-tools-2.1.3/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7276 2023-04-24 22:47:56.000000 aegis-tools-2.1.3/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42189 2023-04-17 16:11:36.000000 aegis-tools-2.1.3/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.206832 aegis-tools-2.1.3/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.3/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.3/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.3/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.3/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-03-13 22:09:08.000000 aegis-tools-2.1.3/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-24 21:25:57.000000 aegis-tools-2.1.3/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.3/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.3/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.3/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.3/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-03-26 04:29:07.000000 aegis-tools-2.1.3/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.3/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.3/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.3/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.3/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.3/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.3/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.3/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.3/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73127 2023-04-24 22:16:45.000000 aegis-tools-2.1.3/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-04-24 22:50:08.000000 aegis-tools-2.1.3/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.949747 aegis-tools-2.1.4/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-05 18:35:21.945747 aegis-tools-2.1.4/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.925747 aegis-tools-2.1.4/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.4/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18100 2022-11-21 04:55:50.000000 aegis-tools-2.1.4/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.4/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.4/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-04-04 22:56:26.000000 aegis-tools-2.1.4/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7276 2023-04-24 22:47:56.000000 aegis-tools-2.1.4/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42564 2023-05-05 18:15:10.000000 aegis-tools-2.1.4/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.937747 aegis-tools-2.1.4/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.4/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.4/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.4/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.4/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-03-13 22:09:08.000000 aegis-tools-2.1.4/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-24 21:25:57.000000 aegis-tools-2.1.4/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.945747 aegis-tools-2.1.4/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.4/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.4/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.4/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.4/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-04-27 02:34:36.000000 aegis-tools-2.1.4/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.4/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.4/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.4/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.4/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.4/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.4/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.4/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.4/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.4/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73309 2023-05-05 18:28:25.000000 aegis-tools-2.1.4/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-05 18:35:21.945747 aegis-tools-2.1.4/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-05-05 18:35:21.000000 aegis-tools-2.1.4/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-05-05 18:35:21.949747 aegis-tools-2.1.4/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-05-05 18:33:29.000000 aegis-tools-2.1.4/setup.py
```

### Comparing `aegis-tools-2.1.3/LICENSE` & `aegis-tools-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/PKG-INFO` & `aegis-tools-2.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.3
+Version: 2.1.4
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.3/README.md` & `aegis-tools-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/aegis_.py` & `aegis-tools-2.1.4/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/build.py` & `aegis-tools-2.1.4/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/config.py` & `aegis-tools-2.1.4/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/database.py` & `aegis-tools-2.1.4/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/hydra.py` & `aegis-tools-2.1.4/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/mailer.py` & `aegis-tools-2.1.4/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/model.py` & `aegis-tools-2.1.4/aegis/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,14 +349,19 @@
         sql = "DELETE FROM google_access WHERE expire_dttm < NOW()"
         return dbconn.execute(sql)
 
     def hard_delete(self):
         sql = "DELETE FROM google_access WHERE google_access_id=%s"
         return db().execute(sql, self['google_access_id'])
 
+    @classmethod
+    def hard_delete_google_user(cls, google_user_id):
+        sql = "DELETE FROM google_access WHERE google_user_id=%s"
+        return db().execute(sql, google_user_id)
+
 
 class GooglePicture(aegis.database.Row):
     table_name = 'google_picture'
     id_column = 'google_picture_id'
     primary_key = ('google_picture_id')
 
     @classmethod
@@ -366,14 +371,19 @@
         sql = "SELECT * FROM google_picture WHERE google_user_id=%s"
         return dbconn.get(sql, google_user_id, cls=cls)
 
     def hard_delete(self):
         sql = "DELETE FROM google_picture WHERE google_picture_id=%s"
         return db().execute(sql, self['google_picture_id'])
 
+    @classmethod
+    def hard_delete_google_user(cls, google_user_id):
+        sql = "DELETE FROM google_picture WHERE google_user_id=%s"
+        return db().execute(sql, google_user_id)
+
 
 class EmailType(aegis.database.Row):
     table_name = 'email_type'
     id_column = 'email_type_id'
 
     @classmethod
     def scan(cls):
```

### Comparing `aegis-tools-2.1.3/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.1.4/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.1.4/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/build-mysql.sql` & `aegis-tools-2.1.4/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/build-pgsql.sql` & `aegis-tools-2.1.4/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.1.4/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/google_signin.sql` & `aegis-tools-2.1.4/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.1.4/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.1.4/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/member_auth.sql` & `aegis-tools-2.1.4/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.1.4/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/sql/reports.sql` & `aegis-tools-2.1.4/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/stdlib.py` & `aegis-tools-2.1.4/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/build.html` & `aegis-tools-2.1.4/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/build_confirm.html` & `aegis-tools-2.1.4/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/build_form.html` & `aegis-tools-2.1.4/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/build_view.html` & `aegis-tools-2.1.4/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/frame.html` & `aegis-tools-2.1.4/aegis/templates/frame.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!DOCTYPE html>
 <html lang="en">
     <head>
-        {% block title %}<title>{{page_title}} {% if options.env != 'prod' %}({{ options.env }}){% end %}</title>{% end %}
+        {% block title %}<title>{{page_title}} {% if options.env != 'prod' %}[{{ options.env }}]{% end %}</title>{% end %}
         <meta charset="UTF-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
         <style nonce="aegis-webapp-frame-rstlne">
           {% include w3.css %}
           h3 { margin: 5px 0; }
           form p {margin: 10px 0; }
           #menu-bar span { margin: 0 .5em;}}
```

### Comparing `aegis-tools-2.1.3/aegis/templates/hydra.html` & `aegis-tools-2.1.4/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/hydra_form.html` & `aegis-tools-2.1.4/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/hydra_queue.html` & `aegis-tools-2.1.4/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/report.html` & `aegis-tools-2.1.4/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/report_form.html` & `aegis-tools-2.1.4/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/reports.html` & `aegis-tools-2.1.4/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/templates/w3.css` & `aegis-tools-2.1.4/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/threadpool.py` & `aegis-tools-2.1.4/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/aegis/webapp.py` & `aegis-tools-2.1.4/aegis/webapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -747,15 +747,15 @@
             logging.warning("Pyreferrer type is search -> organic")
             return self.finish_marketing('organic')
         if pr and pr['type'] == 'social':
             logging.warning("Pyreferrer type is social -> social")
             return self.finish_marketing('social')
         aegis.stdlib.logw(pr, "Pyreferrer")
         # Custom organic "netlocs" not (yet) in pyreferrer
-        organic_netlocs = ['aol.com', 'baidu.com', 'www.daum.net', 'daum.net', 'search.brave.com', 'www.ecosia.org', 'www.msn.com',
+        organic_netlocs = ['aol.com', 'baidu.com', 'www.daum.net', 'daum.net', 'presearch.com', 'search.brave.com', 'www.ecosia.org', 'www.msn.com',
                            'com.google.android.googlequicksearchbox']   # android-app://com.google.android.googlequicksearchbox
         for organic_netloc in organic_netlocs:
             if url_parts and url_parts.netloc.endswith(organic_netloc):
                 logging.warning("Netloc endswith organic domain -> organic")
                 return self.finish_marketing('organic')
         # Mark it as an unknown referral
         logging.warning("Url unknown: %s" % referer)
@@ -1074,15 +1074,19 @@
         return self.redirect('/admin/hydra')
 
 
 class AegisHydra(AegisWeb):
     @tornado.web.authenticated
     def get(self, *args):
         self.enforce_admin()
-        self.tmpl['page_title'] = 'Hydra %s' % options.header_logo
+        if options.header_logo.endswith('svg'):
+            logging.warning("DO SVG")
+            self.tmpl['page_title'] = 'Hydra %s' % options.domain
+        else:
+            self.tmpl['page_title'] = 'Hydra %s' % options.domain
         self.tmpl['hydra_types'] = aegis.model.HydraType.scan()
         self.tmpl['home_link'] = '/'
         self.tmpl['aegis_version'] = pkg_resources.require("aegis-tools")[0].version
         try:
             self.tmpl['app_version'] = pkg_resources.require(aegis.config.get('program_name'))[0].version
         except pkg_resources.ContextualVersionConflict as ex:
             logging.exception(ex)
```

### Comparing `aegis-tools-2.1.3/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.1.4/aegis_tools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.3
+Version: 2.1.4
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.3/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.1.4/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.3/setup.py` & `aegis-tools-2.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import os
 import setuptools
 
 setuptools.setup (
     name = 'aegis-tools',
-    version = '2.1.3',
+    version = '2.1.4',
     description = 'Aegis is a set of battle-tested tools and tricks to help everyone make better software',
     long_description = 'A combination of tools and framework, Aegis has multiple different uses. You can import it and use the thoroughly made and tested functions. You can use it as a natural extension for the tornado web framework. And you can use it to quickly create a new web application with the structure already built-in, and follow along.',
     author = "Michael D'Agosta",
     author_email = 'mdagosta@codebug.com',
     url = 'https://github.com/mdagosta/aegis',
     python_requires='>=3.6',
     packages = ['aegis'],
```

