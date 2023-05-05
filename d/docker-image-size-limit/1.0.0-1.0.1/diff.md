# Comparing `tmp/docker_image_size_limit-1.0.0.tar.gz` & `tmp/docker_image_size_limit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_image_size_limit-1.0.0.tar", max compression
+gzip compressed data, was "docker_image_size_limit-1.0.1.tar", max compression
```

## Comparing `docker_image_size_limit-1.0.0.tar` & `docker_image_size_limit-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-05-03 09:06:13.344278 docker_image_size_limit-1.0.0/LICENSE
--rw-r--r--   0        0        0     3778 2023-05-03 09:06:13.344565 docker_image_size_limit-1.0.0/README.md
--rw-r--r--   0        0        0     1984 2023-05-03 09:06:13.345310 docker_image_size_limit-1.0.0/docker_image_size_limit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 09:06:13.345443 docker_image_size_limit-1.0.0/docker_image_size_limit/py.typed
--rw-r--r--   0        0        0      194 2023-05-03 09:38:19.523655 docker_image_size_limit-1.0.0/docker_image_size_limit/version.py
--rw-r--r--   0        0        0     1353 2023-05-03 09:38:19.526617 docker_image_size_limit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4980 1970-01-01 00:00:00.000000 docker_image_size_limit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-05 07:32:38.588645 docker_image_size_limit-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3778 2023-05-05 07:32:38.588843 docker_image_size_limit-1.0.1/README.md
+-rw-r--r--   0        0        0     1984 2023-05-05 07:32:38.589291 docker_image_size_limit-1.0.1/docker_image_size_limit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:32:38.589412 docker_image_size_limit-1.0.1/docker_image_size_limit/py.typed
+-rw-r--r--   0        0        0      194 2023-05-05 07:32:38.589544 docker_image_size_limit-1.0.1/docker_image_size_limit/version.py
+-rw-r--r--   0        0        0     1387 2023-05-05 07:32:38.590775 docker_image_size_limit-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 docker_image_size_limit-1.0.1/PKG-INFO
```

### Comparing `docker_image_size_limit-1.0.0/LICENSE` & `docker_image_size_limit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_image_size_limit-1.0.0/README.md` & `docker_image_size_limit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `docker_image_size_limit-1.0.0/docker_image_size_limit/__init__.py` & `docker_image_size_limit-1.0.1/docker_image_size_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `docker_image_size_limit-1.0.0/pyproject.toml` & `docker_image_size_limit-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-image-size-limit"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 license = "MIT"
 authors = [
   "Nikita Sobolev <mail@sobolevn.me>"
 ]
 
 readme = "README.md"
@@ -35,14 +35,16 @@
 disl = "docker_image_size_limit:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 docker = ">=3.7,<7.0"
 humanfriendly = ">=4.18,<11.0"
+urllib3 = "<2"
+requests = "<2.29"
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.0"
 pytest-randomly = "^3.12"
 pytest-timeout = "^1.4"
 pytest = "^7.3"
```

### Comparing `docker_image_size_limit-1.0.0/PKG-INFO` & `docker_image_size_limit-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-image-size-limit
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Home-page: https://github.com/wemake-services/docker-image-size-limit
 License: MIT
 Keywords: docker,docker image,size limit,wemake.services,code quality
 Author: Nikita Sobolev
 Author-email: mail@sobolevn.me
 Requires-Python: >=3.8,<4.0
@@ -18,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: docker (>=3.7,<7.0)
 Requires-Dist: humanfriendly (>=4.18,<11.0)
+Requires-Dist: requests (<2.29)
+Requires-Dist: urllib3 (<2)
 Project-URL: Funding, https://github.com/sponsors/wemake-services
 Project-URL: Repository, https://github.com/wemake-services/docker-image-size-limit
 Description-Content-Type: text/markdown
 
 # docker-image-size-limit
 
 [![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)
```

