# Comparing `tmp/autosubmitconfigparser-1.0.27.tar.gz` & `tmp/autosubmitconfigparser-1.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmitconfigparser-1.0.27.tar", last modified: Tue May  2 09:16:02 2023, max compression
+gzip compressed data, was "autosubmitconfigparser-1.0.28.tar", last modified: Fri May  5 11:22:21 2023, max compression
```

## Comparing `autosubmitconfigparser-1.0.27.tar` & `autosubmitconfigparser-1.0.28.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:16:02.150137 autosubmitconfigparser-1.0.27/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-09-23 10:01:03.000000 autosubmitconfigparser-1.0.27/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.27/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-05-02 09:16:02.150137 autosubmitconfigparser-1.0.27/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.27/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        6 2023-05-02 09:15:43.000000 autosubmitconfigparser-1.0.27/VERSION
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmitconfigparser-1.0.27/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:16:02.146137 autosubmitconfigparser-1.0.27/autosubmitconfigparser/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:16:02.146137 autosubmitconfigparser-1.0.27/autosubmitconfigparser/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      162 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/__pycache__/__init__.cpython-37.pyc
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:16:02.146137 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:16:02.146137 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      169 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4187 2022-12-19 09:28:49.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    74789 2023-04-05 09:03:32.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    99981 2023-05-02 08:16:05.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/configcommon.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:16:02.150137 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/autosubmit-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/autosubmit.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/expdef-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/expdef.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/git-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/jobs-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/jobs.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/local-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/platforms-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/platforms.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      408 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/yamlparser.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:16:02.146137 autosubmitconfigparser-1.0.27/autosubmitconfigparser.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-05-02 09:16:02.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1514 2023-05-02 09:16:02.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-05-02 09:16:02.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      305 2023-05-02 09:16:02.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-05-02 09:16:02.000000 autosubmitconfigparser-1.0.27/autosubmitconfigparser.egg-info/top_level.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      591 2022-10-26 08:55:26.000000 autosubmitconfigparser-1.0.27/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:16:02.150137 autosubmitconfigparser-1.0.27/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.27/log/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:16:02.150137 autosubmitconfigparser-1.0.27/log/__pycache__/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      143 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.27/log/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12336 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.27/log/__pycache__/log.cpython-37.pyc
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.27/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.27/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      416 2023-02-07 12:12:28.000000 autosubmitconfigparser-1.0.27/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-05-02 09:16:02.150137 autosubmitconfigparser-1.0.27/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1465 2023-05-02 09:15:43.000000 autosubmitconfigparser-1.0.27/setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1254 2023-01-31 09:30:38.000000 autosubmitconfigparser-1.0.27/test_config.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-09-23 10:01:03.000000 autosubmitconfigparser-1.0.28/CHANGELOG
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.28/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.28/README.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        6 2023-05-04 13:40:57.000000 autosubmitconfigparser-1.0.28/VERSION
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmitconfigparser-1.0.28/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.882628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.886628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      162 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/__pycache__/__init__.cpython-37.pyc
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.886628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.886628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      169 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4187 2022-12-19 09:28:49.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    74789 2023-04-05 09:03:32.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2022-10-26 09:05:46.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/basicconfig.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   100720 2023-05-04 13:02:37.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/configcommon.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.886628 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/autosubmit-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/autosubmit.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/expdef-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/expdef.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/git-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/jobs-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/jobs.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/local-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/platforms-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/platforms.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      408 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/yamlparser.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.882628 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1514 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      314 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-05-05 11:22:21.000000 autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/top_level.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      600 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.28/environment.yml
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.28/log/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/log/__pycache__/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      143 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.28/log/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12336 2022-10-26 14:22:27.000000 autosubmitconfigparser-1.0.28/log/__pycache__/log.cpython-37.pyc
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.28/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.28/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      425 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.28/requeriments.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-05-05 11:22:21.890628 autosubmitconfigparser-1.0.28/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1474 2023-05-05 11:20:51.000000 autosubmitconfigparser-1.0.28/setup.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1254 2023-01-31 09:30:38.000000 autosubmitconfigparser-1.0.28/test_config.py
```

### Comparing `autosubmitconfigparser-1.0.27/PKG-INFO` & `autosubmitconfigparser-1.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.27
+Version: 1.0.28
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.27/README.md` & `autosubmitconfigparser-1.0.28/README.md`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/basicconfig.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/configcommon.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/__pycache__/yamlparser.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/basicconfig.py` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/basicconfig.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/configcommon.py` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/configcommon.py`

 * *Files 1% similar despite different names*

```diff
@@ -621,14 +621,21 @@
                     else:
                         filenames_to_load["PRE"] = custom_conf_directive["PRE"].split(' ')
                 if custom_conf_directive.get('POST', "") != "":
                     if ',' in custom_conf_directive["POST"]:
                         filenames_to_load["POST"] = custom_conf_directive["POST"].split(',')
                     else:
                         filenames_to_load["POST"] = custom_conf_directive["POST"].split(' ')
+        aux_filenames_to_load = filenames_to_load.copy()
+        for file_to_load in aux_filenames_to_load["PRE"]:
+            if file_to_load in self.current_loaded_files:
+                del filenames_to_load[file_to_load]
+        for file_to_load in aux_filenames_to_load["POST"]:
+            if file_to_load in self.current_loaded_files:
+                del filenames_to_load[file_to_load]
         return filenames_to_load
 
     def unify_conf(self,current_data,new_data):
         '''
         Unifies all configuration files into a single dictionary.
         :param current_data: dict with current configuration
         :param new_data: dict with new configuration
@@ -1259,16 +1266,19 @@
     def load_custom_config(self,current_data,filenames_to_load):
         """
         Loads custom config files
         :param current_data: dict with current data
         :param filenames_to_load: list of filenames to load
         :return: current_data_pre,current_data_post with unified data
         """
+
         current_data_pre = {}
         current_data_post = {}
+        if current_data.get('DEFAULT', {}).get('CUSTOM_CONFIG', None) is not None:
+            del current_data["DEFAULT"]["CUSTOM_CONFIG"]
         # at this point, filenames_to_load should be a list of filenames of an specific section PRE or POST.
         for filename in filenames_to_load:
             filename = filename.strip(", ")  # Remove commas and spaces if any
             if filename.startswith("~"):
                 filename = os.path.expanduser(filename)
             current_data["AS_TEMP"] = {}
             current_data["AS_TEMP"]["FILENAME_TO_LOAD"] = filename
@@ -1293,15 +1303,18 @@
                     # Load next level if any
                     custom_conf_directive = current_data.get('DEFAULT', {}).get('CUSTOM_CONFIG', None)
                     filenames_to_load_level = self.parse_custom_conf_directive(custom_conf_directive)
                     if "AS_TEMP" in current_data:
                         del current_data["AS_TEMP"]
                     current_data_pre = self.unify_conf(current_data_pre,self.unify_conf(self.load_custom_config_section(current_data, filenames_to_load_level["PRE"]),current_data))
                     current_data_post = self.unify_conf(current_data_post,self.unify_conf(current_data,self.load_custom_config_section(current_data, filenames_to_load_level["POST"])))
-        return current_data_pre, current_data_post
+        if len(current_data_pre) == 0 and len(current_data_post) == 0:
+            return current_data, current_data
+        else:
+            return current_data_pre, current_data_post
 
     def load_custom_config_section(self,current_data,filenames_to_load):
         """
         Loads a section (PRE or POST ), simple str are also PRE data of the custom config files
         :param current_data: data until now
         :param filenames_to_load: files to load in this section
         :return:
@@ -1345,17 +1358,18 @@
                 non_minimal_conf = self.unify_conf(non_minimal_conf, self.load_config_file(non_minimal_conf, Path(filename)))
             non_minimal_conf = self.load_common_parameters(non_minimal_conf)
             non_minimal_conf = self.substitute_dynamic_variables(non_minimal_conf, max_deep=25)
             # Start loading the custom config files
             # Gets the files to load
             filenames_to_load = self.parse_custom_conf_directive(starter_conf.get("DEFAULT",{}).get("CUSTOM_CONFIG",None))
             # Loads all configuration associated with the project data "pre"
-            custom_conf_pre = self.load_custom_config_section({key:starter_conf[key] for key in ["PROJDIR","ROOTDIR"]},filenames_to_load["PRE"])
+            #custom_conf_pre = self.load_custom_config_section({key:starter_conf[key] for key in ["PROJDIR","ROOTDIR","DEFAULT"]},filenames_to_load["PRE"])
+            custom_conf_pre = self.load_custom_config_section(starter_conf, filenames_to_load["PRE"])
             # Loads all configuration associated with the user data "post"
-            custom_conf_post = self.load_custom_config_section({key:starter_conf[key] for key in ["PROJDIR","ROOTDIR"]},filenames_to_load["POST"])
+            custom_conf_post = self.load_custom_config_section(starter_conf,filenames_to_load["POST"])
             # Unify the dictionaries PROJ(PRE) - $EXPID/CONF - PROJ(POST)
             if not only_experiment_data:
                 self.experiment_data = self.unify_conf(self.unify_conf(custom_conf_pre,non_minimal_conf),custom_conf_post)
             else:
                 self.experiment_data = starter_conf
             # This part is useless, as it is already done
             self.experiment_data = self.substitute_dynamic_variables(self.experiment_data, max_deep=25)
```

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/expdef-dummy.yml` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/expdef-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/expdef.yml` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/expdef.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/jobs-dummy.yml` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/jobs-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/jobs.yml` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/jobs.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/platforms-dummy.yml` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/platforms-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser/config/files/platforms.yml` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser/config/files/platforms.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser.egg-info/PKG-INFO` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.27
+Version: 1.0.28
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 Keywords: climate,weather,workflow,HPC
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `autosubmitconfigparser-1.0.27/autosubmitconfigparser.egg-info/SOURCES.txt` & `autosubmitconfigparser-1.0.28/autosubmitconfigparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/environment.yml` & `autosubmitconfigparser-1.0.28/environment.yml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   - portalocker>=2.3.2
   - requests>=2.27.1
   - bscearth.utils>=0.5.2
   - cryptography>=36.0.1
   - setuptools>=60.8.2
   - six>=1.10.0
   - xlib>=0.21
-  - ruamel.yaml
+  - ruamel.yaml==0.17.21
   - pythondialog
   - pytest
   - nose
   - coverage
   - requests
   - configobj
```

### Comparing `autosubmitconfigparser-1.0.27/log/__pycache__/log.cpython-37.pyc` & `autosubmitconfigparser-1.0.28/log/__pycache__/log.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/log/fd_show.py` & `autosubmitconfigparser-1.0.28/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/log/log.py` & `autosubmitconfigparser-1.0.28/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.27/setup.py` & `autosubmitconfigparser-1.0.28/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autosubmitconfigparser",
-    version="1.0.27",
+    version="1.0.28",
     author="Daniel Beltran Mora",
     author_email="daniel.beltran@bsc.es",
     description="An utility library that allows to read an Autosubmit 4 experiment configuration.",
     keywords=['climate', 'weather', 'workflow', 'HPC'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git",
     include_package_data=True,
     package_data={'files': ['autosubmitconfigparser/conf/files/*']},
     packages=setuptools.find_packages(),
     install_requires=['packaging>19', 'six>=1.10.0', 'configobj>=5.0.6', 'argparse>=1.4.0', 'python-dateutil>=2.8.2',
                        'pyparsing>=3.0.7',
                       'mock>=4.0.3', 'portalocker>=2.3.2', 'networkx>=2.6.3', 'requests>=2.27.1',
                       'bscearth.utils>=0.5.2', 'cryptography>=36.0.1', 'setuptools>=60.8.2',
-                      'pip>=22.0.3', 'ruamel.yaml', 'pythondialog', 'pytest', 'nose', 'coverage', 'PyNaCl>=1.4.0',
+                      'pip>=22.0.3', 'ruamel.yaml==0.17.21', 'pythondialog', 'pytest', 'nose', 'coverage', 'PyNaCl>=1.4.0',
                       'Pygments'],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: POSIX :: Linux"
     ],
```

### Comparing `autosubmitconfigparser-1.0.27/test_config.py` & `autosubmitconfigparser-1.0.28/test_config.py`

 * *Files identical despite different names*

