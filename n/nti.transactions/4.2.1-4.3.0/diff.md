# Comparing `tmp/nti.transactions-4.2.1.tar.gz` & `tmp/nti.transactions-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nti.transactions-4.2.1.tar", last modified: Tue May 25 11:57:34 2021, max compression
+gzip compressed data, was "nti.transactions-4.3.0.tar", last modified: Fri May  5 21:09:42 2023, max compression
```

## Comparing `nti.transactions-4.2.1.tar` & `nti.transactions-4.3.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:34.100738 nti.transactions-4.2.1/
--rw-r--r--   0 jmadden    (501) staff       (20)      467 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/.coveragerc
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:34.088358 nti.transactions-4.2.1/.github/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:34.092958 nti.transactions-4.2.1/.github/workflows/
--rw-r--r--   0 jmadden    (501) staff       (20)     1614 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/.github/workflows/tests.yml
--rw-r--r--   0 jmadden    (501) staff       (20)     3855 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/.pylintrc
--rw-r--r--   0 jmadden    (501) staff       (20)     6710 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/CHANGES.rst
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/INSTALL
--rw-r--r--   0 jmadden    (501) staff       (20)      579 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/LICENSE
--rw-r--r--   0 jmadden    (501) staff       (20)      264 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/MANIFEST.in
--rw-r--r--   0 jmadden    (501) staff       (20)    12869 2021-05-25 11:57:34.101040 nti.transactions-4.2.1/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     3031 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/README.rst
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/TODO
--rw-r--r--   0 jmadden    (501) staff       (20)      146 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/babel.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)       16 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/doc-requirements.txt
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:34.093746 nti.transactions-4.2.1/docs/
--rw-r--r--   0 jmadden    (501) staff       (20)       28 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/docs/changelog.rst
--rw-r--r--   0 jmadden    (501) staff       (20)    11420 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/docs/conf.py
--rw-r--r--   0 jmadden    (501) staff       (20)      811 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/docs/index.rst
--rw-r--r--   0 jmadden    (501) staff       (20)      271 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/nose2.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)      174 2021-05-25 11:57:34.101558 nti.transactions-4.2.1/setup.cfg
--rwxr-xr-x   0 jmadden    (501) staff       (20)     2285 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/setup.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:34.088868 nti.transactions-4.2.1/src/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:34.094006 nti.transactions-4.2.1/src/nti/
--rw-r--r--   0 jmadden    (501) staff       (20)       75 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/__init__.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:34.098764 nti.transactions-4.2.1/src/nti/transactions/
--rw-r--r--   0 jmadden    (501) staff       (20)     1228 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)      650 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/_httpexceptions.py
--rw-r--r--   0 jmadden    (501) staff       (20)      331 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/_loglevels.py
--rw-r--r--   0 jmadden    (501) staff       (20)      605 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/configure.zcml
--rw-r--r--   0 jmadden    (501) staff       (20)     6724 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/interfaces.py
--rw-r--r--   0 jmadden    (501) staff       (20)    33293 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/loop.py
--rw-r--r--   0 jmadden    (501) staff       (20)     7946 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/manager.py
--rw-r--r--   0 jmadden    (501) staff       (20)    15193 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/pyramid_tween.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1834 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/queue.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:34.100509 nti.transactions-4.2.1/src/nti/transactions/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)      238 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)    23066 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/tests/test_loop.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1480 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/tests/test_manager.py
--rw-r--r--   0 jmadden    (501) staff       (20)    14275 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/tests/test_pyramid_tween.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3211 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/tests/test_queue.py
--rw-r--r--   0 jmadden    (501) staff       (20)      791 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/tests/test_transactions.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1046 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti/transactions/transactions.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-05-25 11:57:34.096102 nti.transactions-4.2.1/src/nti.transactions.egg-info/
--rw-r--r--   0 jmadden    (501) staff       (20)    12869 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti.transactions.egg-info/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     1203 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti.transactions.egg-info/SOURCES.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti.transactions.egg-info/dependency_links.txt
--rw-r--r--   0 jmadden    (501) staff       (20)       20 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti.transactions.egg-info/entry_points.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti.transactions.egg-info/namespace_packages.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      310 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti.transactions.egg-info/requires.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti.transactions.egg-info/top_level.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/src/nti.transactions.egg-info/zip-safe
--rw-r--r--   0 jmadden    (501) staff       (20)     1359 2021-05-25 11:57:33.000000 nti.transactions-4.2.1/tox.ini
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.483321 nti.transactions-4.3.0/
+-rw-r--r--   0 jmadden    (501) staff       (20)      467 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/.coveragerc
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.477851 nti.transactions-4.3.0/.github/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.480236 nti.transactions-4.3.0/.github/workflows/
+-rw-r--r--   0 jmadden    (501) staff       (20)     1905 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)      204 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/.gitignore
+-rw-r--r--   0 jmadden    (501) staff       (20)     8996 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/.pylintrc
+-rw-r--r--   0 jmadden    (501) staff       (20)      845 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/.readthedocs.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)     6791 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/CHANGES.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       73 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/COPYRIGHT.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/INSTALL
+-rw-r--r--   0 jmadden    (501) staff       (20)      529 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/LICENSE
+-rw-r--r--   0 jmadden    (501) staff       (20)      278 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/MANIFEST.in
+-rw-r--r--   0 jmadden    (501) staff       (20)    11040 2023-05-05 21:09:42.483392 nti.transactions-4.3.0/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)     3017 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/README.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/TODO
+-rw-r--r--   0 jmadden    (501) staff       (20)      146 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/babel.cfg
+-rw-r--r--   0 jmadden    (501) staff       (20)       16 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/doc-requirements.txt
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.480572 nti.transactions-4.3.0/docs/
+-rw-r--r--   0 jmadden    (501) staff       (20)       28 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/docs/changelog.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)    12629 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/docs/conf.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      811 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/docs/index.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)      271 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/nose2.cfg
+-rw-r--r--   0 jmadden    (501) staff       (20)      174 2023-05-05 21:09:42.483610 nti.transactions-4.3.0/setup.cfg
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     2442 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/setup.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.478098 nti.transactions-4.3.0/src/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.480702 nti.transactions-4.3.0/src/nti/
+-rw-r--r--   0 jmadden    (501) staff       (20)       75 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/__init__.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.482592 nti.transactions-4.3.0/src/nti/transactions/
+-rw-r--r--   0 jmadden    (501) staff       (20)     1267 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      650 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/_httpexceptions.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      331 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/_loglevels.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      605 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/configure.zcml
+-rw-r--r--   0 jmadden    (501) staff       (20)     6724 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/interfaces.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    33567 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/loop.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     7946 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/manager.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    15256 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/pyramid_tween.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1834 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/queue.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.483209 nti.transactions-4.3.0/src/nti/transactions/tests/
+-rw-r--r--   0 jmadden    (501) staff       (20)      238 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/tests/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    23523 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/tests/test_loop.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1480 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/tests/test_manager.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    14339 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/tests/test_pyramid_tween.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3211 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/tests/test_queue.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      791 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/tests/test_transactions.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1046 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti/transactions/transactions.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-05-05 21:09:42.481536 nti.transactions-4.3.0/src/nti.transactions.egg-info/
+-rw-r--r--   0 jmadden    (501) staff       (20)    11040 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti.transactions.egg-info/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)     1198 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti.transactions.egg-info/SOURCES.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti.transactions.egg-info/dependency_links.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti.transactions.egg-info/namespace_packages.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)      407 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti.transactions.egg-info/requires.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti.transactions.egg-info/top_level.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/src/nti.transactions.egg-info/zip-safe
+-rw-r--r--   0 jmadden    (501) staff       (20)     1169 2023-05-05 21:09:42.000000 nti.transactions-4.3.0/tox.ini
```

### Comparing `nti.transactions-4.2.1/CHANGES.rst` & `nti.transactions-4.3.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 
 =========
  Changes
 =========
 
+4.3.0 (2023-05-05)
+==================
+
+- Add support for Python 3.10 and 3.11.
+
+
 4.2.1 (2021-05-25)
 ==================
 
 - When aborting a transaction due to an exception, log the exception
   instead of just the exception type (twice). Exception messages can
   be very helpful in understanding exactly what went wrong and
   possibly how to fix it for transient errors (e.g., a
```

### Comparing `nti.transactions-4.2.1/LICENSE` & `nti.transactions-4.3.0/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-Copyright (c) 2011-2015 NextThought, LLC
-
- Licensed under the Apache License, Version 2.0 (the "License");
- you may not use this software except in compliance with the License.
- You may obtain a copy of the License at
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this software except in compliance with the License.
+You may obtain a copy of the License at
 
      http://www.apache.org/licenses/LICENSE-2.0
 
- Unless required by applicable law or agreed to in writing, software
- distributed under the License is distributed on an "AS IS" BASIS,
- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
- See the License for the specific language governing permissions and
- limitations under the License.
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `nti.transactions-4.2.1/PKG-INFO` & `nti.transactions-4.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,285 +1,293 @@
 Metadata-Version: 2.1
 Name: nti.transactions
-Version: 4.2.1
+Version: 4.3.0
 Summary: NTI Transactions Utility
-Home-page: https://github.com/NextThought/nti.transactions
+Home-page: https://github.com/OpenNTI/nti.transactions
 Author: Jason Madden
 Author-email: jason@nextthought.com
 License: Apache
-Description: ==================
-         nti.transactions
-        ==================
-        
-        
-        .. _transaction: https://pypi.python.org/pypi/transaction
-        
-        .. image:: https://coveralls.io/repos/github/NextThought/nti.transactions/badge.svg?branch=master
-        	:target: https://coveralls.io/github/NextThought/nti.transactions?branch=master
-        
-        .. image:: https://github.com/NextThought/nti.transactions/workflows/tests/badge.svg
-           :target: https://github.com/NextThought/nti.transactions/actions?query=workflow%3Atests
-        
-        .. image:: https://readthedocs.org/projects/ntitransactions/badge/?version=latest
-           :target: https://ntitransactions.readthedocs.io/en/latest/?badge=latest
-           :alt: Documentation Status
-        
-        Extensions to the `transaction`_ package.
-        
-        .. contents::
-        
-        
-        Transaction Management
-        ======================
-        
-        ``nti.transactions.loop.TransactionsLoop`` is a retryable
-        transaction manager. It is conceptually similar to the `attempts`_
-        context manager provided by the transaction package itself, but much
-        more powerful and extensible via subclasses. Features include:
-        
-        - Configurable commit vetos.
-        - Extensible tests for which exceptions should be retried.
-        - The ability to abort the transaction and bypass a potentially
-          expensive commit when there are expected to be no side-effects.
-        - Sleeping between retries.
-        - Extensive logging and timing.
-        
-        The TransactionLoop can be used as-is, or it can be subclassed for
-        customization. For use in a Pyramid tween, for example, a minimal
-        subclass might look like this (see ``nti.transactions.pyramid_tween``
-        for a full-featured tween)::
-        
-          >>> class PyramidTransactionLoop(TransactionLoop):
-          ...    def prep_for_retry(self, number, request):
-          ...        request.make_body_seekable()
-          ...    def describe_transaction(self, request):
-          ...        return request.url
-        
-        Data Managers
-        =============
-        
-        A few `data managers`_ are provided for convenience.
-        
-        The first data manager is used to put an object in a ``queue``
-        (something with the ``full`` and ``put_nowait`` methods) when a
-        transaction succeeds. If the queue is full, then the transaction will
-        not be allowed to commit::
-        
-          >>> from nti.transactions.queue import put_nowait
-          >>> put_nowait(queue, object)
-        
-        This is a special case of the ``ObjectDataManager``, which will call
-        one method with any arguments when a transaction commits. It can be
-        configured to vote on whether the transaction should be allowed to commit.
-        or not. This is useful for, say, putting an item in a Redis queue when
-        the transaction is successful. It can be constructed directly, but the
-        ``do`` function is a shorthand way of joining one to the current
-        transaction::
-        
-          >>> from nti.transactions.manager import do
-          >>> do(print, args=("Committed"))
-        
-        .. caution:: See the documentation of this object for numerous
-        	     warnings about side-effects and its interaction with the
-        	     transaction machinery. Use it with care!
-        
-        .. _attempts: http://zodb.readthedocs.io/en/latest/transactions.html#retrying-transactions
-        .. _data managers: http://zodb.readthedocs.io/en/latest/transactions.html#data-managers
-        
-        =========
-         Changes
-        =========
-        
-        4.2.1 (2021-05-25)
-        ==================
-        
-        - When aborting a transaction due to an exception, log the exception
-          instead of just the exception type (twice). Exception messages can
-          be very helpful in understanding exactly what went wrong and
-          possibly how to fix it for transient errors (e.g., a
-          ``ZODB.POSException.ConflictError`` includes the object ID and
-          class, which can be used to reduce the conflicts). This makes the
-          logging slightly more expensive (when enabled). See `PR 58
-          <https://github.com/NextThought/nti.transactions/pull/58>`_.
-        
-        
-        4.2.0 (2021-02-11)
-        ==================
-        
-        - Add support for Python 3.9.
-        - Move CI from Travis CI to Github Actions.
-        - When the Pyramid tween retries, any volatile attributes (those
-          beginning with ``_v_``) in the request dictionary are deleted. This
-          is inspired by ``persistent`` and meant to facilitate safe caching.
-          When compared to events sent by the transaction loop, there is no
-          specified order. See `issue 54 <https://github.com/NextThought/nti.transactions/issues/54>`_.
-        - Fix various event classes not properly specifying the interface they
-          implement. For example, ``WillFirstAttempt`` now properly implements
-          ``IWillFirstAttempt``, and ``WilLRetryAttempt`` now properly
-          implements ``IWillRetryAttempt``. See `issue 52
-          <https://github.com/NextThought/nti.transactions/issues/52>`_.
-        - Add ``IWillLastAttempt`` as a subclass of ``IWillRetryAttempt`` and
-          the last event emitted.
-        - The Pyramid tween now emits ``IWillRetryAttemptWithRequest``, et al,
-          to provide simple access to the request object.
-        
-        4.1.0 (2020-07-22)
-        ==================
-        
-        - Add logging to the pyramid tween transaction factory to show the
-          settings that are in use.
-        - Add ``TransactionLoop.side_effect_free_log_level``, and change the
-          default value to DEBUG. It is useful to set this to ERROR or higher
-          in tests.
-        - Add ``TransactionLoop.side_effect_free_resource_limit``.
-        
-        
-        4.0.1 (2020-07-18)
-        ==================
-        
-        - Add missing dependency on zope.event.
-        - Fix raising ``AlreadyInTransaction`` error on the second and
-          subsequent calls to a loop when a transaction synchronizer raises an
-          error on the first call. See `issue 49
-          <https://github.com/NextThought/nti.transactions/issues/49>`_.
-        
-        4.0.0 (2019-12-13)
-        ==================
-        
-        - Require at least version 3.0 of the ``transaction`` package.
-        
-        - Drop dependency on the ``dm.transaction.aborthook`` package. That
-          functionality is now natively provided in transaction 3.0.
-        
-        
-        3.1.1 (2019-12-10)
-        ==================
-        
-        - Fix logging of long duration commits. See `issue 44
-          <https://github.com/NextThought/nti.transactions/issues/44>`_.
-        
-        - Add logging and a metric
-          (``transaction.side_effect_free_violation``) for transactions that
-          claim to have no side effects, but which actually result in joined
-          resource managers. This can indicate unnecessarily throwing away
-          work. See `issue 45 <https://github.com/NextThought/nti.transactions/issues/45>`_.
-        
-        
-        3.1.0 (2019-11-29)
-        ==================
-        
-        - Add support for Python 3.8.
-        
-        - Refactor internal implementation details. Instead of importing
-          everything from ``nti.transactions.transactions``, more specific
-          modules are used to group objects by function. The old imports
-          continue to work. In 4.0 they will generate a deprecation warning
-          and in 5.0 they will be removed.
-        
-        - Add a Pyramid tween to manage transactions and transaction retries.
-          Various settings can be configured as Pyramid deployment settings
-          (e.g., in the ini file).
-        
-        - Make the transaction loop increase the time it sleeps between
-          retries following the `random binary exponential backoff algorithm
-          <https://en.wikipedia.org/wiki/Exponential_backoff>`_ used by Ethernet.
-        
-        - Reduce the default number of attempts to 4 (one attempt and 3
-          retries). See `issue 35 <https://github.com/NextThought/nti.transactions/issues/35>`_.
-        
-        - Make the transaction loop emit more metrics. See `issue 31
-          <https://github.com/NextThought/nti.transactions/issues/31>`_.
-        
-        - Make commit logging now always happen at least at the debug level,
-          escalating to warning for long commits. It also includes the number
-          of retries taken and the amount of time spent sleeping. See `issue
-          32 <https://github.com/NextThought/nti.transactions/issues/32>`_.
-        
-        - Make the transaction loop emit events (using ``zope.event``) at certain parts of the
-          transaction lifecycle. See `issue 33 <https://github.com/NextThought/nti.transactions/issues/33>`_.
-        
-        3.0.0 (2019-09-06)
-        ==================
-        
-        - Make ``TransactionLoop`` place its transaction manager in explicit
-          mode. This can be faster and is easier to reason about, but forbids
-          the called handler from manually calling ``begin()``, ``abort()`` or
-          ``commit()``. See `issue 20
-          <https://github.com/NextThought/nti.transactions/issues/20>`_.
-        
-        - Move ``transaction.begin()`` out of the block of code that is
-          retried. Previously, an error there would probably be raised
-          *anyway* and not retried, unless a subclass had made customizations.
-        
-        - Add ``setUp`` and ``tearDown`` methods to TransactionLoop to give
-          subclasses a place to hook into the inners of the transaction loop.
-          This is particularly helpful if they need to do something after the
-          transaction manager has been put in explicit mode. See `issue 22
-          <https://github.com/NextThought/nti.transactions/issues/22>`_.
-        
-        2.0.1 (2019-09-03)
-        ==================
-        
-        - Fix compatibility with perfmetrics 3.0: drop ``from __future__
-          import unicode_literals``.
-        
-        
-        2.0.0 (2018-07-20)
-        ==================
-        
-        - Use the new public ``isRetryableError`` in transaction 2.2. The
-          interface for this package is unchanged, but a major version bump of
-          a dependency necessitates a major bump here. See `issue 12
-          <https://github.com/NextThought/nti.transactions/issues/12>`_.
-        
-        - Test support for Python 3.7; remove test support for Python 3.4.
-        
-        - ``TransactionLoop`` is more careful to not keep traceback objects
-          around, especially on Python 2.
-        
-        1.1.1 (2018-07-19)
-        ==================
-        
-        - When the ``TransactionLoop`` raises a ``CommitFailedError`` from a
-          ``TypeError``, it preserves the original message.
-        
-        - Test support for Python 3.6.
-        
-        1.1.0 (2017-04-17)
-        ==================
-        
-        - Add a new ObjectDataManager that will attempt to execute after
-          other ObjectDataManagers.
-        
-        
-        1.0.0 (2016-07-28)
-        ==================
-        
-        - Add support for Python 3.
-        - Eliminate ZODB dependency. Instead of raising a
-          ``ZODB.POSException.StorageError`` for unexpected ``TypeErrors``
-          during commit, the new class
-          ``nti.transactions.interfaces.CommitFailedError`` is raised.
-        - Introduce a new subclass of ``TransactionError``,
-          ``AbortFailedError`` that is raised when an abort fails due to a
-          system error.
-        
 Keywords: ZODB transaction
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: ZODB
 Provides-Extra: test
 Provides-Extra: gevent
 Provides-Extra: docs
 Provides-Extra: pyramid
+License-File: LICENSE
+
+==================
+ nti.transactions
+==================
+
+
+.. _transaction: https://pypi.python.org/pypi/transaction
+
+.. image:: https://coveralls.io/repos/github/NextThought/nti.transactions/badge.svg?branch=master
+	:target: https://coveralls.io/github/NextThought/nti.transactions?branch=master
+
+.. image:: https://github.com/NextThought/nti.transactions/workflows/tests/badge.svg
+   :target: https://github.com/NextThought/nti.transactions/actions?query=workflow%3Atests
+
+.. image:: https://readthedocs.org/projects/ntitransactions/badge/?version=latest
+   :target: https://ntitransactions.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
+Extensions to the `transaction`_ package.
+
+
+
+Transaction Management
+======================
+
+``nti.transactions.loop.TransactionsLoop`` is a retryable
+transaction manager. It is conceptually similar to the `attempts`_
+context manager provided by the transaction package itself, but much
+more powerful and extensible via subclasses. Features include:
+
+- Configurable commit vetos.
+- Extensible tests for which exceptions should be retried.
+- The ability to abort the transaction and bypass a potentially
+  expensive commit when there are expected to be no side-effects.
+- Sleeping between retries.
+- Extensive logging and timing.
+
+The TransactionLoop can be used as-is, or it can be subclassed for
+customization. For use in a Pyramid tween, for example, a minimal
+subclass might look like this (see ``nti.transactions.pyramid_tween``
+for a full-featured tween)::
+
+  >>> class PyramidTransactionLoop(TransactionLoop):
+  ...    def prep_for_retry(self, number, request):
+  ...        request.make_body_seekable()
+  ...    def describe_transaction(self, request):
+  ...        return request.url
+
+Data Managers
+=============
+
+A few `data managers`_ are provided for convenience.
+
+The first data manager is used to put an object in a ``queue``
+(something with the ``full`` and ``put_nowait`` methods) when a
+transaction succeeds. If the queue is full, then the transaction will
+not be allowed to commit::
+
+  >>> from nti.transactions.queue import put_nowait
+  >>> put_nowait(queue, object)
+
+This is a special case of the ``ObjectDataManager``, which will call
+one method with any arguments when a transaction commits. It can be
+configured to vote on whether the transaction should be allowed to commit.
+or not. This is useful for, say, putting an item in a Redis queue when
+the transaction is successful. It can be constructed directly, but the
+``do`` function is a shorthand way of joining one to the current
+transaction::
+
+  >>> from nti.transactions.manager import do
+  >>> do(print, args=("Committed"))
+
+.. caution:: See the documentation of this object for numerous
+	     warnings about side-effects and its interaction with the
+	     transaction machinery. Use it with care!
+
+.. _attempts: http://zodb.readthedocs.io/en/latest/transactions.html#retrying-transactions
+.. _data managers: http://zodb.readthedocs.io/en/latest/transactions.html#data-managers
+
+=========
+ Changes
+=========
+
+4.3.0 (2023-05-05)
+==================
+
+- Add support for Python 3.10 and 3.11.
+
+
+4.2.1 (2021-05-25)
+==================
+
+- When aborting a transaction due to an exception, log the exception
+  instead of just the exception type (twice). Exception messages can
+  be very helpful in understanding exactly what went wrong and
+  possibly how to fix it for transient errors (e.g., a
+  ``ZODB.POSException.ConflictError`` includes the object ID and
+  class, which can be used to reduce the conflicts). This makes the
+  logging slightly more expensive (when enabled). See `PR 58
+  <https://github.com/NextThought/nti.transactions/pull/58>`_.
+
+
+4.2.0 (2021-02-11)
+==================
+
+- Add support for Python 3.9.
+- Move CI from Travis CI to Github Actions.
+- When the Pyramid tween retries, any volatile attributes (those
+  beginning with ``_v_``) in the request dictionary are deleted. This
+  is inspired by ``persistent`` and meant to facilitate safe caching.
+  When compared to events sent by the transaction loop, there is no
+  specified order. See `issue 54 <https://github.com/NextThought/nti.transactions/issues/54>`_.
+- Fix various event classes not properly specifying the interface they
+  implement. For example, ``WillFirstAttempt`` now properly implements
+  ``IWillFirstAttempt``, and ``WilLRetryAttempt`` now properly
+  implements ``IWillRetryAttempt``. See `issue 52
+  <https://github.com/NextThought/nti.transactions/issues/52>`_.
+- Add ``IWillLastAttempt`` as a subclass of ``IWillRetryAttempt`` and
+  the last event emitted.
+- The Pyramid tween now emits ``IWillRetryAttemptWithRequest``, et al,
+  to provide simple access to the request object.
+
+4.1.0 (2020-07-22)
+==================
+
+- Add logging to the pyramid tween transaction factory to show the
+  settings that are in use.
+- Add ``TransactionLoop.side_effect_free_log_level``, and change the
+  default value to DEBUG. It is useful to set this to ERROR or higher
+  in tests.
+- Add ``TransactionLoop.side_effect_free_resource_limit``.
+
+
+4.0.1 (2020-07-18)
+==================
+
+- Add missing dependency on zope.event.
+- Fix raising ``AlreadyInTransaction`` error on the second and
+  subsequent calls to a loop when a transaction synchronizer raises an
+  error on the first call. See `issue 49
+  <https://github.com/NextThought/nti.transactions/issues/49>`_.
+
+4.0.0 (2019-12-13)
+==================
+
+- Require at least version 3.0 of the ``transaction`` package.
+
+- Drop dependency on the ``dm.transaction.aborthook`` package. That
+  functionality is now natively provided in transaction 3.0.
+
+
+3.1.1 (2019-12-10)
+==================
+
+- Fix logging of long duration commits. See `issue 44
+  <https://github.com/NextThought/nti.transactions/issues/44>`_.
+
+- Add logging and a metric
+  (``transaction.side_effect_free_violation``) for transactions that
+  claim to have no side effects, but which actually result in joined
+  resource managers. This can indicate unnecessarily throwing away
+  work. See `issue 45 <https://github.com/NextThought/nti.transactions/issues/45>`_.
+
+
+3.1.0 (2019-11-29)
+==================
+
+- Add support for Python 3.8.
+
+- Refactor internal implementation details. Instead of importing
+  everything from ``nti.transactions.transactions``, more specific
+  modules are used to group objects by function. The old imports
+  continue to work. In 4.0 they will generate a deprecation warning
+  and in 5.0 they will be removed.
+
+- Add a Pyramid tween to manage transactions and transaction retries.
+  Various settings can be configured as Pyramid deployment settings
+  (e.g., in the ini file).
+
+- Make the transaction loop increase the time it sleeps between
+  retries following the `random binary exponential backoff algorithm
+  <https://en.wikipedia.org/wiki/Exponential_backoff>`_ used by Ethernet.
+
+- Reduce the default number of attempts to 4 (one attempt and 3
+  retries). See `issue 35 <https://github.com/NextThought/nti.transactions/issues/35>`_.
+
+- Make the transaction loop emit more metrics. See `issue 31
+  <https://github.com/NextThought/nti.transactions/issues/31>`_.
+
+- Make commit logging now always happen at least at the debug level,
+  escalating to warning for long commits. It also includes the number
+  of retries taken and the amount of time spent sleeping. See `issue
+  32 <https://github.com/NextThought/nti.transactions/issues/32>`_.
+
+- Make the transaction loop emit events (using ``zope.event``) at certain parts of the
+  transaction lifecycle. See `issue 33 <https://github.com/NextThought/nti.transactions/issues/33>`_.
+
+3.0.0 (2019-09-06)
+==================
+
+- Make ``TransactionLoop`` place its transaction manager in explicit
+  mode. This can be faster and is easier to reason about, but forbids
+  the called handler from manually calling ``begin()``, ``abort()`` or
+  ``commit()``. See `issue 20
+  <https://github.com/NextThought/nti.transactions/issues/20>`_.
+
+- Move ``transaction.begin()`` out of the block of code that is
+  retried. Previously, an error there would probably be raised
+  *anyway* and not retried, unless a subclass had made customizations.
+
+- Add ``setUp`` and ``tearDown`` methods to TransactionLoop to give
+  subclasses a place to hook into the inners of the transaction loop.
+  This is particularly helpful if they need to do something after the
+  transaction manager has been put in explicit mode. See `issue 22
+  <https://github.com/NextThought/nti.transactions/issues/22>`_.
+
+2.0.1 (2019-09-03)
+==================
+
+- Fix compatibility with perfmetrics 3.0: drop ``from __future__
+  import unicode_literals``.
+
+
+2.0.0 (2018-07-20)
+==================
+
+- Use the new public ``isRetryableError`` in transaction 2.2. The
+  interface for this package is unchanged, but a major version bump of
+  a dependency necessitates a major bump here. See `issue 12
+  <https://github.com/NextThought/nti.transactions/issues/12>`_.
+
+- Test support for Python 3.7; remove test support for Python 3.4.
+
+- ``TransactionLoop`` is more careful to not keep traceback objects
+  around, especially on Python 2.
+
+1.1.1 (2018-07-19)
+==================
+
+- When the ``TransactionLoop`` raises a ``CommitFailedError`` from a
+  ``TypeError``, it preserves the original message.
+
+- Test support for Python 3.6.
+
+1.1.0 (2017-04-17)
+==================
+
+- Add a new ObjectDataManager that will attempt to execute after
+  other ObjectDataManagers.
+
+
+1.0.0 (2016-07-28)
+==================
+
+- Add support for Python 3.
+- Eliminate ZODB dependency. Instead of raising a
+  ``ZODB.POSException.StorageError`` for unexpected ``TypeErrors``
+  during commit, the new class
+  ``nti.transactions.interfaces.CommitFailedError`` is raised.
+- Introduce a new subclass of ``TransactionError``,
+  ``AbortFailedError`` that is raised when an abort fails due to a
+  system error.
```

### Comparing `nti.transactions-4.2.1/README.rst` & `nti.transactions-4.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 .. image:: https://readthedocs.org/projects/ntitransactions/badge/?version=latest
    :target: https://ntitransactions.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 Extensions to the `transaction`_ package.
 
-.. contents::
 
 
 Transaction Management
 ======================
 
 ``nti.transactions.loop.TransactionsLoop`` is a retryable
 transaction manager. It is conceptually similar to the `attempts`_
```

### Comparing `nti.transactions-4.2.1/docs/conf.py` & `nti.transactions-4.3.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 release = rqmt.version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #
 # today = ''
 #
 # Else, today_fmt is used as the format for a strftime call.
@@ -137,17 +137,28 @@
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-import sphinx_rtd_theme
-html_theme = 'sphinx_rtd_theme'
-html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
+
+if sys.version_info[0] >= 3:
+    html_theme = 'furo'
+    html_theme_options = {
+        'light_css_variables': {
+            'font-stack': '"SF Pro",-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji"',
+            'font-stack--monospace': '"JetBrainsMono", "JetBrains Mono", "JetBrains Mono Regular", "JetBrainsMono-Regular", ui-monospace, profont, monospace',
+        },
+    }
+else:
+    import sphinx_rtd_theme
+    html_theme = 'sphinx_rtd_theme'
+    html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
+
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
@@ -359,20 +370,34 @@
 intersphinx_mapping = {
     'https://docs.python.org/': None,
     'https://transaction.readthedocs.io/en/latest/': None,
     'https://perfmetrics.readthedocs.io/en/latest/': None,
     'https://pyramid.readthedocs.io/en/latest/': None,
     'https://docs.pylonsproject.org/projects/pyramid-retry/en/latest/': None,
     "https://docs.pylonsproject.org/projects/pyramid-tm/en/latest/": None
+}
 
+intersphinx_mapping = {
+    'python': ('http://docs.python.org/', None,),
+    'sqlalchemy': ('https://docs.sqlalchemy.org', None,),
+    'zodb': ('http://zodb.readthedocs.io/en/latest/', None,),
+    'interface': ('http://zopeinterface.readthedocs.io/en/latest/', None,),
+    'component': ('http://zopecomponent.readthedocs.io/en/latest/', None,),
+
+    'transaction': ('https://transaction.readthedocs.io/en/latest/', None,),
+    'perfmetrics': ('https://perfmetrics.readthedocs.io/en/latest/', None,),
+    'pyramid': ('https://pyramid.readthedocs.io/en/latest/', None,),
+    'pyramid-retry': ('https://docs.pylonsproject.org/projects/pyramid-retry/en/latest/', None,),
+    'pyramid-tm': ("https://docs.pylonsproject.org/projects/pyramid-tm/en/latest/", None),
 }
 
-extlinks = {'issue': ('https://github.com/NextThought/nti.transactions/issues/%s',
+
+extlinks = {'issue': ('https://github.com/OpenNTI/nti.transactions/issues/%s',
                       'issue #'),
-            'pr': ('https://github.com/NextThought/nti.transactions/pull/%s',
+            'pr': ('https://github.com/OpenNTI/nti.transactions/pull/%s',
                    'pull request #')}
 
 # Sphinx 1.8+ prefers this to `autodoc_default_flags`. It's documented that
 # either True or None mean the same thing as just setting the flag, but
 # only None works in 1.8 (True works in 2.0)
 autodoc_default_options = {
     'members': None,
```

### Comparing `nti.transactions-4.2.1/docs/index.rst` & `nti.transactions-4.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nti.transactions-4.2.1/setup.py` & `nti.transactions-4.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import codecs
 from setuptools import setup, find_packages
 
-version = '4.2.1'
+version = '4.3.0'
 
 entry_points = {
     'console_scripts': [
     ],
 }
 
 TESTS_REQUIRE = [
     'coverage',
-    'fudge',
     'nti.testing',
     'pylint',
     'pyramid',
     'zope.component',
     'zope.testrunner',
     'ZODB',
+    'mock; python_version == "2.7"',
 ]
 
 def _read(fname):
     with codecs.open(fname, encoding='UTF-8') as f:
         return f.read()
 
 setup(
@@ -28,28 +28,31 @@
     version=version,
     author='Jason Madden',
     author_email='jason@nextthought.com',
     description="NTI Transactions Utility",
     long_description=_read('README.rst') + _read('CHANGES.rst'),
     license='Apache',
     keywords='ZODB transaction',
-    url='https://github.com/NextThought/nti.transactions',
+    url='https://github.com/OpenNTI/nti.transactions',
     zip_safe=True,
     classifiers=[
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Framework :: ZODB',
     ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
@@ -65,20 +68,19 @@
         'zope.interface',
         'zope.event',
     ],
     extras_require={
         'test': TESTS_REQUIRE,
         'gevent': ['gevent',],
         'docs': [
-            # Sphinx 4 and repoze.sphinx.autointerface 0.8
-            # are incompatible
-            'Sphinx < 4',
+            'Sphinx',
             'repoze.sphinx.autointerface',
             'pyhamcrest',
-            'sphinx_rtd_theme',
+            'furo; python_version >= "3.6"',
+            'sphinx_rtd_theme; python_version < "3.6"',
         ],
         'pyramid': [
             'pyramid >= 1.2',
         ],
     },
     entry_points=entry_points
 )
```

### Comparing `nti.transactions-4.2.1/src/nti/transactions/__init__.py` & `nti.transactions-4.3.0/src/nti/transactions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # Monkey-patches
 ###
 
 # By default, it wants to create a different logger
 # for each and every thread or greenlet. We go through
 # lots of greenlets, so that's lots of loggers
 from transaction import _transaction
+# pylint:disable-next=protected-access
 _transaction._LOGGER = __import__('logging').getLogger('txn.GLOBAL')
 
 # Introduce a 'nti_abort' function that wraps the raw abort as a metric.
 raw_abort = _transaction.Transaction.abort
 raw_abort = getattr(raw_abort, 'im_func', raw_abort) # Py2
 _transaction.Transaction.nti_abort = Metric('transaction.abort', rate=0.1)(raw_abort)
 del raw_abort
```

### Comparing `nti.transactions-4.2.1/src/nti/transactions/_httpexceptions.py` & `nti.transactions-4.3.0/src/nti/transactions/_httpexceptions.py`

 * *Files identical despite different names*

### Comparing `nti.transactions-4.2.1/src/nti/transactions/configure.zcml` & `nti.transactions-4.3.0/src/nti/transactions/configure.zcml`

 * *Files identical despite different names*

### Comparing `nti.transactions-4.2.1/src/nti/transactions/interfaces.py` & `nti.transactions-4.3.0/src/nti/transactions/interfaces.py`

 * *Files identical despite different names*

### Comparing `nti.transactions-4.2.1/src/nti/transactions/loop.py` & `nti.transactions-4.3.0/src/nti/transactions/loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,17 @@
             try:
                 logger.exception("Failed to abort transaction following exception "
                                  "(retrying %s/%s; %r: %s). New exception:",
                                  retryable, number, e, exc_info[1])
             except:  # pylint:disable=I0011,W0702
                 pass
             # We've seen RelStorage do this:
-            # relstorage.cache:427 in after_poll: AttributeError: 'int' object has no attribute 'split' which looks like
+            # relstorage.cache:427 in after_poll:
+            #    AttributeError: 'int' object has no attribute 'split'
+            # which looks like
             # an issue with how it stores checkpoints in memcache.
             # We have no idea what state it's in after that, so we should
             # abort.
 
             # We've seen repoze.sendmail do this:
             # repoze.sendmail.delivery:119 in abort: ValueError "TPC in progress"
             # This appears to happen due to some other component raising an exception
@@ -389,15 +391,16 @@
             # The sendmail object appears to have been `tpc_begin`, but not
             # `tpc_vote`. (This may happen if the original exception was a ReadConflictError?)
             # https://github.com/repoze/repoze.sendmail/issues/31 (introduced in 4.2)
             # Again, no idea what state things are in, so abort with prejudice.
             try:
                 if format_exception is not None:
                     fmt = format_exception(*exc_info)
-                    logger.warning("Failed to abort transaction following exception. Original exception:\n%s",
+                    logger.warning("Failed to abort transaction following exception. "
+                                   "Original exception:\n%s",
                                    '\n'.join(fmt))
             except: # pylint:disable=bare-except
                 exc_info = sys.exc_info()
 
             six.reraise(AbortFailedError, AbortFailedError(repr(exc_info)), exc_info[2])
         finally:
             del exc_info
@@ -528,16 +531,19 @@
     EVT_WILL_RETRY_ATTEMPT = WillRetryAttempt
     #: The event to send before running the handler the last time.
     #: Subclasses may override.
     #:
     #: ..versionadded:: 4.2.0
     EVT_WILL_LAST_ATTEMPT = WillLastAttempt
 
+    # Where actually are we not doing this?
+    # pylint:disable=inconsistent-return-statements
     def __loop(self, txm, note, stats, args, kwargs):
-        # pylint:disable=too-many-branches,too-many-statements,too-many-locals
+        # pylint:disable=too-many-branches,too-many-statements,too-many-locals,too-complex
+
         attempts_remaining = self.attempts
         need_retry = self.attempts > 1
         begin = txm.begin
         unused_descr = self._UNUSED_DESCRIPTION
         sleep_time = 0
         invocation = LoopInvocation(self, self.handler, args, kwargs)
         while attempts_remaining:
@@ -630,14 +636,15 @@
                     # was nominally side-effect free, but resource managers
                     # joined it, so they probably want to do work.
                     # This uses transaction internals, and we don't do a three-arg
                     # getattr(); we want to break if they change.
                     # The list of joined resource managers may be very long
                     # in some cases and it's not always useful to print
                     # all of them.
+                    # pylint:disable=protected-access
                     resources = tx._resources or ()
 
                     if resources:
                         resources = (
                             '(count=%d)' % len(resources)
                             if len(resources) > self.side_effect_free_resource_report_limit
                             else resources
@@ -727,14 +734,15 @@
                 raise # pragma: no cover
 
 
     def __abort_current_transaction_quietly(self, txm):
         self.__abort_transaction_quietly(txm)
         # Ensure we're in a clean state
         # even if abort failed.
+        # pylint:disable=protected-access
         txm._txn = None
 
     @staticmethod
     def __abort_transaction_quietly(tx):
         try:
             tx.abort()
         except Exception: # Ignore. pylint:disable=broad-except
```

### Comparing `nti.transactions-4.2.1/src/nti/transactions/manager.py` & `nti.transactions-4.3.0/src/nti/transactions/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         """
         Construct a data manager. You must pass either the `target` and `method_name` arguments
         or the `call` argument. (You may always pass the `target` argument, which will
         be made available on this object for the use of :meth:`tpc_vote`. )
 
         :param target: An object. Optional if `call` is given. If provided, will be used
             to compute the :meth:`sortKey`.
-        :param string method_name: The name of the attribute to get from `target`. Optional if `callable`
-            is given.
+        :param string method_name: The name of the attribute to get from `target`.
+            Optional if `callable` is given.
         :param callable call: A callable object. Ignored if `target` *and* `method_name` are given.
         :param callable vote: If given, then a callable that will be called during the voting phase.
             It should raise an exception if the transaction will fail.
         :param args: A sequence of arguments to pass to the callable object. Optional.
         :param kwargs: A dictionary of arguments to pass to the callable object. Optional.
         """
         self.target = target
```

### Comparing `nti.transactions-4.2.1/src/nti/transactions/pyramid_tween.py` & `nti.transactions-4.3.0/src/nti/transactions/pyramid_tween.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         - The URL DOES NOT match a configured exception list.
 
     In this version, the configured exception list is not actually
     configurable. It is hardcoded to handle the case of socket.io
     polling (which does have side effects on GET requests), while
     still supporting serving the static resources of socket.io.
     """
-    if request.method == 'GET' or request.method == 'HEAD':
+    if request.method in ('GET', 'HEAD'):
         # GET/HEAD requests must NEVER have side effects.
         if 'socket.io' in request.url:
             # (Unfortunately, socket.io polling does)
             # However, the static resources don't.
 
             # TODO: This needs to be configurable *and* fast.
             #
@@ -235,14 +235,15 @@
         # real world. An internal implementation change (accessing
         # POST) suddenly meant that we couldn't read their body.
         # Unfortunately, the mangling is not fully reversible, since
         # it wasn't encoded in the first place.
 
         # We attempt to fix that here. (This is the best place because
         # we are now sure the body is seekable.)
+        # pylint:disable-next=compare-to-zero
         if attempt_number == 0 \
            and request.method in ('POST', 'PUT') \
            and request.content_type == 'application/x-www-form-urlencoded':
             # This needs tested.
             body = request.body
             # Python 3 treats bytes different than strings. Iteration
             # and indexing don't iterate over one-byte strings, they return
@@ -297,15 +298,16 @@
             # can also be used for other things (such as redirecting what
             # would otherwise be a 404).
             # So we wrap up __call__ and also check for HTTPException there
             # and raise it safely after transaction handling is done.
             # Of course, this is only needed if the exception was actually
             # raised, not deliberately returned (commonly HTTPFound and the like
             # are returned)...raising those could have unintended consequences
-            request._v_nti_raised_exception = True
+
+            request._v_nti_raised_exception = True # pylint:disable=protected-access
             return e
 
     def __call__(self, request): # pylint:disable=arguments-differ
         result = TransactionLoop.__call__(self, request)  # not super() for speed
         if  isinstance(result, HTTPException) and \
             getattr(request, '_v_nti_raised_exception', False):
             raise result
```

### Comparing `nti.transactions-4.2.1/src/nti/transactions/queue.py` & `nti.transactions-4.3.0/src/nti/transactions/queue.py`

 * *Files identical despite different names*

### Comparing `nti.transactions-4.2.1/src/nti/transactions/tests/test_loop.py` & `nti.transactions-4.3.0/src/nti/transactions/tests/test_loop.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from hamcrest import has_property
 from hamcrest import none
 from hamcrest import has_items
 from hamcrest import greater_than_or_equal_to
 from hamcrest import contains_exactly as contains
 from hamcrest import contains_string
 
-import fudge
+
 
 from nti.testing.matchers import is_true
 from nti.testing.matchers import is_false
 from nti.testing.matchers import has_length
 from nti.testing.matchers import validly_provides
 
 from ..interfaces import CommitFailedError
@@ -55,29 +55,36 @@
 from perfmetrics.testing.matchers import is_counter
 from perfmetrics import statsd_client_stack
 
 from ZODB import DB
 from ZODB.DemoStorage import DemoStorage
 from ZODB.POSException import StorageError
 
+try:
+    from unittest import mock
+except ImportError:
+    import mock
+
 
 if str is bytes:
     # The Python 2 version of hamcrest has a bug
     # where it assumes the mismatch_description is
     # not None in one branch.
     from hamcrest.core.core.allof import AllOf
     from hamcrest.core.string_description import StringDescription
     old_func = AllOf.matches.__func__
     def matches(self, item, mismatch_description=None):
         if mismatch_description is None:
             mismatch_description = StringDescription()
+        # pylint:disable-next=too-many-function-args
         return old_func(self, item, mismatch_description)
 
     AllOf.matches = matches
 
+# pylint:disable=protected-access,broad-exception-raised
 
 class Test_Do_Commit(unittest.TestCase):
     class Transaction(object):
         description = u''
         def __init__(self, t=None):
             self.t = t
 
@@ -101,36 +108,36 @@
                     .with_args(
                         self.RaisingCommit(TypeError("A custom message")),
                         '', 0, 0, 0,
                     ),
                     raises(CommitFailedError, "A custom message"))
 
 
-    @fudge.patch('nti.transactions.loop.logger.exception')
+    @mock.patch('nti.transactions.loop.logger.exception')
     def test_commit_raises_assertion_error(self, fake_logger):
-        fake_logger.expects_call()
-
         assert_that(calling(_do_commit)
                     .with_args(
                         self.RaisingCommit(AssertionError), '', 0, 0, 0
                     ),
                     raises(AssertionError))
+        fake_logger.assert_called_once()
+
 
-    @fudge.patch('nti.transactions.loop.logger.exception')
+    @mock.patch('nti.transactions.loop.logger.exception')
     def test_commit_raises_value_error(self, fake_logger):
         fake_logger.expects_call()
 
         assert_that(calling(_do_commit)
                     .with_args(
                         self.RaisingCommit(ValueError),
                         '', 0, 0, 0,
                     ),
                     raises(ValueError))
 
-    @fudge.patch('nti.transactions.loop.logger.exception')
+    @mock.patch('nti.transactions.loop.logger.exception')
     def test_commit_raises_custom_error(self, fake_logger):
         fake_logger.expects_call()
 
         class MyException(Exception):
             pass
 
         try:
@@ -139,42 +146,44 @@
             assert_that(calling(_do_commit)
                         .with_args(
                             self.RaisingCommit(ValueError),
                             '', 0, 0, 0
                         ),
                         raises(MyException))
 
-    @fudge.patch('nti.transactions.loop.logger.log')
+    @mock.patch('nti.transactions.loop.logger.log')
     def test_commit_clean_but_long(self, fake_logger):
         fake_logger.expects_call()
         _do_commit(self.RaisingCommit(None), -1, 0, 0)
 
 
-    @fudge.patch('nti.transactions.loop.logger.isEnabledFor',
-                 'nti.transactions.loop.logger.log')
+
+    @mock.patch('nti.transactions.loop.logger.log')
+    @mock.patch('nti.transactions.loop.logger.isEnabledFor')
     def test_commit_duration_logging_short(self, fake_is_enabled, fake_log):
-        fake_is_enabled.expects_call().returns(True).with_args(logging.DEBUG)
-        fake_log.expects_call()
+        def enabled(lvl):
+            return lvl == logging.DEBUG
+        fake_is_enabled.side_effect = enabled
+
         _do_commit(self.Transaction(), 6, 0, 0)
+        fake_log.assert_called_once()
 
-    @fudge.patch('nti.transactions.loop.logger.isEnabledFor',
-                 'nti.transactions.loop.logger.log')
+    @mock.patch('nti.transactions.loop.logger.log')
+    @mock.patch('nti.transactions.loop.logger.isEnabledFor')
     def test_commit_duration_logging_long(self, fake_is_enabled, fake_log):
-        fake_is_enabled.expects_call().returns(True).with_args(logging.WARNING)
-        fake_log.expects_call()
-        fake_perf_counter = fudge.Fake(
-        ).expects_call(
-        ).returns(
-            0
-        ).next_call(
-        ).returns(
-            10
-        )
+        def enabled(lvl):
+            return lvl == logging.WARNING
+        fake_is_enabled.side_effect = enabled
+        perfs = [10, 0]
+        def perf():
+            return perfs.pop()
+        fake_perf_counter = mock.MagicMock()
+        fake_perf_counter.side_effect = perf
         _do_commit(self.Transaction(), 6, 0, 0, _perf_counter=fake_perf_counter)
-
+        fake_log.assert_called_once()
 
 class TrueStatsDClient(FakeStatsDClient):
     # https://github.com/zodb/perfmetrics/issues/23
     def __bool__(self):
         return True
     __nonzero__ = __bool__
 
@@ -194,19 +203,21 @@
         zope.event.subscribers.append(self.events.append)
 
     def tearDown(self):
         statsd_client_stack.pop()
         zope.event.subscribers.remove(self.events.append)
         transaction.manager.clearSynchs()
 
-    @fudge.patch('nti.transactions.loop._do_commit')
+    @mock.patch('nti.transactions.loop._do_commit')
     def test_trivial(self, fake_commit):
         class Any(object):
             def __eq__(self, other):
                 return True
+            def __hash__(self):
+                return 42
 
         loop = TransactionLoop(lambda a: a, retries=1, long_commit_duration=1, sleep=1)
         r = repr(loop)
         assert_that(r, contains_string('sleep=1'))
         assert_that(r, contains_string('long_commit_duration=1'))
         assert_that(r, contains_string('attempts=2'))
         fake_commit.expects_call().with_args(
@@ -346,14 +357,15 @@
 
         assert_that(calling(TransactionLoop(handler)), raises(ForeignTransactionError))
         assert_that(transaction.manager.manager, has_property('_txn', is_(none())))
 
     def test_setup_teardown(self):
 
         class Loop(TransactionLoop):
+            # false positive pylint:disable=arguments-differ
             setupcalled = teardowncalled = False
             def setUp(self):
                 assert_that(transaction.manager, has_property('explicit', is_true()))
                 self.setupcalled = True
             def tearDown(self):
                 self.teardowncalled = True
 
@@ -457,41 +469,41 @@
         assert_that(self.events[-3], is_(WillSleepBetweenAttempts))
         assert_that(self.events[-1], validly_provides(IWillRetryAttempt))
         assert_that(self.events[-2], validly_provides(IAfterTransactionBegan))
         assert_that(self.events[-3], validly_provides(IWillSleepBetweenAttempts))
 
         assert_that(self.events[-3], has_property('sleep_time', 3.1))
 
-    @fudge.patch('transaction._manager.TransactionManager.begin',
-                 'transaction._manager.TransactionManager.get')
+
+    @mock.patch('transaction._manager.TransactionManager.get', autospec=True)
+    @mock.patch('transaction._manager.TransactionManager.begin', autospec=True)
     def test_note(self, fake_begin, fake_get):
-        fake_tx = fudge.Fake()
-        (fake_tx
-         .expects('note').with_args(u'Hi')
-         .expects('nti_abort')
-         .provides('isDoomed').returns(True))
-        fake_begin.expects_call().returns(fake_tx)
-        fake_get.expects_call().returns(fake_tx)
+        fake_tx = mock.MagicMock()
+        fake_tx.isDoomed.return_value = True
+        fake_begin.return_value = fake_tx
+        fake_get.return_value = fake_tx
+
         class Loop(TransactionLoop):
             def describe_transaction(self, *args, **kwargs):
                 return u"Hi"
 
         result = Loop(lambda: 42)()
         assert_that(result, is_(42))
+        fake_tx.note.assert_called_with(u'Hi')
+        fake_tx.nti_abort.assert_called_once()
 
 
-    @fudge.patch('transaction._manager.TransactionManager.begin',
-                 'transaction._manager.TransactionManager.get')
-    def test_abort_no_side_effect(self, fake_begin, fake_get):
-        fake_tx = fudge.Fake()
-        fake_tx.expects('nti_abort')
-        fake_tx.has_attr(_resources=())
+    @mock.patch('transaction._manager.TransactionManager.begin', autospec=True)
+    @mock.patch('transaction._manager.TransactionManager.get', autospec=True)
+    def test_abort_no_side_effect(self, fake_get, fake_begin):
+        fake_tx = mock.MagicMock()
+        fake_tx._resources = () # pylint:disable=protected-access
 
-        fake_begin.expects_call().returns(fake_tx)
-        fake_get.expects_call().returns(fake_tx)
+        fake_begin.return_value = fake_tx
+        fake_get.return_value = fake_tx
 
 
         class Loop(TransactionLoop):
             side_effect_free = True
 
         result = Loop(lambda: 42)()
         assert_that(result, is_(42))
@@ -501,17 +513,23 @@
                         is_counter(name='transaction.side_effect_free', value=1)))
         assert_that(observations,
                     does_not(
                         has_items(
                             is_counter(name='transaction.side_effect_free_violation')
                         )))
 
-    @fudge.test
+        fake_tx.nti_abort.assert_called_once()
+
     def test_abort_no_side_effect_violation(self):
-        fake_manager = fudge.Fake().is_a_stub()
+        class Mock(mock.MagicMock):
+            def __str__(self):
+                return 'fake:fake_manager'
+            __repr__ = __str__
+
+        fake_manager = Mock()
 
         class Loop(TransactionLoop):
             side_effect_free = True
 
         def handler():
             transaction.get().join(fake_manager)
 
@@ -541,15 +559,15 @@
 
         ex = exc.exception
         assert_that(str(ex),
                     is_("Transaction that was supposed to be side-effect free "
                         "had resource managers (count=1)."))
 
 
-    @fudge.patch('transaction._transaction.Transaction.nti_abort')
+    @mock.patch('transaction._transaction.Transaction.nti_abort')
     def test_abort_doomed(self, fake_abort):
         fake_abort.expects_call()
 
         def handler():
             assert_that(transaction.manager.explicit, is_true())
             transaction.get().doom()
             return 42
@@ -557,72 +575,76 @@
         result = TransactionLoop(handler)()
         assert_that(result, is_(42))
         observations = self.statsd_client.observations
         assert_that(observations,
                     has_items(
                         is_counter(name='transaction.doomed', value=1)))
 
-    @fudge.patch('transaction._manager.TransactionManager.begin',
-                 'transaction._manager.TransactionManager.get')
+
+    @mock.patch('transaction._manager.TransactionManager.get')
+    @mock.patch('transaction._manager.TransactionManager.begin')
     def test_abort_veto(self, fake_begin, fake_get):
-        fake_tx = fudge.Fake()
-        fake_tx.expects('nti_abort')
-        fake_tx.provides('isDoomed').returns(False)
+        fake_tx = mock.MagicMock()
+        fake_tx.isDoomed.return_value = False
 
-        fake_begin.expects_call().returns(fake_tx)
-        fake_get.expects_call().returns(fake_tx)
+        fake_begin.return_value = fake_tx
+        fake_get.return_value = fake_tx
 
         class Loop(TransactionLoop):
             def should_veto_commit(self, result, *args, **kwargs):
                 assert_that(result, is_(42))
                 return True
 
         result = Loop(lambda: 42)()
         assert_that(result, is_(42))
         observations = self.statsd_client.observations
         assert_that(observations,
                     has_items(
                         is_counter(name='transaction.vetoed', value=1)))
 
-    @fudge.patch('transaction._manager.TransactionManager.begin',
-                 'sys.stderr')
-    def test_abort_systemexit(self, fake_begin, fake_stderr):
-        fake_tx = fudge.Fake()
-        fake_tx.expects('abort').raises(ValueError)
-        fake_tx.provides('isDoomed').returns(False)
+        fake_tx.nti_abort.assert_called_once()
 
-        fake_begin.expects_call().returns(fake_tx)
-        fake_stderr.provides('write')
+
+    @mock.patch('transaction._manager.TransactionManager.begin', autospec=True)
+    @mock.patch('sys.stderr', autospec=True)
+    def test_abort_systemexit(self, fake_begin, _fake_stderr):
+        fake_tx = mock.MagicMock()
+        fake_tx.abort.side_effect = ValueError
+        fake_tx.isDoomed.return_value = False
+
+        fake_begin.return_value = fake_tx
 
         def handler():
             raise SystemExit()
 
         loop = TransactionLoop(handler)
         try:
             loop()
             self.fail("Should raise SystemExit") # pragma: no cover
         except SystemExit:
             pass
 
-    @fudge.patch('transaction._manager.TransactionManager.begin',
-                 'nti.transactions.loop.logger.exception',
-                 'nti.transactions.loop.logger.warning')
+
+    @mock.patch('nti.transactions.loop.logger.exception', side_effect=ValueError)
+    @mock.patch('nti.transactions.loop.logger.warning', side_effect=ValueError)
+    @mock.patch('transaction._manager.TransactionManager.begin',)
     def test_abort_exception_raises(self, fake_begin,
-                                    fake_logger, fake_format):
+                                    _fake_logger, _fake_format):
         # begin() returns an object without abort(), which we catch.
-        fake_begin.expects_call().returns_fake()
-
         # Likewise for the things we try to do to log it
-        fake_logger.expects_call().raises(ValueError)
-        fake_format.expects_call().raises(ValueError)
+        fake_begin.return_value = object()
 
         def handler():
             raise Exception()
         loop = TransactionLoop(handler)
-        assert_that(calling(loop), raises(AbortFailedError))
+        with self.assertRaises(AbortFailedError):
+
+
+            loop()
+
 
     def test_abort_on_exception_logs_exception_str(self):
         from zope.testing.loggingsupport import InstalledHandler
         from ZODB.POSException import ConflictError
         import pickle
         logs = InstalledHandler("nti.transactions.loop")
         self.addCleanup(logs.uninstall)
```

### Comparing `nti.transactions-4.2.1/src/nti/transactions/tests/test_manager.py` & `nti.transactions-4.3.0/src/nti/transactions/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `nti.transactions-4.2.1/src/nti/transactions/tests/test_pyramid_tween.py` & `nti.transactions-4.3.0/src/nti/transactions/tests/test_pyramid_tween.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from nti.testing.matchers import has_attr
 from nti.testing.matchers import has_length
 from nti.testing.matchers import validly_provides
 
 from .. import pyramid_tween
 from .._httpexceptions import HTTPBadRequest
 
+# pylint:disable=protected-access,unnecessary-lambda-assignment
 
 class MockRequest(object):
 
     method = 'GET'
     url = '/foo/bar'
     content_type = 'text/plain'
     body = None
```

### Comparing `nti.transactions-4.2.1/src/nti/transactions/tests/test_queue.py` & `nti.transactions-4.3.0/src/nti/transactions/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `nti.transactions-4.2.1/src/nti/transactions/tests/test_transactions.py` & `nti.transactions-4.3.0/src/nti/transactions/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `nti.transactions-4.2.1/src/nti/transactions/transactions.py` & `nti.transactions-4.3.0/src/nti/transactions/transactions.py`

 * *Files identical despite different names*

### Comparing `nti.transactions-4.2.1/src/nti.transactions.egg-info/PKG-INFO` & `nti.transactions-4.3.0/src/nti.transactions.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,285 +1,293 @@
 Metadata-Version: 2.1
 Name: nti.transactions
-Version: 4.2.1
+Version: 4.3.0
 Summary: NTI Transactions Utility
-Home-page: https://github.com/NextThought/nti.transactions
+Home-page: https://github.com/OpenNTI/nti.transactions
 Author: Jason Madden
 Author-email: jason@nextthought.com
 License: Apache
-Description: ==================
-         nti.transactions
-        ==================
-        
-        
-        .. _transaction: https://pypi.python.org/pypi/transaction
-        
-        .. image:: https://coveralls.io/repos/github/NextThought/nti.transactions/badge.svg?branch=master
-        	:target: https://coveralls.io/github/NextThought/nti.transactions?branch=master
-        
-        .. image:: https://github.com/NextThought/nti.transactions/workflows/tests/badge.svg
-           :target: https://github.com/NextThought/nti.transactions/actions?query=workflow%3Atests
-        
-        .. image:: https://readthedocs.org/projects/ntitransactions/badge/?version=latest
-           :target: https://ntitransactions.readthedocs.io/en/latest/?badge=latest
-           :alt: Documentation Status
-        
-        Extensions to the `transaction`_ package.
-        
-        .. contents::
-        
-        
-        Transaction Management
-        ======================
-        
-        ``nti.transactions.loop.TransactionsLoop`` is a retryable
-        transaction manager. It is conceptually similar to the `attempts`_
-        context manager provided by the transaction package itself, but much
-        more powerful and extensible via subclasses. Features include:
-        
-        - Configurable commit vetos.
-        - Extensible tests for which exceptions should be retried.
-        - The ability to abort the transaction and bypass a potentially
-          expensive commit when there are expected to be no side-effects.
-        - Sleeping between retries.
-        - Extensive logging and timing.
-        
-        The TransactionLoop can be used as-is, or it can be subclassed for
-        customization. For use in a Pyramid tween, for example, a minimal
-        subclass might look like this (see ``nti.transactions.pyramid_tween``
-        for a full-featured tween)::
-        
-          >>> class PyramidTransactionLoop(TransactionLoop):
-          ...    def prep_for_retry(self, number, request):
-          ...        request.make_body_seekable()
-          ...    def describe_transaction(self, request):
-          ...        return request.url
-        
-        Data Managers
-        =============
-        
-        A few `data managers`_ are provided for convenience.
-        
-        The first data manager is used to put an object in a ``queue``
-        (something with the ``full`` and ``put_nowait`` methods) when a
-        transaction succeeds. If the queue is full, then the transaction will
-        not be allowed to commit::
-        
-          >>> from nti.transactions.queue import put_nowait
-          >>> put_nowait(queue, object)
-        
-        This is a special case of the ``ObjectDataManager``, which will call
-        one method with any arguments when a transaction commits. It can be
-        configured to vote on whether the transaction should be allowed to commit.
-        or not. This is useful for, say, putting an item in a Redis queue when
-        the transaction is successful. It can be constructed directly, but the
-        ``do`` function is a shorthand way of joining one to the current
-        transaction::
-        
-          >>> from nti.transactions.manager import do
-          >>> do(print, args=("Committed"))
-        
-        .. caution:: See the documentation of this object for numerous
-        	     warnings about side-effects and its interaction with the
-        	     transaction machinery. Use it with care!
-        
-        .. _attempts: http://zodb.readthedocs.io/en/latest/transactions.html#retrying-transactions
-        .. _data managers: http://zodb.readthedocs.io/en/latest/transactions.html#data-managers
-        
-        =========
-         Changes
-        =========
-        
-        4.2.1 (2021-05-25)
-        ==================
-        
-        - When aborting a transaction due to an exception, log the exception
-          instead of just the exception type (twice). Exception messages can
-          be very helpful in understanding exactly what went wrong and
-          possibly how to fix it for transient errors (e.g., a
-          ``ZODB.POSException.ConflictError`` includes the object ID and
-          class, which can be used to reduce the conflicts). This makes the
-          logging slightly more expensive (when enabled). See `PR 58
-          <https://github.com/NextThought/nti.transactions/pull/58>`_.
-        
-        
-        4.2.0 (2021-02-11)
-        ==================
-        
-        - Add support for Python 3.9.
-        - Move CI from Travis CI to Github Actions.
-        - When the Pyramid tween retries, any volatile attributes (those
-          beginning with ``_v_``) in the request dictionary are deleted. This
-          is inspired by ``persistent`` and meant to facilitate safe caching.
-          When compared to events sent by the transaction loop, there is no
-          specified order. See `issue 54 <https://github.com/NextThought/nti.transactions/issues/54>`_.
-        - Fix various event classes not properly specifying the interface they
-          implement. For example, ``WillFirstAttempt`` now properly implements
-          ``IWillFirstAttempt``, and ``WilLRetryAttempt`` now properly
-          implements ``IWillRetryAttempt``. See `issue 52
-          <https://github.com/NextThought/nti.transactions/issues/52>`_.
-        - Add ``IWillLastAttempt`` as a subclass of ``IWillRetryAttempt`` and
-          the last event emitted.
-        - The Pyramid tween now emits ``IWillRetryAttemptWithRequest``, et al,
-          to provide simple access to the request object.
-        
-        4.1.0 (2020-07-22)
-        ==================
-        
-        - Add logging to the pyramid tween transaction factory to show the
-          settings that are in use.
-        - Add ``TransactionLoop.side_effect_free_log_level``, and change the
-          default value to DEBUG. It is useful to set this to ERROR or higher
-          in tests.
-        - Add ``TransactionLoop.side_effect_free_resource_limit``.
-        
-        
-        4.0.1 (2020-07-18)
-        ==================
-        
-        - Add missing dependency on zope.event.
-        - Fix raising ``AlreadyInTransaction`` error on the second and
-          subsequent calls to a loop when a transaction synchronizer raises an
-          error on the first call. See `issue 49
-          <https://github.com/NextThought/nti.transactions/issues/49>`_.
-        
-        4.0.0 (2019-12-13)
-        ==================
-        
-        - Require at least version 3.0 of the ``transaction`` package.
-        
-        - Drop dependency on the ``dm.transaction.aborthook`` package. That
-          functionality is now natively provided in transaction 3.0.
-        
-        
-        3.1.1 (2019-12-10)
-        ==================
-        
-        - Fix logging of long duration commits. See `issue 44
-          <https://github.com/NextThought/nti.transactions/issues/44>`_.
-        
-        - Add logging and a metric
-          (``transaction.side_effect_free_violation``) for transactions that
-          claim to have no side effects, but which actually result in joined
-          resource managers. This can indicate unnecessarily throwing away
-          work. See `issue 45 <https://github.com/NextThought/nti.transactions/issues/45>`_.
-        
-        
-        3.1.0 (2019-11-29)
-        ==================
-        
-        - Add support for Python 3.8.
-        
-        - Refactor internal implementation details. Instead of importing
-          everything from ``nti.transactions.transactions``, more specific
-          modules are used to group objects by function. The old imports
-          continue to work. In 4.0 they will generate a deprecation warning
-          and in 5.0 they will be removed.
-        
-        - Add a Pyramid tween to manage transactions and transaction retries.
-          Various settings can be configured as Pyramid deployment settings
-          (e.g., in the ini file).
-        
-        - Make the transaction loop increase the time it sleeps between
-          retries following the `random binary exponential backoff algorithm
-          <https://en.wikipedia.org/wiki/Exponential_backoff>`_ used by Ethernet.
-        
-        - Reduce the default number of attempts to 4 (one attempt and 3
-          retries). See `issue 35 <https://github.com/NextThought/nti.transactions/issues/35>`_.
-        
-        - Make the transaction loop emit more metrics. See `issue 31
-          <https://github.com/NextThought/nti.transactions/issues/31>`_.
-        
-        - Make commit logging now always happen at least at the debug level,
-          escalating to warning for long commits. It also includes the number
-          of retries taken and the amount of time spent sleeping. See `issue
-          32 <https://github.com/NextThought/nti.transactions/issues/32>`_.
-        
-        - Make the transaction loop emit events (using ``zope.event``) at certain parts of the
-          transaction lifecycle. See `issue 33 <https://github.com/NextThought/nti.transactions/issues/33>`_.
-        
-        3.0.0 (2019-09-06)
-        ==================
-        
-        - Make ``TransactionLoop`` place its transaction manager in explicit
-          mode. This can be faster and is easier to reason about, but forbids
-          the called handler from manually calling ``begin()``, ``abort()`` or
-          ``commit()``. See `issue 20
-          <https://github.com/NextThought/nti.transactions/issues/20>`_.
-        
-        - Move ``transaction.begin()`` out of the block of code that is
-          retried. Previously, an error there would probably be raised
-          *anyway* and not retried, unless a subclass had made customizations.
-        
-        - Add ``setUp`` and ``tearDown`` methods to TransactionLoop to give
-          subclasses a place to hook into the inners of the transaction loop.
-          This is particularly helpful if they need to do something after the
-          transaction manager has been put in explicit mode. See `issue 22
-          <https://github.com/NextThought/nti.transactions/issues/22>`_.
-        
-        2.0.1 (2019-09-03)
-        ==================
-        
-        - Fix compatibility with perfmetrics 3.0: drop ``from __future__
-          import unicode_literals``.
-        
-        
-        2.0.0 (2018-07-20)
-        ==================
-        
-        - Use the new public ``isRetryableError`` in transaction 2.2. The
-          interface for this package is unchanged, but a major version bump of
-          a dependency necessitates a major bump here. See `issue 12
-          <https://github.com/NextThought/nti.transactions/issues/12>`_.
-        
-        - Test support for Python 3.7; remove test support for Python 3.4.
-        
-        - ``TransactionLoop`` is more careful to not keep traceback objects
-          around, especially on Python 2.
-        
-        1.1.1 (2018-07-19)
-        ==================
-        
-        - When the ``TransactionLoop`` raises a ``CommitFailedError`` from a
-          ``TypeError``, it preserves the original message.
-        
-        - Test support for Python 3.6.
-        
-        1.1.0 (2017-04-17)
-        ==================
-        
-        - Add a new ObjectDataManager that will attempt to execute after
-          other ObjectDataManagers.
-        
-        
-        1.0.0 (2016-07-28)
-        ==================
-        
-        - Add support for Python 3.
-        - Eliminate ZODB dependency. Instead of raising a
-          ``ZODB.POSException.StorageError`` for unexpected ``TypeErrors``
-          during commit, the new class
-          ``nti.transactions.interfaces.CommitFailedError`` is raised.
-        - Introduce a new subclass of ``TransactionError``,
-          ``AbortFailedError`` that is raised when an abort fails due to a
-          system error.
-        
 Keywords: ZODB transaction
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: ZODB
 Provides-Extra: test
 Provides-Extra: gevent
 Provides-Extra: docs
 Provides-Extra: pyramid
+License-File: LICENSE
+
+==================
+ nti.transactions
+==================
+
+
+.. _transaction: https://pypi.python.org/pypi/transaction
+
+.. image:: https://coveralls.io/repos/github/NextThought/nti.transactions/badge.svg?branch=master
+	:target: https://coveralls.io/github/NextThought/nti.transactions?branch=master
+
+.. image:: https://github.com/NextThought/nti.transactions/workflows/tests/badge.svg
+   :target: https://github.com/NextThought/nti.transactions/actions?query=workflow%3Atests
+
+.. image:: https://readthedocs.org/projects/ntitransactions/badge/?version=latest
+   :target: https://ntitransactions.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
+Extensions to the `transaction`_ package.
+
+
+
+Transaction Management
+======================
+
+``nti.transactions.loop.TransactionsLoop`` is a retryable
+transaction manager. It is conceptually similar to the `attempts`_
+context manager provided by the transaction package itself, but much
+more powerful and extensible via subclasses. Features include:
+
+- Configurable commit vetos.
+- Extensible tests for which exceptions should be retried.
+- The ability to abort the transaction and bypass a potentially
+  expensive commit when there are expected to be no side-effects.
+- Sleeping between retries.
+- Extensive logging and timing.
+
+The TransactionLoop can be used as-is, or it can be subclassed for
+customization. For use in a Pyramid tween, for example, a minimal
+subclass might look like this (see ``nti.transactions.pyramid_tween``
+for a full-featured tween)::
+
+  >>> class PyramidTransactionLoop(TransactionLoop):
+  ...    def prep_for_retry(self, number, request):
+  ...        request.make_body_seekable()
+  ...    def describe_transaction(self, request):
+  ...        return request.url
+
+Data Managers
+=============
+
+A few `data managers`_ are provided for convenience.
+
+The first data manager is used to put an object in a ``queue``
+(something with the ``full`` and ``put_nowait`` methods) when a
+transaction succeeds. If the queue is full, then the transaction will
+not be allowed to commit::
+
+  >>> from nti.transactions.queue import put_nowait
+  >>> put_nowait(queue, object)
+
+This is a special case of the ``ObjectDataManager``, which will call
+one method with any arguments when a transaction commits. It can be
+configured to vote on whether the transaction should be allowed to commit.
+or not. This is useful for, say, putting an item in a Redis queue when
+the transaction is successful. It can be constructed directly, but the
+``do`` function is a shorthand way of joining one to the current
+transaction::
+
+  >>> from nti.transactions.manager import do
+  >>> do(print, args=("Committed"))
+
+.. caution:: See the documentation of this object for numerous
+	     warnings about side-effects and its interaction with the
+	     transaction machinery. Use it with care!
+
+.. _attempts: http://zodb.readthedocs.io/en/latest/transactions.html#retrying-transactions
+.. _data managers: http://zodb.readthedocs.io/en/latest/transactions.html#data-managers
+
+=========
+ Changes
+=========
+
+4.3.0 (2023-05-05)
+==================
+
+- Add support for Python 3.10 and 3.11.
+
+
+4.2.1 (2021-05-25)
+==================
+
+- When aborting a transaction due to an exception, log the exception
+  instead of just the exception type (twice). Exception messages can
+  be very helpful in understanding exactly what went wrong and
+  possibly how to fix it for transient errors (e.g., a
+  ``ZODB.POSException.ConflictError`` includes the object ID and
+  class, which can be used to reduce the conflicts). This makes the
+  logging slightly more expensive (when enabled). See `PR 58
+  <https://github.com/NextThought/nti.transactions/pull/58>`_.
+
+
+4.2.0 (2021-02-11)
+==================
+
+- Add support for Python 3.9.
+- Move CI from Travis CI to Github Actions.
+- When the Pyramid tween retries, any volatile attributes (those
+  beginning with ``_v_``) in the request dictionary are deleted. This
+  is inspired by ``persistent`` and meant to facilitate safe caching.
+  When compared to events sent by the transaction loop, there is no
+  specified order. See `issue 54 <https://github.com/NextThought/nti.transactions/issues/54>`_.
+- Fix various event classes not properly specifying the interface they
+  implement. For example, ``WillFirstAttempt`` now properly implements
+  ``IWillFirstAttempt``, and ``WilLRetryAttempt`` now properly
+  implements ``IWillRetryAttempt``. See `issue 52
+  <https://github.com/NextThought/nti.transactions/issues/52>`_.
+- Add ``IWillLastAttempt`` as a subclass of ``IWillRetryAttempt`` and
+  the last event emitted.
+- The Pyramid tween now emits ``IWillRetryAttemptWithRequest``, et al,
+  to provide simple access to the request object.
+
+4.1.0 (2020-07-22)
+==================
+
+- Add logging to the pyramid tween transaction factory to show the
+  settings that are in use.
+- Add ``TransactionLoop.side_effect_free_log_level``, and change the
+  default value to DEBUG. It is useful to set this to ERROR or higher
+  in tests.
+- Add ``TransactionLoop.side_effect_free_resource_limit``.
+
+
+4.0.1 (2020-07-18)
+==================
+
+- Add missing dependency on zope.event.
+- Fix raising ``AlreadyInTransaction`` error on the second and
+  subsequent calls to a loop when a transaction synchronizer raises an
+  error on the first call. See `issue 49
+  <https://github.com/NextThought/nti.transactions/issues/49>`_.
+
+4.0.0 (2019-12-13)
+==================
+
+- Require at least version 3.0 of the ``transaction`` package.
+
+- Drop dependency on the ``dm.transaction.aborthook`` package. That
+  functionality is now natively provided in transaction 3.0.
+
+
+3.1.1 (2019-12-10)
+==================
+
+- Fix logging of long duration commits. See `issue 44
+  <https://github.com/NextThought/nti.transactions/issues/44>`_.
+
+- Add logging and a metric
+  (``transaction.side_effect_free_violation``) for transactions that
+  claim to have no side effects, but which actually result in joined
+  resource managers. This can indicate unnecessarily throwing away
+  work. See `issue 45 <https://github.com/NextThought/nti.transactions/issues/45>`_.
+
+
+3.1.0 (2019-11-29)
+==================
+
+- Add support for Python 3.8.
+
+- Refactor internal implementation details. Instead of importing
+  everything from ``nti.transactions.transactions``, more specific
+  modules are used to group objects by function. The old imports
+  continue to work. In 4.0 they will generate a deprecation warning
+  and in 5.0 they will be removed.
+
+- Add a Pyramid tween to manage transactions and transaction retries.
+  Various settings can be configured as Pyramid deployment settings
+  (e.g., in the ini file).
+
+- Make the transaction loop increase the time it sleeps between
+  retries following the `random binary exponential backoff algorithm
+  <https://en.wikipedia.org/wiki/Exponential_backoff>`_ used by Ethernet.
+
+- Reduce the default number of attempts to 4 (one attempt and 3
+  retries). See `issue 35 <https://github.com/NextThought/nti.transactions/issues/35>`_.
+
+- Make the transaction loop emit more metrics. See `issue 31
+  <https://github.com/NextThought/nti.transactions/issues/31>`_.
+
+- Make commit logging now always happen at least at the debug level,
+  escalating to warning for long commits. It also includes the number
+  of retries taken and the amount of time spent sleeping. See `issue
+  32 <https://github.com/NextThought/nti.transactions/issues/32>`_.
+
+- Make the transaction loop emit events (using ``zope.event``) at certain parts of the
+  transaction lifecycle. See `issue 33 <https://github.com/NextThought/nti.transactions/issues/33>`_.
+
+3.0.0 (2019-09-06)
+==================
+
+- Make ``TransactionLoop`` place its transaction manager in explicit
+  mode. This can be faster and is easier to reason about, but forbids
+  the called handler from manually calling ``begin()``, ``abort()`` or
+  ``commit()``. See `issue 20
+  <https://github.com/NextThought/nti.transactions/issues/20>`_.
+
+- Move ``transaction.begin()`` out of the block of code that is
+  retried. Previously, an error there would probably be raised
+  *anyway* and not retried, unless a subclass had made customizations.
+
+- Add ``setUp`` and ``tearDown`` methods to TransactionLoop to give
+  subclasses a place to hook into the inners of the transaction loop.
+  This is particularly helpful if they need to do something after the
+  transaction manager has been put in explicit mode. See `issue 22
+  <https://github.com/NextThought/nti.transactions/issues/22>`_.
+
+2.0.1 (2019-09-03)
+==================
+
+- Fix compatibility with perfmetrics 3.0: drop ``from __future__
+  import unicode_literals``.
+
+
+2.0.0 (2018-07-20)
+==================
+
+- Use the new public ``isRetryableError`` in transaction 2.2. The
+  interface for this package is unchanged, but a major version bump of
+  a dependency necessitates a major bump here. See `issue 12
+  <https://github.com/NextThought/nti.transactions/issues/12>`_.
+
+- Test support for Python 3.7; remove test support for Python 3.4.
+
+- ``TransactionLoop`` is more careful to not keep traceback objects
+  around, especially on Python 2.
+
+1.1.1 (2018-07-19)
+==================
+
+- When the ``TransactionLoop`` raises a ``CommitFailedError`` from a
+  ``TypeError``, it preserves the original message.
+
+- Test support for Python 3.6.
+
+1.1.0 (2017-04-17)
+==================
+
+- Add a new ObjectDataManager that will attempt to execute after
+  other ObjectDataManagers.
+
+
+1.0.0 (2016-07-28)
+==================
+
+- Add support for Python 3.
+- Eliminate ZODB dependency. Instead of raising a
+  ``ZODB.POSException.StorageError`` for unexpected ``TypeErrors``
+  during commit, the new class
+  ``nti.transactions.interfaces.CommitFailedError`` is raised.
+- Introduce a new subclass of ``TransactionError``,
+  ``AbortFailedError`` that is raised when an abort fails due to a
+  system error.
```

### Comparing `nti.transactions-4.2.1/src/nti.transactions.egg-info/SOURCES.txt` & `nti.transactions-4.3.0/src/nti.transactions.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 .coveragerc
+.gitignore
 .pylintrc
+.readthedocs.yml
 CHANGES.rst
+COPYRIGHT.txt
 INSTALL
 LICENSE
 MANIFEST.in
 README.rst
 TODO
 babel.cfg
 doc-requirements.txt
@@ -16,15 +19,14 @@
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 src/nti/__init__.py
 src/nti.transactions.egg-info/PKG-INFO
 src/nti.transactions.egg-info/SOURCES.txt
 src/nti.transactions.egg-info/dependency_links.txt
-src/nti.transactions.egg-info/entry_points.txt
 src/nti.transactions.egg-info/namespace_packages.txt
 src/nti.transactions.egg-info/requires.txt
 src/nti.transactions.egg-info/top_level.txt
 src/nti.transactions.egg-info/zip-safe
 src/nti/transactions/__init__.py
 src/nti/transactions/_httpexceptions.py
 src/nti/transactions/_loglevels.py
```

