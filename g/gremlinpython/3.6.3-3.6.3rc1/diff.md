# Comparing `tmp/gremlinpython-3.6.3.tar.gz` & `tmp/gremlinpython-3.6.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gremlinpython-3.6.3.tar", last modified: Fri May  5 20:15:25 2023, max compression
+gzip compressed data, was "gremlinpython-3.6.3rc1.tar", last modified: Thu Feb 16 17:52:35 2023, max compression
```

## Comparing `gremlinpython-3.6.3.tar` & `gremlinpython-3.6.3rc1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:15:25.928149 gremlinpython-3.6.3/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6045 2023-05-05 20:15:25.930064 gremlinpython-3.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5543 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:15:25.502061 gremlinpython-3.6.3/gremlin_python/
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-05 20:15:25.000000 gremlinpython-3.6.3/gremlin_python/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:15:25.648798 gremlinpython-3.6.3/gremlin_python/driver/
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:15:25.675836 gremlinpython-3.6.3/gremlin_python/driver/aiohttp/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/aiohttp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6228 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/aiohttp/transport.py
--rw-r--r--   0 root         (0) root         (0)     7321 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/client.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/connection.py
--rw-r--r--   0 root         (0) root         (0)     8670 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/driver_remote_connection.py
--rw-r--r--   0 root         (0) root         (0)     8746 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/protocol.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/remote_connection.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/request.py
--rw-r--r--   0 root         (0) root         (0)     2669 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/resultset.py
--rw-r--r--   0 root         (0) root         (0)    10009 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/serializer.py
--rw-r--r--   0 root         (0) root         (0)     1246 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/transport.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/driver/useragent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:15:25.758885 gremlinpython-3.6.3/gremlin_python/process/
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/process/anonymous_traversal.py
--rw-r--r--   0 root         (0) root         (0)    61065 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/process/graph_traversal.py
--rw-r--r--   0 root         (0) root         (0)     9474 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/process/strategies.py
--rw-r--r--   0 root         (0) root         (0)     6078 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/process/translator.py
--rw-r--r--   0 root         (0) root         (0)    22450 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/process/traversal.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/statics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:15:25.786808 gremlinpython-3.6.3/gremlin_python/structure/
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/structure/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/structure/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:15:25.856567 gremlinpython-3.6.3/gremlin_python/structure/io/
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/structure/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37104 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/structure/io/graphbinaryV1.py
--rw-r--r--   0 root         (0) root         (0)    20598 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/structure/io/graphsonV2d0.py
--rw-r--r--   0 root         (0) root         (0)    23918 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/structure/io/graphsonV3d0.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/gremlin_python/structure/io/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:15:25.920261 gremlinpython-3.6.3/gremlinpython.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6045 2023-05-05 20:15:25.000000 gremlinpython-3.6.3/gremlinpython.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1324 2023-05-05 20:15:25.000000 gremlinpython-3.6.3/gremlinpython.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 20:15:25.000000 gremlinpython-3.6.3/gremlinpython.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-05 20:15:25.000000 gremlinpython-3.6.3/gremlinpython.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-05 20:15:25.000000 gremlinpython-3.6.3/gremlinpython.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-05 20:15:25.936242 gremlinpython-3.6.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3069 2023-05-05 20:05:03.000000 gremlinpython-3.6.3/setup.py
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

### Comparing `gremlinpython-3.6.3/LICENSE` & `gremlinpython-3.6.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/MANIFEST.in` & `gremlinpython-3.6.3rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/PKG-INFO` & `gremlinpython-3.6.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinpython
-Version: 3.6.3
+Version: 3.6.3rc1
 Summary: Gremlin-Python for Apache TinkerPop
 Home-page: http://tinkerpop.apache.org
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `gremlinpython-3.6.3/README.rst` & `gremlinpython-3.6.3rc1/README.rst`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/__version__.py` & `gremlinpython-3.6.3rc1/gremlin_python/__version__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 '''
-version   = '3.6.3'
-timestamp = 1683317725
+version   = '3.6.3-rc1'
+timestamp = 1676569955
```

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/aiohttp/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/aiohttp/transport.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/aiohttp/transport.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/client.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,19 +133,15 @@
         self._closed = True
 
     def _close_session(self):
         message = request.RequestMessage(
             processor='session', op='close',
             args={'session': str(self._session)})
         conn = self._pool.get(True)
-        try:
-            write_result_set = conn.write(message).result()
-            return write_result_set.all().result()  # wait for _receive() to finish
-        except protocol.GremlinServerError:
-            pass
+        return conn.write(message).result()
 
     def _get_connection(self):
         protocol = self._protocol_factory()
         return connection.Connection(
             self._url, self._traversal_source, protocol,
             self._transport_factory, self._executor, self._pool,
             headers=self._headers, enable_user_agent_on_connect=self._enable_user_agent_on_connect)
```

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/connection.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/driver_remote_connection.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/driver_remote_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,18 +153,14 @@
                                       headers=self.__headers,
                                       session=uuid.uuid4(),
                                       enable_user_agent_on_connect=self.__enable_user_agent_on_connect,
                                       **self.__transport_kwargs)
         self.__spawned_sessions.append(conn)
         return conn
 
-    def remove_session(self, session_based_connection):
-        session_based_connection.close()
-        self.__spawned_sessions.remove(session_based_connection)
-
     def commit(self):
         log.info("Submitting commit graph operation.")
         return self._client.submit(Bytecode.GraphOp.commit())
 
     def rollback(self):
         log.info("Submitting rollback graph operation.")
         return self._client.submit(Bytecode.GraphOp.rollback())
```

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/protocol.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/protocol.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/remote_connection.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/remote_connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/request.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/request.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/resultset.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/resultset.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/serializer.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/serializer.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/transport.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/transport.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/driver/useragent.py` & `gremlinpython-3.6.3rc1/gremlin_python/driver/useragent.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/process/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/process/anonymous_traversal.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/anonymous_traversal.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/process/graph_traversal.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/graph_traversal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1573,16 +1573,16 @@
         return self.__is_open
 
     def __verify_transaction_state(self, state, error_message):
         if self.__is_open != state:
             raise Exception(error_message)
 
     def __close_session(self, session):
+        self._session_based_connection.close()
         self.__is_open = False
-        self._remote_connection.remove_session(self._session_based_connection)
         return session
 
 
 def V(*args):
     return __.V(*args)
```

### Comparing `gremlinpython-3.6.3/gremlin_python/process/strategies.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/strategies.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/process/translator.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/translator.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/process/traversal.py` & `gremlinpython-3.6.3rc1/gremlin_python/process/traversal.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,31 +161,21 @@
 statics.add_static('set_', Cardinality.set_)
 
 Column = Enum('Column', ' keys values')
 
 statics.add_static('keys', Column.keys)
 statics.add_static('values', Column.values)
 
-# alias from_ and to
-Direction = Enum(
-    value='Direction',
-    names=[
-        ('BOTH', 'BOTH'),
-        ('IN', 'IN'),
-        ('OUT', 'OUT'),
-        ('from_', "OUT"),
-        ('to', 'IN'),
-    ],
-)
+Direction = Enum('Direction', ' BOTH IN OUT')
 
 statics.add_static('OUT', Direction.OUT)
 statics.add_static('IN', Direction.IN)
 statics.add_static('BOTH', Direction.BOTH)
-statics.add_static('from_', Direction.OUT)
-statics.add_static('to', Direction.IN)
+statics.add_static('from_', Direction.IN)
+statics.add_static('to', Direction.BOTH)
 
 GraphSONVersion = Enum('GraphSONVersion', ' V1_0 V2_0 V3_0')
 
 statics.add_static('V1_0', GraphSONVersion.V1_0)
 statics.add_static('V2_0', GraphSONVersion.V2_0)
 statics.add_static('V3_0', GraphSONVersion.V3_0)
```

### Comparing `gremlinpython-3.6.3/gremlin_python/statics.py` & `gremlinpython-3.6.3rc1/gremlin_python/statics.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/structure/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/structure/graph.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/graph.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/structure/io/__init__.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/structure/io/graphbinaryV1.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/graphbinaryV1.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/structure/io/graphsonV2d0.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/graphsonV2d0.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/structure/io/graphsonV3d0.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/graphsonV3d0.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlin_python/structure/io/util.py` & `gremlinpython-3.6.3rc1/gremlin_python/structure/io/util.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/gremlinpython.egg-info/PKG-INFO` & `gremlinpython-3.6.3rc1/gremlinpython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinpython
-Version: 3.6.3
+Version: 3.6.3rc1
 Summary: Gremlin-Python for Apache TinkerPop
 Home-page: http://tinkerpop.apache.org
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `gremlinpython-3.6.3/gremlinpython.egg-info/SOURCES.txt` & `gremlinpython-3.6.3rc1/gremlinpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.3/setup.py` & `gremlinpython-3.6.3rc1/setup.py`

 * *Files identical despite different names*

