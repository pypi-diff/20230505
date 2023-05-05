# Comparing `tmp/gwdatafind-server-1.2.1.tar.gz` & `tmp/gwdatafind-server-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdatafind-server-1.2.1.tar", last modified: Wed Apr 12 18:21:20 2023, max compression
+gzip compressed data, was "gwdatafind-server-1.2.2.tar", last modified: Fri May  5 16:41:57 2023, max compression
```

## Comparing `gwdatafind-server-1.2.1.tar` & `gwdatafind-server-1.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.120871 gwdatafind-server-1.2.1/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    35149 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/LICENSE
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      175 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/MANIFEST.in
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-04-12 18:21:20.120871 gwdatafind-server-1.2.1/PKG-INFO
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      627 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/README.md
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/config/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      691 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/gunicorn.conf
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6737 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/gunicorn.conf.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2174 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/gwdatafind-server.ini
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      386 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/gwdatafind-server.service
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      698 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/wsgi.conf
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/debian/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2079 2023-04-12 17:49:45.000000 gwdatafind-server-1.2.1/debian/changelog
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        2 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/compat
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1446 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/control
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1048 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/copyright
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/gwdatafind-server.docs
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      212 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/gwdatafind-server.install
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/python3-gwdatafind-server.docs
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       30 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/python3-gwdatafind-server.install
--rwxrwxr-x   0 duncan    (1001) duncan    (1001)       82 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/rules
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/debian/source/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       12 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/source/format
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/gwdatafind_server/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      543 2023-04-12 17:49:45.000000 gwdatafind-server-1.2.1/gwdatafind_server/__init__.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/gwdatafind_server/api/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      200 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/api/__init__.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      669 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/api/base.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1914 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/api/utils.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    11084 2023-04-11 18:10:54.000000 gwdatafind-server-1.2.1/gwdatafind_server/api/v1.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4223 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/app.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4894 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/authentication.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     8011 2023-04-06 20:05:11.000000 gwdatafind-server-1.2.1/gwdatafind_server/cache.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      974 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/config.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/PKG-INFO
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1158 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/SOURCES.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        1 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/dependency_links.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/requires.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       18 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/top_level.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      727 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/pyproject.toml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4806 2023-04-12 17:49:45.000000 gwdatafind-server-1.2.1/python-gwdatafind-server.spec
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1475 2023-04-12 18:21:20.120871 gwdatafind-server-1.2.1/setup.cfg
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      196 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/setup.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.120871 gwdatafind-server-1.2.1/tests/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      702 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/cache.dat
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      369 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/conftest.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/grid-mapfile
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      546 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/gwdatafind-server.ini
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4722 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_api_v1.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      335 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_app.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2518 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_authentication_scitokens.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1505 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_authentication_x509.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      790 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_config.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      480 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/utils.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)    35149 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/LICENSE
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      175 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/MANIFEST.in
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/PKG-INFO
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      627 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/README.md
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.394240 gwdatafind-server-1.2.2/config/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      691 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/gunicorn.conf
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     6737 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/gunicorn.conf.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2174 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/gwdatafind-server.ini
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      386 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/gwdatafind-server.service
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      698 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/wsgi.conf
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.394240 gwdatafind-server-1.2.2/debian/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2294 2023-05-05 16:33:14.000000 gwdatafind-server-1.2.2/debian/changelog
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)        2 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/compat
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1446 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/control
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1048 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/copyright
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/gwdatafind-server.docs
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      212 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/gwdatafind-server.install
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/python3-gwdatafind-server.docs
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       30 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/python3-gwdatafind-server.install
+-rwxrwxr-x   0 duncan    (1001) duncan    (1001)       82 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/rules
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.394240 gwdatafind-server-1.2.2/debian/source/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       12 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/source/format
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.394240 gwdatafind-server-1.2.2/gwdatafind_server/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      543 2023-05-05 16:33:14.000000 gwdatafind-server-1.2.2/gwdatafind_server/__init__.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/gwdatafind_server/api/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      200 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/api/__init__.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      669 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/api/base.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1914 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/api/utils.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)    10881 2023-05-05 16:10:07.000000 gwdatafind-server-1.2.2/gwdatafind_server/api/v1.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     4223 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/app.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     4894 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/authentication.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     8011 2023-04-06 20:05:11.000000 gwdatafind-server-1.2.2/gwdatafind_server/cache.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      974 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/config.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/PKG-INFO
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1158 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)        1 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/requires.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       18 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/top_level.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      727 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/pyproject.toml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     4955 2023-05-05 16:33:14.000000 gwdatafind-server-1.2.2/python-gwdatafind-server.spec
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1475 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/setup.cfg
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      196 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/setup.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/tests/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      702 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/cache.dat
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      369 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/conftest.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/grid-mapfile
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      546 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/gwdatafind-server.ini
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     5654 2023-05-05 16:10:07.000000 gwdatafind-server-1.2.2/tests/test_api_v1.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      335 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/test_app.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2518 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/test_authentication_scitokens.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1505 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/test_authentication_x509.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      790 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/test_config.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      480 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/utils.py
```

### Comparing `gwdatafind-server-1.2.1/LICENSE` & `gwdatafind-server-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/PKG-INFO` & `gwdatafind-server-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdatafind-server
-Version: 1.2.1
+Version: 1.2.2
 Summary: The server library for the GWDataFind service
 Home-page: https://git.ligo.org/computing/gwdatafind/server
 Author: Duncan Meacher
 Author-email: duncan.meacher@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://git.ligo.org/computing/gwdatafind/server/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/gwdatafind/server/
```

### Comparing `gwdatafind-server-1.2.1/README.md` & `gwdatafind-server-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/config/gunicorn.conf` & `gwdatafind-server-1.2.2/config/gunicorn.conf`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/config/gunicorn.conf.py` & `gwdatafind-server-1.2.2/config/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/config/gwdatafind-server.ini` & `gwdatafind-server-1.2.2/config/gwdatafind-server.ini`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/config/wsgi.conf` & `gwdatafind-server-1.2.2/config/wsgi.conf`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/debian/changelog` & `gwdatafind-server-1.2.2/debian/changelog`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+gwdatafind-server (1.2.2-1) stable; urgency=low
+
+  * Fixed bug in single file queries
+  * Fixed bug in search for fractional GPS times
+
+ -- Duncan Meacher <duncan.meacher@ligo.org>  Fri, 05 May 2023 00:00:00 +0100
+
 gwdatafind-server (1.2.1-1) stable; urgency=low
 
   * Added comment handling in cache file
   * Updated default SciToken issue and scope
   * Added ability to search for fractional GPS times
 
  -- Duncan Meacher <duncan.meacher@ligo.org>  Fri, 07 Apr 2023 00:00:00 +0100
```

### Comparing `gwdatafind-server-1.2.1/debian/control` & `gwdatafind-server-1.2.2/debian/control`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/debian/copyright` & `gwdatafind-server-1.2.2/debian/copyright`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server/__init__.py` & `gwdatafind-server-1.2.2/gwdatafind_server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 data discover mechanism for data files.
 
 Users provide a few key details as part of an HTTP(S)
 query and receive URLs that indicate the locations
 of the relevant data.
 """
 
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 
 from .app import GWDataFindApp
 from .config import get_config_path
 
 
 def create_app():
     """Create an instance of the application
```

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server/api/base.py` & `gwdatafind-server-1.2.2/gwdatafind_server/api/base.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server/api/utils.py` & `gwdatafind-server-1.2.2/gwdatafind_server/api/utils.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server/api/v1.py` & `gwdatafind-server-1.2.2/gwdatafind_server/api/v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -195,31 +195,30 @@
 @handle_errors_as_json
 @authentication.validate
 def find_url(ext, site, tag, filename):
     """Return URL(s) for a given filename
     """
     # parse GPS information from filename
     _, _, start, dur = filename.split('-')
-    dur = dur[:-len(ext)].rstrip('.')
+    dur = float(dur[:-len(ext)].rstrip('.'))
+    start = float(start)
+    end = start + dur
     # find urls
     return list(_find_urls(
         ext,
         site,
         tag,
-        int(start),
-        int(start + dur),
+        start,
+        end,
     ))
 
 
-@blueprint.route('<ext>/<site>/<tag>/<int:start>,<int:end>')  # for --ping
-@blueprint.route('<ext>/<site>/<tag>/<int:start>,<int:end>.json')
-@blueprint.route('<ext>/<site>/<tag>/<int:start>,<int:end>/<urltype>.json')
-@blueprint.route('<ext>/<site>/<tag>/<float:start>,<float:end>')  # for --ping
-@blueprint.route('<ext>/<site>/<tag>/<float:start>,<float:end>.json')
-@blueprint.route('<ext>/<site>/<tag>/<float:start>,<float:end>/<urltype>.json')
+@blueprint.route('<ext>/<site>/<tag>/<start>,<end>')  # for --ping
+@blueprint.route('<ext>/<site>/<tag>/<start>,<end>.json')
+@blueprint.route('<ext>/<site>/<tag>/<start>,<end>/<urltype>.json')
 @handle_errors_as_json
 @authentication.validate
 def find_urls(ext, site, tag, start, end, urltype=None):
     """Find all URLs in a given GPS time interval
     """
     return list(_find_urls(
         ext,
@@ -263,15 +262,15 @@
 def _find_urls(ext, site, tag, start, end, urltype=None, match=None,
                latest=False):
     """Find all URLs for the given GPS interval
     """
     cache = get_dataset_cache(ext, site, tag)
 
     # parse file paths
-    search = segment(start, end)
+    search = segment(float(start), float(end))
     lfns = defaultdict(list)
     maxgps = -1e9  # something absurdly old
     for (path, cdur), seglist in cache.items():
         # if running a 'latest' URL search, restrict the search to
         # the most recent available segment for this frametype
         if latest and seglist:  # 'if seglist' to prevent IndexError
             # get latest segment for this path
```

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server/app.py` & `gwdatafind-server-1.2.2/gwdatafind_server/app.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server/authentication.py` & `gwdatafind-server-1.2.2/gwdatafind_server/authentication.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server/cache.py` & `gwdatafind-server-1.2.2/gwdatafind_server/cache.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server/config.py` & `gwdatafind-server-1.2.2/gwdatafind_server/config.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server.egg-info/PKG-INFO` & `gwdatafind-server-1.2.2/gwdatafind_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdatafind-server
-Version: 1.2.1
+Version: 1.2.2
 Summary: The server library for the GWDataFind service
 Home-page: https://git.ligo.org/computing/gwdatafind/server
 Author: Duncan Meacher
 Author-email: duncan.meacher@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://git.ligo.org/computing/gwdatafind/server/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/gwdatafind/server/
```

### Comparing `gwdatafind-server-1.2.1/gwdatafind_server.egg-info/SOURCES.txt` & `gwdatafind-server-1.2.2/gwdatafind_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/pyproject.toml` & `gwdatafind-server-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/python-gwdatafind-server.spec` & `gwdatafind-server-1.2.2/python-gwdatafind-server.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define srcname gwdatafind-server
-%define version 1.2.1
+%define version 1.2.2
 %define release 1
 
 Name:      python-%{srcname}
 Version:   %{version}
 Release:   %{release}%{?dist}
 Summary:   The server app for the GWDataFind service
 License:   GPLv3+
@@ -124,14 +124,17 @@
 %license LICENSE
 %{_datadir}/%{srcname}/
 %{_unitdir}/%{srcname}.service
 
 # -- changelog
 
 %changelog
+* Fri May 05 2023 Duncan Meacher <duncan.meacher@ligo.org> 1.2.2-1
+- Fixed bug in single file queries
+- Fixed bug in search for fractional GPS times
 * Fri Apr 07 2023 Duncan Meacher <duncan.meacher@ligo.org> 1.2.1-1
 - Added comment handling in cache file
 - Updated default SciToken issue and scope
 - Added ability to search for fractional GPS times
 * Thu Apr 21 2022 Duncan Meacher <duncan.meacher@ligo.org> 1.2.0-1
 - Added full SciToken authentication support
 - Updated README to point to documentation pages
```

### Comparing `gwdatafind-server-1.2.1/setup.cfg` & `gwdatafind-server-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/tests/cache.dat` & `gwdatafind-server-1.2.2/tests/cache.dat`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/tests/gwdatafind-server.ini` & `gwdatafind-server-1.2.2/tests/gwdatafind-server.ini`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/tests/test_api_v1.py` & `gwdatafind-server-1.2.2/tests/test_api_v1.py`

 * *Files 13% similar despite different names*

```diff
@@ -77,20 +77,20 @@
 
 @mock.patch.object(api_utils, "_DEFAULT_GSIFTP_HOST", new="testhost")
 def test_find_url(client):
     """Test the `find_url` view
     """
     resp = client.get(
         "/services/data/v1"
-        "/h5/L/L1_TEST_1/L-L1_TEST_1-1000000004-4.h5.json",
+        "/h5/L/L1_TEST_1/L-L1_TEST_1-1000000000-4.h5.json",
     )
     assert resp.status_code == 200
     assert resp.json == [
-        "file://localhost/test/path/L-L1_TEST_1-1000000004-4.h5",
-        "gsiftp://testhost:15000/test/path/L-L1_TEST_1-1000000004-4.h5",
+        "file://localhost/test/path/L-L1_TEST_1-1000000000-4.h5",
+        "gsiftp://testhost:15000/test/path/L-L1_TEST_1-1000000000-4.h5",
     ]
 
 
 @mock.patch.object(api_utils, "_DEFAULT_GSIFTP_HOST", new="testhost")
 def test_find_urls(client):
     """Test the `find_urls` view with no special options
     """
@@ -129,14 +129,37 @@
     assert resp.status_code == 200
     assert sorted(resp.json) == [
         "file://localhost/test/preferred/path/H-H1_TEST_1-1000000000-8.h5",
     ]
 
 
 @mock.patch.object(api_utils, "_DEFAULT_GSIFTP_HOST", new="testhost")
+@pytest.mark.parametrize(("start", "end"), [
+    (1000000003.5, 1000000012.5),
+    (1000000003, 1000000012.5),
+    (1000000003.5, 1000000013),
+])
+def test_find_urls_noninteger(client, start, end):
+    """Test the `find_urls` view with non-integer GPS times.
+    """
+    resp = client.get(
+        f"/services/data/v1/gwf/L/L1_TEST_1/{start},{end}.json",
+    )
+    assert resp.status_code == 200
+    assert sorted(resp.json) == [
+        "file://localhost/test/path/L-L1_TEST_1-1000000000-4.gwf",
+        "file://localhost/test/path/L-L1_TEST_1-1000000004-4.gwf",
+        "file://localhost/test/path2/L-L1_TEST_1-1000000012-4.gwf",
+        "gsiftp://testhost:15000/test/path/L-L1_TEST_1-1000000000-4.gwf",
+        "gsiftp://testhost:15000/test/path/L-L1_TEST_1-1000000004-4.gwf",
+        "gsiftp://testhost:15000/test/path2/L-L1_TEST_1-1000000012-4.gwf",
+    ]
+
+
+@mock.patch.object(api_utils, "_DEFAULT_GSIFTP_HOST", new="testhost")
 def test_find_latest(client):
     """Test the `find_latest` view
     """
     resp = client.get(
         "/services/data/v1/gwf/L/L1_TEST_1/latest.json",
     )
     assert resp.status_code == 200
```

### Comparing `gwdatafind-server-1.2.1/tests/test_authentication_scitokens.py` & `gwdatafind-server-1.2.2/tests/test_authentication_scitokens.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/tests/test_authentication_x509.py` & `gwdatafind-server-1.2.2/tests/test_authentication_x509.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.1/tests/test_config.py` & `gwdatafind-server-1.2.2/tests/test_config.py`

 * *Files identical despite different names*

