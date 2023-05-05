# Comparing `tmp/hyperdb-python-0.1.2.tar.gz` & `tmp/hyperdb-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdb-python-0.1.2.tar", last modified: Mon Apr 17 03:23:30 2023, max compression
+gzip compressed data, was "hyperdb-python-0.1.3.tar", last modified: Fri May  5 03:06:37 2023, max compression
```

## Comparing `hyperdb-python-0.1.2.tar` & `hyperdb-python-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-04-17 03:23:30.748813 hyperdb-python-0.1.2/
--rw-r--r--   0 jdagdelen   (501) staff       (20)     1070 2023-04-16 06:27:54.000000 hyperdb-python-0.1.2/LICENSE
--rw-r--r--   0 jdagdelen   (501) staff       (20)     3086 2023-04-17 03:23:30.748634 hyperdb-python-0.1.2/PKG-INFO
--rw-r--r--   0 jdagdelen   (501) staff       (20)     2430 2023-04-17 03:20:48.000000 hyperdb-python-0.1.2/README.md
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-04-17 03:23:30.747668 hyperdb-python-0.1.2/hyperdb/
--rw-r--r--   0 jdagdelen   (501) staff       (20)       22 2023-04-16 07:55:26.000000 hyperdb-python-0.1.2/hyperdb/__init__.py
--rw-r--r--   0 jdagdelen   (501) staff       (20)     1444 2023-04-16 20:27:48.000000 hyperdb-python-0.1.2/hyperdb/galaxy_brain_math_shit.py
--rw-r--r--   0 jdagdelen   (501) staff       (20)     3591 2023-04-17 03:20:48.000000 hyperdb-python-0.1.2/hyperdb/hyperdb.py
-drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-04-17 03:23:30.748423 hyperdb-python-0.1.2/hyperdb_python.egg-info/
--rw-r--r--   0 jdagdelen   (501) staff       (20)     3086 2023-04-17 03:23:30.000000 hyperdb-python-0.1.2/hyperdb_python.egg-info/PKG-INFO
--rw-r--r--   0 jdagdelen   (501) staff       (20)      288 2023-04-17 03:23:30.000000 hyperdb-python-0.1.2/hyperdb_python.egg-info/SOURCES.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)        1 2023-04-17 03:23:30.000000 hyperdb-python-0.1.2/hyperdb_python.egg-info/dependency_links.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)       13 2023-04-17 03:23:30.000000 hyperdb-python-0.1.2/hyperdb_python.egg-info/requires.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)        8 2023-04-17 03:23:30.000000 hyperdb-python-0.1.2/hyperdb_python.egg-info/top_level.txt
--rw-r--r--   0 jdagdelen   (501) staff       (20)       38 2023-04-17 03:23:30.748860 hyperdb-python-0.1.2/setup.cfg
--rw-r--r--   0 jdagdelen   (501) staff       (20)      937 2023-04-17 03:23:15.000000 hyperdb-python-0.1.2/setup.py
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:37.204128 hyperdb-python-0.1.3/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     1070 2023-04-16 06:27:54.000000 hyperdb-python-0.1.3/LICENSE
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     3141 2023-05-05 03:06:37.203943 hyperdb-python-0.1.3/PKG-INFO
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     2485 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/README.md
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:37.202419 hyperdb-python-0.1.3/hyperdb/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       22 2023-04-16 07:55:26.000000 hyperdb-python-0.1.3/hyperdb/__init__.py
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     1733 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/hyperdb/galaxy_brain_math_shit.py
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     4887 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/hyperdb/hyperdb.py
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:37.203279 hyperdb-python-0.1.3/hyperdb_python.egg-info/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)     3141 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/PKG-INFO
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      343 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)        1 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       13 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/requires.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       14 2023-05-05 03:06:37.000000 hyperdb-python-0.1.3/hyperdb_python.egg-info/top_level.txt
+-rw-r--r--   0 jdagdelen   (501) staff       (20)       38 2023-05-05 03:06:37.204179 hyperdb-python-0.1.3/setup.cfg
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      937 2023-05-05 03:06:12.000000 hyperdb-python-0.1.3/setup.py
+drwxr-xr-x   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:37.203722 hyperdb-python-0.1.3/tests/
+-rw-r--r--   0 jdagdelen   (501) staff       (20)        0 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/tests/__init__.py
+-rw-r--r--   0 jdagdelen   (501) staff       (20)      498 2023-05-05 03:06:29.000000 hyperdb-python-0.1.3/tests/test_galaxy_brain_math_shit.py
```

### Comparing `hyperdb-python-0.1.2/LICENSE` & `hyperdb-python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdb-python-0.1.2/PKG-INFO` & `hyperdb-python-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdb-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: A hyper-fast local vector database for use with LLM Agents.
 Home-page: https://github.com/jdagdelen/hyperdb
 Author: John Dagdelen
 Author-email: jjdagdelen@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,16 @@
 <img src="https://github.com/jdagdelen/hyperDB/blob/main/_static/logo.png?raw=true" width="400" alt="HyperDB Logo">
 </div>
 
 A hyper-fast local vector database for use with LLM Agents. 
 
 Want to invest? [Now accepting SAFEs ($35M cap minimum.)](https://www.youtube.com/watch?v=QH2-TGUlwu4)
 
+Join the [HyperDBiscord](https://discord.gg/8YQzexAA)
+
 ## Advantages
 * Simple interface compatible with _all_ large language model agents. 
 * Highly optimized C++ backend vector store with HW accelerated operations via MKL BLAS. 
 * Enables users to index documents with advanced features such as _ids_ and _metadata_.
 
 ## Installation
```

### Comparing `hyperdb-python-0.1.2/README.md` & `hyperdb-python-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 <img src="https://github.com/jdagdelen/hyperDB/blob/main/_static/logo.png?raw=true" width="400" alt="HyperDB Logo">
 </div>
 
 A hyper-fast local vector database for use with LLM Agents. 
 
 Want to invest? [Now accepting SAFEs ($35M cap minimum.)](https://www.youtube.com/watch?v=QH2-TGUlwu4)
 
+Join the [HyperDBiscord](https://discord.gg/8YQzexAA)
+
 ## Advantages
 * Simple interface compatible with _all_ large language model agents. 
 * Highly optimized C++ backend vector store with HW accelerated operations via MKL BLAS. 
 * Enables users to index documents with advanced features such as _ids_ and _metadata_.
 
 ## Installation
```

### Comparing `hyperdb-python-0.1.2/hyperdb/galaxy_brain_math_shit.py` & `hyperdb-python-0.1.3/hyperdb/galaxy_brain_math_shit.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,12 +24,20 @@
     def random_change(value):
         return value + random.uniform(-0.2, 0.2)
 
     similarities = cosine_similarity(vectors, query_vector)
     derrida_similarities = np.vectorize(random_change)(similarities)
     return derrida_similarities
 
+def adams_similarity(vectors, query_vector):
+    def adams_change(value):
+        return 0.42
+
+    similarities = cosine_similarity(vectors, query_vector)
+    adams_similarities = np.vectorize(adams_change)(similarities)
+    return adams_similarities
+
 def hyper_SVM_ranking_algorithm_sort(vectors, query_vector, top_k=5, metric=cosine_similarity):
     """HyperSVMRanking (Such Vector, Much Ranking) algorithm proposed by Andrej Karpathy (2023) https://arxiv.org/abs/2303.18231"""
     similarities = metric(vectors, query_vector)
     top_indices = np.argsort(similarities, axis=0)[-top_k:][::-1]
-    return top_indices.flatten()
+    return top_indices.flatten(), similarities[top_indices].flatten()
```

### Comparing `hyperdb-python-0.1.2/hyperdb_python.egg-info/PKG-INFO` & `hyperdb-python-0.1.3/hyperdb_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdb-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: A hyper-fast local vector database for use with LLM Agents.
 Home-page: https://github.com/jdagdelen/hyperdb
 Author: John Dagdelen
 Author-email: jjdagdelen@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,16 @@
 <img src="https://github.com/jdagdelen/hyperDB/blob/main/_static/logo.png?raw=true" width="400" alt="HyperDB Logo">
 </div>
 
 A hyper-fast local vector database for use with LLM Agents. 
 
 Want to invest? [Now accepting SAFEs ($35M cap minimum.)](https://www.youtube.com/watch?v=QH2-TGUlwu4)
 
+Join the [HyperDBiscord](https://discord.gg/8YQzexAA)
+
 ## Advantages
 * Simple interface compatible with _all_ large language model agents. 
 * Highly optimized C++ backend vector store with HW accelerated operations via MKL BLAS. 
 * Enables users to index documents with advanced features such as _ids_ and _metadata_.
 
 ## Installation
```

### Comparing `hyperdb-python-0.1.2/setup.py` & `hyperdb-python-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hyperdb-python",
-    version="0.1.2",
+    version="0.1.3",
     author="John Dagdelen",
     author_email="jjdagdelen@gmail.com",
     description="A hyper-fast local vector database for use with LLM Agents.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jdagdelen/hyperdb",
     packages=find_packages(),
```

