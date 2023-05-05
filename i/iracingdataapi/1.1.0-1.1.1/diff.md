# Comparing `tmp/iracingdataapi-1.1.0.tar.gz` & `tmp/iracingdataapi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iracingdataapi-1.1.0.tar", last modified: Tue Mar 21 10:18:02 2023, max compression
+gzip compressed data, was "iracingdataapi-1.1.1.tar", last modified: Fri May  5 19:23:26 2023, max compression
```

## Comparing `iracingdataapi-1.1.0.tar` & `iracingdataapi-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-03-21 10:18:02.007675 iracingdataapi-1.1.0/
--rw-r--r--   0 jasondilworth   (501) staff       (20)     1073 2022-03-24 20:31:50.000000 iracingdataapi-1.1.0/LICENSE
--rw-r--r--   0 jasondilworth   (501) staff       (20)       17 2022-03-24 21:34:57.000000 iracingdataapi-1.1.0/MANIFEST.in
--rw-r--r--   0 jasondilworth   (501) staff       (20)     3274 2023-03-21 10:18:02.007529 iracingdataapi-1.1.0/PKG-INFO
--rw-r--r--   0 jasondilworth   (501) staff       (20)     2715 2023-03-21 10:14:30.000000 iracingdataapi-1.1.0/README.md
--rw-r--r--   0 jasondilworth   (501) staff       (20)       38 2023-03-21 10:18:02.007716 iracingdataapi-1.1.0/setup.cfg
--rw-r--r--   0 jasondilworth   (501) staff       (20)      893 2023-02-20 09:58:57.000000 iracingdataapi-1.1.0/setup.py
-drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-03-21 10:18:02.004819 iracingdataapi-1.1.0/src/
-drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-03-21 10:18:02.005989 iracingdataapi-1.1.0/src/iracingdataapi/
--rw-r--r--   0 jasondilworth   (501) staff       (20)        0 2022-03-24 20:28:11.000000 iracingdataapi-1.1.0/src/iracingdataapi/__init__.py
--rw-r--r--   0 jasondilworth   (501) staff       (20)    44912 2023-03-20 15:23:15.000000 iracingdataapi-1.1.0/src/iracingdataapi/client.py
-drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-03-21 10:18:02.007320 iracingdataapi-1.1.0/src/iracingdataapi.egg-info/
--rw-r--r--   0 jasondilworth   (501) staff       (20)     3274 2023-03-21 10:18:01.000000 iracingdataapi-1.1.0/src/iracingdataapi.egg-info/PKG-INFO
--rw-r--r--   0 jasondilworth   (501) staff       (20)      307 2023-03-21 10:18:02.000000 iracingdataapi-1.1.0/src/iracingdataapi.egg-info/SOURCES.txt
--rw-r--r--   0 jasondilworth   (501) staff       (20)        1 2023-03-21 10:18:01.000000 iracingdataapi-1.1.0/src/iracingdataapi.egg-info/dependency_links.txt
--rw-r--r--   0 jasondilworth   (501) staff       (20)        9 2023-03-21 10:18:02.000000 iracingdataapi-1.1.0/src/iracingdataapi.egg-info/requires.txt
--rw-r--r--   0 jasondilworth   (501) staff       (20)       15 2023-03-21 10:18:02.000000 iracingdataapi-1.1.0/src/iracingdataapi.egg-info/top_level.txt
+drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:23:26.063277 iracingdataapi-1.1.1/
+-rw-r--r--   0 jasondilworth   (501) staff       (20)     1073 2022-03-24 20:31:50.000000 iracingdataapi-1.1.1/LICENSE
+-rw-r--r--   0 jasondilworth   (501) staff       (20)       17 2022-03-24 21:34:57.000000 iracingdataapi-1.1.1/MANIFEST.in
+-rw-r--r--   0 jasondilworth   (501) staff       (20)     3403 2023-05-05 19:23:26.063111 iracingdataapi-1.1.1/PKG-INFO
+-rw-r--r--   0 jasondilworth   (501) staff       (20)     2844 2023-05-05 19:20:23.000000 iracingdataapi-1.1.1/README.md
+-rw-r--r--   0 jasondilworth   (501) staff       (20)       38 2023-05-05 19:23:26.063313 iracingdataapi-1.1.1/setup.cfg
+-rw-r--r--   0 jasondilworth   (501) staff       (20)      893 2023-05-05 19:20:34.000000 iracingdataapi-1.1.1/setup.py
+drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:23:26.059609 iracingdataapi-1.1.1/src/
+drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:23:26.061550 iracingdataapi-1.1.1/src/iracingdataapi/
+-rw-r--r--   0 jasondilworth   (501) staff       (20)        0 2022-03-24 20:28:11.000000 iracingdataapi-1.1.1/src/iracingdataapi/__init__.py
+-rw-r--r--   0 jasondilworth   (501) staff       (20)    45626 2023-05-05 19:16:47.000000 iracingdataapi-1.1.1/src/iracingdataapi/client.py
+drwxr-xr-x   0 jasondilworth   (501) staff       (20)        0 2023-05-05 19:23:26.062868 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/
+-rw-r--r--   0 jasondilworth   (501) staff       (20)     3403 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/PKG-INFO
+-rw-r--r--   0 jasondilworth   (501) staff       (20)      307 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jasondilworth   (501) staff       (20)        1 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jasondilworth   (501) staff       (20)        9 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/requires.txt
+-rw-r--r--   0 jasondilworth   (501) staff       (20)       15 2023-05-05 19:23:26.000000 iracingdataapi-1.1.1/src/iracingdataapi.egg-info/top_level.txt
```

### Comparing `iracingdataapi-1.1.0/LICENSE` & `iracingdataapi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iracingdataapi-1.1.0/PKG-INFO` & `iracingdataapi-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iracingdataapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple wrapper around the iRacing General Data API
 Home-page: https://github.com/jasondilworth56/iracingdataapi
 Author: Jason Dilworth
 Author-email: hello@jasondilworth.co.uk
 Project-URL: Bug Tracker, https://github.com/jasondilworth56/iracingdataapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,14 +43,19 @@
 All available methods of `irDataClient` are included in `client.py`.
 
 # Contributing
 
 I welcome all pull requests for improvements or missing endpoints over time as they are added by iRacing.
 
 # Changelog
+
+**1.1.1**
+-   Bug fix for some 5xx errors that are thrown by iRacing
+-   Added the `season_spectator_subsessionids()` endpoint
+
 **1.1.0**
 -   Added docstrings to all methods for developer experience
 -   Renamed `series()` to `get_series()` for consistency. **Breaking change:** For that same consistency, `series` has been reimplemented as a property which returns the series with their assets. To amend your implementation, either switch to `get_series()` or remove any brackets in your call of `series`.
 -   Renamed `get_carclass()` to `get_carclasses()` to be more consistent with other endpoints. **NOTE:** `get_carclass()` will be removed in a future release.
 -   Added assets to the returned data of `tracks`. If you prefer not to get those assets, use `get_tracks()`.
 -   Removed redundant cookie handling code, as that is all handled within `requests.Session`
 -   Fixed a ratelimiting error
```

### Comparing `iracingdataapi-1.1.0/README.md` & `iracingdataapi-1.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 All available methods of `irDataClient` are included in `client.py`.
 
 # Contributing
 
 I welcome all pull requests for improvements or missing endpoints over time as they are added by iRacing.
 
 # Changelog
+
+**1.1.1**
+-   Bug fix for some 5xx errors that are thrown by iRacing
+-   Added the `season_spectator_subsessionids()` endpoint
+
 **1.1.0**
 -   Added docstrings to all methods for developer experience
 -   Renamed `series()` to `get_series()` for consistency. **Breaking change:** For that same consistency, `series` has been reimplemented as a property which returns the series with their assets. To amend your implementation, either switch to `get_series()` or remove any brackets in your call of `series`.
 -   Renamed `get_carclass()` to `get_carclasses()` to be more consistent with other endpoints. **NOTE:** `get_carclass()` will be removed in a future release.
 -   Added assets to the returned data of `tracks`. If you prefer not to get those assets, use `get_tracks()`.
 -   Removed redundant cookie handling code, as that is all handled within `requests.Session`
 -   Fixed a ratelimiting error
```

### Comparing `iracingdataapi-1.1.0/setup.py` & `iracingdataapi-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iracingdataapi",
-    version="1.1.0",
+    version="1.1.1",
     author="Jason Dilworth",
     author_email="hello@jasondilworth.co.uk",
     description="A simple wrapper around the iRacing General Data API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jasondilworth56/iracingdataapi",
     project_urls={
```

### Comparing `iracingdataapi-1.1.0/src/iracingdataapi/client.py` & `iracingdataapi-1.1.1/src/iracingdataapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,29 +67,29 @@
                 reset_datetime = datetime.fromtimestamp(int(ratelimit_reset))
                 delta = reset_datetime - datetime.now()
                 if delta.total_seconds() > 0:
                     time.sleep(delta.total_seconds())
             return self._get_resource_or_link(url, payload=payload)
 
         if r.status_code != 200:
-            raise RuntimeError(r.json())
+            raise RuntimeError("Unhandled Non-200 response", r)
         data = r.json()
         if not isinstance(data, list) and "link" in data.keys():
             return [data.get("link"), True]
         else:
             return [data, False]
 
     def _get_resource(self, endpoint, payload=None):
         request_url = self._build_url(endpoint)
         resource_obj, is_link = self._get_resource_or_link(request_url, payload=payload)
         if not is_link:
             return resource_obj
         r = self.session.get(resource_obj)
         if r.status_code != 200:
-            raise RuntimeError(r.json())
+            raise RuntimeError("Unhandled Non-200 response", r)
         return r.json()
 
     def _get_chunks(self, chunks):
         if not isinstance(chunks, dict):
             # if there are no chunks, return an empty list for compatibility
             return []
         base_url = chunks.get("base_download_url")
@@ -1129,14 +1129,33 @@
         if start_from:
             payload["from"] = start_from
         if include_end_after_from:
             payload["include_end_after_from"] = include_end_after_from
 
         return self._get_resource("/data/season/race_guide", payload=payload)
 
+    def season_spectator_subsessionids(self, event_types:list=[2,3,4,5]):
+        """Get the current list of subsession IDs for a given event type
+        
+        Args:
+            event_types (list): A list of integers that match with iRacing event types as follows:
+                2: Practise
+                3: Qualify
+                4: Time Trial
+                5: Race
+
+        Returns:
+            list: a list of the matching subsession IDs
+        """
+        payload = {}
+        if event_types:
+            payload["event_types": ",".join(event_types)]
+        
+        return self._get_resource("/data/season/spectator_subsessionids", payload=payload)
+
     def get_series(self):
         """Get all the current official iRacing series.
 
         Returns:
             list: a list containing all the official iRacing series.
 
         """
```

### Comparing `iracingdataapi-1.1.0/src/iracingdataapi.egg-info/PKG-INFO` & `iracingdataapi-1.1.1/src/iracingdataapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iracingdataapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple wrapper around the iRacing General Data API
 Home-page: https://github.com/jasondilworth56/iracingdataapi
 Author: Jason Dilworth
 Author-email: hello@jasondilworth.co.uk
 Project-URL: Bug Tracker, https://github.com/jasondilworth56/iracingdataapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,14 +43,19 @@
 All available methods of `irDataClient` are included in `client.py`.
 
 # Contributing
 
 I welcome all pull requests for improvements or missing endpoints over time as they are added by iRacing.
 
 # Changelog
+
+**1.1.1**
+-   Bug fix for some 5xx errors that are thrown by iRacing
+-   Added the `season_spectator_subsessionids()` endpoint
+
 **1.1.0**
 -   Added docstrings to all methods for developer experience
 -   Renamed `series()` to `get_series()` for consistency. **Breaking change:** For that same consistency, `series` has been reimplemented as a property which returns the series with their assets. To amend your implementation, either switch to `get_series()` or remove any brackets in your call of `series`.
 -   Renamed `get_carclass()` to `get_carclasses()` to be more consistent with other endpoints. **NOTE:** `get_carclass()` will be removed in a future release.
 -   Added assets to the returned data of `tracks`. If you prefer not to get those assets, use `get_tracks()`.
 -   Removed redundant cookie handling code, as that is all handled within `requests.Session`
 -   Fixed a ratelimiting error
```

