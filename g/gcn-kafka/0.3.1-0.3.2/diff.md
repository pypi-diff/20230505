# Comparing `tmp/gcn-kafka-0.3.1.tar.gz` & `tmp/gcn-kafka-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcn-kafka-0.3.1.tar", last modified: Tue Apr 18 00:53:21 2023, max compression
+gzip compressed data, was "gcn-kafka-0.3.2.tar", last modified: Fri May  5 01:38:21 2023, max compression
```

## Comparing `gcn-kafka-0.3.1.tar` & `gcn-kafka-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/gcn_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/oidc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/gcn_kafka/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/test/test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/test/test_oidc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/gcn_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:38:21.404692 gcn-kafka-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:38:21.404692 gcn-kafka-0.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:38:21.404692 gcn-kafka-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-05 01:38:21.404692 gcn-kafka-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:38:21.404692 gcn-kafka-0.3.2/gcn_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/gcn_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 01:38:21.000000 gcn-kafka-0.3.2/gcn_kafka/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/gcn_kafka/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/gcn_kafka/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/gcn_kafka/oidc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:38:21.404692 gcn-kafka-0.3.2/gcn_kafka/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/gcn_kafka/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/gcn_kafka/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/gcn_kafka/test/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/gcn_kafka/test/test_oidc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:38:21.404692 gcn-kafka-0.3.2/gcn_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-05 01:38:21.000000 gcn-kafka-0.3.2/gcn_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-05 01:38:21.000000 gcn-kafka-0.3.2/gcn_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:38:21.000000 gcn-kafka-0.3.2/gcn_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-05 01:38:21.000000 gcn-kafka-0.3.2/gcn_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 01:38:21.000000 gcn-kafka-0.3.2/gcn_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:38:21.404692 gcn-kafka-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 01:37:59.000000 gcn-kafka-0.3.2/tox.ini
```

### Comparing `gcn-kafka-0.3.1/.github/workflows/codeql-analysis.yml` & `gcn-kafka-0.3.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.1/LICENSE.txt` & `gcn-kafka-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.1/PKG-INFO` & `gcn-kafka-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcn-kafka
-Version: 0.3.1
+Version: 0.3.2
 Summary: Kafka client for NASA's General Coordinates Network (GCN)
 Author-email: Leo Singer <leo.p.singer@nasa.gov>, Tom Barclay <tb@umbc.edu>, Eric Burns <ericburns@lsu.edu>
 License: CC0-1.0
 Project-URL: source, https://github.com/nasa-gcn/gcn-kafka-python
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `gcn-kafka-0.3.1/README.md` & `gcn-kafka-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.1/gcn_kafka/core.py` & `gcn-kafka-0.3.2/gcn_kafka/core.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.1/gcn_kafka/env.py` & `gcn-kafka-0.3.2/gcn_kafka/env.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.1/gcn_kafka/oidc.py` & `gcn-kafka-0.3.2/gcn_kafka/oidc.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.1/gcn_kafka/test/test_core.py` & `gcn-kafka-0.3.2/gcn_kafka/test/test_core.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.1/gcn_kafka/test/test_oidc.py` & `gcn-kafka-0.3.2/gcn_kafka/test/test_oidc.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.1/gcn_kafka.egg-info/PKG-INFO` & `gcn-kafka-0.3.2/gcn_kafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcn-kafka
-Version: 0.3.1
+Version: 0.3.2
 Summary: Kafka client for NASA's General Coordinates Network (GCN)
 Author-email: Leo Singer <leo.p.singer@nasa.gov>, Tom Barclay <tb@umbc.edu>, Eric Burns <ericburns@lsu.edu>
 License: CC0-1.0
 Project-URL: source, https://github.com/nasa-gcn/gcn-kafka-python
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `gcn-kafka-0.3.1/gcn_kafka.egg-info/SOURCES.txt` & `gcn-kafka-0.3.2/gcn_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.1/pyproject.toml` & `gcn-kafka-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Topic :: Scientific/Engineering :: Astronomy",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: System :: Networking"
 ]
 dependencies = [
     "authlib",
     "certifi",
-    "confluent-kafka >= 1.6.1, != 2.1.0",
+    "confluent-kafka >= 1.6.1, != 2.1.0, != 2.1.1",
     "requests",
     "typing-extensions; python_version<='3.7'"
 ]
 requires-python = ">=3.7"
 dynamic = [ "version" ]
 
 [project.urls]
```

