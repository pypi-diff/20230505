# Comparing `tmp/citrusdb-0.1.3.tar.gz` & `tmp/citrusdb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.1.3.tar", last modified: Fri Apr 21 10:47:53 2023, max compression
+gzip compressed data, was "citrusdb-0.2.0.tar", last modified: Fri May  5 19:00:03 2023, max compression
```

## Comparing `citrusdb-0.1.3.tar` & `citrusdb-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.150783 citrusdb-0.1.3/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.1.3/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)      690 2023-04-21 10:47:53.150654 citrusdb-0.1.3/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      181 2023-04-21 09:07:38.000000 citrusdb-0.1.3/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.148960 citrusdb-0.1.3/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)       81 2023-04-21 10:45:02.000000 citrusdb-0.1.3/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.149997 citrusdb-0.1.3/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:33:43.000000 citrusdb-0.1.3/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     4442 2023-04-21 10:45:02.000000 citrusdb-0.1.3/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.148285 citrusdb-0.1.3/citrusdb/db/
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.150261 citrusdb-0.1.3/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:03:22.000000 citrusdb-0.1.3/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1415 2023-04-21 10:45:02.000000 citrusdb-0.1.3/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.150496 citrusdb-0.1.3/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-17 05:54:34.000000 citrusdb-0.1.3/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      355 2023-04-21 10:45:02.000000 citrusdb-0.1.3/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.149735 citrusdb-0.1.3/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)      690 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      387 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        9 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/top_level.txt
--rw-r--r--   0 debabrata   (501) staff       (20)      598 2023-04-21 10:47:18.000000 citrusdb-0.1.3/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-04-21 10:47:53.150817 citrusdb-0.1.3/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      771 2023-04-21 10:47:30.000000 citrusdb-0.1.3/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.677889 citrusdb-0.2.0/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.2.0/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)      690 2023-05-05 19:00:03.677761 citrusdb-0.2.0/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      181 2023-04-21 09:07:38.000000 citrusdb-0.2.0/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.676127 citrusdb-0.2.0/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)       81 2023-04-21 10:45:02.000000 citrusdb-0.2.0/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.677096 citrusdb-0.2.0/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:33:43.000000 citrusdb-0.2.0/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     4620 2023-05-05 18:46:52.000000 citrusdb-0.2.0/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.675249 citrusdb-0.2.0/citrusdb/db/
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.677353 citrusdb-0.2.0/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:03:22.000000 citrusdb-0.2.0/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1478 2023-05-05 18:46:52.000000 citrusdb-0.2.0/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.677589 citrusdb-0.2.0/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-17 05:54:34.000000 citrusdb-0.2.0/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-05 18:46:52.000000 citrusdb-0.2.0/citrusdb/embedding/openai.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-05-05 19:00:03.676832 citrusdb-0.2.0/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)      690 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      387 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        9 2023-05-05 19:00:03.000000 citrusdb-0.2.0/citrusdb.egg-info/top_level.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)      598 2023-05-05 18:55:40.000000 citrusdb-0.2.0/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-05-05 19:00:03.677924 citrusdb-0.2.0/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      771 2023-05-05 18:55:26.000000 citrusdb-0.2.0/setup.py
```

### Comparing `citrusdb-0.1.3/LICENSE` & `citrusdb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.1.3/PKG-INFO` & `citrusdb-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.1.3
+Version: 0.2.0
 Summary: citrus.
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `citrusdb-0.1.3/citrusdb/api/local.py` & `citrusdb-0.2.0/citrusdb/api/local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 import pickle
-from typing import List, Optional
+from typing import Any, List, Optional
+from numpy import float32
+from numpy._typing import NDArray
 from citrusdb.db.index.hnswlib import HnswIndex
 
 
 class LocalAPI:
     _db: HnswIndex
     _parameters: dict
 
     def __init__(self):
-        self._db = HnswIndex(id="test")
+        self._db = HnswIndex(id="citrus")
 
     def create_index(
         self,
         max_elements: int = 1000,
         persist_directory: Optional[str] = None,
-        M: int = 16,
+        M: int = 64,
         ef_construction: int = 200,
         allow_replace_deleted: bool = False,
     ):
         self._parameters = {
             "index_name": "citrus",
             "max_elements": max_elements,
             "persist_directory": persist_directory,
@@ -60,25 +62,25 @@
                 allow_replace_deleted=allow_replace_deleted,
             )
 
     def add(
         self,
         ids,
         documents: Optional[List[str]] = None,
-        embedding: Optional[List[List[float]]] = None,
+        embedding: Optional[NDArray[float32]] = None,
     ):
-        if embedding == None and documents == None:
+        if embedding is None and documents is None:
             raise ValueError("Please provide either embeddings or documents.")
 
-        if documents:
+        if documents is not None:
             from citrusdb.embedding.openai import get_embeddings
 
             embedding = get_embeddings(documents)
 
-        if embedding:
+        if embedding is not None:
             embedding_dim = len(embedding[0])
             index_dim = self._db.get_dimension()
 
             # Check whether the dimensions are equal
             if embedding_dim != index_dim:
                 raise ValueError(
                     f"Embedding dimenstion ({embedding_dim}) and index "
@@ -114,26 +116,29 @@
     def _save_params(self):
         output_file = os.path.join(
             self._parameters["persist_directory"], ".citrus_params"
         )
         with open(output_file, "wb") as f:
             pickle.dump(self._parameters, f)
 
+    def set_ef(self, ef: int):
+        self._db.set_ef(ef)
+
     def query(
         self,
-        document: Optional[str] = None,
-        query_embedding: Optional[List[float]] = None,
+        documents: Optional[List[str]] = None,
+        query_embeddings: Optional[NDArray[float32]] = None,
         k=1,
     ):
-        if query_embedding == None and document == None:
+        if query_embeddings is None and documents is None:
             raise ValueError("Please provide either an embedding" + " or a document.")
 
-        if document:
+        if documents is not None:
             from citrusdb.embedding.openai import get_embeddings
 
-            embedding = get_embeddings([document])
-            query_embedding = embedding[0]
+            embeddings = get_embeddings(documents)
+            query_embeddings = embeddings
 
-        return self._db.knn_query(query_embedding, k)
+        return self._db.knn_query(query_embeddings, k)
 
     def get_status(self):
         self._db.get_status()
```

### Comparing `citrusdb-0.1.3/citrusdb/db/index/hnswlib.py` & `citrusdb-0.2.0/citrusdb/db/index/hnswlib.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,38 +6,42 @@
     _index: hnswlib.Index
 
     def __init__(self, id, space="cosine", dim=1536):
         self._id = id
         self._index = hnswlib.Index(space=space, dim=dim)
 
     def init_index(
-        self, max_elements=1000, M=16, ef_construction=200, allow_replace_deleted=False
+        self, max_elements=1000, M=64, ef_construction=200, allow_replace_deleted=False
     ):
         self._index.init_index(max_elements, M, ef_construction, allow_replace_deleted)
 
     def add_items(self, data, ids, replace_deleted=False):
         max_elements = self._index.max_elements
         curr_elements = self._index.element_count
 
         # Increase index size
         if curr_elements + len(data) > max_elements:
             new_size = max(curr_elements + len(data), 2 * max_elements)
             self._index.resize_index(new_size)
 
         self._index.add_items(data, ids, replace_deleted)
 
-    def knn_query(self, query_embedding, k=1):
-        labels, distances = self._index.knn_query(query_embedding, k)
-        return labels[0], distances
+    def knn_query(self, query_embeddings, k=1):
+        labels, distances = self._index.knn_query(query_embeddings, k)
+        return labels, distances
+
+    def set_ef(self, ef: int):
+        self._index.set_ef(ef)
 
     def get_dimension(self):
         return self._index.dim
 
     def load_index(self, path: str, allow_replace_deleted=False):
         self._index.load_index(path, allow_replace_deleted=allow_replace_deleted)
 
     def save_index(self, path: str):
         self._index.save_index(path)
 
     def get_status(self):
         print("Max elements", self._index.max_elements)
         print("Current elements", self._index.element_count)
+
```

### Comparing `citrusdb-0.1.3/citrusdb.egg-info/PKG-INFO` & `citrusdb-0.2.0/citrusdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.1.3
+Version: 0.2.0
 Summary: citrus.
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `citrusdb-0.1.3/pyproject.toml` & `citrusdb-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.1.3"
+version = "0.2.0"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "citrus."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `citrusdb-0.1.3/setup.py` & `citrusdb-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.1.3",
+    version="0.2.0",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=find_packages(exclude=["demo"]),
```

