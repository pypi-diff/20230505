# Comparing `tmp/shazamio-0.4.0.0.tar.gz` & `tmp/shazamio-0.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shazamio-0.4.0.0.tar", max compression
+gzip compressed data, was "shazamio-0.4.0.1.tar", max compression
```

## Comparing `shazamio-0.4.0.0.tar` & `shazamio-0.4.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1063 2023-05-05 06:25:35.115534 shazamio-0.4.0.0/LICENSE.txt
--rw-r--r--   0        0        0    10440 2023-05-05 06:25:35.115534 shazamio-0.4.0.0/README.md
--rw-r--r--   0        0        0     1036 2023-05-05 06:25:51.027648 shazamio-0.4.0.0/pyproject.toml
--rw-r--r--   0        0        0      172 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/__init__.py
--rw-r--r--   0        0        0    11516 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/algorithm.py
--rw-r--r--   0        0        0    14285 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/api.py
--rw-r--r--   0        0        0      667 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/client.py
--rw-r--r--   0        0        0     2509 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/converter.py
--rw-r--r--   0        0        0      832 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/enums.py
--rw-r--r--   0        0        0      168 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/exceptions.py
--rw-r--r--   0        0        0     3458 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/factory.py
--rw-r--r--   0        0        0     1526 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/factory_misc.py
--rw-r--r--   0        0        0     2805 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/misc.py
--rw-r--r--   0        0        0        0 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/__init__.py
--rw-r--r--   0        0        0     1863 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/full_albums.py
--rw-r--r--   0        0        0     1487 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/last_release.py
--rw-r--r--   0        0        0     1337 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/simular_artists.py
--rw-r--r--   0        0        0     1406 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/top_music.py
--rw-r--r--   0        0        0     1817 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/top_song.py
--rw-r--r--   0        0        0     2752 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artists.py
--rw-r--r--   0        0        0      345 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/attributes.py
--rw-r--r--   0        0        0      455 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/base.py
--rw-r--r--   0        0        0      464 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/enums.py
--rw-r--r--   0        0        0      138 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/errors.py
--rw-r--r--   0        0        0     4122 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/schemas/models.py
--rw-r--r--   0        0        0      526 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/schemas/photos.py
--rw-r--r--   0        0        0       71 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/schemas/urls.py
--rw-r--r--   0        0        0      956 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/serializers.py
--rw-r--r--   0        0        0     9880 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/signature.py
--rw-r--r--   0        0        0      164 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/typehints.py
--rw-r--r--   0        0        0     7017 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/user_agent.py
--rw-r--r--   0        0        0     1863 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/utils.py
--rw-r--r--   0        0        0    11573 1970-01-01 00:00:00.000000 shazamio-0.4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-05 09:08:16.240331 shazamio-0.4.0.1/LICENSE.txt
+-rw-r--r--   0        0        0    10302 2023-05-05 09:08:16.240331 shazamio-0.4.0.1/README.md
+-rw-r--r--   0        0        0     1036 2023-05-05 09:08:35.384330 shazamio-0.4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/__init__.py
+-rw-r--r--   0        0        0    11516 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/algorithm.py
+-rw-r--r--   0        0        0    14285 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/api.py
+-rw-r--r--   0        0        0      667 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/client.py
+-rw-r--r--   0        0        0     2509 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/converter.py
+-rw-r--r--   0        0        0      832 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/enums.py
+-rw-r--r--   0        0        0      168 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/exceptions.py
+-rw-r--r--   0        0        0     3458 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/factory.py
+-rw-r--r--   0        0        0     1526 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/factory_misc.py
+-rw-r--r--   0        0        0     2805 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/misc.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/schemas/artist/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/schemas/artist/views/__init__.py
+-rw-r--r--   0        0        0     1863 2023-05-05 09:08:16.248331 shazamio-0.4.0.1/shazamio/schemas/artist/views/full_albums.py
+-rw-r--r--   0        0        0     1487 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/artist/views/last_release.py
+-rw-r--r--   0        0        0     1337 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/artist/views/simular_artists.py
+-rw-r--r--   0        0        0     1406 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/artist/views/top_music.py
+-rw-r--r--   0        0        0     1817 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/artist/views/top_song.py
+-rw-r--r--   0        0        0     2752 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/artists.py
+-rw-r--r--   0        0        0      345 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/attributes.py
+-rw-r--r--   0        0        0      455 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/base.py
+-rw-r--r--   0        0        0      464 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/enums.py
+-rw-r--r--   0        0        0      138 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/errors.py
+-rw-r--r--   0        0        0     4122 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/models.py
+-rw-r--r--   0        0        0      526 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/photos.py
+-rw-r--r--   0        0        0       71 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/schemas/urls.py
+-rw-r--r--   0        0        0      956 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/serializers.py
+-rw-r--r--   0        0        0     9880 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/signature.py
+-rw-r--r--   0        0        0      164 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/typehints.py
+-rw-r--r--   0        0        0     7017 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/user_agent.py
+-rw-r--r--   0        0        0     1863 2023-05-05 09:08:16.252331 shazamio-0.4.0.1/shazamio/utils.py
+-rw-r--r--   0        0        0    11435 1970-01-01 00:00:00.000000 shazamio-0.4.0.1/PKG-INFO
```

### Comparing `shazamio-0.4.0.0/LICENSE.txt` & `shazamio-0.4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/README.md` & `shazamio-0.4.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 <p align="center">
-<img src="https://img.shields.io/lgtm/grade/python/github/dotX12/waio" alt="https://img.shields.io/lgtm/grade/python/github/dotX12/waio">
 <img src="https://scrutinizer-ci.com/g/dotX12/ShazamIO/badges/quality-score.png?b=master" alt="https://scrutinizer-ci.com/g/dotX12/ShazamIO/">
 <img src="https://scrutinizer-ci.com/g/dotX12/ShazamIO/badges/code-intelligence.svg?b=master" alt="https://scrutinizer-ci.com/g/dotX12/ShazamIO/">
 <img src="https://scrutinizer-ci.com/g/dotX12/ShazamIO/badges/build.png?b=master" alt="https://scrutinizer-ci.com/g/dotX12/ShazamIO/">
 <img src="https://badge.fury.io/py/shazamio.svg" alt="https://badge.fury.io/py/shazamio">
 <img src="https://pepy.tech/badge/shazamio" alt="https://pepy.tech/project/shazamio">
 <img src="https://pepy.tech/badge/shazamio/month" alt="https://pepy.tech/project/shazamio">
 <img src="https://img.shields.io/github/license/dotX12/shazamio.svg" alt="https://github.com/dotX12/ShazamIO/blob/master/LICENSE.txt">
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-    [https://img.shields.io/lgtm/grade/python/github/dotX12/waio] [https://
- scrutinizer-ci.com/g/dotX12/ShazamIO/] [https://scrutinizer-ci.com/g/dotX12/
-     ShazamIO/] [https://scrutinizer-ci.com/g/dotX12/ShazamIO/] [https://
+[https://scrutinizer-ci.com/g/dotX12/ShazamIO/] [https://scrutinizer-ci.com/g/
+  dotX12/ShazamIO/] [https://scrutinizer-ci.com/g/dotX12/ShazamIO/] [https://
    badge.fury.io/py/shazamio] [https://pepy.tech/project/shazamio] [https://
  pepy.tech/project/shazamio] [https://github.com/dotX12/ShazamIO/blob/master/
                                  LICENSE.txt]
 
  [https://user-images.githubusercontent.com/64792903/109359596-ca561a00-7896-
  11eb-9c93-9cf1f283b1a5.png] ðµ Is a FREE asynchronous library from reverse
 engineered Shazam API written in Python 3.8+ with asyncio and aiohttp. Includes
```

### Comparing `shazamio-0.4.0.0/pyproject.toml` & `shazamio-0.4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shazamio"
-version = "0.4.0.0"
+version = "0.4.0.1"
 description = "Is a asynchronous framework from reverse engineered Shazam API written in Python 3.8+ with asyncio and aiohttp."
 authors = ["dotX12"]
 license = "MIT License"
 keywords = ["python", "shazam", "music", "recognize", "api", "async", "asyncio", "aiohttp", "identification"]
 readme = "README.md"
 homepage = "https://github.com/dotX12/ShazamIO"
 repository = "https://github.com/dotX12/ShazamIO"
```

### Comparing `shazamio-0.4.0.0/shazamio/algorithm.py` & `shazamio-0.4.0.1/shazamio/algorithm.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/api.py` & `shazamio-0.4.0.1/shazamio/api.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/client.py` & `shazamio-0.4.0.1/shazamio/client.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/converter.py` & `shazamio-0.4.0.1/shazamio/converter.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/enums.py` & `shazamio-0.4.0.1/shazamio/enums.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/factory.py` & `shazamio-0.4.0.1/shazamio/factory.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/factory_misc.py` & `shazamio-0.4.0.1/shazamio/factory_misc.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/misc.py` & `shazamio-0.4.0.1/shazamio/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     )
     GENRE_COUNTRY = (
         "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
         "/genre-country-chart-{country}-{genre}?pageSize={limit}&startFrom={offset}"
     )
     RELATED_SONGS = (
         "https://cdn.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
-        "/track-similarities-id-{track_id}?startFrom={limit}&pageSize={offset}&connected=&channel="
+        "/track-similarities-id-{track_id}?startFrom={offset}&pageSize={limit}&connected=&channel="
     )
     SEARCH_ARTIST = (
         "https://www.shazam.com/services/search/v4/{language}/{endpoint_country}/web"
         "/search?term={query}&limit={limit}&offset={offset}&types=artists"
     )
     SEARCH_MUSIC = (
         "https://www.shazam.com/services/search/v3/{language}/{endpoint_country}/web"
```

### Comparing `shazamio-0.4.0.0/shazamio/schemas/artist/views/full_albums.py` & `shazamio-0.4.0.1/shazamio/schemas/artist/views/full_albums.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/schemas/artist/views/last_release.py` & `shazamio-0.4.0.1/shazamio/schemas/artist/views/last_release.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/schemas/artist/views/simular_artists.py` & `shazamio-0.4.0.1/shazamio/schemas/artist/views/simular_artists.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/schemas/artist/views/top_music.py` & `shazamio-0.4.0.1/shazamio/schemas/artist/views/top_music.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/schemas/artist/views/top_song.py` & `shazamio-0.4.0.1/shazamio/schemas/artist/views/top_song.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/schemas/artists.py` & `shazamio-0.4.0.1/shazamio/schemas/artists.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/schemas/models.py` & `shazamio-0.4.0.1/shazamio/schemas/models.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/schemas/photos.py` & `shazamio-0.4.0.1/shazamio/schemas/photos.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/serializers.py` & `shazamio-0.4.0.1/shazamio/serializers.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/signature.py` & `shazamio-0.4.0.1/shazamio/signature.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/user_agent.py` & `shazamio-0.4.0.1/shazamio/user_agent.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/shazamio/utils.py` & `shazamio-0.4.0.1/shazamio/utils.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.4.0.0/PKG-INFO` & `shazamio-0.4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shazamio
-Version: 0.4.0.0
+Version: 0.4.0.1
 Summary: Is a asynchronous framework from reverse engineered Shazam API written in Python 3.8+ with asyncio and aiohttp.
 Home-page: https://github.com/dotX12/ShazamIO
 License: MIT
 Keywords: python,shazam,music,recognize,api,async,asyncio,aiohttp,identification
 Author: dotX12
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,14 @@
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.20.3,<0.21.0)
 Project-URL: Repository, https://github.com/dotX12/ShazamIO
 Description-Content-Type: text/markdown
 
 <p align="center">
-<img src="https://img.shields.io/lgtm/grade/python/github/dotX12/waio" alt="https://img.shields.io/lgtm/grade/python/github/dotX12/waio">
 <img src="https://scrutinizer-ci.com/g/dotX12/ShazamIO/badges/quality-score.png?b=master" alt="https://scrutinizer-ci.com/g/dotX12/ShazamIO/">
 <img src="https://scrutinizer-ci.com/g/dotX12/ShazamIO/badges/code-intelligence.svg?b=master" alt="https://scrutinizer-ci.com/g/dotX12/ShazamIO/">
 <img src="https://scrutinizer-ci.com/g/dotX12/ShazamIO/badges/build.png?b=master" alt="https://scrutinizer-ci.com/g/dotX12/ShazamIO/">
 <img src="https://badge.fury.io/py/shazamio.svg" alt="https://badge.fury.io/py/shazamio">
 <img src="https://pepy.tech/badge/shazamio" alt="https://pepy.tech/project/shazamio">
 <img src="https://pepy.tech/badge/shazamio/month" alt="https://pepy.tech/project/shazamio">
 <img src="https://img.shields.io/github/license/dotX12/shazamio.svg" alt="https://github.com/dotX12/ShazamIO/blob/master/LICENSE.txt">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shazamio Version: 0.4.0.0 Summary: Is a
+Metadata-Version: 2.1 Name: shazamio Version: 0.4.0.1 Summary: Is a
 asynchronous framework from reverse engineered Shazam API written in Python
 3.8+ with asyncio and aiohttp. Home-page: https://github.com/dotX12/ShazamIO
 License: MIT Keywords:
 python,shazam,music,recognize,api,async,asyncio,aiohttp,identification Author:
 dotX12 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -10,17 +10,16 @@
 Language :: Python :: 3.11 Requires-Dist: aiofiles (>=22.1.0,<23.0.0) Requires-
 Dist: aiohttp (>=3.8.3,<4.0.0) Requires-Dist: anyio (>=3.6.2,<4.0.0) Requires-
 Dist: dataclass-factory (==2.16) Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0) Requires-Dist: pydub
 (>=0.25.1,<0.26.0) Requires-Dist: pytest (>=7.2.0,<8.0.0) Requires-Dist:
 pytest-asyncio (>=0.20.3,<0.21.0) Project-URL: Repository, https://github.com/
 dotX12/ShazamIO Description-Content-Type: text/markdown
-    [https://img.shields.io/lgtm/grade/python/github/dotX12/waio] [https://
- scrutinizer-ci.com/g/dotX12/ShazamIO/] [https://scrutinizer-ci.com/g/dotX12/
-     ShazamIO/] [https://scrutinizer-ci.com/g/dotX12/ShazamIO/] [https://
+[https://scrutinizer-ci.com/g/dotX12/ShazamIO/] [https://scrutinizer-ci.com/g/
+  dotX12/ShazamIO/] [https://scrutinizer-ci.com/g/dotX12/ShazamIO/] [https://
    badge.fury.io/py/shazamio] [https://pepy.tech/project/shazamio] [https://
  pepy.tech/project/shazamio] [https://github.com/dotX12/ShazamIO/blob/master/
                                  LICENSE.txt]
 
  [https://user-images.githubusercontent.com/64792903/109359596-ca561a00-7896-
  11eb-9c93-9cf1f283b1a5.png] ðµ Is a FREE asynchronous library from reverse
 engineered Shazam API written in Python 3.8+ with asyncio and aiohttp. Includes
```

