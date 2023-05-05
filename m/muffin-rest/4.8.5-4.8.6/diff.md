# Comparing `tmp/muffin_rest-4.8.5.tar.gz` & `tmp/muffin_rest-4.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-4.8.5.tar", max compression
+gzip compressed data, was "muffin_rest-4.8.6.tar", max compression
```

## Comparing `muffin_rest-4.8.5.tar` & `muffin_rest-4.8.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1082 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/LICENSE
--rw-r--r--   0        0        0     2616 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/README.rst
--rw-r--r--   0        0        0     1242 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/errors.py
--rw-r--r--   0        0        0     5187 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/filters.py
--rw-r--r--   0        0        0    10377 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/handler.py
--rw-r--r--   0        0        0     4842 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8808 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/options.py
--rw-r--r--   0        0        0     5372 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2418 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     1111 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     2270 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0        0 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2515 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6397 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     4058 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/swagger.html
--rw-r--r--   0        0        0      455 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/types.py
--rw-r--r--   0        0        0     2113 2023-05-05 05:25:13.036401 muffin_rest-4.8.5/muffin_rest/utils.py
--rw-r--r--   0        0        0     2670 2023-05-05 05:25:13.040401 muffin_rest-4.8.5/pyproject.toml
--rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 muffin_rest-4.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/LICENSE
+-rw-r--r--   0        0        0     2616 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/README.rst
+-rw-r--r--   0        0        0     1242 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5187 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10377 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4842 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-05-05 05:29:29.487872 muffin_rest-4.8.6/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8808 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/options.py
+-rw-r--r--   0        0        0     5372 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2418 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     1111 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1076 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     2270 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0        0 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2515 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6397 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2460 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     4058 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      455 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/types.py
+-rw-r--r--   0        0        0     2113 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2670 2023-05-05 05:29:29.491874 muffin_rest-4.8.6/pyproject.toml
+-rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 muffin_rest-4.8.6/PKG-INFO
```

### Comparing `muffin_rest-4.8.5/LICENSE` & `muffin_rest-4.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/README.rst` & `muffin_rest-4.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/__init__.py` & `muffin_rest-4.8.6/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/api.py` & `muffin_rest-4.8.6/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/errors.py` & `muffin_rest-4.8.6/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/filters.py` & `muffin_rest-4.8.6/muffin_rest/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/handler.py` & `muffin_rest-4.8.6/muffin_rest/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/mongo/__init__.py` & `muffin_rest-4.8.6/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/mongo/filters.py` & `muffin_rest-4.8.6/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/mongo/schema.py` & `muffin_rest-4.8.6/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/mongo/sorting.py` & `muffin_rest-4.8.6/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/mongo/utils.py` & `muffin_rest-4.8.6/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/openapi.py` & `muffin_rest-4.8.6/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/options.py` & `muffin_rest-4.8.6/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/peewee/__init__.py` & `muffin_rest-4.8.6/muffin_rest/peewee/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/peewee/filters.py` & `muffin_rest-4.8.6/muffin_rest/peewee/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/peewee/openapi.py` & `muffin_rest-4.8.6/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/peewee/options.py` & `muffin_rest-4.8.6/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/peewee/schemas.py` & `muffin_rest-4.8.6/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/peewee/sorting.py` & `muffin_rest-4.8.6/muffin_rest/peewee/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/redoc.html` & `muffin_rest-4.8.6/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/sorting.py` & `muffin_rest-4.8.6/muffin_rest/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-4.8.6/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-4.8.6/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-4.8.6/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/swagger.html` & `muffin_rest-4.8.6/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/muffin_rest/utils.py` & `muffin_rest-4.8.6/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.5/pyproject.toml` & `muffin_rest-4.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "4.8.5"
+version = "4.8.6"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-4.8.5/PKG-INFO` & `muffin_rest-4.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 4.8.5
+Version: 4.8.6
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

