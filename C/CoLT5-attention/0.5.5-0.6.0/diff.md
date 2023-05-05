# Comparing `tmp/CoLT5-attention-0.5.5.tar.gz` & `tmp/CoLT5-attention-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.5.5.tar", last modified: Thu May  4 21:26:34 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.6.0.tar", last modified: Fri May  5 16:21:40 2023, max compression
```

## Comparing `CoLT5-attention-0.5.5.tar` & `CoLT5-attention-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:26:34.520100 CoLT5-attention-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:26:34.516100 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 21:26:34.000000 CoLT5-attention-0.5.5/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 21:26:34.520100 CoLT5-attention-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:26:34.520100 CoLT5-attention-0.5.5/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)    29424 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:26:34.520100 CoLT5-attention-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 21:26:03.000000 CoLT5-attention-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 16:21:40.000000 CoLT5-attention-0.6.0/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29733 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:21:40.651231 CoLT5-attention-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-05 16:21:26.000000 CoLT5-attention-0.6.0/setup.py
```

### Comparing `CoLT5-attention-0.5.5/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.6.0/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.5.5
+Version: 0.6.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.5.5/LICENSE` & `CoLT5-attention-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.5/PKG-INFO` & `CoLT5-attention-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.5.5
+Version: 0.6.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.5.5/README.md` & `CoLT5-attention-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,27 +163,26 @@
 ## Todo
 
 - [x] add the coordinate descent method as another router
 - [x] allow for multi-headed routing (multiple routing tokens), only for key-values
 - [x] add an autoregressive version of the conditionally routed attention
 - [x] test out the autoregressive version and verify that more routed key / value tokens lead to better results - it works
 - [x] make flash attention compatible
-
-- [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
-- [ ] fused coordinate descent kernel using triton
+- [x] fused coordinate descent kernel using triton
     - [x] forwards        
     - [x] backwards
-    - [x] add some tests and benchmark for triton vs plain pytorch coor_descent - 10x faster for forward, 4x faster for backwards and memory saved is n_iters times
+    - [x] benchmark triton vs plain pytorch coor_descent - 50 iterations with 4 segments - 17x faster for forward (7.23 vs 0.41), 7.2x faster for backwards (5.77 vs 0.80)
     - [x] fall back on plain coordinate descent for cpu
     - [x] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
     - [x] fix masking in coordinate descent
     - [x] simplified some logic within the triton kernel and the problem went away. probably some tiny quirk with the compiler
     - [x] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached. to get around this initially, one can fold a million token sequence into ~9 131k and uniformly route. offer uniform routing scheme within router itself
     - [x] remove sinkhorn and cumulative softmax approaches and cleanup; neither can work as well as coordinate descent
-    - [ ] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
+    - [x] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
+- [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -81,35 +81,35 @@
 use_flash_attn = True # use flash attention in heavy branch ).cuda() attn_out =
 attn(tokens) + tokens # (2, 8192, 512) - output of attention with residual
 (prenorm is included) ``` ## Todo - [x] add the coordinate descent method as
 another router - [x] allow for multi-headed routing (multiple routing tokens),
 only for key-values - [x] add an autoregressive version of the conditionally
 routed attention - [x] test out the autoregressive version and verify that more
 routed key / value tokens lead to better results - it works - [x] make flash
-attention compatible - [ ] create a variant of CoLT5 for high resolution
-feature maps (image attention) - then try out for diffusion - [ ] fused
-coordinate descent kernel using triton - [x] forwards - [x] backwards - [x] add
-some tests and benchmark for triton vs plain pytorch coor_descent - 10x faster
-for forward, 4x faster for backwards and memory saved is n_iters times - [x]
-fall back on plain coordinate descent for cpu - [x] handle edge case for when a
-row is completely masked out for triton, or simply enforce it never to be so -
-[x] fix masking in coordinate descent - [x] simplified some logic within the
-triton kernel and the problem went away. probably some tiny quirk with the
-compiler - [x] maximum block size in triton allowed is 131k, make sure at least
-quarter of million sequence length can be reached. to get around this
-initially, one can fold a million token sequence into ~9 131k and uniformly
-route. offer uniform routing scheme within router itself - [x] remove sinkhorn
-and cumulative softmax approaches and cleanup; neither can work as well as
-coordinate descent - [ ] allow for saving intermediates every number of
-iterations - trading memory for recompute efficiency during backwards ##
-Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster
-Long-Range Transformers with Conditional Computation}, author = {Joshua Ainslie
-and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and
-Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay
-and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
+attention compatible - [x] fused coordinate descent kernel using triton - [x]
+forwards - [x] backwards - [x] benchmark triton vs plain pytorch coor_descent -
+50 iterations with 4 segments - 17x faster for forward (7.23 vs 0.41), 7.2x
+faster for backwards (5.77 vs 0.80) - [x] fall back on plain coordinate descent
+for cpu - [x] handle edge case for when a row is completely masked out for
+triton, or simply enforce it never to be so - [x] fix masking in coordinate
+descent - [x] simplified some logic within the triton kernel and the problem
+went away. probably some tiny quirk with the compiler - [x] maximum block size
+in triton allowed is 131k, make sure at least quarter of million sequence
+length can be reached. to get around this initially, one can fold a million
+token sequence into ~9 131k and uniformly route. offer uniform routing scheme
+within router itself - [x] remove sinkhorn and cumulative softmax approaches
+and cleanup; neither can work as well as coordinate descent - [x] allow for
+saving intermediates every number of iterations - trading memory for recompute
+efficiency during backwards - [ ] create a variant of CoLT5 for high resolution
+feature maps (image attention) - then try out for diffusion ## Citations
+```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
+Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
+Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
+Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
+Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
 {Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
 tiled neural network computations}, author = {Philippe Tillet and H. Kung and
 D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
 on Machine Learning and Programming Languages}, year = {2019} } ``` ```bibtex
 @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
 Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
 Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
```

### Comparing `CoLT5-attention-0.5.5/colt5_attention/attend.py` & `CoLT5-attention-0.6.0/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.5/colt5_attention/coor_descent.py` & `CoLT5-attention-0.6.0/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.5.5/colt5_attention/transformer_block.py` & `CoLT5-attention-0.6.0/colt5_attention/transformer_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,33 +202,34 @@
     finally, used successfully by this paper for routing to heavy branch attention / feedforward
     """
 
     def __init__(
         self,
         dim,
         straight_through = True,
-        n_iters = 50,           # 50 iterations in the paper
-        fetch_k_ratio = 9 / 8,  # in the paper, they do a bit slightly higher k (times this ratio) for better learning
-        eps = 1.,               # the epsilon for coordinate descent. in CoLT5 paper they used 1. apparently
+        n_iters = 50,                   # 50 iterations in the paper
+        fetch_k_ratio = 9 / 8,          # in the paper, they do a bit slightly higher k (times this ratio) for better learning
+        eps = 1.,                       # the epsilon for coordinate descent. in CoLT5 paper they used 1. apparently
         num_routing_tokens = 1,
         use_triton = False,
-        route_block_size = None
+        route_block_size = None,
+        triton_checkpoint_segments = 4  # whether to recompute the coordinate descent in segments, with 4 and 50 iterations, backwards is sped up 3x times at the expense of forwards and some memory for saving initial a and b
     ):
         super().__init__()
         assert fetch_k_ratio >= 1.
         self.eps = eps
 
         self.n_iters = n_iters
         self.fetch_k_ratio = fetch_k_ratio
 
         self.coor_descent = coor_descent
 
         if use_triton:
             from colt5_attention.triton_coor_descent import triton_coor_descent
-            self.coor_descent = triton_coor_descent
+            self.coor_descent = partial(triton_coor_descent, checkpoint_segments = triton_checkpoint_segments)
 
         self.is_one_routing_token = num_routing_tokens == 1
         self.num_routing_tokens = num_routing_tokens
 
         self.route_block_size = route_block_size
 
         self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
```

### Comparing `CoLT5-attention-0.5.5/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.6.0/colt5_attention/triton_coor_descent.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,81 +21,98 @@
 assert version.parse(triton.__version__) >= version.parse('2.0')
 
 # helper functions
 
 def exists(val):
     return val is not None
 
+def default(val, d):
+    return val if exists(val) else d
+
 def calc_num_warps(block_size):
     num_warps = 4
     if block_size >= 2048:
         num_warps = 8
     if block_size >= 4096:
         num_warps = 16
     return num_warps
 
 def pack_one(t, pattern):
     return pack([t], pattern)
 
 def unpack_one(t, ps, pattern):
     return unpack(t, ps, pattern)[0]    
 
+def num_to_groups(num, groups):
+    assert 0 < groups <= num
+    floor = num // groups
+    remainder = num % groups
+    out = []
+    for ind in range(groups):
+        out.append(floor + int(ind < remainder))
+    assert sum(out) == num
+    return out
+
 # forwards
 
 @triton.jit
 def coor_descent_kernel_forward(
-    output_ptr,
+    a_ptr,
+    b_ptr,
     input_ptr,
     mask_ptr,
     k_ptr,
-    output_row_stride,
+    a_row_stride,
+    b_row_stride,
     input_row_stride,
     mask_row_stride,
     k_row_stride,
     n_iters,
     eps,
     n_cols,
     BLOCK_SIZE: tl.constexpr
 ):
     row_idx = tl.program_id(0)
-
-    row_start_ptr = input_ptr + row_idx * input_row_stride
-    k_ptr = k_ptr + row_idx * k_row_stride
-
     col_offsets = tl.arange(0, BLOCK_SIZE)
-    input_ptrs = row_start_ptr + col_offsets
-
     col_mask = col_offsets < n_cols
 
     # load mask as ints (for some reason as boolean breaks triton)
 
     mask_start_ptr = mask_ptr + row_idx * mask_row_stride
     mask_ptrs = mask_start_ptr + col_offsets
 
     mask_ints = tl.load(mask_ptrs, mask = col_mask, other = 0)
     mask = mask_ints == 1
 
+    # load a and b
+
+    a_ptr = a_ptr + row_idx * a_row_stride
+    a = tl.load(a_ptr)
+
+    b_start_ptr = b_ptr + row_idx * b_row_stride
+    b_ptrs = b_start_ptr + col_offsets
+    b = tl.load(b_ptrs, mask = col_mask, other = 0)
+
     # load the scores s
 
+    row_start_ptr = input_ptr + row_idx * input_row_stride
+    input_ptrs = row_start_ptr + col_offsets
     s = tl.load(input_ptrs, mask = mask, other = -float('inf'))
 
     # load k - controls the sparsity of output
 
+    k_ptr = k_ptr + row_idx * k_row_stride
     k = tl.load(k_ptr)
 
+    # initialize some constants
+
     constant = tl.log(k) * eps
 
     inv_eps = 1. / eps
 
-    # initialize a and b for coordinate descent
-
-    a = k * 0 # init a to 0, triton needs to know shape and type outside loop
-
-    b = -s
-
     for _ in range(n_iters):        
 
         a = (s + b) * inv_eps
         a = tl.where(mask, a, -float('inf'))
 
         # stable log sum exp
 
@@ -108,37 +125,38 @@
         a = constant - eps * log_sum_exp
 
         # update b
 
         b = s + a
         b = tl.where(b >= 0., -b, 0.)
 
-    s = tl.exp((s + a + b) * inv_eps)
+    # store a and b
 
-    output_row_start_ptr = output_ptr + row_idx * output_row_stride
-    output_ptrs = output_row_start_ptr + col_offsets
-
-    s = tl.where(mask, s, 0.)
-    tl.store(output_ptrs, s)
+    tl.store(a_ptr, a)
+    tl.store(b_ptrs, b, mask = col_mask)
 
 # backwards
 
 @triton.jit
 def coor_descent_kernel_backward(
-    output_ptr,
     dk_ptr,
     input_ptr,
+    a_ptr,
+    b_ptr,
     mask_ptr,
     ds_ptr,
+    db_ptr,
     k_ptr,
-    output_row_stride,
     dk_row_stride,
     input_row_stride,
+    a_row_stride,
+    b_row_stride,
     mask_row_stride,
     ds_row_stride,
+    db_row_stride,
     k_row_stride,
     n_iters,
     eps,
     n_cols,
     BLOCK_SIZE: tl.constexpr
 ):
     row_idx = tl.program_id(0)
@@ -152,14 +170,23 @@
 
     mask_start_ptr = mask_ptr + row_idx * mask_row_stride
     mask_ptrs = mask_start_ptr + col_offsets
 
     mask_ints = tl.load(mask_ptrs, mask = col_mask, other = 0)
     mask = mask_ints == 1
 
+     # load a and b
+
+    a_ptr = a_ptr + row_idx * a_row_stride
+    init_a = tl.load(a_ptr)
+
+    b_start_ptr = b_ptr + row_idx * b_row_stride
+    b_ptrs = b_start_ptr + col_offsets
+    init_b = tl.load(b_ptrs, mask = mask, other = 0)
+
     # load input
 
     row_start_ptr = input_ptr + row_idx * input_row_stride
     input_ptrs = row_start_ptr + col_offsets
 
     s = tl.load(input_ptrs, mask = mask, other = -float('inf'))
 
@@ -173,30 +200,29 @@
     # load initial ds
 
     ds_row_start_ptr = ds_ptr + row_idx * ds_row_stride
     ds_ptrs = ds_row_start_ptr + col_offsets
 
     ds = tl.load(ds_ptrs, mask = mask, other = 0.)
 
-    # initial a and b
+    # load initial db
 
-    init_a = k * 0
-    init_b = -s
+    db_row_start_ptr = db_ptr + row_idx * db_row_stride
+    db_ptrs = db_row_start_ptr + col_offsets
 
-    # output, which is dx (ds) and dk
+    db = tl.load(db_ptrs, mask = mask, other = 0.)
 
-    dk = 0.
+    # load initial dk
 
-    # temp variables
+    dk_ptr = dk_ptr + row_idx * dk_row_stride
+    dk = tl.load(dk_ptr)
 
-    last_da = k * 0
+    # temp variables
 
     inv_eps = 1. / eps
-
-    db = ds
     last_da = tl.sum(ds, axis = 0)
 
     # backwards
 
     for ind in range(n_iters):
         a = init_a
         b = init_b
@@ -240,48 +266,46 @@
         dsb = da * -softmax
 
         ds += dsb
         db = dsb
 
         last_da = 0.
 
-    ds += -db
-
-    dk *= eps / k
-
     # store dk
 
-    dk_ptr = dk_ptr + row_idx * dk_row_stride
     tl.store(dk_ptr, dk)
 
-    # store output
-
-    output_row_start_ptr = output_ptr + row_idx * output_row_stride
-    output_ptrs = output_row_start_ptr + col_offsets
+    # store ds
 
     ds = tl.where(mask, ds, 0.)
-    tl.store(output_ptrs, ds)
+    tl.store(ds_ptrs, ds)
+
+    # store db
+
+    db = tl.where(mask, db, 0.)
+    tl.store(db_ptrs, db)
 
 # function forwards and backwards
 
 class _coor_descent(autograd.Function):
     @classmethod
     def forward(
         self,
         ctx,
         x,
         n_iters,
         k,
         eps,
-        mask
+        mask,
+        checkpoint_segments
     ):
         assert n_iters > 0
         assert x.is_cuda, 'triton coordinate descent must be on cuda'
 
-        batch, requires_grad = x.shape[0], x.requires_grad
+        batch, requires_grad, device = x.shape[0], x.requires_grad, x.device
 
         if not exists(mask):
             mask = torch.ones_like(x, dtype = torch.bool, device = x.device)
 
         x, shape = pack_one(x, '* n')
         mask, _ = pack_one(mask, '* n')
 
@@ -299,35 +323,51 @@
 
         BLOCK_SIZE = triton.next_power_of_2(n_cols)
 
         assert BLOCK_SIZE <= 131072, 'the maximum block size allowed is 131072 for triton cuda kernel - set the `route_block_size` for the CoordinateDescentRouter to be this value or less in order to uniformly route to get around this limitation'
 
         num_warps = calc_num_warps(BLOCK_SIZE)
 
-        y = torch.empty_like(x)
+        a = torch.zeros_like(k)
+        b = -x
 
-        coor_descent_kernel_forward[(n_rows,)](
-            y,
-            x,
-            mask_ints,
-            k,
-            y.stride(0),
-            x.stride(0),
-            mask_ints.stride(0),
-            k.stride(0),
-            n_iters,
-            eps,
-            n_cols,
-            num_warps = num_warps,
-            BLOCK_SIZE = BLOCK_SIZE,
-        )
+        checkpoint_in_segments = checkpoint_segments > 1
+        checkpointed_a = torch.empty((checkpoint_segments - 1, n_rows), device = device, dtype = a.dtype)
+        checkpointed_b = torch.empty((checkpoint_segments - 1, n_rows, n_cols), device = device, dtype = b.dtype)
+
+        for ind, segment_iters in enumerate(num_to_groups(n_iters, checkpoint_segments)):
+            is_first = 0
+
+            if not is_first and checkpoint_in_segments:
+                checkpointed_a[ind - 1] = a
+                checkpointed_b[ind - 1] = b
+
+            coor_descent_kernel_forward[(n_rows,)](
+                a,
+                b,
+                x,
+                mask_ints,
+                k,
+                a.stride(0),
+                b.stride(0),
+                x.stride(0),
+                mask_ints.stride(0),
+                k.stride(0),
+                segment_iters,
+                eps,
+                n_cols,
+                num_warps = num_warps,
+                BLOCK_SIZE = BLOCK_SIZE,
+            )
+
+        y = torch.exp((a[..., None] + b + x) / eps)
 
         if requires_grad:
-            ctx.args = (n_iters, eps)
-            ctx.save_for_backward(x, y, k, mask)
+            ctx.args = (n_iters, checkpoint_segments, eps)
+            ctx.save_for_backward(x, y, k, mask, checkpointed_a, checkpointed_b)
 
         y = unpack_one(y, shape, '* n')
 
         return y
 
     @classmethod
     def backward(
@@ -335,66 +375,83 @@
         ctx,
         grad_probs
     ):
         assert grad_probs.is_cuda
 
         batch = grad_probs.shape[0]
 
-        n_iters, eps = ctx.args
-        x, y, k, mask = ctx.saved_tensors
+        n_iters, checkpoint_segments, eps = ctx.args
+        x, y, k, mask, checkpointed_a, checkpointed_b = ctx.saved_tensors
 
         grad_probs, shape = pack_one(grad_probs, '* n')
 
         if exists(mask):
             grad_probs = grad_probs.masked_fill(~mask, 0.)
 
-        ds = grad_probs * y / eps
-
         n_rows, n_cols = grad_probs.shape
 
         BLOCK_SIZE = triton.next_power_of_2(n_cols)
         num_warps = calc_num_warps(BLOCK_SIZE)
 
-        dx = torch.empty_like(grad_probs)
-        dk = torch.empty_like(k)
+        ds = grad_probs * y / eps
+        db = ds.clone()
+        dk = torch.zeros_like(k)
 
         mask_int = mask.int()
 
-        coor_descent_kernel_backward[(n_rows,)](
-            dx,
-            dk,
-            x,
-            mask_int,
-            ds,
-            k,
-            dx.stride(0),
-            dk.stride(0),
-            x.stride(0),
-            mask_int.stride(0),
-            ds.stride(0),
-            k.stride(0),
-            n_iters,
-            eps,
-            n_cols,
-            num_warps = num_warps,
-            BLOCK_SIZE = BLOCK_SIZE
+        a = torch.zeros_like(k)
+        b = -x
+
+        items = zip(
+            reversed([a, *checkpointed_a.unbind(dim = 0)]),
+            reversed([b, *checkpointed_b.unbind(dim = 0)]),
+            reversed(num_to_groups(n_iters, checkpoint_segments))
         )
 
-        dx = unpack_one(dx, shape, '* n')
+        for init_a, init_b, segment_iters, in items:
+            coor_descent_kernel_backward[(n_rows,)](
+                dk,
+                x,
+                init_a,
+                init_b,
+                mask_int,
+                ds,
+                db,
+                k,
+                dk.stride(0),
+                x.stride(0),
+                init_a.stride(0),
+                init_b.stride(0),
+                mask_int.stride(0),
+                ds.stride(0),
+                db.stride(0),
+                k.stride(0),
+                segment_iters,
+                eps,
+                n_cols,
+                num_warps = num_warps,
+                BLOCK_SIZE = BLOCK_SIZE
+            )
+
+        ds += -db
+        ds = unpack_one(ds, shape, '* n')
 
         if not k.requires_grad:
             dk = None
+        else:
+            dk *= eps / k
 
-        return dx, None, dk, None, None
+        return ds, None, dk, None, None, None
 
 def triton_coor_descent(
     s,
     *,
     n_iters,
     k,
     eps = 1e-1,
-    mask = None
+    mask = None,
+    checkpoint_segments = 1
 ):
     if not s.is_cuda:
         return coor_descent(s, n_iters = n_iters, k = k, eps = eps, mask = mask)
 
-    return _coor_descent.apply(s, n_iters, k, eps, mask)
+    return _coor_descent.apply(s, n_iters, k, eps, mask, checkpoint_segments)
```

### Comparing `CoLT5-attention-0.5.5/setup.py` & `CoLT5-attention-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.5.5',
+  version = '0.6.0',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

