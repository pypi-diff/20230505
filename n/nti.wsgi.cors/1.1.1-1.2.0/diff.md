# Comparing `tmp/nti.wsgi.cors-1.1.1.tar.gz` & `tmp/nti.wsgi.cors-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nti.wsgi.cors-1.1.1.tar", last modified: Tue Apr 20 14:34:29 2021, max compression
+gzip compressed data, was "nti.wsgi.cors-1.2.0.tar", last modified: Fri May  5 18:23:02 2023, max compression
```

## Comparing `nti.wsgi.cors-1.1.1.tar` & `nti.wsgi.cors-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,48 @@
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-04-20 14:34:29.219737 nti.wsgi.cors-1.1.1/
--rw-r--r--   0 jmadden    (501) staff       (20)      528 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/.coveragerc
--rw-r--r--   0 jmadden    (501) staff       (20)       14 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/.nti_cover_package
--rw-r--r--   0 jmadden    (501) staff       (20)       85 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/AUTHORS
--rw-r--r--   0 jmadden    (501) staff       (20)      368 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/CHANGES.rst
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/INSTALL
--rw-r--r--   0 jmadden    (501) staff       (20)      594 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/LICENSE
--rw-r--r--   0 jmadden    (501) staff       (20)      364 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/MANIFEST.in
--rw-r--r--   0 jmadden    (501) staff       (20)     1973 2021-04-20 14:34:29.219888 nti.wsgi.cors-1.1.1/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)      427 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/README.rst
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/TODO
--rw-r--r--   0 jmadden    (501) staff       (20)      366 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/babel.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)      168 2021-04-20 14:34:29.220367 nti.wsgi.cors-1.1.1/setup.cfg
--rwxr-xr-x   0 jmadden    (501) staff       (20)     1958 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/setup.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-04-20 14:34:29.210242 nti.wsgi.cors-1.1.1/src/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-04-20 14:34:29.215427 nti.wsgi.cors-1.1.1/src/nti/
--rw-r--r--   0 jmadden    (501) staff       (20)       75 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/src/nti/__init__.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-04-20 14:34:29.218181 nti.wsgi.cors-1.1.1/src/nti/wsgi/
--rw-r--r--   0 jmadden    (501) staff       (20)       75 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/src/nti/wsgi/__init__.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-04-20 14:34:29.218854 nti.wsgi.cors-1.1.1/src/nti/wsgi/cors/
--rw-r--r--   0 jmadden    (501) staff       (20)      320 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/src/nti/wsgi/cors/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     9227 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/src/nti/wsgi/cors/cors.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-04-20 14:34:29.219486 nti.wsgi.cors-1.1.1/src/nti/wsgi/cors/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)     1002 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/src/nti/wsgi/cors/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2234 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/src/nti/wsgi/cors/tests/test_cors.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-04-20 14:34:29.217899 nti.wsgi.cors-1.1.1/src/nti.wsgi.cors.egg-info/
--rw-r--r--   0 jmadden    (501) staff       (20)     1973 2021-04-20 14:34:29.000000 nti.wsgi.cors-1.1.1/src/nti.wsgi.cors.egg-info/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)      651 2021-04-20 14:34:29.000000 nti.wsgi.cors-1.1.1/src/nti.wsgi.cors.egg-info/SOURCES.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2021-04-20 14:34:29.000000 nti.wsgi.cors-1.1.1/src/nti.wsgi.cors.egg-info/dependency_links.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      125 2021-04-20 14:34:29.000000 nti.wsgi.cors-1.1.1/src/nti.wsgi.cors.egg-info/entry_points.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2021-04-20 14:34:29.000000 nti.wsgi.cors-1.1.1/src/nti.wsgi.cors.egg-info/namespace_packages.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      220 2021-04-20 14:34:29.000000 nti.wsgi.cors-1.1.1/src/nti.wsgi.cors.egg-info/requires.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2021-04-20 14:34:29.000000 nti.wsgi.cors-1.1.1/src/nti.wsgi.cors.egg-info/top_level.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2021-04-20 14:34:29.000000 nti.wsgi.cors-1.1.1/src/nti.wsgi.cors.egg-info/zip-safe
--rw-r--r--   0 jmadden    (501) staff       (20)      227 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/tox.ini
--rw-r--r--   0 jmadden    (501) staff       (20)        6 2021-04-20 14:34:28.000000 nti.wsgi.cors-1.1.1/version.txt
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.287869 nti.wsgi.cors-1.2.0/
+-rw-r--r--   0 jmadden    (501) staff       (20)      528 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/.coveragerc
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.283172 nti.wsgi.cors-1.2.0/.github/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.285804 nti.wsgi.cors-1.2.0/.github/workflows/
+-rw-r--r--   0 jmadden    (501) staff       (20)     1905 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)      353 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/.gitignore
+-rw-r--r--   0 jmadden    (501) staff       (20)       14 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/.nti_cover_package
+-rw-r--r--   0 jmadden    (501) staff       (20)     8996 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/.pylintrc
+-rw-r--r--   0 jmadden    (501) staff       (20)      845 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/.readthedocs.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)       85 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/AUTHORS
+-rw-r--r--   0 jmadden    (501) staff       (20)      449 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/CHANGES.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       73 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/COPYRIGHT.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/INSTALL
+-rw-r--r--   0 jmadden    (501) staff       (20)      529 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/LICENSE
+-rw-r--r--   0 jmadden    (501) staff       (20)      411 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/MANIFEST.in
+-rw-r--r--   0 jmadden    (501) staff       (20)     2152 2023-05-05 18:23:02.287932 nti.wsgi.cors-1.2.0/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)      581 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/README.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/TODO
+-rw-r--r--   0 jmadden    (501) staff       (20)      366 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/babel.cfg
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.286242 nti.wsgi.cors-1.2.0/docs/
+-rw-r--r--   0 jmadden    (501) staff       (20)     7610 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/docs/Makefile
+-rw-r--r--   0 jmadden    (501) staff       (20)      267 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/docs/api.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     4547 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/docs/conf.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      207 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/docs/index.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)      168 2023-05-05 18:23:02.288147 nti.wsgi.cors-1.2.0/setup.cfg
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     2234 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/setup.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.283439 nti.wsgi.cors-1.2.0/src/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.286338 nti.wsgi.cors-1.2.0/src/nti/
+-rw-r--r--   0 jmadden    (501) staff       (20)       75 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/src/nti/__init__.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.287340 nti.wsgi.cors-1.2.0/src/nti/wsgi/
+-rw-r--r--   0 jmadden    (501) staff       (20)       75 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/src/nti/wsgi/__init__.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.287541 nti.wsgi.cors-1.2.0/src/nti/wsgi/cors/
+-rw-r--r--   0 jmadden    (501) staff       (20)      377 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/src/nti/wsgi/cors/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     9249 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/src/nti/wsgi/cors/cors.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.287742 nti.wsgi.cors-1.2.0/src/nti/wsgi/cors/tests/
+-rw-r--r--   0 jmadden    (501) staff       (20)      963 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/src/nti/wsgi/cors/tests/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     2234 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/src/nti/wsgi/cors/tests/test_cors.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 18:23:02.287226 nti.wsgi.cors-1.2.0/src/nti.wsgi.cors.egg-info/
+-rw-r--r--   0 jmadden    (501) staff       (20)     2152 2023-05-05 18:23:02.000000 nti.wsgi.cors-1.2.0/src/nti.wsgi.cors.egg-info/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)      786 2023-05-05 18:23:02.000000 nti.wsgi.cors-1.2.0/src/nti.wsgi.cors.egg-info/SOURCES.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-05-05 18:23:02.000000 nti.wsgi.cors-1.2.0/src/nti.wsgi.cors.egg-info/dependency_links.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)      124 2023-05-05 18:23:02.000000 nti.wsgi.cors-1.2.0/src/nti.wsgi.cors.egg-info/entry_points.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2023-05-05 18:23:02.000000 nti.wsgi.cors-1.2.0/src/nti.wsgi.cors.egg-info/namespace_packages.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)      288 2023-05-05 18:23:02.000000 nti.wsgi.cors-1.2.0/src/nti.wsgi.cors.egg-info/requires.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2023-05-05 18:23:02.000000 nti.wsgi.cors-1.2.0/src/nti.wsgi.cors.egg-info/top_level.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-05-05 18:23:02.000000 nti.wsgi.cors-1.2.0/src/nti.wsgi.cors.egg-info/zip-safe
+-rw-r--r--   0 jmadden    (501) staff       (20)     1167 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/tox.ini
+-rw-r--r--   0 jmadden    (501) staff       (20)        6 2023-05-05 18:23:01.000000 nti.wsgi.cors-1.2.0/version.txt
```

### Comparing `nti.wsgi.cors-1.1.1/.coveragerc` & `nti.wsgi.cors-1.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `nti.wsgi.cors-1.1.1/LICENSE` & `nti.wsgi.cors-1.2.0/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-Copyright (c) 2011-2013 NextThought, LLC
-
- Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this software except in compliance with the License.
-   You may obtain a copy of the License at
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this software except in compliance with the License.
+You may obtain a copy of the License at
 
      http://www.apache.org/licenses/LICENSE-2.0
 
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `nti.wsgi.cors-1.1.1/setup.py` & `nti.wsgi.cors-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,27 +25,31 @@
 setup(
     name='nti.wsgi.cors',
     version=_read('version.txt').strip(),
     author='Jason Madden',
     author_email='jason@nextthought.com',
     description="Support for CORS in a WSGI environment",
     long_description=(_read('README.rst') + '\n\n' + _read('CHANGES.rst')),
-    url="https://github.com/NextThought/nti.wsgi.cors",
+    url="https://github.com/OpenNTI/nti.wsgi.cors",
     license='Apache',
     keywords='wsgi cors',
     classifiers=[
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Operating System :: OS Independent',
+        'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     zip_safe=True,
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
@@ -56,13 +60,14 @@
         'greenlet ; platform_python_implementation=="CPython"'
     ],
     extras_require={
         'test': TESTS_REQUIRE,
         'docs':  [
             'Sphinx',
             'repoze.sphinx.autointerface',
-            'sphinx_rtd_theme',
+            'furo; python_version >= "3.6"',
+            'sphinx_rtd_theme; python_version < "3.6"',
         ] + TESTS_REQUIRE,
     },
     entry_points=entry_points,
     test_suite="nti.wsgi.cors.tests",
 )
```

### Comparing `nti.wsgi.cors-1.1.1/src/nti/wsgi/cors/cors.py` & `nti.wsgi.cors-1.2.0/src/nti/wsgi/cors/cors.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,29 +19,33 @@
 #: Exceptions we will ignore for middleware purposes
 import greenlet
 
 #: The exceptions in this list will be considered expected
 #: and not create error reports from Paste. Instead, Paste
 #: will raise them, and they will be caught here. Paste will
 #: catch everything else.
+#:
 #: .. todo:: We need to move this to its own middleware.
 EXPECTED_EXCEPTIONS = (
     # During restarts this can be generated
     greenlet.GreenletExit,
     # As can this, more commonly the more we use non-blocking IO
     SystemExit,
-    # Most commonly (almost only) seen buffering request bodies. May have some false negatives, though.
-    # Also seen when a umysqldb connection fails; hard to determine when that can be retryable; this
-    # is one of those false-negatives
+    # Most commonly (almost only) seen buffering request bodies. May
+    # have some false negatives, though. Also seen when a umysqldb
+    # connection fails; hard to determine when that can be retryable;
+    # this is one of those false-negatives
     IOError,
 )
 
 # Previously this contained:
-# transaction.interfaces.DoomedTransaction, # This should never get here with the transaction middleware in place
-# pyramid.httpexceptions.HTTPException, # Pyramid is beneath us, so this
+# transaction.interfaces.DoomedTransaction,
+# This should never get here with the transaction middleware in place
+# pyramid.httpexceptions.HTTPException,
+# Pyramid is beneath us, so this
 # should never get here either
 
 try:
     # If we can get ZODB, lets also treat as expected
     # some of its exceptions. These aren't actually
     # "expected", in the sense that they are still errors
     # and need to be dealt with. Instead, they are "expected"
@@ -126,15 +130,15 @@
 
     def __init__(self, app):
         self._app = app
 
     def __call__(self, environ, start_response):
         # Support CORS
         if 'HTTP_ORIGIN' in environ:
-            start_response = self._CORSInjectingStartResponse(environ,start_response)
+            start_response = self._CORSInjectingStartResponse(environ, start_response)
 
         result = None
         environ.setdefault(
             'paste.expected_exceptions',
             []).extend(EXPECTED_EXCEPTIONS)
         try:
             result = self._app(environ, start_response)
@@ -142,16 +146,17 @@
             # We don't do anything fancy, just log and continue
             logger.exception("Failed to handle request")
             result = (('Failed to handle request ' + str(e)).encode("utf-8"),)
             start_response('500 Internal Server Error',
                            [('Content-Type', 'text/plain')],
                            sys.exc_info())
 
-        # Everything else we allow to propagate. This might kill the gunicorn worker and cause it to respawn
-        # If so, it will be printed on stderr and captured by supervisor
+        # Everything else we allow to propagate. This might kill the
+        # gunicorn worker and cause it to respawn If so, it will be
+        # printed on stderr and captured by supervisor
 
         return result
 
     class _CORSInjectingStartResponse(object):
         """
         A callable object that wraps a start_response callable to inject
         CORS headers.
@@ -202,15 +207,15 @@
                     'Access-Control-Allow-Headers'] = ', '.join(ACCES_CONTROL_HEADERS)
                 theHeaders[
                     'Access-Control-Expose-Headers'] = 'Location, Warning'
 
             return self._start_response(status, headers, exc_info)
 
 
-def cors_filter_factory(app, global_conf=None):
+def cors_filter_factory(app, _global_conf=None):
     """
     Paste filter factory to include :class:`CORSInjector`
     """
     return CORSInjector(app)
 
 
 class CORSOptionHandler(object):
@@ -235,12 +240,12 @@
         if environ['REQUEST_METHOD'] == 'OPTIONS':
             start_response('200 OK', [('Content-Type', 'text/plain')])
             return (b'',)
 
         return self._app(environ, start_response)
 
 
-def cors_option_filter_factory(app, global_conf=None):
+def cors_option_filter_factory(app, _global_conf=None):
     """
     Paste filter factory to include :class:`CORSOptionHandler`
     """
     return CORSOptionHandler(app)
```

### Comparing `nti.wsgi.cors-1.1.1/src/nti/wsgi/cors/tests/__init__.py` & `nti.wsgi.cors-1.2.0/src/nti/wsgi/cors/tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __docformat__ = "restructuredtext en"
 
 # disable: accessing protected members, too many methods
 # pylint: disable=W0212,R0904
 
 from zope.component.hooks import setHooks
 
-from nti.testing.layers import find_test
+
 from nti.testing.layers import GCLayerMixin
 from nti.testing.layers import ZopeComponentLayer
 from nti.testing.layers import ConfiguringLayerMixin
 
 import zope.testing.cleanup
 
 
@@ -28,13 +28,13 @@
 
     @classmethod
     def tearDown(cls):
         cls.tearDownPackages()
         zope.testing.cleanup.cleanUp()
 
     @classmethod
-    def testSetUp(cls, test=None):
+    def testSetUp(cls, _test=None):
         setHooks()
 
     @classmethod
     def testTearDown(cls):
         pass
```

### Comparing `nti.wsgi.cors-1.1.1/src/nti/wsgi/cors/tests/test_cors.py` & `nti.wsgi.cors-1.2.0/src/nti/wsgi/cors/tests/test_cors.py`

 * *Files identical despite different names*

