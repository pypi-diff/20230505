# Comparing `tmp/swh.journal-1.3.2.tar.gz` & `tmp/swh.journal-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.journal-1.3.2.tar", last modified: Thu May  4 09:42:11 2023, max compression
+gzip compressed data, was "dist/swh.journal-1.3.3.tar", last modified: Fri May  5 11:43:48 2023, max compression
```

## Comparing `swh.journal-1.3.2.tar` & `swh.journal-1.3.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-04 09:42:08.000000 swh.journal-1.3.2/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-05-04 09:42:08.000000 swh.journal-1.3.2/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-04 09:42:08.000000 swh.journal-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-04 09:42:08.000000 swh.journal-1.3.2/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-04 09:42:08.000000 swh.journal-1.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-05-04 09:42:08.000000 swh.journal-1.3.2/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-04 09:42:08.000000 swh.journal-1.3.2/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-05-04 09:42:08.000000 swh.journal-1.3.2/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-04 09:42:08.000000 swh.journal-1.3.2/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-05-04 09:42:11.000000 swh.journal-1.3.2/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      767 2023-05-04 09:42:08.000000 swh.journal-1.3.2/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/example-journal-client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      344 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3204 2023-05-04 09:42:08.000000 swh.journal-1.3.2/docs/journal-clients.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      466 2023-05-04 09:42:08.000000 swh.journal-1.3.2/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-04 09:42:08.000000 swh.journal-1.3.2/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-05-04 09:42:08.000000 swh.journal-1.3.2/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-04 09:42:08.000000 swh.journal-1.3.2/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-04 09:42:08.000000 swh.journal-1.3.2/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      277 2023-05-04 09:42:08.000000 swh.journal-1.3.2/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-04 09:42:11.000000 swh.journal-1.3.2/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2336 2023-05-04 09:42:08.000000 swh.journal-1.3.2/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh/journal/
--rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17402 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     7859 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3624 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/serializers.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh/journal/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      521 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/journal_data.py
--rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/log4j.properties
--rw-r--r--   0 jenkins    (115) docker     (999)    18361 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1807 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_inmemory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7988 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2183 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3181 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2465 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/tests/test_stream.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh/journal/writer/
--rw-r--r--   0 jenkins    (115) docker     (999)     2110 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1753 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/inmemory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1156 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9719 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/kafka.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-05-04 09:42:08.000000 swh.journal-1.3.2/swh/journal/writer/stream.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-04 09:42:11.000000 swh.journal-1.3.2/swh.journal.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1246 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      127 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-04 09:42:10.000000 swh.journal-1.3.2/swh.journal.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1539 2023-05-04 09:42:08.000000 swh.journal-1.3.2/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-05 11:43:46.000000 swh.journal-1.3.3/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-05-05 11:43:46.000000 swh.journal-1.3.3/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-05 11:43:46.000000 swh.journal-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-05 11:43:46.000000 swh.journal-1.3.3/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-05 11:43:46.000000 swh.journal-1.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-05-05 11:43:46.000000 swh.journal-1.3.3/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-05 11:43:46.000000 swh.journal-1.3.3/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-05-05 11:43:46.000000 swh.journal-1.3.3/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-05 11:43:46.000000 swh.journal-1.3.3/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-05-05 11:43:48.000000 swh.journal-1.3.3/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      767 2023-05-05 11:43:46.000000 swh.journal-1.3.3/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/example-journal-client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      344 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3204 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/journal-clients.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      466 2023-05-05 11:43:46.000000 swh.journal-1.3.3/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-05 11:43:46.000000 swh.journal-1.3.3/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-05-05 11:43:46.000000 swh.journal-1.3.3/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-05 11:43:46.000000 swh.journal-1.3.3/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-05 11:43:46.000000 swh.journal-1.3.3/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      382 2023-05-05 11:43:46.000000 swh.journal-1.3.3/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-05 11:43:48.000000 swh.journal-1.3.3/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2336 2023-05-05 11:43:46.000000 swh.journal-1.3.3/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh/journal/
+-rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17402 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     7859 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3624 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/serializers.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh/journal/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      521 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/journal_data.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/log4j.properties
+-rw-r--r--   0 jenkins    (115) docker     (999)    18361 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1807 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_inmemory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7988 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2183 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3181 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2465 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_stream.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh/journal/writer/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2110 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1753 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/inmemory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1156 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9719 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/kafka.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/stream.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1246 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1539 2023-05-05 11:43:46.000000 swh.journal-1.3.3/tox.ini
```

### Comparing `swh.journal-1.3.2/.pre-commit-config.yaml` & `swh.journal-1.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/CODE_OF_CONDUCT.md` & `swh.journal-1.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/LICENSE` & `swh.journal-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/PKG-INFO` & `swh.journal-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.3.2
+Version: 1.3.3
 Summary: Software Heritage Journal utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DJNL/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-journal
```

### Comparing `swh.journal-1.3.2/README.md` & `swh.journal-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/docs/example-journal-client.py` & `swh.journal-1.3.3/docs/example-journal-client.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/docs/journal-clients.rst` & `swh.journal-1.3.3/docs/journal-clients.rst`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/setup.py` & `swh.journal-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/client.py` & `swh.journal-1.3.3/swh/journal/client.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/pytest_plugin.py` & `swh.journal-1.3.3/swh/journal/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/serializers.py` & `swh.journal-1.3.3/swh/journal/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/tests/journal_data.py` & `swh.journal-1.3.3/swh/journal/tests/journal_data.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/tests/test_client.py` & `swh.journal-1.3.3/swh/journal/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/tests/test_inmemory.py` & `swh.journal-1.3.3/swh/journal/tests/test_inmemory.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/tests/test_kafka_writer.py` & `swh.journal-1.3.3/swh/journal/tests/test_kafka_writer.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/tests/test_pytest_plugin.py` & `swh.journal-1.3.3/swh/journal/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/tests/test_serializers.py` & `swh.journal-1.3.3/swh/journal/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/tests/test_stream.py` & `swh.journal-1.3.3/swh/journal/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/writer/__init__.py` & `swh.journal-1.3.3/swh/journal/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/writer/inmemory.py` & `swh.journal-1.3.3/swh/journal/writer/inmemory.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/writer/interface.py` & `swh.journal-1.3.3/swh/journal/writer/interface.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/writer/kafka.py` & `swh.journal-1.3.3/swh/journal/writer/kafka.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh/journal/writer/stream.py` & `swh.journal-1.3.3/swh/journal/writer/stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/swh.journal.egg-info/PKG-INFO` & `swh.journal-1.3.3/swh.journal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.3.2
+Version: 1.3.3
 Summary: Software Heritage Journal utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DJNL/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-journal
```

### Comparing `swh.journal-1.3.2/swh.journal.egg-info/SOURCES.txt` & `swh.journal-1.3.3/swh.journal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.2/tox.ini` & `swh.journal-1.3.3/tox.ini`

 * *Files identical despite different names*

