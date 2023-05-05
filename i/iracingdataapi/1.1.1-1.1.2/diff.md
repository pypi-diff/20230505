# Comparing `tmp/iracingdataapi-1.1.1.tar.gz` & `tmp/iracingdataapi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iracingdataapi-1.1.1.tar", last modified: Fri May  5 19:23:26 2023, max compression
+gzip compressed data, was "iracingdataapi-1.1.2.tar", last modified: Fri May  5 19:27:53 2023, max compression
```

## Comparing `iracingdataapi-1.1.1.tar` & `iracingdataapi-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:23:26.063277 iracingdataapi-1.1.1/
--rw-r--r--   0 jasondilworth   (501) staff       (20)     1073 2022-03-24 20:31:50.000000 iracingdataapi-1.1.1/LICENSE
--rw-r--r--   0 jasondilworth   (501) staff       (20)       17 2022-03-24 21:34:57.000000 iracingdataapi-1.1.1/MANIFEST.in
--rw-r--r--   0 jasondilworth   (501) staff       (20)     3403 2023-05-05 19:23:26.063111 iracingdataapi-1.1.1/PKG-INFO
--rw-r--r--   0 jasondilworth   (501) staff       (20)     2844 2023-05-05 19:20:23.000000 iracingdataapi-1.1.1/README.md
--rw-r--r--   0 jasondilworth   (501) staff       (20)       38 2023-05-05 19:23:26.063313 iracingdataapi-1.1.1/setup.cfg
--rw-r--r--   0 jasondilworth   (501) staff       (20)      893 2023-05-05 19:20:34.000000 iracingdataapi-1.1.1/setup.py
-drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:23:26.059609 iracingdataapi-1.1.1/src/
-drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:23:26.061550 iracingdataapi-1.1.1/src/iracingdataapi/
--rw-r--r--   0 jasondilworth   (501) staff       (20)        0 2022-03-24 20:28:11.000000 iracingdataapi-1.1.1/src/iracingdataapi/__init__.py
--rw-r--r--   0 jasondilworth   (501) staff       (20)    45626 2023-05-05 19:16:47.000000 iracingdataapi-1.1.1/src/iracingdataapi/client.py
-drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:23:26.062868 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/
--rw-r--r--   0 jasondilworth   (501) staff       (20)     3403 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/PKG-INFO
--rw-r--r--   0 jasondilworth   (501) staff       (20)      307 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/SOURCES.txt
--rw-r--r--   0 jasondilworth   (501) staff       (20)        1 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/dependency_links.txt
--rw-r--r--   0 jasondilworth   (501) staff       (20)        9 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/requires.txt
--rw-r--r--   0 jasondilworth   (501) staff       (20)       15 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/top_level.txt
+drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:27:53.709516 iracingdataapi-1.1.2/
+-rw-r--r--   0 jasondilworth   (501) staff       (20)     1073 2022-03-24 20:31:50.000000 iracingdataapi-1.1.2/LICENSE
+-rw-r--r--   0 jasondilworth   (501) staff       (20)       17 2022-03-24 21:34:57.000000 iracingdataapi-1.1.2/MANIFEST.in
+-rw-r--r--   0 jasondilworth   (501) staff       (20)     3403 2023-05-05 19:27:53.709381 iracingdataapi-1.1.2/PKG-INFO
+-rw-r--r--   0 jasondilworth   (501) staff       (20)     2844 2023-05-05 19:27:30.000000 iracingdataapi-1.1.2/README.md
+-rw-r--r--   0 jasondilworth   (501) staff       (20)       38 2023-05-05 19:27:53.709551 iracingdataapi-1.1.2/setup.cfg
+-rw-r--r--   0 jasondilworth   (501) staff       (20)      893 2023-05-05 19:27:27.000000 iracingdataapi-1.1.2/setup.py
+drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:27:53.706830 iracingdataapi-1.1.2/src/
+drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:27:53.707900 iracingdataapi-1.1.2/src/iracingdataapi/
+-rw-r--r--   0 jasondilworth   (501) staff       (20)        0 2022-03-24 20:28:11.000000 iracingdataapi-1.1.2/src/iracingdataapi/__init__.py
+-rw-r--r--   0 jasondilworth   (501) staff       (20)    45644 2023-05-05 19:26:56.000000 iracingdataapi-1.1.2/src/iracingdataapi/client.py
+drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:27:53.709181 iracingdataapi-1.1.2/src/iracingdataapi.egg-info/
+-rw-r--r--   0 jasondilworth   (501) staff       (20)     3403 2023-05-05 19:27:53.000000 iracingdataapi-1.1.2/src/iracingdataapi.egg-info/PKG-INFO
+-rw-r--r--   0 jasondilworth   (501) staff       (20)      307 2023-05-05 19:27:53.000000 iracingdataapi-1.1.2/src/iracingdataapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jasondilworth   (501) staff       (20)        1 2023-05-05 19:27:53.000000 iracingdataapi-1.1.2/src/iracingdataapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jasondilworth   (501) staff       (20)        9 2023-05-05 19:27:53.000000 iracingdataapi-1.1.2/src/iracingdataapi.egg-info/requires.txt
+-rw-r--r--   0 jasondilworth   (501) staff       (20)       15 2023-05-05 19:27:53.000000 iracingdataapi-1.1.2/src/iracingdataapi.egg-info/top_level.txt
```

### Comparing `iracingdataapi-1.1.1/LICENSE` & `iracingdataapi-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iracingdataapi-1.1.1/PKG-INFO` & `iracingdataapi-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iracingdataapi
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple wrapper around the iRacing General Data API
 Home-page: https://github.com/jasondilworth56/iracingdataapi
 Author: Jason Dilworth
 Author-email: hello@jasondilworth.co.uk
 Project-URL: Bug Tracker, https://github.com/jasondilworth56/iracingdataapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -44,15 +44,15 @@
 
 # Contributing
 
 I welcome all pull requests for improvements or missing endpoints over time as they are added by iRacing.
 
 # Changelog
 
-**1.1.1**
+**1.1.2**
 -   Bug fix for some 5xx errors that are thrown by iRacing
 -   Added the `season_spectator_subsessionids()` endpoint
 
 **1.1.0**
 -   Added docstrings to all methods for developer experience
 -   Renamed `series()` to `get_series()` for consistency. **Breaking change:** For that same consistency, `series` has been reimplemented as a property which returns the series with their assets. To amend your implementation, either switch to `get_series()` or remove any brackets in your call of `series`.
 -   Renamed `get_carclass()` to `get_carclasses()` to be more consistent with other endpoints. **NOTE:** `get_carclass()` will be removed in a future release.
```

### Comparing `iracingdataapi-1.1.1/README.md` & `iracingdataapi-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # Contributing
 
 I welcome all pull requests for improvements or missing endpoints over time as they are added by iRacing.
 
 # Changelog
 
-**1.1.1**
+**1.1.2**
 -   Bug fix for some 5xx errors that are thrown by iRacing
 -   Added the `season_spectator_subsessionids()` endpoint
 
 **1.1.0**
 -   Added docstrings to all methods for developer experience
 -   Renamed `series()` to `get_series()` for consistency. **Breaking change:** For that same consistency, `series` has been reimplemented as a property which returns the series with their assets. To amend your implementation, either switch to `get_series()` or remove any brackets in your call of `series`.
 -   Renamed `get_carclass()` to `get_carclasses()` to be more consistent with other endpoints. **NOTE:** `get_carclass()` will be removed in a future release.
```

### Comparing `iracingdataapi-1.1.1/setup.py` & `iracingdataapi-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iracingdataapi",
-    version="1.1.1",
+    version="1.1.2",
     author="Jason Dilworth",
     author_email="hello@jasondilworth.co.uk",
     description="A simple wrapper around the iRacing General Data API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jasondilworth56/iracingdataapi",
     project_urls={
```

### Comparing `iracingdataapi-1.1.1/src/iracingdataapi/client.py` & `iracingdataapi-1.1.2/src/iracingdataapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1144,15 +1144,15 @@
                 5: Race
 
         Returns:
             list: a list of the matching subsession IDs
         """
         payload = {}
         if event_types:
-            payload["event_types": ",".join(event_types)]
+            payload["event_types": ",".join([str(x) for x in event_types])]
         
         return self._get_resource("/data/season/spectator_subsessionids", payload=payload)
 
     def get_series(self):
         """Get all the current official iRacing series.
 
         Returns:
```

### Comparing `iracingdataapi-1.1.1/src/iracingdataapi.egg-info/PKG-INFO` & `iracingdataapi-1.1.2/src/iracingdataapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iracingdataapi
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple wrapper around the iRacing General Data API
 Home-page: https://github.com/jasondilworth56/iracingdataapi
 Author: Jason Dilworth
 Author-email: hello@jasondilworth.co.uk
 Project-URL: Bug Tracker, https://github.com/jasondilworth56/iracingdataapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -44,15 +44,15 @@
 
 # Contributing
 
 I welcome all pull requests for improvements or missing endpoints over time as they are added by iRacing.
 
 # Changelog
 
-**1.1.1**
+**1.1.2**
 -   Bug fix for some 5xx errors that are thrown by iRacing
 -   Added the `season_spectator_subsessionids()` endpoint
 
 **1.1.0**
 -   Added docstrings to all methods for developer experience
 -   Renamed `series()` to `get_series()` for consistency. **Breaking change:** For that same consistency, `series` has been reimplemented as a property which returns the series with their assets. To amend your implementation, either switch to `get_series()` or remove any brackets in your call of `series`.
 -   Renamed `get_carclass()` to `get_carclasses()` to be more consistent with other endpoints. **NOTE:** `get_carclass()` will be removed in a future release.
```

