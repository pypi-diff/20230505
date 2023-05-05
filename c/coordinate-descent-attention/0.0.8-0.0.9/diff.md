# Comparing `tmp/coordinate-descent-attention-0.0.8.tar.gz` & `tmp/coordinate-descent-attention-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coordinate-descent-attention-0.0.8.tar", last modified: Thu May  4 02:39:36 2023, max compression
+gzip compressed data, was "coordinate-descent-attention-0.0.9.tar", last modified: Fri May  5 19:01:34 2023, max compression
```

## Comparing `coordinate-descent-attention-0.0.8.tar` & `coordinate-descent-attention-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/coordinate_descent_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention/coordinate_descent_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 02:39:36.000000 coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 02:39:36.315890 coordinate-descent-attention-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-04 02:39:20.000000 coordinate-descent-attention-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:01:34.524150 coordinate-descent-attention-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 19:01:20.000000 coordinate-descent-attention-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-05 19:01:34.524150 coordinate-descent-attention-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-05 19:01:20.000000 coordinate-descent-attention-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:01:34.524150 coordinate-descent-attention-0.0.9/coordinate_descent_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-05 19:01:20.000000 coordinate-descent-attention-0.0.9/coordinate_descent_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 19:01:20.000000 coordinate-descent-attention-0.0.9/coordinate_descent_attention/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-05 19:01:20.000000 coordinate-descent-attention-0.0.9/coordinate_descent_attention/coordinate_descent_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:01:34.524150 coordinate-descent-attention-0.0.9/coordinate_descent_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-05 19:01:34.000000 coordinate-descent-attention-0.0.9/coordinate_descent_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-05 19:01:34.000000 coordinate-descent-attention-0.0.9/coordinate_descent_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:01:34.000000 coordinate-descent-attention-0.0.9/coordinate_descent_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 19:01:34.000000 coordinate-descent-attention-0.0.9/coordinate_descent_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 19:01:34.000000 coordinate-descent-attention-0.0.9/coordinate_descent_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:01:34.524150 coordinate-descent-attention-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-05 19:01:20.000000 coordinate-descent-attention-0.0.9/setup.py
```

### Comparing `coordinate-descent-attention-0.0.8/LICENSE` & `coordinate-descent-attention-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coordinate-descent-attention-0.0.8/PKG-INFO` & `coordinate-descent-attention-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coordinate-descent-attention
-Version: 0.0.8
+Version: 0.0.9
 Summary: Coordinate Descent Attention - Pytorch
 Home-page: https://github.com/lucidrains/coodinate-descent-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coordinate-descent-attention-0.0.8/README.md` & `coordinate-descent-attention-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `coordinate-descent-attention-0.0.8/coordinate_descent_attention/autoregressive_wrapper.py` & `coordinate-descent-attention-0.0.9/coordinate_descent_attention/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `coordinate-descent-attention-0.0.8/coordinate_descent_attention/coordinate_descent_attention.py` & `coordinate-descent-attention-0.0.9/coordinate_descent_attention/coordinate_descent_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,16 @@
             causal_mask = repeat(causal_mask, 'i j -> b h i j', b = sim.shape[0], h = sim.shape[1])
 
             attn = triton_coor_descent(
                 sim,
                 n_iters = self.coor_descent_iters,
                 k = sparsity_k,
                 eps = self.coor_descent_eps,
-                mask = ~causal_mask
+                mask = ~causal_mask,
+                checkpoint_segments = self.coor_descent_iters // 10
             )
 
         else:
             sim = sim.masked_fill(causal_mask, -torch.finfo(sim.dtype).max)
             attn = sim.softmax(dim = -1)
 
         # aggregate
```

### Comparing `coordinate-descent-attention-0.0.8/coordinate_descent_attention.egg-info/PKG-INFO` & `coordinate-descent-attention-0.0.9/coordinate_descent_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coordinate-descent-attention
-Version: 0.0.8
+Version: 0.0.9
 Summary: Coordinate Descent Attention - Pytorch
 Home-page: https://github.com/lucidrains/coodinate-descent-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coordinate-descent-attention-0.0.8/setup.py` & `coordinate-descent-attention-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'coordinate-descent-attention',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Coordinate Descent Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/coodinate-descent-attention',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'attention mechanism'
   ],
   install_requires=[
     'einops>=0.6.1',
     'torch>=1.6',
-    'colt5-attention>=0.5.2'
+    'colt5-attention>=0.6.2'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

