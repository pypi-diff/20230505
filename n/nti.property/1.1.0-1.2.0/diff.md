# Comparing `tmp/nti.property-1.1.0.tar.gz` & `tmp/nti.property-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nti.property-1.1.0.tar", last modified: Thu Sep 13 11:52:23 2018, max compression
+gzip compressed data, was "nti.property-1.2.0.tar", last modified: Fri May  5 15:48:55 2023, max compression
```

## Comparing `nti.property-1.1.0.tar` & `nti.property-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,53 @@
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2018-09-13 11:52:23.000000 nti.property-1.1.0/
--rw-r--r--   0 jmadden    (501) staff       (20)     1898 2018-09-13 11:52:23.000000 nti.property-1.1.0/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)      271 2018-09-13 11:52:22.000000 nti.property-1.1.0/nose2.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2018-09-13 11:52:22.000000 nti.property-1.1.0/INSTALL
--rw-r--r--   0 jmadden    (501) staff       (20)      593 2018-09-13 11:52:22.000000 nti.property-1.1.0/LICENSE
--rw-r--r--   0 jmadden    (501) staff       (20)      125 2018-09-13 11:52:22.000000 nti.property-1.1.0/AUTHORS
--rw-r--r--   0 jmadden    (501) staff       (20)      364 2018-09-13 11:52:22.000000 nti.property-1.1.0/MANIFEST.in
--rw-r--r--   0 jmadden    (501) staff       (20)       13 2018-09-13 11:52:22.000000 nti.property-1.1.0/.nti_cover_package
--rw-r--r--   0 jmadden    (501) staff       (20)      391 2018-09-13 11:52:22.000000 nti.property-1.1.0/.coveragerc
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2018-09-13 11:52:22.000000 nti.property-1.1.0/TODO
--rwxr-xr-x   0 jmadden    (501) staff       (20)     1813 2018-09-13 11:52:22.000000 nti.property-1.1.0/setup.py
--rw-r--r--   0 jmadden    (501) staff       (20)      516 2018-09-13 11:52:22.000000 nti.property-1.1.0/tox.ini
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2018-09-13 11:52:23.000000 nti.property-1.1.0/doc/
--rw-r--r--   0 jmadden    (501) staff       (20)      225 2018-09-13 11:52:22.000000 nti.property-1.1.0/doc/index.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     7610 2018-09-13 11:52:22.000000 nti.property-1.1.0/doc/Makefile
--rw-r--r--   0 jmadden    (501) staff       (20)    10775 2018-09-13 11:52:22.000000 nti.property-1.1.0/doc/conf.py
--rw-r--r--   0 jmadden    (501) staff       (20)      586 2018-09-13 11:52:22.000000 nti.property-1.1.0/doc/api.rst
--rw-r--r--   0 jmadden    (501) staff       (20)      166 2018-09-13 11:52:23.000000 nti.property-1.1.0/setup.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)      146 2018-09-13 11:52:22.000000 nti.property-1.1.0/babel.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)      529 2018-09-13 11:52:22.000000 nti.property-1.1.0/README.rst
--rw-r--r--   0 jmadden    (501) staff       (20)        6 2018-09-13 11:52:22.000000 nti.property-1.1.0/version.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      270 2018-09-13 11:52:22.000000 nti.property-1.1.0/CHANGES.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       75 2018-09-13 11:52:22.000000 nti.property-1.1.0/doc-requirements.txt
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti.property.egg-info/
--rw-r--r--   0 jmadden    (501) staff       (20)     1898 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti.property.egg-info/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti.property.egg-info/zip-safe
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti.property.egg-info/namespace_packages.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      911 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti.property.egg-info/SOURCES.txt
--rw-r--r--   0 jmadden    (501) staff       (20)       20 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti.property.egg-info/entry_points.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      212 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti.property.egg-info/requires.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti.property.egg-info/top_level.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti.property.egg-info/dependency_links.txt
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti/property/
--rw-r--r--   0 jmadden    (501) staff       (20)     4672 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/property.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2018-09-13 11:52:23.000000 nti.property-1.1.0/src/nti/property/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)      228 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     4850 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/tests/test_property.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1249 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/tests/test_schema.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3488 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/tests/test_urlproperty.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1886 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/tests/test_dataurl.py
--rw-r--r--   0 jmadden    (501) staff       (20)      159 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     6229 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/urlproperty.py
--rw-r--r--   0 jmadden    (501) staff       (20)     4544 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/dataurl.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1001 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/property/schema.py
--rw-r--r--   0 jmadden    (501) staff       (20)       75 2018-09-13 11:52:22.000000 nti.property-1.1.0/src/nti/__init__.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.895282 nti.property-1.2.0/
+-rw-r--r--   0 jmadden    (501) staff       (20)      391 2023-05-05 15:48:55.000000 nti.property-1.2.0/.coveragerc
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.890119 nti.property-1.2.0/.github/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.892865 nti.property-1.2.0/.github/workflows/
+-rw-r--r--   0 jmadden    (501) staff       (20)     1905 2023-05-05 15:48:55.000000 nti.property-1.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)      353 2023-05-05 15:48:55.000000 nti.property-1.2.0/.gitignore
+-rw-r--r--   0 jmadden    (501) staff       (20)       13 2023-05-05 15:48:55.000000 nti.property-1.2.0/.nti_cover_package
+-rw-r--r--   0 jmadden    (501) staff       (20)     8996 2023-05-05 15:48:55.000000 nti.property-1.2.0/.pylintrc
+-rw-r--r--   0 jmadden    (501) staff       (20)      529 2023-05-05 15:48:55.000000 nti.property-1.2.0/.travis.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)      125 2023-05-05 15:48:55.000000 nti.property-1.2.0/AUTHORS
+-rw-r--r--   0 jmadden    (501) staff       (20)      361 2023-05-05 15:48:55.000000 nti.property-1.2.0/CHANGES.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       73 2023-05-05 15:48:55.000000 nti.property-1.2.0/COPYRIGHT.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.000000 nti.property-1.2.0/INSTALL
+-rw-r--r--   0 jmadden    (501) staff       (20)      529 2023-05-05 15:48:55.000000 nti.property-1.2.0/LICENSE
+-rw-r--r--   0 jmadden    (501) staff       (20)      386 2023-05-05 15:48:55.000000 nti.property-1.2.0/MANIFEST.in
+-rw-r--r--   0 jmadden    (501) staff       (20)     2171 2023-05-05 15:48:55.895344 nti.property-1.2.0/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)      717 2023-05-05 15:48:55.000000 nti.property-1.2.0/README.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.000000 nti.property-1.2.0/TODO
+-rw-r--r--   0 jmadden    (501) staff       (20)      146 2023-05-05 15:48:55.000000 nti.property-1.2.0/babel.cfg
+-rw-r--r--   0 jmadden    (501) staff       (20)       75 2023-05-05 15:48:55.000000 nti.property-1.2.0/doc-requirements.txt
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.893270 nti.property-1.2.0/docs/
+-rw-r--r--   0 jmadden    (501) staff       (20)     7610 2023-05-05 15:48:55.000000 nti.property-1.2.0/docs/Makefile
+-rw-r--r--   0 jmadden    (501) staff       (20)      586 2023-05-05 15:48:55.000000 nti.property-1.2.0/docs/api.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     4546 2023-05-05 15:48:55.000000 nti.property-1.2.0/docs/conf.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      225 2023-05-05 15:48:55.000000 nti.property-1.2.0/docs/index.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)      271 2023-05-05 15:48:55.000000 nti.property-1.2.0/nose2.cfg
+-rw-r--r--   0 jmadden    (501) staff       (20)      166 2023-05-05 15:48:55.895564 nti.property-1.2.0/setup.cfg
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     2140 2023-05-05 15:48:55.000000 nti.property-1.2.0/setup.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.890372 nti.property-1.2.0/src/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.893363 nti.property-1.2.0/src/nti/
+-rw-r--r--   0 jmadden    (501) staff       (20)       75 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/__init__.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.894638 nti.property-1.2.0/src/nti/property/
+-rw-r--r--   0 jmadden    (501) staff       (20)      185 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     4553 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/dataurl.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     4680 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/property.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1001 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/schema.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.895169 nti.property-1.2.0/src/nti/property/tests/
+-rw-r--r--   0 jmadden    (501) staff       (20)      228 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/tests/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1933 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/tests/test_dataurl.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     5408 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/tests/test_property.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1264 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/tests/test_schema.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3545 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/tests/test_urlproperty.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     6281 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti/property/urlproperty.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 15:48:55.894072 nti.property-1.2.0/src/nti.property.egg-info/
+-rw-r--r--   0 jmadden    (501) staff       (20)     2171 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti.property.egg-info/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)      947 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti.property.egg-info/SOURCES.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti.property.egg-info/dependency_links.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti.property.egg-info/namespace_packages.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)      280 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti.property.egg-info/requires.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti.property.egg-info/top_level.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-05-05 15:48:55.000000 nti.property-1.2.0/src/nti.property.egg-info/zip-safe
+-rw-r--r--   0 jmadden    (501) staff       (20)     1166 2023-05-05 15:48:55.000000 nti.property-1.2.0/tox.ini
+-rw-r--r--   0 jmadden    (501) staff       (20)        6 2023-05-05 15:48:55.000000 nti.property-1.2.0/version.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nti.property-1.1.0/LICENSE` & `nti.property-1.2.0/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-Copyright (c) 2011-2017 NextThought, LLC
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
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `nti.property-1.1.0/setup.py` & `nti.property-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,26 +19,31 @@
 setup(
     name='nti.property',
     version=_read('version.txt').strip(),
     author='Jason Madden',
     author_email='jason@nextthought.com',
     description="NTI Property",
     long_description=(_read('README.rst') + '\n\n' + _read("CHANGES.rst")),
-    url="https://github.com/NextThought/nti.property",
+    url="https://github.com/OpenNTI/nti.property",
     license='Apache',
     keywords='Property',
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
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
     ],
     zip_safe=True,
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
@@ -53,13 +58,15 @@
         'zope.schema >= 4.7.0',
     ],
     extras_require={
         'test': TESTS_REQUIRE,
         'docs': [
             'Sphinx',
             'repoze.sphinx.autointerface',
-            'sphinx_rtd_theme'
+            'furo; python_version >= "3.6"',
+            'sphinx_rtd_theme; python_version < "3.6"',
+
         ],
     },
     entry_points=entry_points,
     test_suite="nti.property.tests",
 )
```

### Comparing `nti.property-1.1.0/doc/Makefile` & `nti.property-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nti.property-1.1.0/doc/api.rst` & `nti.property-1.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `nti.property-1.1.0/src/nti.property.egg-info/SOURCES.txt` & `nti.property-1.2.0/src/nti.property.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 .coveragerc
+.gitignore
 .nti_cover_package
+.pylintrc
+.travis.yml
 AUTHORS
 CHANGES.rst
+COPYRIGHT.txt
 INSTALL
 LICENSE
 MANIFEST.in
 README.rst
 TODO
 babel.cfg
 doc-requirements.txt
 nose2.cfg
 setup.cfg
 setup.py
 tox.ini
 version.txt
-doc/Makefile
-doc/api.rst
-doc/conf.py
-doc/index.rst
+.github/workflows/tests.yml
+docs/Makefile
+docs/api.rst
+docs/conf.py
+docs/index.rst
 src/nti/__init__.py
 src/nti.property.egg-info/PKG-INFO
 src/nti.property.egg-info/SOURCES.txt
 src/nti.property.egg-info/dependency_links.txt
-src/nti.property.egg-info/entry_points.txt
 src/nti.property.egg-info/namespace_packages.txt
 src/nti.property.egg-info/requires.txt
 src/nti.property.egg-info/top_level.txt
 src/nti.property.egg-info/zip-safe
 src/nti/property/__init__.py
 src/nti/property/dataurl.py
 src/nti/property/property.py
```

### Comparing `nti.property-1.1.0/src/nti/property/property.py` & `nti.property-1.2.0/src/nti/property/property.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,25 +117,33 @@
             of the object that will be adapted to IAnnotations. Most often this will
             be ``context`` when used inside an adapter.
     """
 
     if doc is None:
         doc = 'Alias for annotation ' + annotation_name
 
-    factory = IAnnotations
+
     if annotation_property:
-        factory = lambda self: IAnnotations(getattr(self, annotation_property))
+        def factory(self):
+            return IAnnotations(getattr(self, annotation_property))
+    else:
+        factory = IAnnotations
+
+    def fget(self):
+        # pylint:disable-next=too-many-function-args
+        return factory(self).get(annotation_name, default)
+
+    def fset(self, nv):
+        factory(self)[annotation_name] = nv
+
 
-    fget = lambda self: factory(self).get(annotation_name, default)
-    fset = lambda self, nv: operator.setitem(factory(self),
-                                             annotation_name,
-                                             nv)
-    fdel = None
     if delete:
         def fdel(self):
             try:
                 del factory(self)[annotation_name]
             except KeyError:
                 if not delete_quiet:
                     raise
+    else:
+        fdel = None
 
     return property(fget, fset, fdel, doc=doc)
```

### Comparing `nti.property-1.1.0/src/nti/property/tests/test_property.py` & `nti.property-1.2.0/src/nti/property/tests/test_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,16 +143,14 @@
         del x.the_alias
         assert_that(x, has_property('the_alias', 1))
 
         # quiet re-del
         del x.the_alias
         assert_that(x, has_property('the_alias', 1))
 
-        class Y(dict):
-            pass
 
         # Annotation based on a property, that can't be deleted
         # quietly
         @interface.implementer(an_interfaces.IAnnotations)
         class Z(dict):
 
             the_alias = annotation_alias('the.key',
@@ -169,14 +167,31 @@
         del z.the_alias
         assert_that(z, has_property('the_alias', 1))
 
         with self.assertRaises(KeyError):
             del z.the_alias
         assert_that(z, has_property('the_alias', 1))
 
+        # Annotation that can't be
+        # deleted at all
+        @interface.implementer(an_interfaces.IAnnotations)
+        class ZZ(dict):
+            the_alias = annotation_alias('the.key',
+                                         delete=False,
+                                         default=1)
+
+            def __init__(self):
+                self.context = X()
+
+        z = ZZ()
+        z['the.key'] = 42
+        assert_that(z, has_property('the_alias', 42))
+        with self.assertRaises(AttributeError):
+            del z.the_alias
+        assert_that(z, has_property('the_alias', 42))
 
     def test_lazy_on_class(self):
 
         class X(dict):
 
             @LazyOnClass
             def _foo(self):
```

### Comparing `nti.property-1.1.0/src/nti/property/tests/test_schema.py` & `nti.property-1.2.0/src/nti/property/tests/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 from hamcrest import same_instance
 from hamcrest import has_property
 
 from nti.property.schema import DataURI
 
 from zope.schema.interfaces import InvalidURI
 
-GIF_DATAURL = 'data:image/gif;base64,R0lGODlhCwALAIAAAAAA3pn/ZiH5BAEAAAEALAAAAAALAAsAAAIUhA+hkcuO4lmNVindo7qyrIXiGBYAOw=='
+GIF_DATAURL = (
+    'data:image/gif;base64,'
+    'R0lGODlhCwALAIAAAAAA3pn/ZiH5BAEAAAEALAAAAAALAAsAAAIUhA+hkcuO4lmNVindo7qyrIXiGBYAOw=='
+)
 
 
 class TestSchema(unittest.TestCase):
 
     def test_data_url_class(self):
         value = DataURI.is_valid_data_uri(GIF_DATAURL)
         assert_that(value, is_(True))
```

### Comparing `nti.property-1.1.0/src/nti/property/tests/test_urlproperty.py` & `nti.property-1.2.0/src/nti/property/tests/test_urlproperty.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 from zope.schema.interfaces import InvalidURI
 from zope.schema.interfaces import ConstraintNotSatisfied
 
 
 from nti.property.urlproperty import UrlProperty
 
 
-GIF_DATAURL = 'data:image/gif;base64,R0lGODlhCwALAIAAAAAA3pn/ZiH5BAEAAAEALAAAAAALAAsAAAIUhA+hkcuO4lmNVindo7qyrIXiGBYAOw=='
+GIF_DATAURL = (
+    'data:image/gif;base64,'
+    'R0lGODlhCwALAIAAAAAA3pn/ZiH5BAEAAAEALAAAAAALAAsAAAIUhA+hkcuO4lmNVindo7qyrIXiGBYAOw=='
+)
+
+# pylint:disable=unnecessary-dunder-call
 
 class TestURLProperty(unittest.TestCase):
 
     def test_getitem(self):
         prop = UrlProperty()
         getter = prop.make_getitem()
         with self.assertRaises(KeyError):
```

### Comparing `nti.property-1.1.0/src/nti/property/tests/test_dataurl.py` & `nti.property-1.2.0/src/nti/property/tests/test_dataurl.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,24 @@
 from hamcrest import has_property
 
 from nti.property.dataurl import encode
 from nti.property.dataurl import decode
 from nti.property.dataurl import DataURL
 
 
-GIF_DATAURL = 'data:image/gif;base64,R0lGODlhCwALAIAAAAAA3pn/ZiH5BAEAAAEALAAAAAALAAsAAAIUhA+hkcuO4lmNVindo7qyrIXiGBYAOw=='
-GIF_DATA = b'GIF89a\x0b\x00\x0b\x00\x80\x00\x00\x00\x00\xde\x99\xfff!\xf9\x04\x01\x00\x00\x01\x00,\x00\x00\x00\x00\x0b\x00\x0b\x00\x00\x02\x14\x84\x0f\xa1\x91\xcb\x8e\xe2Y\x8dV)\xdd\xa3\xba\xb2\xac\x85\xe2\x18\x16\x00;'
+GIF_DATAURL = (
+    'data:image/gif;base64,'
+    'R0lGODlhCwALAIAAAAAA3pn/ZiH5BAEAAAEALAAAAAALAAsAAAIUhA+hkcuO4lmNVindo7qyrIXiGBYAOw=='
+)
+GIF_DATA = (
+    b'GIF89a\x0b\x00\x0b\x00\x80\x00\x00\x00\x00\xde\x99\xfff!'
+    b'\xf9\x04\x01\x00\x00\x01\x00,\x00\x00\x00\x00\x0b\x00\x0b'
+    b'\x00\x00\x02\x14\x84\x0f\xa1\x91\xcb\x8e\xe2Y\x8dV)\xdd'
+    b'\xa3\xba\xb2\xac\x85\xe2\x18\x16\x00;'
+)
 
 class TestDataURL(unittest.TestCase):
 
     def test_data_url_class(self):
         url = DataURL(GIF_DATAURL)
         assert_that(url, has_property('mimeType', 'image/gif'))
         assert_that(url, has_property('data', is_not(none())))
```

### Comparing `nti.property-1.1.0/src/nti/property/urlproperty.py` & `nti.property-1.2.0/src/nti/property/urlproperty.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,16 @@
 
     def get_file(self, instance):
         """
         Return the :class:`zope.file.interfaces.IFile` for the instance
         if there is one, otherwise None.
         """
         the_file = self._getattr(instance, self.file_attr_name, None)
-        if IFile.providedBy(the_file):
-            return the_file
+        # pylint:disable-next=no-value-for-parameter
+        return (the_file if IFile.providedBy(the_file) else None)
 
     def __get__(self, instance, owner):
         if instance is None:
             return self
 
         the_file = self.get_file(instance)
         if the_file is not None:
```

### Comparing `nti.property-1.1.0/src/nti/property/dataurl.py` & `nti.property-1.2.0/src/nti/property/dataurl.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
 
 def decode(data_url):
     """
     Decodes a data URL into raw bytes and metadata.
 
     :param data_url: The data url string.
-            If a mime-type definition is missing in the metadata,
-            ``text/plain;charset=US-ASCII`` will be used as default mime-type.
+       If a mime-type definition is missing in the metadata,
+       ``text/plain;charset=US-ASCII`` will be used as default mime-type.
     :returns: A 2-tuple: ``(bytes, mime_type_string)``
-            The mime_type string will not be parsed. See :func:`zope.contenttype.parse.parse` for that.
+       The mime_type string will not be parsed. See :func:`zope.contenttype.parse.parse` for that.
     """
 
     if isinstance(data_url, DataURL):
         return data_url.data, data_url.mimeType
     return _do_decode(data_url)
 
 
@@ -93,15 +93,16 @@
            mime_type='text/plain',
            charset=_marker,
            encoder="base64"):
     """
     Encodes raw bytes into a data URL scheme string.
 
     :param raw_bytes: Raw bytes
-    :param mime_type: The mime type, e.g. ``b"text/css"`` or ``b"image/png"``. Default ``b"text/plain"``.
+    :param mime_type: The mime type, e.g.
+         ``b"text/css"`` or ``b"image/png"``. Default ``b"text/plain"``.
     :param charset: Set to ``b"utf-8"`` if you want the data URL to contain a ``b"charset=utf-8"``
             component. Default ``b'US-ASCII'``. This does not mean however, that your
             raw_bytes will be encoded by this function. You must ensure that
             if you specify, ``b"utf-8"`` (or anything else) as the encoding, you
             have encoded your raw data appropriately.
 
             .. note:: This function employs a heuristic to know when to default this
@@ -115,15 +116,16 @@
         raise TypeError("only raw bytes can be encoded")
 
     if encoder == "base64":
         _encode = b64encode
         codec = ";base64,"
     else:
         # We want ASCII bytes.
-        _encode = lambda data: quote(data).encode('ascii')
+        def _encode(data):
+            return quote(data).encode('ascii')
         codec = ","
     mime_type = mime_type or ""
 
     if charset is _marker:
         if mime_type.startswith('text/'):
             charset = _def_charset
         else:
```

### Comparing `nti.property-1.1.0/src/nti/property/schema.py` & `nti.property-1.2.0/src/nti/property/schema.py`

 * *Files identical despite different names*

