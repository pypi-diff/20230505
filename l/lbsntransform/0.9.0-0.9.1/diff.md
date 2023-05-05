# Comparing `tmp/lbsntransform-0.9.0.tar.gz` & `tmp/lbsntransform-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbsntransform-0.9.0.tar", last modified: Wed Oct 23 12:13:27 2019, max compression
+gzip compressed data, was "dist/lbsntransform-0.9.1.tar", last modified: Wed Oct 23 12:53:44 2019, max compression
```

## Comparing `lbsntransform-0.9.0.tar` & `lbsntransform-0.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     2582 2019-06-03 09:17:09.000000 lbsntransform-0.9.0/.gitattributes
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1413 2019-08-22 12:31:22.000000 lbsntransform-0.9.0/.gitignore
--rw-rw-rw-   0 alex      (1000) alex      (1000)    35576 2019-06-03 09:17:09.000000 lbsntransform-0.9.0/LICENSE.md
--rwxrwxrwx   0 alex      (1000) alex      (1000)      126 2019-01-09 09:33:41.000000 lbsntransform-0.9.0/MANIFEST.in
--rw-rw-rw-   0 alex      (1000) alex      (1000)    13951 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/PKG-INFO
--rw-rw-rw-   0 alex      (1000) alex      (1000)    11776 2019-07-12 17:06:50.000000 lbsntransform-0.9.0/README.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1615 2019-06-05 05:17:51.000000 lbsntransform-0.9.0/cx_setup.py
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform/
--rw-rw-rw-   0 alex      (1000) alex      (1000)      550 2019-06-05 05:17:51.000000 lbsntransform-0.9.0/lbsntransform/__init__.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     5843 2019-09-17 06:32:23.000000 lbsntransform-0.9.0/lbsntransform/__main__.py
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform/classes/
--rwxrwxrwx   0 alex      (1000) alex      (1000)        0 2018-07-25 12:50:21.000000 lbsntransform-0.9.0/lbsntransform/classes/__init__.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     2508 2019-09-17 09:13:38.000000 lbsntransform-0.9.0/lbsntransform/classes/db_connection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6738 2019-10-21 12:17:34.000000 lbsntransform-0.9.0/lbsntransform/classes/field_mapping_fb.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     9349 2019-09-17 06:32:23.000000 lbsntransform-0.9.0/lbsntransform/classes/field_mapping_flickr.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    33691 2019-08-27 14:16:20.000000 lbsntransform-0.9.0/lbsntransform/classes/field_mapping_twitter.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    18059 2019-08-27 14:16:20.000000 lbsntransform-0.9.0/lbsntransform/classes/field_mapping_yfcc100m.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    28821 2019-10-21 12:17:34.000000 lbsntransform-0.9.0/lbsntransform/classes/helper_functions.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    17615 2019-09-17 09:13:38.000000 lbsntransform-0.9.0/lbsntransform/classes/load_data.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    19798 2019-09-18 12:12:03.000000 lbsntransform-0.9.0/lbsntransform/classes/shared_structure_proto_lbsndb.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    14605 2019-08-27 14:16:20.000000 lbsntransform-0.9.0/lbsntransform/classes/store_csv.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    34020 2019-10-23 12:12:16.000000 lbsntransform-0.9.0/lbsntransform/classes/submit_data.py
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform/config/
--rwxrwxrwx   0 alex      (1000) alex      (1000)        0 2018-07-25 11:34:03.000000 lbsntransform-0.9.0/lbsntransform/config/__init__.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    17038 2019-08-27 14:16:20.000000 lbsntransform-0.9.0/lbsntransform/config/config.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     6037 2019-09-17 06:32:23.000000 lbsntransform-0.9.0/lbsntransform/lbsntransform_.py
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform/tests/
--rwxrwxrwx   0 alex      (1000) alex      (1000)        2 2018-07-24 13:44:05.000000 lbsntransform-0.9.0/lbsntransform/tests/__init__.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)      910 2018-12-05 12:05:34.000000 lbsntransform-0.9.0/lbsntransform/tests/tests.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2019-10-23 12:13:19.000000 lbsntransform-0.9.0/lbsntransform/version.py
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform.egg-info/
--rwxrwxrwx   0 alex      (1000) alex      (1000)    13951 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform.egg-info/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)     1007 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform.egg-info/SOURCES.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)        1 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform.egg-info/dependency_links.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)       63 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform.egg-info/entry_points.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)       74 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform.egg-info/requires.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)       14 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/lbsntransform.egg-info/top_level.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2019-10-23 12:13:27.000000 lbsntransform-0.9.0/setup.cfg
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1272 2019-06-05 05:17:51.000000 lbsntransform-0.9.0/setup.py
+drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     2582 2019-06-03 09:17:09.000000 lbsntransform-0.9.1/.gitattributes
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1413 2019-08-22 12:31:22.000000 lbsntransform-0.9.1/.gitignore
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    35576 2019-06-03 09:17:09.000000 lbsntransform-0.9.1/LICENSE.md
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      126 2019-01-09 09:33:41.000000 lbsntransform-0.9.1/MANIFEST.in
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    13951 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/PKG-INFO
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    11776 2019-07-12 17:06:50.000000 lbsntransform-0.9.1/README.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1615 2019-06-05 05:17:51.000000 lbsntransform-0.9.1/cx_setup.py
+drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      550 2019-06-05 05:17:51.000000 lbsntransform-0.9.1/lbsntransform/__init__.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     5843 2019-09-17 06:32:23.000000 lbsntransform-0.9.1/lbsntransform/__main__.py
+drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform/classes/
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        0 2018-07-25 12:50:21.000000 lbsntransform-0.9.1/lbsntransform/classes/__init__.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     2508 2019-09-17 09:13:38.000000 lbsntransform-0.9.1/lbsntransform/classes/db_connection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6738 2019-10-21 12:17:34.000000 lbsntransform-0.9.1/lbsntransform/classes/field_mapping_fb.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     9349 2019-09-17 06:32:23.000000 lbsntransform-0.9.1/lbsntransform/classes/field_mapping_flickr.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    33691 2019-08-27 14:16:20.000000 lbsntransform-0.9.1/lbsntransform/classes/field_mapping_twitter.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    18059 2019-08-27 14:16:20.000000 lbsntransform-0.9.1/lbsntransform/classes/field_mapping_yfcc100m.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    28821 2019-10-21 12:17:34.000000 lbsntransform-0.9.1/lbsntransform/classes/helper_functions.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    17615 2019-09-17 09:13:38.000000 lbsntransform-0.9.1/lbsntransform/classes/load_data.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    19798 2019-09-18 12:12:03.000000 lbsntransform-0.9.1/lbsntransform/classes/shared_structure_proto_lbsndb.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    14605 2019-08-27 14:16:20.000000 lbsntransform-0.9.1/lbsntransform/classes/store_csv.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    34020 2019-10-23 12:12:16.000000 lbsntransform-0.9.1/lbsntransform/classes/submit_data.py
+drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform/config/
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        0 2018-07-25 11:34:03.000000 lbsntransform-0.9.1/lbsntransform/config/__init__.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    17038 2019-08-27 14:16:20.000000 lbsntransform-0.9.1/lbsntransform/config/config.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     6037 2019-09-17 06:32:23.000000 lbsntransform-0.9.1/lbsntransform/lbsntransform_.py
+drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform/tests/
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        2 2018-07-24 13:44:05.000000 lbsntransform-0.9.1/lbsntransform/tests/__init__.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      910 2018-12-05 12:05:34.000000 lbsntransform-0.9.1/lbsntransform/tests/tests.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2019-10-23 12:53:37.000000 lbsntransform-0.9.1/lbsntransform/version.py
+drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform.egg-info/
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    13951 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform.egg-info/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     1007 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        1 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       63 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform.egg-info/entry_points.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       70 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform.egg-info/requires.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       14 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/lbsntransform.egg-info/top_level.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2019-10-23 12:53:44.000000 lbsntransform-0.9.1/setup.cfg
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1268 2019-10-23 12:51:25.000000 lbsntransform-0.9.1/setup.py
```

### Comparing `lbsntransform-0.9.0/.gitattributes` & `lbsntransform-0.9.1/.gitattributes`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/.gitignore` & `lbsntransform-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/LICENSE.md` & `lbsntransform-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/PKG-INFO` & `lbsntransform-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbsntransform
-Version: 0.9.0
+Version: 0.9.1
 Summary: Location based social network (LBSN) data structure format & transfer tool
 Home-page: https://gitlab.vgiscience.de/lbsn/lbsntransform
 Author: Alexander Dunkel
 Author-email: alexander.dunkel@tu-dresden.de
 License: GNU GPLv3 or any higher
 Description: ![PyPI version](https://lbsn.vgiscience.org/lbsntransform/pypi.svg) ![pylint](https://lbsn.vgiscience.org/lbsntransform/pylint.svg) ![pipeline](https://lbsn.vgiscience.org/lbsntransform/pipeline.svg)
```

### Comparing `lbsntransform-0.9.0/README.md` & `lbsntransform-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/cx_setup.py` & `lbsntransform-0.9.1/cx_setup.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/__init__.py` & `lbsntransform-0.9.1/lbsntransform/__init__.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/__main__.py` & `lbsntransform-0.9.1/lbsntransform/__main__.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/db_connection.py` & `lbsntransform-0.9.1/lbsntransform/classes/db_connection.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/field_mapping_fb.py` & `lbsntransform-0.9.1/lbsntransform/classes/field_mapping_fb.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/field_mapping_flickr.py` & `lbsntransform-0.9.1/lbsntransform/classes/field_mapping_flickr.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/field_mapping_twitter.py` & `lbsntransform-0.9.1/lbsntransform/classes/field_mapping_twitter.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/field_mapping_yfcc100m.py` & `lbsntransform-0.9.1/lbsntransform/classes/field_mapping_yfcc100m.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/helper_functions.py` & `lbsntransform-0.9.1/lbsntransform/classes/helper_functions.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/load_data.py` & `lbsntransform-0.9.1/lbsntransform/classes/load_data.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/shared_structure_proto_lbsndb.py` & `lbsntransform-0.9.1/lbsntransform/classes/shared_structure_proto_lbsndb.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/store_csv.py` & `lbsntransform-0.9.1/lbsntransform/classes/store_csv.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/classes/submit_data.py` & `lbsntransform-0.9.1/lbsntransform/classes/submit_data.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/config/config.py` & `lbsntransform-0.9.1/lbsntransform/config/config.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/lbsntransform_.py` & `lbsntransform-0.9.1/lbsntransform/lbsntransform_.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform/tests/tests.py` & `lbsntransform-0.9.1/lbsntransform/tests/tests.py`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/lbsntransform.egg-info/PKG-INFO` & `lbsntransform-0.9.1/lbsntransform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbsntransform
-Version: 0.9.0
+Version: 0.9.1
 Summary: Location based social network (LBSN) data structure format & transfer tool
 Home-page: https://gitlab.vgiscience.de/lbsn/lbsntransform
 Author: Alexander Dunkel
 Author-email: alexander.dunkel@tu-dresden.de
 License: GNU GPLv3 or any higher
 Description: ![PyPI version](https://lbsn.vgiscience.org/lbsntransform/pypi.svg) ![pylint](https://lbsn.vgiscience.org/lbsntransform/pylint.svg) ![pipeline](https://lbsn.vgiscience.org/lbsntransform/pipeline.svg)
```

### Comparing `lbsntransform-0.9.0/lbsntransform.egg-info/SOURCES.txt` & `lbsntransform-0.9.1/lbsntransform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbsntransform-0.9.0/setup.py` & `lbsntransform-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       author='Alexander Dunkel',
       author_email='alexander.dunkel@tu-dresden.de',
       url='https://gitlab.vgiscience.de/lbsn/lbsntransform',
       license='GNU GPLv3 or any higher',
       packages=['lbsntransform'],
       include_package_data=True,
       install_requires=[
-          'lbsnstructure>=0.2.6.211',
+          'lbsnstructure>=0.5.0',
           'protobuf',
           'psycopg2',
           'ppygis3',
           'shapely',
           'emoji',
           'requests'
       ],
```

