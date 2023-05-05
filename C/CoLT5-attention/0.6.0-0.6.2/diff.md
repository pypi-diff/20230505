# Comparing `tmp/CoLT5-attention-0.6.0.tar.gz` & `tmp/CoLT5-attention-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.6.0.tar", last modified: Fri May  5 16:21:40 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.6.2.tar", last modified: Fri May  5 16:53:20 2023, max compression
```

## Comparing `CoLT5-attention-0.6.0.tar` & `CoLT5-attention-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)    29733 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29733 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/setup.py
```

### Comparing `CoLT5-attention-0.6.0/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.6.2/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.6.0
+Version: 0.6.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.6.0/LICENSE` & `CoLT5-attention-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.6.0/PKG-INFO` & `CoLT5-attention-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.6.0
+Version: 0.6.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.6.0/README.md` & `CoLT5-attention-0.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -166,22 +166,24 @@
 - [x] allow for multi-headed routing (multiple routing tokens), only for key-values
 - [x] add an autoregressive version of the conditionally routed attention
 - [x] test out the autoregressive version and verify that more routed key / value tokens lead to better results - it works
 - [x] make flash attention compatible
 - [x] fused coordinate descent kernel using triton
     - [x] forwards        
     - [x] backwards
-    - [x] benchmark triton vs plain pytorch coor_descent - 50 iterations with 4 segments - 17x faster for forward (7.23 vs 0.41), 7.2x faster for backwards (5.77 vs 0.80)
+    - [x] benchmark triton vs plain pytorch coor_descent - 50 iterations with 4 segments - 18.5x faster for forward (7.23 vs 0.39), 7.2x faster for backwards (5.77 vs 0.80)
     - [x] fall back on plain coordinate descent for cpu
     - [x] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
     - [x] fix masking in coordinate descent
     - [x] simplified some logic within the triton kernel and the problem went away. probably some tiny quirk with the compiler
     - [x] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached. to get around this initially, one can fold a million token sequence into ~9 131k and uniformly route. offer uniform routing scheme within router itself
     - [x] remove sinkhorn and cumulative softmax approaches and cleanup; neither can work as well as coordinate descent
     - [x] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
+    - [x] in-place write to checkpointed a and b tensor for potentially savings on forward when recompute segments is high
+
 - [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
```

#### html2text {}

```diff
@@ -83,35 +83,36 @@
 (prenorm is included) ``` ## Todo - [x] add the coordinate descent method as
 another router - [x] allow for multi-headed routing (multiple routing tokens),
 only for key-values - [x] add an autoregressive version of the conditionally
 routed attention - [x] test out the autoregressive version and verify that more
 routed key / value tokens lead to better results - it works - [x] make flash
 attention compatible - [x] fused coordinate descent kernel using triton - [x]
 forwards - [x] backwards - [x] benchmark triton vs plain pytorch coor_descent -
-50 iterations with 4 segments - 17x faster for forward (7.23 vs 0.41), 7.2x
+50 iterations with 4 segments - 18.5x faster for forward (7.23 vs 0.39), 7.2x
 faster for backwards (5.77 vs 0.80) - [x] fall back on plain coordinate descent
 for cpu - [x] handle edge case for when a row is completely masked out for
 triton, or simply enforce it never to be so - [x] fix masking in coordinate
 descent - [x] simplified some logic within the triton kernel and the problem
 went away. probably some tiny quirk with the compiler - [x] maximum block size
 in triton allowed is 131k, make sure at least quarter of million sequence
 length can be reached. to get around this initially, one can fold a million
 token sequence into ~9 131k and uniformly route. offer uniform routing scheme
 within router itself - [x] remove sinkhorn and cumulative softmax approaches
 and cleanup; neither can work as well as coordinate descent - [x] allow for
 saving intermediates every number of iterations - trading memory for recompute
-efficiency during backwards - [ ] create a variant of CoLT5 for high resolution
-feature maps (image attention) - then try out for diffusion ## Citations
-```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
-Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
-Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
-Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
-Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
-{Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
-tiled neural network computations}, author = {Philippe Tillet and H. Kung and
-D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
-on Machine Learning and Programming Languages}, year = {2019} } ``` ```bibtex
-@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
-Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
-Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
-booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ```
+efficiency during backwards - [x] in-place write to checkpointed a and b tensor
+for potentially savings on forward when recompute segments is high - [ ] create
+a variant of CoLT5 for high resolution feature maps (image attention) - then
+try out for diffusion ## Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL,
+title = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
+author = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on
+and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and
+James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023}
+} ``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
+language and compiler for tiled neural network computations}, author =
+{Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
+SIGPLAN International Workshop on Machine Learning and Programming Languages},
+year = {2019} } ``` ```bibtex @inproceedings{dao2022flashattention, title =
+{Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-
+Awareness}, author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra,
+Atri and R{\'e}, Christopher}, booktitle = {Advances in Neural Information
+Processing Systems}, year = {2022} } ```
```

### Comparing `CoLT5-attention-0.6.0/colt5_attention/attend.py` & `CoLT5-attention-0.6.2/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.6.0/colt5_attention/coor_descent.py` & `CoLT5-attention-0.6.2/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.6.0/colt5_attention/transformer_block.py` & `CoLT5-attention-0.6.2/colt5_attention/transformer_block.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.6.0/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.6.2/colt5_attention/triton_coor_descent.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,19 +57,19 @@
 @triton.jit
 def coor_descent_kernel_forward(
     a_ptr,
     b_ptr,
     input_ptr,
     mask_ptr,
     k_ptr,
-    a_row_stride,
+    a_iter_stride,
     b_row_stride,
+    b_iter_stride,
     input_row_stride,
     mask_row_stride,
-    k_row_stride,
     n_iters,
     eps,
     n_cols,
     BLOCK_SIZE: tl.constexpr
 ):
     row_idx = tl.program_id(0)
     col_offsets = tl.arange(0, BLOCK_SIZE)
@@ -81,30 +81,30 @@
     mask_ptrs = mask_start_ptr + col_offsets
 
     mask_ints = tl.load(mask_ptrs, mask = col_mask, other = 0)
     mask = mask_ints == 1
 
     # load a and b
 
-    a_ptr = a_ptr + row_idx * a_row_stride
+    a_ptr = a_ptr + row_idx
     a = tl.load(a_ptr)
 
     b_start_ptr = b_ptr + row_idx * b_row_stride
     b_ptrs = b_start_ptr + col_offsets
     b = tl.load(b_ptrs, mask = col_mask, other = 0)
 
     # load the scores s
 
     row_start_ptr = input_ptr + row_idx * input_row_stride
     input_ptrs = row_start_ptr + col_offsets
     s = tl.load(input_ptrs, mask = mask, other = -float('inf'))
 
     # load k - controls the sparsity of output
 
-    k_ptr = k_ptr + row_idx * k_row_stride
+    k_ptr = k_ptr + row_idx
     k = tl.load(k_ptr)
 
     # initialize some constants
 
     constant = tl.log(k) * eps
 
     inv_eps = 1. / eps
@@ -125,39 +125,39 @@
         a = constant - eps * log_sum_exp
 
         # update b
 
         b = s + a
         b = tl.where(b >= 0., -b, 0.)
 
-    # store a and b
+    # store a and b for next round
 
-    tl.store(a_ptr, a)
-    tl.store(b_ptrs, b, mask = col_mask)
+    next_a_ptrs = a_ptr + a_iter_stride
+    next_b_ptrs = b_ptrs + b_iter_stride
+
+    tl.store(next_a_ptrs, a)
+    tl.store(next_b_ptrs, b, mask = col_mask)
 
 # backwards
 
 @triton.jit
 def coor_descent_kernel_backward(
     dk_ptr,
     input_ptr,
     a_ptr,
     b_ptr,
     mask_ptr,
     ds_ptr,
     db_ptr,
     k_ptr,
-    dk_row_stride,
     input_row_stride,
-    a_row_stride,
     b_row_stride,
     mask_row_stride,
     ds_row_stride,
     db_row_stride,
-    k_row_stride,
     n_iters,
     eps,
     n_cols,
     BLOCK_SIZE: tl.constexpr
 ):
     row_idx = tl.program_id(0)
     col_offsets = tl.arange(0, BLOCK_SIZE)
@@ -172,15 +172,15 @@
     mask_ptrs = mask_start_ptr + col_offsets
 
     mask_ints = tl.load(mask_ptrs, mask = col_mask, other = 0)
     mask = mask_ints == 1
 
      # load a and b
 
-    a_ptr = a_ptr + row_idx * a_row_stride
+    a_ptr = a_ptr + row_idx
     init_a = tl.load(a_ptr)
 
     b_start_ptr = b_ptr + row_idx * b_row_stride
     b_ptrs = b_start_ptr + col_offsets
     init_b = tl.load(b_ptrs, mask = mask, other = 0)
 
     # load input
@@ -188,15 +188,15 @@
     row_start_ptr = input_ptr + row_idx * input_row_stride
     input_ptrs = row_start_ptr + col_offsets
 
     s = tl.load(input_ptrs, mask = mask, other = -float('inf'))
 
     # load k - controls the sparsity of output
 
-    k_ptr = k_ptr + row_idx * k_row_stride
+    k_ptr = k_ptr + row_idx
 
     k = tl.load(k_ptr)
     constant = tl.log(k) * eps
 
     # load initial ds
 
     ds_row_start_ptr = ds_ptr + row_idx * ds_row_stride
@@ -209,15 +209,15 @@
     db_row_start_ptr = db_ptr + row_idx * db_row_stride
     db_ptrs = db_row_start_ptr + col_offsets
 
     db = tl.load(db_ptrs, mask = mask, other = 0.)
 
     # load initial dk
 
-    dk_ptr = dk_ptr + row_idx * dk_row_stride
+    dk_ptr = dk_ptr + row_idx
     dk = tl.load(dk_ptr)
 
     # temp variables
 
     inv_eps = 1. / eps
     last_da = tl.sum(ds, axis = 0)
 
@@ -297,15 +297,15 @@
         eps,
         mask,
         checkpoint_segments
     ):
         assert n_iters > 0
         assert x.is_cuda, 'triton coordinate descent must be on cuda'
 
-        batch, requires_grad, device = x.shape[0], x.requires_grad, x.device
+        batch, requires_grad, device, dtype = x.shape[0], x.requires_grad, x.device, x.dtype
 
         if not exists(mask):
             mask = torch.ones_like(x, dtype = torch.bool, device = x.device)
 
         x, shape = pack_one(x, '* n')
         mask, _ = pack_one(mask, '* n')
 
@@ -323,49 +323,48 @@
 
         BLOCK_SIZE = triton.next_power_of_2(n_cols)
 
         assert BLOCK_SIZE <= 131072, 'the maximum block size allowed is 131072 for triton cuda kernel - set the `route_block_size` for the CoordinateDescentRouter to be this value or less in order to uniformly route to get around this limitation'
 
         num_warps = calc_num_warps(BLOCK_SIZE)
 
-        a = torch.zeros_like(k)
-        b = -x
+        checkpointed_a = torch.empty((checkpoint_segments + 1, n_rows), device = device, dtype = dtype)
+        checkpointed_b = torch.empty((checkpoint_segments + 1, n_rows, n_cols), device = device, dtype = dtype)
 
-        checkpoint_in_segments = checkpoint_segments > 1
-        checkpointed_a = torch.empty((checkpoint_segments - 1, n_rows), device = device, dtype = a.dtype)
-        checkpointed_b = torch.empty((checkpoint_segments - 1, n_rows, n_cols), device = device, dtype = b.dtype)
+        checkpointed_a[0] = torch.zeros_like(k)
+        checkpointed_b[0] = -x
 
         for ind, segment_iters in enumerate(num_to_groups(n_iters, checkpoint_segments)):
-            is_first = 0
-
-            if not is_first and checkpoint_in_segments:
-                checkpointed_a[ind - 1] = a
-                checkpointed_b[ind - 1] = b
+            is_last = ind == (checkpoint_segments - 1)
 
             coor_descent_kernel_forward[(n_rows,)](
-                a,
-                b,
+                checkpointed_a[ind],
+                checkpointed_b[ind],
                 x,
                 mask_ints,
                 k,
-                a.stride(0),
-                b.stride(0),
+                checkpointed_a.stride(0),
+                n_cols,
+                checkpointed_b.stride(0),
                 x.stride(0),
                 mask_ints.stride(0),
-                k.stride(0),
                 segment_iters,
                 eps,
                 n_cols,
                 num_warps = num_warps,
                 BLOCK_SIZE = BLOCK_SIZE,
             )
 
-        y = torch.exp((a[..., None] + b + x) / eps)
+        last_a, last_b = map(lambda t: t[-1], (checkpointed_a, checkpointed_b))
+        y = torch.exp((last_a[..., None] + last_b + x) / eps)
 
         if requires_grad:
+            checkpointed_a = checkpointed_a[:-1]
+            checkpointed_b = checkpointed_b[:-1]
+
             ctx.args = (n_iters, checkpoint_segments, eps)
             ctx.save_for_backward(x, y, k, mask, checkpointed_a, checkpointed_b)
 
         y = unpack_one(y, shape, '* n')
 
         return y
 
@@ -394,41 +393,35 @@
 
         ds = grad_probs * y / eps
         db = ds.clone()
         dk = torch.zeros_like(k)
 
         mask_int = mask.int()
 
-        a = torch.zeros_like(k)
-        b = -x
-
         items = zip(
-            reversed([a, *checkpointed_a.unbind(dim = 0)]),
-            reversed([b, *checkpointed_b.unbind(dim = 0)]),
+            reversed(checkpointed_a.unbind(dim = 0)),
+            reversed(checkpointed_b.unbind(dim = 0)),
             reversed(num_to_groups(n_iters, checkpoint_segments))
         )
 
         for init_a, init_b, segment_iters, in items:
             coor_descent_kernel_backward[(n_rows,)](
                 dk,
                 x,
                 init_a,
                 init_b,
                 mask_int,
                 ds,
                 db,
                 k,
-                dk.stride(0),
                 x.stride(0),
-                init_a.stride(0),
                 init_b.stride(0),
                 mask_int.stride(0),
                 ds.stride(0),
                 db.stride(0),
-                k.stride(0),
                 segment_iters,
                 eps,
                 n_cols,
                 num_warps = num_warps,
                 BLOCK_SIZE = BLOCK_SIZE
             )
```

### Comparing `CoLT5-attention-0.6.0/setup.py` & `CoLT5-attention-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.6.0',
+  version = '0.6.2',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

