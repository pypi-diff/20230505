# Comparing `tmp/openmodule_commands-11.0.2.tar.gz` & `tmp/openmodule_commands-11.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-11.0.2.tar", last modified: Thu Mar 16 09:24:41 2023, max compression
+gzip compressed data, was "openmodule_commands-11.0.3.tar", last modified: Fri May  5 16:34:09 2023, max compression
```

## Comparing `openmodule_commands-11.0.2.tar` & `openmodule_commands-11.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 09:24:41.778632 openmodule_commands-11.0.2/
--rw-r--r--   0 root         (0) root         (0)      266 2023-03-16 09:24:41.000000 openmodule_commands-11.0.2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     6574 2023-03-16 09:24:41.000000 openmodule_commands-11.0.2/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      618 2023-03-16 09:24:41.778632 openmodule_commands-11.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-03-16 09:24:25.000000 openmodule_commands-11.0.2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 09:24:41.778632 openmodule_commands-11.0.2/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2023-03-16 09:24:41.000000 openmodule_commands-11.0.2/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-03-16 09:24:41.000000 openmodule_commands-11.0.2/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 09:24:41.000000 openmodule_commands-11.0.2/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-03-16 09:24:41.000000 openmodule_commands-11.0.2/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 09:24:41.000000 openmodule_commands-11.0.2/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-03-16 09:24:41.000000 openmodule_commands-11.0.2/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-16 09:24:41.000000 openmodule_commands-11.0.2/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-03-16 09:24:41.778632 openmodule_commands-11.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-03-16 09:24:25.000000 openmodule_commands-11.0.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-03-16 09:24:25.000000 openmodule_commands-11.0.2/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:34:09.916428 openmodule_commands-11.0.3/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     6535 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      618 2023-05-05 16:34:09.916428 openmodule_commands-11.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-05-05 16:33:53.000000 openmodule_commands-11.0.3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:34:09.916428 openmodule_commands-11.0.3/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-05 16:34:09.000000 openmodule_commands-11.0.3/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-05-05 16:34:09.916428 openmodule_commands-11.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-05-05 16:33:53.000000 openmodule_commands-11.0.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-05-05 16:33:53.000000 openmodule_commands-11.0.3/translate.py
```

### Comparing `openmodule_commands-11.0.2/ChangeLog` & `openmodule_commands-11.0.3/ChangeLog`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+v11.0.3
+-------
+
+* Fixed typo, added compute\_id as label to all metrics, convert all label values to string
+* touch to get rid of skip ci on my commit
+* docs update [skip ci]
+* main test function deprecated and documentation for main tests added
+
 v11.0.2
 -------
 
 * fixed get\_no\_exception in SettingsMocker
 * Update database.md [skip ci]
 * Update database.md [skip ci]
 * Update database.md [skip ci]
@@ -159,13 +167,7 @@
 * fixes a unicode issue
 
 v6.1.2
 ------
 
 * count message uses lazy settings resource, import cleanup
 * fixes a timezone issue where the timezone of the local system would change results
-* removed double entry from merge
-* merge from branch feature/recurrence
-* removed print
-* settings module now module instead of path, developer errors removed from non openmodule test
-* migration notice for tox.ini change [skip ci]
-* allow externals bash added for tox v4, and if fixed
```

### Comparing `openmodule_commands-11.0.2/PKG-INFO` & `openmodule_commands-11.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 11.0.2
+Version: 11.0.3
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.0.2/__init__.py` & `openmodule_commands-11.0.3/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.0.2/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-11.0.3/openmodule_commands.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 11.0.2
+Version: 11.0.3
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.0.2/setup.cfg` & `openmodule_commands-11.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.0.2/setup.py` & `openmodule_commands-11.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.0.2/translate.py` & `openmodule_commands-11.0.3/translate.py`

 * *Files identical despite different names*

