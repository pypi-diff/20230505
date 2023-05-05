# Comparing `tmp/gremlinpython-3.6.2.tar.gz` & `tmp/gremlinpython-3.6.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gremlinpython-3.6.2.tar", last modified: Thu Jan 26 23:46:26 2023, max compression
+gzip compressed data, was "gremlinpython-3.6.3rc1.tar", last modified: Thu Feb 16 17:52:35 2023, max compression
```

## Comparing `gremlinpython-3.6.2.tar` & `gremlinpython-3.6.3rc1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:46:26.639960 gremlinpython-3.6.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      814 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      170 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6045 2023-01-26 23:46:26.641751 gremlinpython-3.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5543 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:46:26.195157 gremlinpython-3.6.2/gremlin_python/
--rw-r--r--   0 root         (0) root         (0)      850 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-01-26 23:46:25.000000 gremlinpython-3.6.2/gremlin_python/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:46:26.347040 gremlinpython-3.6.2/gremlin_python/driver/
--rw-r--r--   0 root         (0) root         (0)      850 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:46:26.372391 gremlinpython-3.6.2/gremlin_python/driver/aiohttp/
--rw-r--r--   0 root         (0) root         (0)      787 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/aiohttp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6228 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/aiohttp/transport.py
--rw-r--r--   0 root         (0) root         (0)     7147 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/client.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/connection.py
--rw-r--r--   0 root         (0) root         (0)     8507 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/driver_remote_connection.py
--rw-r--r--   0 root         (0) root         (0)     8746 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/protocol.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/remote_connection.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/request.py
--rw-r--r--   0 root         (0) root         (0)     2669 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/resultset.py
--rw-r--r--   0 root         (0) root         (0)    10009 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/serializer.py
--rw-r--r--   0 root         (0) root         (0)     1246 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/transport.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/driver/useragent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:46:26.462941 gremlinpython-3.6.2/gremlin_python/process/
--rw-r--r--   0 root         (0) root         (0)      850 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/process/anonymous_traversal.py
--rw-r--r--   0 root         (0) root         (0)    61033 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/process/graph_traversal.py
--rw-r--r--   0 root         (0) root         (0)     9474 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/process/strategies.py
--rw-r--r--   0 root         (0) root         (0)     6078 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/process/translator.py
--rw-r--r--   0 root         (0) root         (0)    22294 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/process/traversal.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/statics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:46:26.489617 gremlinpython-3.6.2/gremlin_python/structure/
--rw-r--r--   0 root         (0) root         (0)      852 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/structure/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/structure/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:46:26.559836 gremlinpython-3.6.2/gremlin_python/structure/io/
--rw-r--r--   0 root         (0) root         (0)      852 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/structure/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37104 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/structure/io/graphbinaryV1.py
--rw-r--r--   0 root         (0) root         (0)    20598 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/structure/io/graphsonV2d0.py
--rw-r--r--   0 root         (0) root         (0)    23918 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/structure/io/graphsonV3d0.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/gremlin_python/structure/io/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 23:46:26.632118 gremlinpython-3.6.2/gremlinpython.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6045 2023-01-26 23:46:25.000000 gremlinpython-3.6.2/gremlinpython.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1324 2023-01-26 23:46:26.000000 gremlinpython-3.6.2/gremlinpython.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 23:46:25.000000 gremlinpython-3.6.2/gremlinpython.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      135 2023-01-26 23:46:25.000000 gremlinpython-3.6.2/gremlinpython.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-26 23:46:25.000000 gremlinpython-3.6.2/gremlinpython.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-01-26 23:46:26.651889 gremlinpython-3.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3044 2023-01-26 23:36:17.000000 gremlinpython-3.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/
+-rw-rw-r--   0 root         (0) root         (0)    11357 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      814 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      170 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6048 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5543 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/gremlin_python/
+-rw-rw-r--   0 root         (0) root         (0)      850 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      808 2023-02-16 17:52:35.000000 gremlinpython-3.6.3rc1/gremlin_python/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/gremlin_python/driver/
+-rw-rw-r--   0 root         (0) root         (0)      850 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/gremlin_python/driver/aiohttp/
+-rw-rw-r--   0 root         (0) root         (0)      787 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/aiohttp/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6228 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/aiohttp/transport.py
+-rw-rw-r--   0 root         (0) root         (0)     7147 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/client.py
+-rw-rw-r--   0 root         (0) root         (0)     3395 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/connection.py
+-rw-rw-r--   0 root         (0) root         (0)     8507 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/driver_remote_connection.py
+-rw-rw-r--   0 root         (0) root         (0)     8746 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/protocol.py
+-rw-rw-r--   0 root         (0) root         (0)     3014 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/remote_connection.py
+-rw-rw-r--   0 root         (0) root         (0)      953 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/request.py
+-rw-rw-r--   0 root         (0) root         (0)     2669 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/resultset.py
+-rw-rw-r--   0 root         (0) root         (0)    10009 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/serializer.py
+-rw-rw-r--   0 root         (0) root         (0)     1246 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/transport.py
+-rw-rw-r--   0 root         (0) root         (0)     1675 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/driver/useragent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/gremlin_python/process/
+-rw-rw-r--   0 root         (0) root         (0)      850 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/process/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2448 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/process/anonymous_traversal.py
+-rw-rw-r--   0 root         (0) root         (0)    61033 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/process/graph_traversal.py
+-rw-rw-r--   0 root         (0) root         (0)     9474 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/process/strategies.py
+-rw-rw-r--   0 root         (0) root         (0)     6078 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/process/translator.py
+-rw-rw-r--   0 root         (0) root         (0)    22294 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/process/traversal.py
+-rw-rw-r--   0 root         (0) root         (0)     2849 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/statics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/gremlin_python/structure/
+-rw-rw-r--   0 root         (0) root         (0)      852 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/structure/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4365 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/structure/graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/gremlin_python/structure/io/
+-rw-rw-r--   0 root         (0) root         (0)      852 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/structure/io/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    37104 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/structure/io/graphbinaryV1.py
+-rw-rw-r--   0 root         (0) root         (0)    20598 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/structure/io/graphsonV2d0.py
+-rw-rw-r--   0 root         (0) root         (0)    23918 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/structure/io/graphsonV3d0.py
+-rw-rw-r--   0 root         (0) root         (0)     1846 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/gremlin_python/structure/io/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/gremlinpython.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     6048 2023-02-16 17:52:35.000000 gremlinpython-3.6.3rc1/gremlinpython.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1324 2023-02-16 17:52:35.000000 gremlinpython-3.6.3rc1/gremlinpython.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-02-16 17:52:35.000000 gremlinpython-3.6.3rc1/gremlinpython.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      153 2023-02-16 17:52:35.000000 gremlinpython-3.6.3rc1/gremlinpython.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       15 2023-02-16 17:52:35.000000 gremlinpython-3.6.3rc1/gremlinpython.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      256 2023-02-16 17:52:35.373970 gremlinpython-3.6.3rc1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3069 2023-02-16 17:46:41.000000 gremlinpython-3.6.3rc1/setup.py
```

### Comparing `gremlinpython-3.6.2/LICENSE` & `gremlinpython-3.6.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/MANIFEST.in` & `gremlinpython-3.6.3rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/PKG-INFO` & `gremlinpython-3.6.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinpython
-Version: 3.6.2
+Version: 3.6.3rc1
 Summary: Gremlin-Python for Apache TinkerPop
 Home-page: http://tinkerpop.apache.org
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `gremlinpython-3.6.2/README.rst` & `gremlinpython-3.6.3rc1/README.rst`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/__version__.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/aiohttp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-'''
-Licensed to the Apache Software Foundation (ASF) under one
-or more contributor license agreements.  See the NOTICE file
-distributed with this work for additional information
-regarding copyright ownership.  The ASF licenses this file
-to you under the Apache License, Version 2.0 (the
-"License"); you may not use this file except in compliance
-with the License.  You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing,
-software distributed under the License is distributed on an
-"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-KIND, either express or implied.  See the License for the
-specific language governing permissions and limitations
-under the License.
-'''
-version   = '3.6.2'
-timestamp = 1674776785
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
```

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/aiohttp/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,7 +12,9 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
+
+__author__ = 'Marko A. Rodriguez (http://markorodriguez.com)'
```

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/aiohttp/transport.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/aiohttp/transport.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/client.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/client.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/connection.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/driver_remote_connection.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/driver_remote_connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/protocol.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/protocol.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/remote_connection.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/remote_connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/request.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/request.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/resultset.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/resultset.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/serializer.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/serializer.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/transport.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/transport.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/driver/useragent.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/useragent.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/process/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
-#
+# 
 # http://www.apache.org/licenses/LICENSE-2.0
-#
+# 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
```

### Comparing `gremlinpython-3.6.2/gremlin_python/process/anonymous_traversal.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/anonymous_traversal.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/process/graph_traversal.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/process/strategies.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/strategies.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/process/translator.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/translator.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/process/traversal.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/traversal.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/statics.py` & `gremlinpython-3.6.3rc1/gremlin_python/statics.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/structure/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/structure/graph.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/graph.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/structure/io/graphbinaryV1.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/graphbinaryV1.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/structure/io/graphsonV2d0.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/graphsonV2d0.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/structure/io/graphsonV3d0.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/graphsonV3d0.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlin_python/structure/io/util.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/util.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/gremlinpython.egg-info/PKG-INFO` & `gremlinpython-3.6.3rc1/gremlinpython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinpython
-Version: 3.6.2
+Version: 3.6.3rc1
 Summary: Gremlin-Python for Apache TinkerPop
 Home-page: http://tinkerpop.apache.org
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `gremlinpython-3.6.2/gremlinpython.egg-info/SOURCES.txt` & `gremlinpython-3.6.3rc1/gremlinpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.2/setup.py` & `gremlinpython-3.6.3rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,17 @@
 # Load version
 from gremlin_python import __version__
 
 version = __version__.version
 
 install_requires = [
     'nest_asyncio',
-    'aiohttp>=3.8.0,<=3.8.1',
+    'aiohttp>=3.8.0,<4.0.0',
     'aenum>=1.4.5,<4.0.0',
+    'six>=1.10.0,<2.0.0',
     'isodate>=0.6.0,<1.0.0'
 ]
 
 if sys.version_info < (3, 5):
     install_requires += ['pyparsing>=2.4.7,<3.0.0']
 
 setup(
```

