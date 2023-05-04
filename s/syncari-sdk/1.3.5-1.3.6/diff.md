# Comparing `tmp/syncari-sdk-1.3.5.tar.gz` & `tmp/syncari-sdk-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncari-sdk-1.3.5.tar", last modified: Thu Mar 23 22:13:59 2023, max compression
+gzip compressed data, was "syncari-sdk-1.3.6.tar", last modified: Thu May  4 23:36:04 2023, max compression
```

## Comparing `syncari-sdk-1.3.5.tar` & `syncari-sdk-1.3.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-03-23 22:13:59.131910 syncari-sdk-1.3.5/
--rw-r--r--   0 vraman     (501) staff       (20)      299 2023-03-23 22:13:59.131607 syncari-sdk-1.3.5/PKG-INFO
--rw-r--r--   0 vraman     (501) staff       (20)       78 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/README.md
--rw-r--r--   0 vraman     (501) staff       (20)       38 2023-03-23 22:13:59.131995 syncari-sdk-1.3.5/setup.cfg
--rwxr-xr-x   0 vraman     (501) staff       (20)      554 2023-03-23 20:27:49.000000 syncari-sdk-1.3.5/setup.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-03-23 22:13:59.122821 syncari-sdk-1.3.5/syncari/
--rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/syncari/__init__.py
--rw-r--r--   0 vraman     (501) staff       (20)      699 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/syncari/logger.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-03-23 22:13:59.125292 syncari-sdk-1.3.5/syncari/models/
--rw-r--r--   0 vraman     (501) staff       (20)       64 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/syncari/models/__init__.py
--rw-r--r--   0 vraman     (501) staff       (20)     3935 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/syncari/models/core.py
--rw-r--r--   0 vraman     (501) staff       (20)     2505 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/syncari/models/request.py
--rw-r--r--   0 vraman     (501) staff       (20)     2273 2023-03-23 20:10:51.000000 syncari-sdk-1.3.5/syncari/models/schema.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-03-23 22:13:59.126285 syncari-sdk-1.3.5/syncari/rest/
--rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/syncari/rest/__init__.py
--rw-r--r--   0 vraman     (501) staff       (20)     4011 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/syncari/rest/client.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-03-23 22:13:59.127366 syncari-sdk-1.3.5/syncari/synapse/
--rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/syncari/synapse/__init__.py
--rw-r--r--   0 vraman     (501) staff       (20)    10308 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/syncari/synapse/abstract_synapse.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-03-23 22:13:59.129257 syncari-sdk-1.3.5/syncari_sdk.egg-info/
--rw-r--r--   0 vraman     (501) staff       (20)      299 2023-03-23 22:13:59.000000 syncari-sdk-1.3.5/syncari_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vraman     (501) staff       (20)      569 2023-03-23 22:13:59.000000 syncari-sdk-1.3.5/syncari_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vraman     (501) staff       (20)        1 2023-03-23 22:13:59.000000 syncari-sdk-1.3.5/syncari_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vraman     (501) staff       (20)       39 2023-03-23 22:13:59.000000 syncari-sdk-1.3.5/syncari_sdk.egg-info/requires.txt
--rw-r--r--   0 vraman     (501) staff       (20)       19 2023-03-23 22:13:59.000000 syncari-sdk-1.3.5/syncari_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-03-23 22:13:59.131005 syncari-sdk-1.3.5/unit_tests/
--rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/unit_tests/__init__.py
--rw-r--r--   0 vraman     (501) staff       (20)     7319 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/unit_tests/test_mock_synapse.py
--rw-r--r--   0 vraman     (501) staff       (20)     6299 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/unit_tests/test_response_validations.py
--rw-r--r--   0 vraman     (501) staff       (20)     1962 2023-03-23 20:00:03.000000 syncari-sdk-1.3.5/unit_tests/test_rest_client.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.868011 syncari-sdk-1.3.6/
+-rw-r--r--   0 blesson    (501) staff       (20)      338 2023-05-04 23:36:04.867882 syncari-sdk-1.3.6/PKG-INFO
+-rw-r--r--   0 blesson    (501) staff       (20)       78 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/README.md
+-rw-r--r--   0 blesson    (501) staff       (20)       38 2023-05-04 23:36:04.868048 syncari-sdk-1.3.6/setup.cfg
+-rwxr-xr-x   0 blesson    (501) staff       (20)      562 2023-05-04 23:35:07.000000 syncari-sdk-1.3.6/setup.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.860679 syncari-sdk-1.3.6/syncari/
+-rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)      699 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/logger.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.861587 syncari-sdk-1.3.6/syncari/models/
+-rw-r--r--   0 blesson    (501) staff       (20)       64 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/models/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)     3935 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/models/core.py
+-rw-r--r--   0 blesson    (501) staff       (20)     2505 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/models/request.py
+-rw-r--r--   0 blesson    (501) staff       (20)     2273 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/models/schema.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.861841 syncari-sdk-1.3.6/syncari/rest/
+-rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/rest/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)     4010 2023-05-04 23:35:13.000000 syncari-sdk-1.3.6/syncari/rest/client.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.862562 syncari-sdk-1.3.6/syncari/synapse/
+-rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/synapse/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)    10308 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/syncari/synapse/abstract_synapse.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.863263 syncari-sdk-1.3.6/syncari_sdk.egg-info/
+-rw-r--r--   0 blesson    (501) staff       (20)      338 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 blesson    (501) staff       (20)      569 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 blesson    (501) staff       (20)        1 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 blesson    (501) staff       (20)       47 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/requires.txt
+-rw-r--r--   0 blesson    (501) staff       (20)       19 2023-05-04 23:36:04.000000 syncari-sdk-1.3.6/syncari_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-05-04 23:36:04.867687 syncari-sdk-1.3.6/unit_tests/
+-rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/unit_tests/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)     7319 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/unit_tests/test_mock_synapse.py
+-rw-r--r--   0 blesson    (501) staff       (20)     6299 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/unit_tests/test_response_validations.py
+-rw-r--r--   0 blesson    (501) staff       (20)     1962 2023-05-04 22:58:58.000000 syncari-sdk-1.3.6/unit_tests/test_rest_client.py
```

### Comparing `syncari-sdk-1.3.5/setup.py` & `syncari-sdk-1.3.6/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='syncari-sdk',
-    version='1.3.5',
+    version='1.3.6',
     description='Syncari Synapse Development Kit',
     author='Syncari',
     author_email='dev@syncari.com',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='TBD',
     packages=find_packages(exclude=('unittests')),
     install_requires=[
         'pydantic~=1.6',
         'requests',
-        'urllib3',
+        'urllib3==1.26.0',
         'backoff'
     ],
     python_requires='>=3.7.0',
 )
```

### Comparing `syncari-sdk-1.3.5/syncari/logger.py` & `syncari-sdk-1.3.6/syncari/logger.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.5/syncari/models/core.py` & `syncari-sdk-1.3.6/syncari/models/core.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.5/syncari/models/request.py` & `syncari-sdk-1.3.6/syncari/models/request.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.5/syncari/models/schema.py` & `syncari-sdk-1.3.6/syncari/models/schema.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.5/syncari/rest/client.py` & `syncari-sdk-1.3.6/syncari/rest/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.auth_config = auth_config
         self.rest_url = base_url
         self._session = requests.Session()
 
         retry_strategy = Retry(
             total=3,
             status_forcelist=[429, 500, 502, 503, 504],
-            method_whitelist=["HEAD", "GET", "OPTIONS"]
+            allowed_methods=["HEAD", "GET", "OPTIONS"]
         )
         adapter = HTTPAdapter(max_retries=retry_strategy)
 
         adapter = requests.adapters.HTTPAdapter(max_retries=3)
         self._session.mount('https://', adapter)
 
     def get(self, path, **kwargs):
```

### Comparing `syncari-sdk-1.3.5/syncari/synapse/abstract_synapse.py` & `syncari-sdk-1.3.6/syncari/synapse/abstract_synapse.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.5/syncari_sdk.egg-info/SOURCES.txt` & `syncari-sdk-1.3.6/syncari_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.5/unit_tests/test_mock_synapse.py` & `syncari-sdk-1.3.6/unit_tests/test_mock_synapse.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.5/unit_tests/test_response_validations.py` & `syncari-sdk-1.3.6/unit_tests/test_response_validations.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.5/unit_tests/test_rest_client.py` & `syncari-sdk-1.3.6/unit_tests/test_rest_client.py`

 * *Files identical despite different names*

