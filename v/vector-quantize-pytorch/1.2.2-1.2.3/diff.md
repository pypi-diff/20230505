# Comparing `tmp/vector_quantize_pytorch-1.2.2.tar.gz` & `tmp/vector_quantize_pytorch-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.2.2.tar", last modified: Sun Apr 23 16:54:32 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.2.3.tar", last modified: Fri May  5 17:31:27 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.2.2.tar` & `vector_quantize_pytorch-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:54:32.642778 vector_quantize_pytorch-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 16:54:32.642778 vector_quantize_pytorch-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:54:32.642778 vector_quantize_pytorch-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:54:32.638778 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    22280 2023-04-23 16:54:18.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:54:32.638778 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 16:54:32.000000 vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.2.2/LICENSE` & `vector_quantize_pytorch-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.2/PKG-INFO` & `vector_quantize_pytorch-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.2.2
+Version: 1.2.3
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.2.2/README.md` & `vector_quantize_pytorch-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.2/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,15 @@
         num_codebooks = 1,
         kmeans_init = False,
         kmeans_iters = 10,
         sync_kmeans = True,
         decay = 0.8,
         eps = 1e-5,
         threshold_ema_dead_code = 2,
+        reset_cluster_size = None,
         use_ddp = False,
         learnable_codebook = False,
         sample_codebook_temp = 0
     ):
         super().__init__()
         self.decay = decay
         init_fn = uniform_init if not kmeans_init else torch.zeros
@@ -204,14 +205,15 @@
 
         self.codebook_size = codebook_size
         self.num_codebooks = num_codebooks
 
         self.kmeans_iters = kmeans_iters
         self.eps = eps
         self.threshold_ema_dead_code = threshold_ema_dead_code
+        self.reset_cluster_size = default(reset_cluster_size, threshold_ema_dead_code)
         self.sample_codebook_temp = sample_codebook_temp
 
         assert not (use_ddp and num_codebooks > 1 and kmeans_init), 'kmeans init is not compatible with multiple codebooks in distributed environment for now'
 
         self.sample_fn = sample_vectors_distributed if use_ddp and sync_kmeans else batched_sample_vectors
         self.kmeans_all_reduce_fn = distributed.all_reduce if use_ddp and sync_kmeans else noop
         self.all_reduce_fn = distributed.all_reduce if use_ddp else noop
@@ -246,15 +248,20 @@
 
     def replace(self, batch_samples, batch_mask):
         for ind, (samples, mask) in enumerate(zip(batch_samples.unbind(dim = 0), batch_mask.unbind(dim = 0))):
             if not torch.any(mask):
                 continue
 
             sampled = self.sample_fn(rearrange(samples, '... -> 1 ...'), mask.sum().item())
-            self.embed.data[ind][mask] = rearrange(sampled, '1 ... -> ...')
+            sampled = rearrange(sampled, '1 ... -> ...')
+            
+            self.embed.data[ind][mask] = sampled
+
+            self.cluster_size.data[ind][mask] = self.reset_cluster_size
+            self.embed_avg.data[ind][mask] = sampled * self.reset_cluster_size
 
     def expire_codes_(self, batch_samples):
         if self.threshold_ema_dead_code == 0:
             return
 
         expired_codes = self.cluster_size < self.threshold_ema_dead_code
 
@@ -319,14 +326,15 @@
         num_codebooks = 1,
         kmeans_init = False,
         kmeans_iters = 10,
         sync_kmeans = True,
         decay = 0.8,
         eps = 1e-5,
         threshold_ema_dead_code = 2,
+        reset_cluster_size = None,
         use_ddp = False,
         learnable_codebook = False,
         sample_codebook_temp = 0.
     ):
         super().__init__()
         self.decay = decay
 
@@ -337,14 +345,15 @@
 
         self.codebook_size = codebook_size
         self.num_codebooks = num_codebooks
 
         self.kmeans_iters = kmeans_iters
         self.eps = eps
         self.threshold_ema_dead_code = threshold_ema_dead_code
+        self.reset_cluster_size = default(reset_cluster_size, threshold_ema_dead_code)
         self.sample_codebook_temp = sample_codebook_temp
 
         self.sample_fn = sample_vectors_distributed if use_ddp and sync_kmeans else batched_sample_vectors
         self.kmeans_all_reduce_fn = distributed.all_reduce if use_ddp and sync_kmeans else noop
         self.all_reduce_fn = distributed.all_reduce if use_ddp else noop
 
         self.register_buffer('initted', torch.Tensor([not kmeans_init]))
@@ -378,15 +387,18 @@
         batch_samples = l2norm(batch_samples)
 
         for ind, (samples, mask) in enumerate(zip(batch_samples.unbind(dim = 0), batch_mask.unbind(dim = 0))):
             if not torch.any(mask):
                 continue
 
             sampled = self.sample_fn(rearrange(samples, '... -> 1 ...'), mask.sum().item())
-            self.embed.data[ind][mask] = rearrange(sampled, '1 ... -> ...')
+            sampled = rearrange(sampled, '1 ... -> ...')
+
+            self.embed.data[ind][mask] = sampled
+            self.cluster_size.data[ind][mask] = self.reset_cluster_size            
 
     def expire_codes_(self, batch_samples):
         if self.threshold_ema_dead_code == 0:
             return
 
         expired_codes = self.cluster_size < self.threshold_ema_dead_code
```

### Comparing `vector_quantize_pytorch-1.2.2/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.2.2
+Version: 1.2.3
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

