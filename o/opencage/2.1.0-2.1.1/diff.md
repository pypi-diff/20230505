# Comparing `tmp/opencage-2.1.0.tar.gz` & `tmp/opencage-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencage-2.1.0.tar", last modified: Thu Oct 13 21:54:54 2022, max compression
+gzip compressed data, was "opencage-2.1.1.tar", last modified: Thu Apr 20 10:22:36 2023, max compression
```

## Comparing `opencage-2.1.0.tar` & `opencage-2.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-10-13 21:54:54.000000 opencage-2.1.0/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1513 2021-03-13 15:19:05.000000 opencage-2.1.0/LICENSE.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4911 2022-10-13 21:54:54.000000 opencage-2.1.0/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3854 2022-10-13 18:53:56.000000 opencage-2.1.0/README.md
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-10-13 21:54:54.000000 opencage-2.1.0/opencage/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      128 2021-03-13 15:18:50.000000 opencage-2.1.0/opencage/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10877 2022-10-13 21:18:40.000000 opencage-2.1.0/opencage/geocoder.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-10-13 21:54:54.000000 opencage-2.1.0/opencage.egg-info/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4911 2022-10-13 21:54:54.000000 opencage-2.1.0/opencage.egg-info/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      542 2022-10-13 21:54:54.000000 opencage-2.1.0/opencage.egg-info/SOURCES.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2022-10-13 21:54:54.000000 opencage-2.1.0/opencage.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2021-07-14 23:40:07.000000 opencage-2.1.0/opencage.egg-info/not-zip-safe
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       50 2022-10-13 21:54:54.000000 opencage-2.1.0/opencage.egg-info/requires.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       14 2022-10-13 21:54:54.000000 opencage-2.1.0/opencage.egg-info/top_level.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       38 2022-10-13 21:54:54.000000 opencage-2.1.0/setup.cfg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2145 2022-10-13 21:32:59.000000 opencage-2.1.0/setup.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-10-13 21:54:54.000000 opencage-2.1.0/test/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       34 2021-07-14 22:29:28.000000 opencage-2.1.0/test/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1924 2021-07-14 22:29:28.000000 opencage-2.1.0/test/test_all.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1444 2021-07-14 22:29:28.000000 opencage-2.1.0/test/test_async.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      659 2021-07-14 22:29:28.000000 opencage-2.1.0/test/test_error_blocked.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1114 2021-07-14 22:29:28.000000 opencage-2.1.0/test/test_error_invalid_input.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      656 2021-07-14 22:29:28.000000 opencage-2.1.0/test/test_error_not_authorized.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1229 2021-07-14 22:29:28.000000 opencage-2.1.0/test/test_error_ratelimit_exceeded.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1278 2022-10-13 21:26:37.000000 opencage-2.1.0/test/test_error_unknown.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      870 2021-07-14 22:29:28.000000 opencage-2.1.0/test/test_flotify_dict.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      771 2021-07-14 22:29:28.000000 opencage-2.1.0/test/test_reverse.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1151 2021-07-14 22:29:28.000000 opencage-2.1.0/test/test_session.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-20 10:22:36.616745 opencage-2.1.1/
+-rw-r--r--   0 mtm        (501) staff       (20)     1513 2021-06-22 16:46:46.000000 opencage-2.1.1/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     5197 2023-04-20 10:22:36.616461 opencage-2.1.1/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     4139 2023-04-20 10:16:06.000000 opencage-2.1.1/README.md
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-20 10:22:36.606443 opencage-2.1.1/opencage/
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2021-06-22 16:46:46.000000 opencage-2.1.1/opencage/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)    11035 2023-04-20 10:13:02.000000 opencage-2.1.1/opencage/geocoder.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-20 10:22:36.608750 opencage-2.1.1/opencage.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     5197 2023-04-20 10:22:36.000000 opencage-2.1.1/opencage.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      542 2023-04-20 10:22:36.000000 opencage-2.1.1/opencage.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-20 10:22:36.000000 opencage-2.1.1/opencage.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-04-20 10:22:36.000000 opencage-2.1.1/opencage.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)       50 2023-04-20 10:22:36.000000 opencage-2.1.1/opencage.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       14 2023-04-20 10:22:36.000000 opencage-2.1.1/opencage.egg-info/top_level.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       38 2023-04-20 10:22:36.616881 opencage-2.1.1/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     2166 2023-04-20 10:18:01.000000 opencage-2.1.1/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-04-20 10:22:36.616017 opencage-2.1.1/test/
+-rw-r--r--   0 mtm        (501) staff       (20)       34 2021-06-22 16:46:46.000000 opencage-2.1.1/test/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1930 2023-03-13 13:14:23.000000 opencage-2.1.1/test/test_all.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1528 2023-03-13 13:14:23.000000 opencage-2.1.1/test/test_async.py
+-rw-r--r--   0 mtm        (501) staff       (20)      675 2023-01-04 21:23:23.000000 opencage-2.1.1/test/test_error_blocked.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1096 2023-01-04 21:23:23.000000 opencage-2.1.1/test/test_error_invalid_input.py
+-rw-r--r--   0 mtm        (501) staff       (20)      672 2023-01-04 21:23:23.000000 opencage-2.1.1/test/test_error_not_authorized.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1306 2023-03-13 13:14:23.000000 opencage-2.1.1/test/test_error_ratelimit_exceeded.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1314 2023-03-13 13:14:23.000000 opencage-2.1.1/test/test_error_unknown.py
+-rw-r--r--   0 mtm        (501) staff       (20)      870 2021-06-22 16:46:46.000000 opencage-2.1.1/test/test_flotify_dict.py
+-rw-r--r--   0 mtm        (501) staff       (20)      771 2021-06-22 16:46:46.000000 opencage-2.1.1/test/test_reverse.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1347 2023-03-13 13:14:23.000000 opencage-2.1.1/test/test_session.py
```

### Comparing `opencage-2.1.0/LICENSE.txt` & `opencage-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opencage-2.1.0/PKG-INFO` & `opencage-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: opencage
-Version: 2.1.0
+Version: 2.1.1
 Summary: Wrapper module for the OpenCage Geocoder API
 Home-page: https://github.com/OpenCageData/python-opencage-geocoder/
 Download-URL: https://github.com/OpenCageData/python-opencage-geocoder/tarball/2.1.0
 Author: OpenCage GmbH
 Author-email: info@opencagedata.com
 License: BSD
 Keywords: geocoding,geocoder
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # OpenCage Geocoding Module for Python
@@ -32,19 +32,23 @@
 ## Build Status / Code Quality / etc
 
 [![PyPI version](https://badge.fury.io/py/opencage.svg)](https://badge.fury.io/py/opencage)
 [![Downloads](https://pepy.tech/badge/opencage/month)](https://pepy.tech/project/opencage)
 [![Versions](https://img.shields.io/pypi/pyversions/opencage)](https://pypi.org/project/opencage/)
 ![GitHub contributors](https://img.shields.io/github/contributors/opencagedata/python-opencage-geocoder)
 [![Build Status](https://travis-ci.com/OpenCageData/python-opencage-geocoder.svg?branch=master)](https://travis-ci.com/OpenCageData/python-opencage-geocoder)
-[![Twitter Follow](https://img.shields.io/twitter/follow/OpenCage?label=Follow%20OpenCage&style=social)](https://twitter.com/opencage)
+![Mastodon Follow](https://img.shields.io/mastodon/follow/109287663468501769?domain=https%3A%2F%2Fen.osm.town%2F&style=social)
+
+## Tutorial
+
+You can find a [comprehensive tutorial for using this module on the OpenCage site](https://opencagedata.com/tutorials/geocode-in-python).
 
 ## Usage
 
-Supports Python 3.6 or newer. Use the older opencage 1.x releases if you need Python 2.7 support.
+Supports Python 3.7 or newer. Use the older opencage 1.x releases if you need Python 2.7 support.
 
 Install the module:
 
 ```bash
 pip install opencage
 ```
 
@@ -58,42 +62,42 @@
 as a parameter to the geocoder modules's constructor:
 
 ```python
 key = 'your-api-key-here'
 geocoder = OpenCageGeocode(key)
 ```
 
-Pass a string containing the query or address to be geocoded to the modules's `geocode` method:
+Pass a string containing the query or address to be geocoded to the modules' `geocode` method:
 
 ```python
-query = "82 Clerkenwell Road, London"
-result = geocoder.geocode(query)
+query = '82 Clerkenwell Road, London'
+results = geocoder.geocode(query)
 ```
 
-You can add [additional parameters](https://opencagedata.com/api#forward):
+You can add [additional parameters](https://opencagedata.com/api#forward-opt):
 
 ```python
-result = geocoder.geocode('London', no_annotations=1, language='es')
+results = geocoder.geocode('London', no_annotations=1, language='es')
 ```
 
-You can use the proximity parameter to provide the geocoder with a hint:
+For example you can use the proximity parameter to provide the geocoder with a hint:
 
 ```python
-result = geocoder.geocode('London', proximity='42.828576, -81.406643')
-print(result[0]['formatted'])
+results = geocoder.geocode('London', proximity='42.828576, -81.406643')
+print(results[0]['formatted'])
 # u'London, ON N6A 3M8, Canada'
 ```
 
 
 ### Reverse geocoding
 
 Turn a lat/long into an address with the ``reverse_geocode`` method:
 
 ```python
-results = geocoder.reverse_geocode(51.51024, -0.10303)
+result = geocoder.reverse_geocode(51.51024, -0.10303)
 ```
 
 ### Sessions
 
 You can reuse your HTTP connection for multiple requests by
 using a `with` block. This can help performance when making
 a lot of requests:
@@ -101,34 +105,37 @@
 ```python
 queries = ['82 Clerkenwell Road, London', ...]
 with OpenCageGeocode(key) as geocoder:
     # Queries reuse the same HTTP connection
     results = [geocoder.geocode(query) for query in queries]
 ```
 
-### Asycronous requests
+### Asyncronous requests
 
 You can run requests in parallel with the `geocode_async` and `reverse_geocode_async`
 method which have the same parameters and response as their synronous counterparts.
 You will need at least Python 3.7 and the `asyncio` and `aiohttp` packages installed.
 
 ```python
 async with OpenCageGeocode(key) as geocoder:
     results = await geocoder.geocode_async(address)
 ```
 
-For a more complete example and links to futher tutorials on asycronous IO see
+For a more complete example and links to futher tutorials on asyncronous IO see
 `batch.py` in the `examples` directory.
 
 ### Exceptions
 
 If anything goes wrong, then an exception will be raised:
- * ``InvalidInputError`` for non-unicode query strings
- * ``UnknownError`` if there's some problem with the API (bad results, 500 status code, etc)
- * ``RateLimitExceededError`` if you go past your rate limit
+
+ * `InvalidInputError` for non-unicode query strings
+ * `NotAuthorizedError` if API key is missing, invalid syntax or disabled
+ * `ForbiddenError` API key is blocked or suspended
+ * `RateLimitExceededError` if you go past your rate limit
+ * `UnknownError` if there's some problem with the API (bad results, 500 status code, etc)
 
 
 ## Copyright & License
 
 This software is copyright OpenCage GmbH.
 Please see `LICENSE.txt`
```

### Comparing `opencage-2.1.0/README.md` & `opencage-2.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 ## Build Status / Code Quality / etc
 
 [![PyPI version](https://badge.fury.io/py/opencage.svg)](https://badge.fury.io/py/opencage)
 [![Downloads](https://pepy.tech/badge/opencage/month)](https://pepy.tech/project/opencage)
 [![Versions](https://img.shields.io/pypi/pyversions/opencage)](https://pypi.org/project/opencage/)
 ![GitHub contributors](https://img.shields.io/github/contributors/opencagedata/python-opencage-geocoder)
 [![Build Status](https://travis-ci.com/OpenCageData/python-opencage-geocoder.svg?branch=master)](https://travis-ci.com/OpenCageData/python-opencage-geocoder)
-[![Twitter Follow](https://img.shields.io/twitter/follow/OpenCage?label=Follow%20OpenCage&style=social)](https://twitter.com/opencage)
+![Mastodon Follow](https://img.shields.io/mastodon/follow/109287663468501769?domain=https%3A%2F%2Fen.osm.town%2F&style=social)
+
+## Tutorial
+
+You can find a [comprehensive tutorial for using this module on the OpenCage site](https://opencagedata.com/tutorials/geocode-in-python).
 
 ## Usage
 
-Supports Python 3.6 or newer. Use the older opencage 1.x releases if you need Python 2.7 support.
+Supports Python 3.7 or newer. Use the older opencage 1.x releases if you need Python 2.7 support.
 
 Install the module:
 
 ```bash
 pip install opencage
 ```
 
@@ -32,42 +36,42 @@
 as a parameter to the geocoder modules's constructor:
 
 ```python
 key = 'your-api-key-here'
 geocoder = OpenCageGeocode(key)
 ```
 
-Pass a string containing the query or address to be geocoded to the modules's `geocode` method:
+Pass a string containing the query or address to be geocoded to the modules' `geocode` method:
 
 ```python
-query = "82 Clerkenwell Road, London"
-result = geocoder.geocode(query)
+query = '82 Clerkenwell Road, London'
+results = geocoder.geocode(query)
 ```
 
-You can add [additional parameters](https://opencagedata.com/api#forward):
+You can add [additional parameters](https://opencagedata.com/api#forward-opt):
 
 ```python
-result = geocoder.geocode('London', no_annotations=1, language='es')
+results = geocoder.geocode('London', no_annotations=1, language='es')
 ```
 
-You can use the proximity parameter to provide the geocoder with a hint:
+For example you can use the proximity parameter to provide the geocoder with a hint:
 
 ```python
-result = geocoder.geocode('London', proximity='42.828576, -81.406643')
-print(result[0]['formatted'])
+results = geocoder.geocode('London', proximity='42.828576, -81.406643')
+print(results[0]['formatted'])
 # u'London, ON N6A 3M8, Canada'
 ```
 
 
 ### Reverse geocoding
 
 Turn a lat/long into an address with the ``reverse_geocode`` method:
 
 ```python
-results = geocoder.reverse_geocode(51.51024, -0.10303)
+result = geocoder.reverse_geocode(51.51024, -0.10303)
 ```
 
 ### Sessions
 
 You can reuse your HTTP connection for multiple requests by
 using a `with` block. This can help performance when making
 a lot of requests:
@@ -75,34 +79,37 @@
 ```python
 queries = ['82 Clerkenwell Road, London', ...]
 with OpenCageGeocode(key) as geocoder:
     # Queries reuse the same HTTP connection
     results = [geocoder.geocode(query) for query in queries]
 ```
 
-### Asycronous requests
+### Asyncronous requests
 
 You can run requests in parallel with the `geocode_async` and `reverse_geocode_async`
 method which have the same parameters and response as their synronous counterparts.
 You will need at least Python 3.7 and the `asyncio` and `aiohttp` packages installed.
 
 ```python
 async with OpenCageGeocode(key) as geocoder:
     results = await geocoder.geocode_async(address)
 ```
 
-For a more complete example and links to futher tutorials on asycronous IO see
+For a more complete example and links to futher tutorials on asyncronous IO see
 `batch.py` in the `examples` directory.
 
 ### Exceptions
 
 If anything goes wrong, then an exception will be raised:
- * ``InvalidInputError`` for non-unicode query strings
- * ``UnknownError`` if there's some problem with the API (bad results, 500 status code, etc)
- * ``RateLimitExceededError`` if you go past your rate limit
+
+ * `InvalidInputError` for non-unicode query strings
+ * `NotAuthorizedError` if API key is missing, invalid syntax or disabled
+ * `ForbiddenError` API key is blocked or suspended
+ * `RateLimitExceededError` if you go past your rate limit
+ * `UnknownError` if there's some problem with the API (bad results, 500 status code, etc)
 
 
 ## Copyright & License
 
 This software is copyright OpenCage GmbH.
 Please see `LICENSE.txt`
```

#### html2text {}

```diff
@@ -3,48 +3,51 @@
 [![PyPI version](https://badge.fury.io/py/opencage.svg)](https://badge.fury.io/
 py/opencage) [![Downloads](https://pepy.tech/badge/opencage/month)](https://
 pepy.tech/project/opencage) [![Versions](https://img.shields.io/pypi/
 pyversions/opencage)](https://pypi.org/project/opencage/) ![GitHub
 contributors](https://img.shields.io/github/contributors/opencagedata/python-
 opencage-geocoder) [![Build Status](https://travis-ci.com/OpenCageData/python-
 opencage-geocoder.svg?branch=master)](https://travis-ci.com/OpenCageData/
-python-opencage-geocoder) [![Twitter Follow](https://img.shields.io/twitter/
-follow/OpenCage?label=Follow%20OpenCage&style=social)](https://twitter.com/
-opencage) ## Usage Supports Python 3.6 or newer. Use the older opencage 1.x
-releases if you need Python 2.7 support. Install the module: ```bash pip
-install opencage ``` Load the module: ```python from opencage.geocoder import
-OpenCageGeocode ``` Create an instance of the geocoder module, passing a valid
-OpenCage Data Geocoder API key as a parameter to the geocoder modules's
-constructor: ```python key = 'your-api-key-here' geocoder = OpenCageGeocode
-(key) ``` Pass a string containing the query or address to be geocoded to the
-modules's `geocode` method: ```python query = "82 Clerkenwell Road, London"
-result = geocoder.geocode(query) ``` You can add [additional parameters](https:
-//opencagedata.com/api#forward): ```python result = geocoder.geocode('London',
-no_annotations=1, language='es') ``` You can use the proximity parameter to
-provide the geocoder with a hint: ```python result = geocoder.geocode('London',
-proximity='42.828576, -81.406643') print(result[0]['formatted']) # u'London, ON
-N6A 3M8, Canada' ``` ### Reverse geocoding Turn a lat/long into an address with
-the ``reverse_geocode`` method: ```python results = geocoder.reverse_geocode
-(51.51024, -0.10303) ``` ### Sessions You can reuse your HTTP connection for
-multiple requests by using a `with` block. This can help performance when
-making a lot of requests: ```python queries = ['82 Clerkenwell Road, London',
-...] with OpenCageGeocode(key) as geocoder: # Queries reuse the same HTTP
-connection results = [geocoder.geocode(query) for query in queries] ``` ###
-Asycronous requests You can run requests in parallel with the `geocode_async`
-and `reverse_geocode_async` method which have the same parameters and response
-as their synronous counterparts. You will need at least Python 3.7 and the
-`asyncio` and `aiohttp` packages installed. ```python async with
-OpenCageGeocode(key) as geocoder: results = await geocoder.geocode_async
+python-opencage-geocoder) ![Mastodon Follow](https://img.shields.io/mastodon/
+follow/109287663468501769?domain=https%3A%2F%2Fen.osm.town%2F&style=social) ##
+Tutorial You can find a [comprehensive tutorial for using this module on the
+OpenCage site](https://opencagedata.com/tutorials/geocode-in-python). ## Usage
+Supports Python 3.7 or newer. Use the older opencage 1.x releases if you need
+Python 2.7 support. Install the module: ```bash pip install opencage ``` Load
+the module: ```python from opencage.geocoder import OpenCageGeocode ``` Create
+an instance of the geocoder module, passing a valid OpenCage Data Geocoder API
+key as a parameter to the geocoder modules's constructor: ```python key =
+'your-api-key-here' geocoder = OpenCageGeocode(key) ``` Pass a string
+containing the query or address to be geocoded to the modules' `geocode`
+method: ```python query = '82 Clerkenwell Road, London' results =
+geocoder.geocode(query) ``` You can add [additional parameters](https://
+opencagedata.com/api#forward-opt): ```python results = geocoder.geocode
+('London', no_annotations=1, language='es') ``` For example you can use the
+proximity parameter to provide the geocoder with a hint: ```python results =
+geocoder.geocode('London', proximity='42.828576, -81.406643') print(results[0]
+['formatted']) # u'London, ON N6A 3M8, Canada' ``` ### Reverse geocoding Turn a
+lat/long into an address with the ``reverse_geocode`` method: ```python result
+= geocoder.reverse_geocode(51.51024, -0.10303) ``` ### Sessions You can reuse
+your HTTP connection for multiple requests by using a `with` block. This can
+help performance when making a lot of requests: ```python queries = ['82
+Clerkenwell Road, London', ...] with OpenCageGeocode(key) as geocoder: #
+Queries reuse the same HTTP connection results = [geocoder.geocode(query) for
+query in queries] ``` ### Asyncronous requests You can run requests in parallel
+with the `geocode_async` and `reverse_geocode_async` method which have the same
+parameters and response as their synronous counterparts. You will need at least
+Python 3.7 and the `asyncio` and `aiohttp` packages installed. ```python async
+with OpenCageGeocode(key) as geocoder: results = await geocoder.geocode_async
 (address) ``` For a more complete example and links to futher tutorials on
-asycronous IO see `batch.py` in the `examples` directory. ### Exceptions If
-anything goes wrong, then an exception will be raised: * ``InvalidInputError``
-for non-unicode query strings * ``UnknownError`` if there's some problem with
-the API (bad results, 500 status code, etc) * ``RateLimitExceededError`` if you
-go past your rate limit ## Copyright & License This software is copyright
-OpenCage GmbH. Please see `LICENSE.txt` ### Who is OpenCage GmbH?
-[opencage_logo_300_150.png] We run a worldwide [geocoding API](https://
-opencagedata.com/api) and [geosearch](https://opencagedata.com/geosearch)
-service based on open data. Learn more [about us](https://opencagedata.com/
-about). We also run [Geomob](https://thegeomob.com), a series of regular
-meetups for location based service creators, where we do our best to highlight
-geoinnovation. If you like geo stuff, you will probably enjoy [the Geomob
-podcast](https://thegeomob.com/podcast/).
+asyncronous IO see `batch.py` in the `examples` directory. ### Exceptions If
+anything goes wrong, then an exception will be raised: * `InvalidInputError`
+for non-unicode query strings * `NotAuthorizedError` if API key is missing,
+invalid syntax or disabled * `ForbiddenError` API key is blocked or suspended *
+`RateLimitExceededError` if you go past your rate limit * `UnknownError` if
+there's some problem with the API (bad results, 500 status code, etc) ##
+Copyright & License This software is copyright OpenCage GmbH. Please see
+`LICENSE.txt` ### Who is OpenCage GmbH? [opencage_logo_300_150.png] We run a
+worldwide [geocoding API](https://opencagedata.com/api) and [geosearch](https:/
+/opencagedata.com/geosearch) service based on open data. Learn more [about us]
+(https://opencagedata.com/about). We also run [Geomob](https://thegeomob.com),
+a series of regular meetups for location based service creators, where we do
+our best to highlight geoinnovation. If you like geo stuff, you will probably
+enjoy [the Geomob podcast](https://thegeomob.com/podcast/).
```

### Comparing `opencage-2.1.0/opencage/geocoder.py` & `opencage-2.1.1/opencage/geocoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import os
 import requests
 import backoff
 
 try:
     import aiohttp
-    aiohttp_avaiable = True
+    AIOHTTP_AVAILABLE = True
 except ImportError:
-    aiohttp_avaiable = False
+    AIOHTTP_AVAILABLE = False
 
 def backoff_max_time():
     return int(os.environ.get('BACKOFF_MAX_TIME', '120'))
 
 class OpenCageGeocodeError(Exception):
 
     """Base class for all errors/exceptions that can happen when geocoding."""
@@ -58,15 +58,17 @@
         """Constructor."""
         super().__init__()
         self.reset_time = reset_time
         self.reset_to = reset_to
 
     def __unicode__(self):
         """Convert exception to a string."""
-        return "Your rate limit has expired. It will reset to {0} on {1}".format(self.reset_to, self.reset_time.isoformat())
+        return ("Your rate limit has expired. "
+                f"It will reset to {self.reset_to} on {self.reset_time.isoformat()}"
+                )
 
     __str__ = __unicode__
 
 
 class NotAuthorizedError(OpenCageGeocodeError):
 
     """
@@ -109,15 +111,15 @@
 
         >>> geocoder = OpenCageGeocode('your-key-here')
 
     Query:
 
         >>> geocoder.geocode("London")
 
-    Reverse geocode a latitude & longitude into a point:
+    Reverse geocode a latitude & longitude into a place:
 
         >>> geocoder.reverse_geocode(51.5104, -0.1021)
 
     """
 
     url = 'https://api.opencagedata.com/geocode/v1/json'
     key = ''
@@ -133,34 +135,35 @@
 
     def __exit__(self, *args):
         self.session.close()
         self.session = None
         return False
 
     async def __aenter__(self):
-        if not aiohttp_avaiable:
+        if not AIOHTTP_AVAILABLE:
             raise AioHttpError("You must install `aiohttp` to use async methods")
 
         self.session = aiohttp.ClientSession()
         return self
 
     async def __aexit__(self, *args):
         await self.session.close()
         self.session = None
         return False
 
     def geocode(self, query, **kwargs):
         """
-        Given a string to search for, return the results from OpenCage's Geocoder.
+        Given a string to search for, return the list (array) of results from OpenCage's Geocoder.
 
         :param string query: String to search for
 
         :returns: Dict results
         :raises InvalidInputError: if the query string is not a unicode string
-        :raises RateLimitExceededError: if you have exceeded the number of queries you can make. Exception says when you can try again
+        :raises RateLimitExceededError: if you have exceeded the number of queries you can make.
+        :                                  Exception says when you can try again
         :raises UnknownError: if something goes wrong with the OpenCage API
 
         """
 
         if self.session and isinstance(self.session, aiohttp.client.ClientSession):
             raise AioHttpError("Cannot use `geocode` in an async context, use `gecode_async`.")
 
@@ -169,26 +172,26 @@
 
         return floatify_latlng(response['results'])
 
     async def geocode_async(self, query, **kwargs):
         """
         Aync version of `geocode`.
 
-        Given a string to search for, return the results from OpenCage's Geocoder.
+        Given a string to search for, return the list (array) of results from OpenCage's Geocoder.
 
         :param string query: String to search for
 
         :returns: Dict results
         :raises InvalidInputError: if the query string is not a unicode string
-        :raises RateLimitExceededError: if you have exceeded the number of queries you can make. Exception says when you can try again
+        :raises RateLimitExceededError: if exceeded number of queries you can make. You can try again
         :raises UnknownError: if something goes wrong with the OpenCage API
 
         """
 
-        if not aiohttp_avaiable:
+        if not AIOHTTP_AVAILABLE:
             raise AioHttpError("You must install `aiohttp` to use async methods.")
 
         if not self.session:
             raise AioHttpError("Async methods must be used inside an async context.")
 
         if not isinstance(self.session, aiohttp.client.ClientSession):
             raise AioHttpError("You must use `geocode_async` in an async context.")
@@ -202,87 +205,94 @@
         """
         Given a latitude & longitude, return an address for that point from OpenCage's Geocoder.
 
         :param lat: Latitude
         :param lng: Longitude
         :return: Results from OpenCageData
         :rtype: dict
-        :raises RateLimitExceededError: if you have exceeded the number of queries you can make. Exception says when you can try again
+        :raises RateLimitExceededError: if you have exceeded the number of queries you can make.
+        :                                  Exception says when you can try again
         :raises UnknownError: if something goes wrong with the OpenCage API
         """
         return self.geocode(_query_for_reverse_geocoding(lat, lng), **kwargs)
 
     async def reverse_geocode_async(self, lat, lng, **kwargs):
         """
         Aync version of `reverse_geocode`.
 
         Given a latitude & longitude, return an address for that point from OpenCage's Geocoder.
 
         :param lat: Latitude
         :param lng: Longitude
         :return: Results from OpenCageData
         :rtype: dict
-        :raises RateLimitExceededError: if you have exceeded the number of queries you can make. Exception says when you can try again
+        :raises RateLimitExceededError: if exceeded number of queries you can make. You can try again
         :raises UnknownError: if something goes wrong with the OpenCage API
         """
         return await self.geocode_async(_query_for_reverse_geocoding(lat, lng), **kwargs)
 
     @backoff.on_exception(
         backoff.expo,
         (UnknownError, requests.exceptions.RequestException),
         max_tries=5, max_time=backoff_max_time)
     def _opencage_request(self, params):
 
         if self.session:
             response = self.session.get(self.url, params=params)
         else:
-            response = requests.get(self.url, params=params)
+            response = requests.get(self.url, params=params) # pylint: disable=missing-timeout
 
         try:
             response_json = response.json()
-        except ValueError as e:
-            raise UnknownError("Non-JSON result from server") from e
+        except ValueError as excinfo:
+            raise UnknownError("Non-JSON result from server") from excinfo
 
         if response.status_code == 401:
             raise NotAuthorizedError()
 
         if response.status_code == 403:
             raise ForbiddenError()
 
-        if (response.status_code == 402 or response.status_code == 429):
+        if response.status_code in (402, 429):
             # Rate limit exceeded
-            reset_time = datetime.utcfromtimestamp(response_json['rate']['reset'])
-            raise RateLimitExceededError(reset_to=int(response_json['rate']['limit']), reset_time=reset_time)
+            reset_time = datetime.utcfromtimestamp(response.json()['rate']['reset'])
+            raise RateLimitExceededError(
+                reset_to=int(response.json()['rate']['limit']),
+                reset_time=reset_time
+            )
 
         if response.status_code == 500:
             raise UnknownError("500 status code from API")
 
         if 'results' not in response_json:
             raise UnknownError("JSON from API doesn't have a 'results' key")
 
         return response_json
 
     async def _opencage_async_request(self, params):
         async with self.session.get(self.url, params=params) as response:
             try:
                 response_json = await response.json()
-            except ValueError as e:
-                raise UnknownError("Non-JSON result from server") from e
+            except ValueError as excinfo:
+                raise UnknownError("Non-JSON result from server") from excinfo
 
             if response.status == 401:
                 raise NotAuthorizedError()
 
             if response.status == 403:
                 raise ForbiddenError()
 
-            if (response.status == 402 or response.status == 429):
+            if response.status in (402, 429):
                 # Rate limit exceeded
                 print(response_json)
                 reset_time = datetime.utcfromtimestamp(response_json['rate']['reset'])
-                raise RateLimitExceededError(reset_to=int(response_json['rate']['limit']), reset_time=reset_time)
+                raise RateLimitExceededError(
+                    reset_to=int(response_json['rate']['limit']),
+                    reset_time=reset_time
+                )
 
             if response.status == 500:
                 raise UnknownError("500 status code from API")
 
             if 'results' not in response_json:
                 raise UnknownError("JSON from API doesn't have a 'results' key")
 
@@ -302,15 +312,15 @@
     Given a lat & lng, what's the string search query.
 
     If the API changes, change this function. Only for internal use.
     """
     # have to do some stupid f/Decimal/str stuff to (a) ensure we get as much
     # decimal places as the user already specified and (b) to ensure we don't
     # get e-5 stuff
-    return "{0:f},{1:f}".format(Decimal(str(lat)), Decimal(str(lng)))
+    return f"{Decimal(str(lat)):f},{Decimal(str(lng)):f}"
 
 
 def float_if_float(float_string):
     """
     Given a float string, returns the float value.
     On value error returns the original string.
     """
@@ -332,13 +342,14 @@
     If the API returns the lat/lng as strings, and not numbers, then this
     function will 'clean them up' to be floats.
     """
     if isinstance(input_value, collections.abc.Mapping):
         if len(input_value) == 2 and sorted(input_value.keys()) == ['lat', 'lng']:
             # This dict has only 2 keys 'lat' & 'lon'
             return {'lat': float_if_float(input_value["lat"]), 'lng': float_if_float(input_value["lng"])}
-        else:
-            return dict((key, floatify_latlng(value)) for key, value in input_value.items())
-    elif isinstance(input_value, collections.abc.MutableSequence):
+
+        return dict((key, floatify_latlng(value)) for key, value in input_value.items())
+
+    if isinstance(input_value, collections.abc.MutableSequence):
         return [floatify_latlng(x) for x in input_value]
-    else:
-        return input_value
+
+    return input_value
```

### Comparing `opencage-2.1.0/opencage.egg-info/PKG-INFO` & `opencage-2.1.1/opencage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: opencage
-Version: 2.1.0
+Version: 2.1.1
 Summary: Wrapper module for the OpenCage Geocoder API
 Home-page: https://github.com/OpenCageData/python-opencage-geocoder/
 Download-URL: https://github.com/OpenCageData/python-opencage-geocoder/tarball/2.1.0
 Author: OpenCage GmbH
 Author-email: info@opencagedata.com
 License: BSD
 Keywords: geocoding,geocoder
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # OpenCage Geocoding Module for Python
@@ -32,19 +32,23 @@
 ## Build Status / Code Quality / etc
 
 [![PyPI version](https://badge.fury.io/py/opencage.svg)](https://badge.fury.io/py/opencage)
 [![Downloads](https://pepy.tech/badge/opencage/month)](https://pepy.tech/project/opencage)
 [![Versions](https://img.shields.io/pypi/pyversions/opencage)](https://pypi.org/project/opencage/)
 ![GitHub contributors](https://img.shields.io/github/contributors/opencagedata/python-opencage-geocoder)
 [![Build Status](https://travis-ci.com/OpenCageData/python-opencage-geocoder.svg?branch=master)](https://travis-ci.com/OpenCageData/python-opencage-geocoder)
-[![Twitter Follow](https://img.shields.io/twitter/follow/OpenCage?label=Follow%20OpenCage&style=social)](https://twitter.com/opencage)
+![Mastodon Follow](https://img.shields.io/mastodon/follow/109287663468501769?domain=https%3A%2F%2Fen.osm.town%2F&style=social)
+
+## Tutorial
+
+You can find a [comprehensive tutorial for using this module on the OpenCage site](https://opencagedata.com/tutorials/geocode-in-python).
 
 ## Usage
 
-Supports Python 3.6 or newer. Use the older opencage 1.x releases if you need Python 2.7 support.
+Supports Python 3.7 or newer. Use the older opencage 1.x releases if you need Python 2.7 support.
 
 Install the module:
 
 ```bash
 pip install opencage
 ```
 
@@ -58,42 +62,42 @@
 as a parameter to the geocoder modules's constructor:
 
 ```python
 key = 'your-api-key-here'
 geocoder = OpenCageGeocode(key)
 ```
 
-Pass a string containing the query or address to be geocoded to the modules's `geocode` method:
+Pass a string containing the query or address to be geocoded to the modules' `geocode` method:
 
 ```python
-query = "82 Clerkenwell Road, London"
-result = geocoder.geocode(query)
+query = '82 Clerkenwell Road, London'
+results = geocoder.geocode(query)
 ```
 
-You can add [additional parameters](https://opencagedata.com/api#forward):
+You can add [additional parameters](https://opencagedata.com/api#forward-opt):
 
 ```python
-result = geocoder.geocode('London', no_annotations=1, language='es')
+results = geocoder.geocode('London', no_annotations=1, language='es')
 ```
 
-You can use the proximity parameter to provide the geocoder with a hint:
+For example you can use the proximity parameter to provide the geocoder with a hint:
 
 ```python
-result = geocoder.geocode('London', proximity='42.828576, -81.406643')
-print(result[0]['formatted'])
+results = geocoder.geocode('London', proximity='42.828576, -81.406643')
+print(results[0]['formatted'])
 # u'London, ON N6A 3M8, Canada'
 ```
 
 
 ### Reverse geocoding
 
 Turn a lat/long into an address with the ``reverse_geocode`` method:
 
 ```python
-results = geocoder.reverse_geocode(51.51024, -0.10303)
+result = geocoder.reverse_geocode(51.51024, -0.10303)
 ```
 
 ### Sessions
 
 You can reuse your HTTP connection for multiple requests by
 using a `with` block. This can help performance when making
 a lot of requests:
@@ -101,34 +105,37 @@
 ```python
 queries = ['82 Clerkenwell Road, London', ...]
 with OpenCageGeocode(key) as geocoder:
     # Queries reuse the same HTTP connection
     results = [geocoder.geocode(query) for query in queries]
 ```
 
-### Asycronous requests
+### Asyncronous requests
 
 You can run requests in parallel with the `geocode_async` and `reverse_geocode_async`
 method which have the same parameters and response as their synronous counterparts.
 You will need at least Python 3.7 and the `asyncio` and `aiohttp` packages installed.
 
 ```python
 async with OpenCageGeocode(key) as geocoder:
     results = await geocoder.geocode_async(address)
 ```
 
-For a more complete example and links to futher tutorials on asycronous IO see
+For a more complete example and links to futher tutorials on asyncronous IO see
 `batch.py` in the `examples` directory.
 
 ### Exceptions
 
 If anything goes wrong, then an exception will be raised:
- * ``InvalidInputError`` for non-unicode query strings
- * ``UnknownError`` if there's some problem with the API (bad results, 500 status code, etc)
- * ``RateLimitExceededError`` if you go past your rate limit
+
+ * `InvalidInputError` for non-unicode query strings
+ * `NotAuthorizedError` if API key is missing, invalid syntax or disabled
+ * `ForbiddenError` API key is blocked or suspended
+ * `RateLimitExceededError` if you go past your rate limit
+ * `UnknownError` if there's some problem with the API (bad results, 500 status code, etc)
 
 
 ## Copyright & License
 
 This software is copyright OpenCage GmbH.
 Please see `LICENSE.txt`
```

### Comparing `opencage-2.1.0/opencage.egg-info/SOURCES.txt` & `opencage-2.1.1/opencage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opencage-2.1.0/setup.py` & `opencage-2.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 if os.environ.get('USER', '') == 'vagrant':
     del os.link
 
 
 ROOT_DIR = os.path.dirname(__file__)
 SOURCE_DIR = os.path.join(ROOT_DIR)
 
-if sys.version_info < (3, 5):
+if sys.version_info < (3, 6):
     raise RuntimeError(
-        "opencage requires Python 3.6 or newer"
-        "Use older opencage 1.x for Python 2.7 or 3.5"
+        "opencage requires Python 3.7 or newer"
+        "Use older opencage 1.x for Python 2.7 or 3.6"
     )
 
 # try for travis
 try:
-    with open(os.path.join(SOURCE_DIR, 'README.md')) as f:
-        long_description = f.read()
+    with open(os.path.join(SOURCE_DIR, 'README.md'), encoding="utf-8") as f:
+        LONG_DESCRIPTION = f.read()
 except FileNotFoundError:
-    long_description = ""
+    LONG_DESCRIPTION = ""
 
 setup(
     name="opencage",
-    version="2.1.0",
+    version="2.1.1",
     description="Wrapper module for the OpenCage Geocoder API",
-    long_description=long_description,
+    long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author="OpenCage GmbH",
     author_email="info@opencagedata.com",
     url="https://github.com/OpenCageData/python-opencage-geocoder/",
     download_url="https://github.com/OpenCageData/python-opencage-geocoder/tarball/2.1.0",
     license="BSD",
     packages=find_packages(),
@@ -44,27 +44,27 @@
     classifiers=[
         'Environment :: Web Environment',
         "Development Status :: 5 - Production/Stable",
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         "Programming Language :: Python :: 3 :: Only",
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: GIS',
         'Topic :: Utilities'
     ],
     install_requires=[
         'Requests>=2.2.0',
         'pyopenssl>=0.15.1',
         'backoff>=1.10.0'
     ],
-    test_suite='tests',
+    test_suite='pytest',
     tests_require=[
         'httpretty>=0.9.6',
-        'pylint==2.9.1',
+        'pylint==2.15.9',
         'pytest>=6.0'
     ],
 )
```

### Comparing `opencage-2.1.0/test/test_all.py` & `opencage-2.1.1/test/test_all.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,56 +10,63 @@
 
 # reduce maximum backoff retry time from 120s to 1s
 os.environ['BACKOFF_MAX_TIME'] = '1'
 
 
 geocoder = OpenCageGeocode('abcde')
 
+def _any_result_around(results, lat=None, lon=None):
+    for result in results:
+        if (abs(result['geometry']['lat'] - lat) < 0.05 and
+            abs(result['geometry']['lng'] - lon) < 0.05):
+            return True
+    return False
+
 @httprettified
 def test_gb_postcode():
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
-        body=Path('test/fixtures/uk_postcode.json').read_text()
+        body=Path('test/fixtures/uk_postcode.json').read_text(encoding="utf-8")
     )
 
     results = geocoder.geocode("EC1M 5RF")
-    assert any((abs(result['geometry']['lat'] - 51.5201666) < 0.05 and abs(result['geometry']['lng'] - -0.0985142) < 0.05) for result in results)
+    assert _any_result_around(results, lat=51.5201666, lon=-0.0985142)
 
 
 @httprettified
 def test_australia():
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
-        body=Path('test/fixtures/mudgee_australia.json').read_text()
+        body=Path('test/fixtures/mudgee_australia.json').read_text(encoding="utf-8")
     )
 
     results = geocoder.geocode("Mudgee, Australia")
-    assert any((abs(result['geometry']['lat'] - -32.5980702) < 0.05 and abs(result['geometry']['lng'] - 149.5886383) < 0.05) for result in results)
+    assert _any_result_around(results, lat=-32.5980702, lon=149.5886383)
 
 
 @httprettified
-def testMunster():
+def test_munster():
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
-        body=Path('test/fixtures/muenster.json').read_text()
+        body=Path('test/fixtures/muenster.json').read_text(encoding="utf-8")
     )
 
     results = geocoder.geocode("Münster")
-    assert any((abs(result['geometry']['lat'] - 51.9625101) < 0.05 and abs(result['geometry']['lng'] - 7.6251879) < 0.05) for result in results)
+    assert _any_result_around(results, lat=51.9625101, lon=7.6251879)
 
 @httprettified
-def testDonostia():
+def test_donostia():
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
-        body=Path('test/fixtures/donostia.json').read_text()
+        body=Path('test/fixtures/donostia.json').read_text(encoding="utf-8")
 
     )
 
     results =geocoder.geocode("Donostia")
-    assert any((abs(result['geometry']['lat'] - 43.300836) < 0.05 and abs(result['geometry']['lng'] - -1.9809529) < 0.05) for result in results)
+    assert _any_result_around(results, lat=43.300836, lon=-1.9809529)
 
     # test that the results are in unicode
     assert results[0]['formatted'] == 'San Sebastián, Autonomous Community of the Basque Country, Spain'
```

### Comparing `opencage-2.1.0/test/test_async.py` & `opencage-2.1.1/test/test_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,41 @@
 
 import pytest
 
 from opencage.geocoder import ForbiddenError, OpenCageGeocode, AioHttpError
 
 # NOTE: Testing keys https://opencagedata.com/api#testingkeys
 
+@pytest.mark.asyncio
 async def test_success():
     async with OpenCageGeocode('6d0e711d72d74daeb2b0bfd2a5cdfdba') as geocoder:
         results = await geocoder.geocode_async("EC1M 5RF")
         assert any(
             abs(result['geometry']['lat'] - 51.952659 < 0.05 and
             abs(result['geometry']['lng'] - 7.632473) < 0.05)
             for result in results
         )
 
+@pytest.mark.asyncio
 async def test_failure():
     async with OpenCageGeocode('6c79ee8e1ca44ad58ad1fc493ba9542f') as geocoder:
         with pytest.raises(ForbiddenError) as excinfo:
             await geocoder.geocode_async("Atlantis")
 
         assert str(excinfo.value) == 'Your API key has been blocked or suspended.'
 
+@pytest.mark.asyncio
 async def test_without_async_session():
     geocoder = OpenCageGeocode('4372eff77b8343cebfc843eb4da4ddc4')
 
     with pytest.raises(AioHttpError) as excinfo:
         await geocoder.geocode_async("Atlantis")
 
     assert str(excinfo.value) == 'Async methods must be used inside an async context.'
 
+@pytest.mark.asyncio
 async def test_using_non_async_method():
     async with OpenCageGeocode('6d0e711d72d74daeb2b0bfd2a5cdfdba') as geocoder:
         with pytest.raises(AioHttpError) as excinfo:
             await geocoder.geocode("Atlantis")
 
     assert str(excinfo.value) == 'Cannot use `geocode` in an async context, use `gecode_async`.'
```

### Comparing `opencage-2.1.0/test/test_error_blocked.py` & `opencage-2.1.1/test/test_error_blocked.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 geocoder = OpenCageGeocode('2e10e5e828262eb243ec0b54681d699a') # will always return 403
 
 @httprettified
 def test_api_key_blocked():
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
-        body=Path('test/fixtures/403_apikey_disabled.json').read_text(),
+        body=Path('test/fixtures/403_apikey_disabled.json').read_text(encoding="utf-8"),
         status=403,
     )
 
     with pytest.raises(ForbiddenError) as excinfo:
         geocoder.geocode("whatever")
     assert str(excinfo.value) == 'Your API key has been blocked or suspended.'
```

### Comparing `opencage-2.1.0/test/test_error_invalid_input.py` & `opencage-2.1.1/test/test_error_invalid_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 
     # But if it isn't a unicode string, it should give error
     utf8_string = "xxá".encode("utf-8")
     latin1_string = "xxá".encode("latin1")
 
     with pytest.raises(InvalidInputError) as excinfo:
         geocoder.geocode(utf8_string)
-    assert str(excinfo.value) == "Input must be a unicode string, not {0!r}".format(utf8_string)
+    assert str(excinfo.value) == f"Input must be a unicode string, not {utf8_string!r}"
     assert excinfo.value.bad_value == utf8_string
 
     with pytest.raises(InvalidInputError) as excinfo:
         geocoder.geocode(latin1_string)
-    assert str(excinfo.value) == "Input must be a unicode string, not {0!r}".format(latin1_string)
+    assert str(excinfo.value) == f"Input must be a unicode string, not {latin1_string!r}"
     assert excinfo.value.bad_value == latin1_string
```

### Comparing `opencage-2.1.0/test/test_error_not_authorized.py` & `opencage-2.1.1/test/test_error_not_authorized.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 geocoder = OpenCageGeocode('unauthorized-key')
 
 @httprettified
 def test_api_key_not_authorized():
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
-        body=Path('test/fixtures/401_not_authorized.json').read_text(),
+        body=Path('test/fixtures/401_not_authorized.json').read_text(encoding="utf-8"),
         status=401,
     )
 
     with pytest.raises(NotAuthorizedError) as excinfo:
         geocoder.geocode("whatever")
     assert str(excinfo.value) == 'Your API key is not authorized. You may have entered it incorrectly.'
```

### Comparing `opencage-2.1.0/test/test_error_ratelimit_exceeded.py` & `opencage-2.1.1/test/test_error_ratelimit_exceeded.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,33 @@
 geocoder = OpenCageGeocode('abcde')
 
 @httprettified
 def test_no_rate_limit():
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
-        body=Path('test/fixtures/no_ratelimit.json').read_text()
+        body=Path('test/fixtures/no_ratelimit.json').read_text(encoding="utf-8")
     )
     # shouldn't raise an exception
     geocoder.geocode("whatever")
 
 
 @httprettified
 def test_rate_limit_exceeded():
     # 4372eff77b8343cebfc843eb4da4ddc4 will always return 402
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
-        body=Path('test/fixtures/402_rate_limit_exceeded.json').read_text(),
+        body=Path('test/fixtures/402_rate_limit_exceeded.json').read_text(encoding="utf-8"),
         status=402,
-        adding_headers={'X-RateLimit-Limit': '2500', 'X-RateLimit-Remaining': '0', 'X-RateLimit-Reset': '1402185600'},
+        adding_headers={
+            'X-RateLimit-Limit': '2500',
+            'X-RateLimit-Remaining': '0',
+            'X-RateLimit-Reset': '1402185600'
+        }
     )
 
     with pytest.raises(RateLimitExceededError) as excinfo:
         geocoder.geocode("whatever")
     assert str(excinfo.value) == 'Your rate limit has expired. It will reset to 2500 on 2021-03-08T00:00:00'
     assert excinfo.value.reset_to == 2500
     assert excinfo.value.reset_time == datetime.datetime(2021, 3, 8, 0, 0)
```

### Comparing `opencage-2.1.0/test/test_error_unknown.py` & `opencage-2.1.1/test/test_error_unknown.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 def test_http_500_status():
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
         status=500,
     )
 
-    with pytest.raises(UnknownError) as e:
+    with pytest.raises(UnknownError) as excinfo:
         geocoder.geocode('whatever')
 
-    assert str(e.value) == '500 status code from API'
+    assert str(excinfo.value) == '500 status code from API'
 
 @httprettified
 def test_non_json():
     "These kinds of errors come from webserver and may not be JSON"
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
         body='<html><body><h1>503 Service Unavailable</h1></body></html>',
         forcing_headers={
             'Content-Type': 'text/html',
         },
         status=503
     )
 
-    with pytest.raises(UnknownError) as e:
+    with pytest.raises(UnknownError) as excinfo:
         geocoder.geocode('whatever')
 
-    assert str(e.value) == 'Non-JSON result from server'
+    assert str(excinfo.value) == 'Non-JSON result from server'
 
 @httprettified
 def test_no_results_key():
     httpretty.register_uri(
         httpretty.GET,
         geocoder.url,
         body='{"spam": "eggs"}',
     )
 
-    with pytest.raises(UnknownError) as e:
+    with pytest.raises(UnknownError) as excinfo:
         geocoder.geocode('whatever')
 
-    assert str(e.value) == "JSON from API doesn't have a 'results' key"
+    assert str(excinfo.value) == "JSON from API doesn't have a 'results' key"
```

### Comparing `opencage-2.1.0/test/test_flotify_dict.py` & `opencage-2.1.1/test/test_flotify_dict.py`

 * *Files identical despite different names*

### Comparing `opencage-2.1.0/test/test_reverse.py` & `opencage-2.1.1/test/test_reverse.py`

 * *Files identical despite different names*

### Comparing `opencage-2.1.0/test/test_session.py` & `opencage-2.1.1/test/test_session.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,33 +5,39 @@
 import httpretty
 import pytest
 
 from httpretty import httprettified
 from opencage.geocoder import OpenCageGeocode
 from opencage.geocoder import NotAuthorizedError
 
+def _any_result_around(results, lat=None, lon=None):
+    for result in results:
+        if (abs(result['geometry']['lat'] - lat) < 0.05 and
+            abs(result['geometry']['lng'] - lon) < 0.05):
+            return True
+    return False
 
 @httprettified
 def test_success():
     with OpenCageGeocode('abcde') as geocoder:
         httpretty.register_uri(
             httpretty.GET,
             geocoder.url,
-            body=Path('test/fixtures/uk_postcode.json').read_text()
+            body=Path('test/fixtures/uk_postcode.json').read_text(encoding="utf-8")
         )
 
         results = geocoder.geocode("EC1M 5RF")
-        assert any((abs(result['geometry']['lat'] - 51.5201666) < 0.05 and abs(result['geometry']['lng'] - -0.0985142) < 0.05) for result in results)
+        assert _any_result_around(results, lat=51.5201666, lon=-0.0985142)
 
 @httprettified
 def test_failure():
     with OpenCageGeocode('unauthorized-key') as geocoder:
         httpretty.register_uri(
             httpretty.GET,
             geocoder.url,
-            body=Path('test/fixtures/401_not_authorized.json').read_text(),
+            body=Path('test/fixtures/401_not_authorized.json').read_text(encoding="utf-8"),
             status=401,
         )
 
         with pytest.raises(NotAuthorizedError) as excinfo:
             geocoder.geocode("whatever")
         assert str(excinfo.value) == 'Your API key is not authorized. You may have entered it incorrectly.'
```

