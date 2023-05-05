# Comparing `tmp/rotary-embedding-torch-0.2.2.tar.gz` & `tmp/rotary-embedding-torch-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary-embedding-torch-0.2.2.tar", last modified: Fri Apr 28 21:11:05 2023, max compression
+gzip compressed data, was "rotary-embedding-torch-0.2.3.tar", last modified: Fri May  5 21:54:49 2023, max compression
```

## Comparing `rotary-embedding-torch-0.2.2.tar` & `rotary-embedding-torch-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/rotary_embedding_torch/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch/rotary_embedding_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 21:11:05.000000 rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:11:05.331723 rotary-embedding-torch-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-28 21:10:52.000000 rotary-embedding-torch-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:54:49.509802 rotary-embedding-torch-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 21:54:35.000000 rotary-embedding-torch-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 21:54:49.509802 rotary-embedding-torch-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-05 21:54:35.000000 rotary-embedding-torch-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:54:49.509802 rotary-embedding-torch-0.2.3/rotary_embedding_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-05 21:54:35.000000 rotary-embedding-torch-0.2.3/rotary_embedding_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-05 21:54:35.000000 rotary-embedding-torch-0.2.3/rotary_embedding_torch/rotary_embedding_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:54:49.509802 rotary-embedding-torch-0.2.3/rotary_embedding_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 21:54:49.000000 rotary-embedding-torch-0.2.3/rotary_embedding_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 21:54:49.000000 rotary-embedding-torch-0.2.3/rotary_embedding_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:54:49.000000 rotary-embedding-torch-0.2.3/rotary_embedding_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 21:54:49.000000 rotary-embedding-torch-0.2.3/rotary_embedding_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 21:54:49.000000 rotary-embedding-torch-0.2.3/rotary_embedding_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:54:49.509802 rotary-embedding-torch-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-05 21:54:35.000000 rotary-embedding-torch-0.2.3/setup.py
```

### Comparing `rotary-embedding-torch-0.2.2/LICENSE` & `rotary-embedding-torch-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rotary-embedding-torch-0.2.2/PKG-INFO` & `rotary-embedding-torch-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.2.2
+Version: 0.2.3
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.2.2/README.md` & `rotary-embedding-torch-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rotary-embedding-torch-0.2.2/rotary_embedding_torch/rotary_embedding_torch.py` & `rotary-embedding-torch-0.2.3/rotary_embedding_torch/rotary_embedding_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             return self.cache[cache_key]
 
         if callable(t):
             t = t()
 
         scale = 1.
         if self.use_xpos:
-            power = t - (len(t) // 2) / self.scale_base
+            power = (t - len(t) // 2) / self.scale_base
             scale = self.scale ** rearrange(power, 'n -> n 1')
             scale = torch.cat((scale, scale), dim = -1)
 
         if exists(cache_key):
             self.cache[cache_key] = scale
 
         return scale
```

### Comparing `rotary-embedding-torch-0.2.2/rotary_embedding_torch.egg-info/PKG-INFO` & `rotary-embedding-torch-0.2.3/rotary_embedding_torch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.2.2
+Version: 0.2.3
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.2.2/setup.py` & `rotary-embedding-torch-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rotary-embedding-torch',
   packages = find_packages(),
-  version = '0.2.2',
+  version = '0.2.3',
   license='MIT',
   description = 'Rotary Embedding - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/rotary-embedding-torch',
   keywords = [
```

