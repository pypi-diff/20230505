# Comparing `tmp/tensorizer-1.0.1.tar.gz` & `tmp/tensorizer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorizer-1.0.1.tar", last modified: Wed Mar 22 01:38:11 2023, max compression
+gzip compressed data, was "tensorizer-1.1.0.tar", last modified: Fri May  5 20:46:36 2023, max compression
```

## Comparing `tensorizer-1.0.1.tar` & `tensorizer-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 esyra     (1000) esyra     (1000)        0 2023-03-22 01:38:11.363676 tensorizer-1.0.1/
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     7407 2023-03-07 19:10:06.000000 tensorizer-1.0.1/CMakeLists.txt
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     1049 2023-03-16 20:33:00.000000 tensorizer-1.0.1/LICENSE
--rw-rw-r--   0 esyra     (1000) esyra     (1000)       48 2023-03-20 20:37:06.000000 tensorizer-1.0.1/MANIFEST.in
--rw-rw-r--   0 esyra     (1000) esyra     (1000)    21099 2023-03-22 01:38:11.363676 tensorizer-1.0.1/PKG-INFO
--rw-rw-r--   0 esyra     (1000) esyra     (1000)    20298 2023-03-21 16:32:51.000000 tensorizer-1.0.1/README.md
-drwxrwxr-x   0 esyra     (1000) esyra     (1000)        0 2023-03-22 01:38:11.351676 tensorizer-1.0.1/proto/
--rw-rw-r--   0 esyra     (1000) esyra     (1000)       52 2023-03-07 19:10:06.000000 tensorizer-1.0.1/proto/requirements.txt
--rw-rw-r--   0 esyra     (1000) esyra     (1000)      921 2023-03-07 19:10:06.000000 tensorizer-1.0.1/proto/tensors.proto
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     1112 2023-03-22 01:37:26.000000 tensorizer-1.0.1/pyproject.toml
--rw-rw-r--   0 esyra     (1000) esyra     (1000)       38 2023-03-22 01:38:11.363676 tensorizer-1.0.1/setup.cfg
-drwxrwxr-x   0 esyra     (1000) esyra     (1000)        0 2023-03-22 01:38:11.355677 tensorizer-1.0.1/tensorizer/
--rw-rw-r--   0 esyra     (1000) esyra     (1000)      183 2023-03-21 16:32:51.000000 tensorizer-1.0.1/tensorizer/__init__.py
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     6709 2023-03-21 16:32:51.000000 tensorizer-1.0.1/tensorizer/_wide_pipes.py
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     5370 2023-03-21 16:32:51.000000 tensorizer-1.0.1/tensorizer/protobuf.py
--rw-rw-r--   0 esyra     (1000) esyra     (1000)    43510 2023-03-21 16:37:33.000000 tensorizer-1.0.1/tensorizer/serialization.py
--rw-rw-r--   0 esyra     (1000) esyra     (1000)    24734 2023-03-22 01:37:26.000000 tensorizer-1.0.1/tensorizer/stream_io.py
--rw-rw-r--   0 esyra     (1000) esyra     (1000)      921 2023-03-07 19:10:06.000000 tensorizer-1.0.1/tensorizer/tensors.proto
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     4121 2023-03-07 19:10:06.000000 tensorizer-1.0.1/tensorizer/tensors_pb2.py
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     3873 2023-03-21 16:32:51.000000 tensorizer-1.0.1/tensorizer/utils.py
-drwxrwxr-x   0 esyra     (1000) esyra     (1000)        0 2023-03-22 01:38:11.355677 tensorizer-1.0.1/tensorizer.egg-info/
--rw-rw-r--   0 esyra     (1000) esyra     (1000)    21099 2023-03-22 01:38:11.000000 tensorizer-1.0.1/tensorizer.egg-info/PKG-INFO
--rw-rw-r--   0 esyra     (1000) esyra     (1000)      752 2023-03-22 01:38:11.000000 tensorizer-1.0.1/tensorizer.egg-info/SOURCES.txt
--rw-rw-r--   0 esyra     (1000) esyra     (1000)        1 2023-03-22 01:38:11.000000 tensorizer-1.0.1/tensorizer.egg-info/dependency_links.txt
--rw-rw-r--   0 esyra     (1000) esyra     (1000)       72 2023-03-22 01:38:11.000000 tensorizer-1.0.1/tensorizer.egg-info/requires.txt
--rw-rw-r--   0 esyra     (1000) esyra     (1000)       11 2023-03-22 01:38:11.000000 tensorizer-1.0.1/tensorizer.egg-info/top_level.txt
-drwxrwxr-x   0 esyra     (1000) esyra     (1000)        0 2023-03-22 01:38:11.359676 tensorizer-1.0.1/tensors/
--rw-rw-r--   0 esyra     (1000) esyra     (1000)        0 2023-03-07 19:10:06.000000 tensorizer-1.0.1/tensors/__init__.py
-drwxrwxr-x   0 esyra     (1000) esyra     (1000)        0 2023-03-22 01:38:11.359676 tensorizer-1.0.1/tensors/__pycache__/
--rw-rw-r--   0 esyra     (1000) esyra     (1000)      145 2023-03-16 22:38:55.000000 tensorizer-1.0.1/tensors/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     2631 2023-03-16 22:39:04.000000 tensorizer-1.0.1/tensors/__pycache__/tensors_pb2.cpython-310.pyc
--rw-rw-r--   0 esyra     (1000) esyra     (1000)      100 2023-03-07 19:10:06.000000 tensorizer-1.0.1/tensors/go.mod
--rw-rw-r--   0 esyra     (1000) esyra     (1000)      739 2023-03-07 19:10:06.000000 tensorizer-1.0.1/tensors/go.sum
--rw-rw-r--   0 esyra     (1000) esyra     (1000)    18826 2023-03-07 19:10:06.000000 tensorizer-1.0.1/tensors/tensors.pb.go
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     4846 2023-03-07 19:10:06.000000 tensorizer-1.0.1/tensors/tensors_pb.d.ts
--rw-rw-r--   0 esyra     (1000) esyra     (1000)    29992 2023-03-07 19:10:06.000000 tensorizer-1.0.1/tensors/tensors_pb.js
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     4121 2023-03-07 19:10:06.000000 tensorizer-1.0.1/tensors/tensors_pb2.py
-drwxrwxr-x   0 esyra     (1000) esyra     (1000)        0 2023-03-22 01:38:11.363676 tensorizer-1.0.1/tests/
--rw-rw-r--   0 esyra     (1000) esyra     (1000)    10673 2023-03-22 01:37:26.000000 tensorizer-1.0.1/tests/test_serialization.py
--rw-rw-r--   0 esyra     (1000) esyra     (1000)     5869 2023-03-21 16:57:25.000000 tensorizer-1.0.1/tests/test_stream_io.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.964947 tensorizer-1.1.0/
+-rw-rw-r--   0 root         (0) root         (0)     7407 2023-03-07 19:10:06.000000 tensorizer-1.1.0/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-1.1.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       48 2023-03-20 20:37:06.000000 tensorizer-1.1.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)    21912 2023-05-05 20:46:36.964947 tensorizer-1.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    21111 2023-05-02 19:45:36.000000 tensorizer-1.1.0/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.936947 tensorizer-1.1.0/proto/
+-rw-rw-r--   0 root         (0) root         (0)       52 2023-03-07 19:10:06.000000 tensorizer-1.1.0/proto/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-1.1.0/proto/tensors.proto
+-rw-rw-r--   0 root         (0) root         (0)     1530 2023-05-02 20:22:23.000000 tensorizer-1.1.0/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-05-05 20:46:36.964947 tensorizer-1.1.0/setup.cfg
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.944947 tensorizer-1.1.0/tensorizer/
+-rw-rw-r--   0 root         (0) root         (0)      183 2023-05-02 18:44:59.000000 tensorizer-1.1.0/tensorizer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6709 2023-05-02 19:17:39.000000 tensorizer-1.1.0/tensorizer/_wide_pipes.py
+-rw-rw-r--   0 root         (0) root         (0)     5415 2023-05-02 19:22:34.000000 tensorizer-1.1.0/tensorizer/protobuf.py
+-rw-rw-r--   0 root         (0) root         (0)    46239 2023-05-02 19:18:50.000000 tensorizer-1.1.0/tensorizer/serialization.py
+-rw-rw-r--   0 root         (0) root         (0)    26472 2023-05-02 19:18:13.000000 tensorizer-1.1.0/tensorizer/stream_io.py
+-rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensorizer/tensors.proto
+-rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-1.1.0/tensorizer/tensors_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    12109 2023-05-05 20:43:52.000000 tensorizer-1.1.0/tensorizer/utils.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.948947 tensorizer-1.1.0/tensorizer.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)    21912 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      768 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       11 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/top_level.txt
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.956947 tensorizer-1.1.0/tensors/
+-rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-1.1.0/tensors/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/__init__.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.960947 tensorizer-1.1.0/tensors/__pycache__/
+-rw-rw-r--   0 root         (0) root         (0)      145 2023-03-16 22:38:55.000000 tensorizer-1.1.0/tensors/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 root         (0) root         (0)     2631 2023-03-16 22:39:04.000000 tensorizer-1.1.0/tensors/__pycache__/tensors_pb2.cpython-310.pyc
+-rw-rw-r--   0 root         (0) root         (0)      100 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/go.mod
+-rw-rw-r--   0 root         (0) root         (0)      739 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/go.sum
+-rw-rw-r--   0 root         (0) root         (0)    18826 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/tensors.pb.go
+-rw-rw-r--   0 root         (0) root         (0)     4846 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/tensors_pb.d.ts
+-rw-rw-r--   0 root         (0) root         (0)    29992 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/tensors_pb.js
+-rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-1.1.0/tensors/tensors_pb2.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.960947 tensorizer-1.1.0/tests/
+-rw-rw-r--   0 root         (0) root         (0)    10621 2023-05-02 19:38:57.000000 tensorizer-1.1.0/tests/test_serialization.py
+-rw-rw-r--   0 root         (0) root         (0)     5871 2023-05-02 19:40:40.000000 tensorizer-1.1.0/tests/test_stream_io.py
```

### Comparing `tensorizer-1.0.1/CMakeLists.txt` & `tensorizer-1.1.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/LICENSE` & `tensorizer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/PKG-INFO` & `tensorizer-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorizer
-Version: 1.0.1
+Version: 1.1.0
 Summary: A tool for fast PyTorch module, model, and tensor serialization + deserialization.
 Author: CoreWeave
 License: MIT License
 Project-URL: Homepage, https://github.com/coreweave/tensorizer
 Keywords: tensorizer,machine learning,serialization,tensor,pytorch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -94,31 +94,31 @@
 The below example serializes the `EleutherAI/gpt-j-6B` model to an S3
 endpoint. It assumes that you have already configured your S3
 credentials in `~/.s3cfg`.
 
 **NOTE:** Loading and serializing `gpt-j-6B` will take a lot of CPU RAM,
 up to `~20GB`. Additionally, when loading `gpt-j-6B` into a GPU, you
 will need about `~16GB` of VRAM. If you don't have that much RAM or VRAM,
-you can use the smaller `gpt-neo-125m` model instead.
+you can use the smaller `gpt-neo-125M` model instead.
 
 **NOTE2:** The below examples require the `transformers` and `accelerate`
 libraries. You can install them with `pip`:
 ```bash
 python -m pip install transformers accelerate
 ```
 
 [serialize.py](examples/serialize.py)
 ```python
-from transformers import AutoModelForCausalLM
-from tensorizer import TensorSerializer
 import torch
+from tensorizer import TensorSerializer
+from transformers import AutoModelForCausalLM
 
 model_ref = "EleutherAI/gpt-j-6B"
 # For less intensive requirements, swap above with the line below:
-# model_ref = "EleutherAI/gpt-neo-125m"
+# model_ref = "EleutherAI/gpt-neo-125M"
 model_name = model_ref.split("/")[-1]
 # Change this to your S3 bucket.
 s3_bucket = "bucket"
 s3_uri = f"s3://{s3_bucket}/{model_name}.tensors"
 
 model = AutoModelForCausalLM.from_pretrained(
     model_ref,
@@ -141,42 +141,34 @@
 endpoint into the `torch.nn.Module`.
 
 The below example loads the `EleutherAI/gpt-j-6B` model from an S3
 endpoint.
 
 [deserialize.py](examples/deserialize.py)
 ```python
-import torch
-import os
 import time
+import torch
 from tensorizer import TensorDeserializer
 from tensorizer.utils import no_init_or_tensor, convert_bytes, get_mem_usage
-from collections import OrderedDict
-
-# disable missing keys and unexpected key warnings
-os.environ["TRANSFORMERS_VERBOSITY"] = "error"
 
 from transformers import AutoModelForCausalLM, AutoTokenizer, AutoConfig
 
 model_ref = "EleutherAI/gpt-j-6B"
 # To run this at home, swap this with the line below for a smaller example:
-# model_ref = "EleutherAI/gpt-neo-125m"
+# model_ref = "EleutherAI/gpt-neo-125M"
 model_name = model_ref.split("/")[-1]
 # Change this to your S3 bucket.
 s3_bucket = "bucket"
 s3_uri = f"s3://{s3_bucket}/{model_name}.tensors"
 
 config = AutoConfig.from_pretrained(model_ref)
 
 # This ensures that the model is not initialized.
-model = no_init_or_tensor(
-    lambda: AutoModelForCausalLM.from_pretrained(
-        None, config=config, state_dict=OrderedDict()
-    )
-)
+with no_init_or_tensor():
+    model = AutoModelForCausalLM.from_config(config)
 
 before_mem = get_mem_usage()
 
 # Lazy load the tensors from S3 into the model.
 start = time.time()
 deserializer = TensorDeserializer(s3_uri, plaid_mode=True)
 deserializer.load_into_module(model)
@@ -184,27 +176,30 @@
 
 # Brag about how fast we are.
 total_bytes_str = convert_bytes(deserializer.total_tensor_bytes)
 duration = end - start
 per_second = convert_bytes(deserializer.total_tensor_bytes / duration)
 after_mem = get_mem_usage()
 deserializer.close()
-print(f"Deserialized {total_bytes_str} in {end - start:0.2f}s, {per_second}")
+print(f"Deserialized {total_bytes_str} in {end - start:0.2f}s, {per_second}/s")
 print(f"Memory usage before: {before_mem}")
 print(f"Memory usage after: {after_mem}")
 
 # Tokenize and generate
 model.eval()
 tokenizer = AutoTokenizer.from_pretrained(model_ref)
+eos = tokenizer.eos_token_id
 input_ids = tokenizer.encode(
     "¡Hola! Encantado de conocerte. hoy voy a", return_tensors="pt"
 ).to("cuda")
 
 with torch.no_grad():
-    output = model.generate(input_ids, max_new_tokens=50, do_sample=True)
+    output = model.generate(
+        input_ids, max_new_tokens=50, do_sample=True, pad_token_id=eos
+    )
 
 print(f"Output: {tokenizer.decode(output[0], skip_special_tokens=True)}")
 ```
 
 It should produce output similar to the following, with GPT-J-6B:
 ```
 Deserialized model in 6.25 seconds
@@ -221,82 +216,82 @@
 and `hf_main()` serializes
 [HuggingFace Transformers](https://github.com/huggingface/transformers) models.
 
 ## Available Pre-Tensorized Models on the CoreWeave Cloud
 
 The following models are available on the CoreWeave Cloud for free, and can be
 used with the `TensorDeserializer` class. The S3 support defaults to the
-`accel-object.ord1.coreweave.com` endpoint, and the bucket to use `tensorized`.
+`accel-object.ord1.coreweave.com` endpoint, and the bucket to use as `tensorized`.
 
 We name the keys in the S3 bucket after the HuggingFace model identifier, and
 append the `/fp16` suffix for the half-precision version.
 
 For example, the S3 URI for the `EleutherAI/gpt-j-6B` model is:
 `s3://tensorized/EleutherAI/gpt-j-6B/fp16/model.tensors`
 
 The below table shows the available models and their S3 URIs.
 
 ### Large Language Models
 
-| Model                                                                     | Precision | S3 URI  |
-|---------------------------------------------------------------------------|-----------|---------|
-| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-125M/model.tensors` |
-| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-125M/fp16/model.tensors` |
-| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/model.tensors` |
-| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/fp16/model.tensors` |
-| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/model.tensors` |
-| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/fp16/model.tensors` |
-| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)         | `fp32`    | `s3://tensorized/EleutherAI/gpt-j-6B/model.tensors` |
-| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)         | `fp16`    | `s3://tensorized/EleutherAI/gpt-j-6B/fp16/model.tensors` |
-| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neox-20b/model.tensors` |
-| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neox-20b/fp16/model.tensors` |
-| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)     | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m/model.tensors` |
-| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)     | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m/fp16/model.tensors` |
-| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b/model.tensors` |
-| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-1.4b/fp16/model.tensors` |
-| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b/model.tensors` |
-| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-2.8b/fp16/model.tensors` |
-| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b/model.tensors` |
-| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-6.9b/fp16/model.tensors` |
-| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)     | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b/model.tensors` |
-| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)     | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b/fp16/model.tensors` |
-| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/model.tensors` |
-| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-1.4b-deduped](https://huggingface.co/EleutherAI/pythia-1.4b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b-deduped/model.tensors` |
+| Model                                                                                   | Precision | S3 URI                                                              |
+|-----------------------------------------------------------------------------------------|-----------|---------------------------------------------------------------------|
+| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-125M/model.tensors`             |
+| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-125M/fp16/model.tensors`        |
+| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/model.tensors`             |
+| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/fp16/model.tensors`        |
+| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/model.tensors`             |
+| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/fp16/model.tensors`        |
+| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)                       | `fp32`    | `s3://tensorized/EleutherAI/gpt-j-6B/model.tensors`                 |
+| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)                       | `fp16`    | `s3://tensorized/EleutherAI/gpt-j-6B/fp16/model.tensors`            |
+| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neox-20b/model.tensors`             |
+| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neox-20b/fp16/model.tensors`        |
+| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)                   | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m/model.tensors`               |
+| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)                   | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m/fp16/model.tensors`          |
+| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)                 | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b/model.tensors`              |
+| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)                 | `fp16`    | `s3://tensorized/EleutherAI/pythia-1.4b/fp16/model.tensors`         |
+| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)                 | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b/model.tensors`              |
+| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)                 | `fp16`    | `s3://tensorized/EleutherAI/pythia-2.8b/fp16/model.tensors`         |
+| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)                 | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b/model.tensors`              |
+| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)                 | `fp16`    | `s3://tensorized/EleutherAI/pythia-6.9b/fp16/model.tensors`         |
+| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)                   | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b/model.tensors`               |
+| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)                   | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b/fp16/model.tensors`          |
+| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/model.tensors`       |
+| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/fp16/model.tensors`  |
+| [EleutherAI/pythia-1.4b-deduped](https://huggingface.co/EleutherAI/pythia-1.4b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b-deduped/model.tensors`      |
 | [EleutherAI/pythia-1.4b-deduped](https://huggingface.co/EleutherAI/pythia-1.4b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-1.4b-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-2.8b-deduped](https://huggingface.co/EleutherAI/pythia-2.8b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b-deduped/model.tensors` |
+| [EleutherAI/pythia-2.8b-deduped](https://huggingface.co/EleutherAI/pythia-2.8b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b-deduped/model.tensors`      |
 | [EleutherAI/pythia-2.8b-deduped](https://huggingface.co/EleutherAI/pythia-2.8b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-2.8b-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-6.9b-deduped](https://huggingface.co/EleutherAI/pythia-6.9b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b-deduped/model.tensors` |
+| [EleutherAI/pythia-6.9b-deduped](https://huggingface.co/EleutherAI/pythia-6.9b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b-deduped/model.tensors`      |
 | [EleutherAI/pythia-6.9b-deduped](https://huggingface.co/EleutherAI/pythia-6.9b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-6.9b-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/model.tensors` |
-| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/model.tensors` |
-| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/model.tensors` |
-| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/model.tensors` |
-| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/model.tensors` |
-| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/model.tensors` |
-| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/fp16/model.tensors` |
-| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono) | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-mono/model.tensors` |
-| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono) | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-mono/fp16/model.tensors` |
-| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi) | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-multi/model.tensors` |
-| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi) | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-multi/fp16/model.tensors` |
-| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi) | `fp32`    | `s3://tensorized/Salesforce/codegen-2B-multi/model.tensors` |
-| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi) | `fp16`    | `s3://tensorized/Salesforce/codegen-2B-multi/fp16/model.tensors` |
-| [Salesforce/codgen-6B-mono](https://huggingface.co/Salesforce/codgen-6B-mono) | `fp32`    | `s3://tensorized/Salesforce/codgen-6B-mono/model.tensors` |
-| [Salesforce/codgen-6B-mono](https://huggingface.co/Salesforce/codgen-6B-mono) | `fp16`    | `s3://tensorized/Salesforce/codgen-6B-mono/fp16/model.tensors` |
-| [Salesforce/codgen-6B-multi](https://huggingface.co/Salesforce/codgen-6B-multi) | `fp32`    | `s3://tensorized/Salesforce/codgen-6B-multi/model.tensors` |
-| [Salesforce/codgen-6B-multi](https://huggingface.co/Salesforce/codgen-6B-multi) | `fp16`    | `s3://tensorized/Salesforce/codgen-6B-multi/fp16/model.tensors` |
-| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono) | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-mono/model.tensors` |
-| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono) | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-mono/fp16/model.tensors` |
-| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi) | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-multi/model.tensors` |
-| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi) | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-multi/fp16/model.tensors` |
+| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/model.tensors`       |
+| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/fp16/model.tensors`  |
+| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/model.tensors`         |
+| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/model.tensors`         |
+| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/model.tensors`         |
+| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/model.tensors`         |
+| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B)         | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/model.tensors`          |
+| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B)         | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/fp16/model.tensors`     |
+| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono)     | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-mono/model.tensors`        |
+| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono)     | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-mono/fp16/model.tensors`   |
+| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi)   | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-multi/model.tensors`       |
+| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi)   | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-multi/fp16/model.tensors`  |
+| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi)       | `fp32`    | `s3://tensorized/Salesforce/codegen-2B-multi/model.tensors`         |
+| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi)       | `fp16`    | `s3://tensorized/Salesforce/codegen-2B-multi/fp16/model.tensors`    |
+| [Salesforce/codegen-6B-mono](https://huggingface.co/Salesforce/codegen-6B-mono)         | `fp32`    | `s3://tensorized/Salesforce/codegen-6B-mono/model.tensors`          |
+| [Salesforce/codegen-6B-mono](https://huggingface.co/Salesforce/codegen-6B-mono)         | `fp16`    | `s3://tensorized/Salesforce/codegen-6B-mono/fp16/model.tensors`     |
+| [Salesforce/codegen-6B-multi](https://huggingface.co/Salesforce/codegen-6B-multi)       | `fp32`    | `s3://tensorized/Salesforce/codegen-6B-multi/model.tensors`         |
+| [Salesforce/codegen-6B-multi](https://huggingface.co/Salesforce/codegen-6B-multi)       | `fp16`    | `s3://tensorized/Salesforce/codegen-6B-multi/fp16/model.tensors`    |
+| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono)       | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-mono/model.tensors`         |
+| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono)       | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-mono/fp16/model.tensors`    |
+| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi)     | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-multi/model.tensors`        |
+| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi)     | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-multi/fp16/model.tensors`   |
 
 ## S3 Usage Notes
 `tensorizer` uses the `boto3` library to interact with S3. The easiest way
 to use `tensorizer` with S3 is to configure your S3 credentials in
 `~/.s3cfg`.
 
 If you don't want to use `~/.s3cfg`, or wish to use a `.s3cfg` config file
@@ -342,15 +337,15 @@
 endpoint once the object is cached.
 
 **NOTE2:** The cache above does not get invalidated when the object is updated
 in S3. If you update an object in S3, you will need to wait for the cache to
 expire before you can download the updated object. This takes 24 hours since
 the last download.
 
-For this reason, it is recommended to use an unique S3 key for each version
+For this reason, it is recommended to use a unique S3 key for each version
 of a model if you use the `accel-object.ord1.coreweave.com` endpoint.
 
 ## Additional Features
 `tensorizer` has a few additional features that make it more useful than
 just a serialization/deserialization tool.
 
 ### Plaid Mode
```

### Comparing `tensorizer-1.0.1/README.md` & `tensorizer-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -74,31 +74,31 @@
 The below example serializes the `EleutherAI/gpt-j-6B` model to an S3
 endpoint. It assumes that you have already configured your S3
 credentials in `~/.s3cfg`.
 
 **NOTE:** Loading and serializing `gpt-j-6B` will take a lot of CPU RAM,
 up to `~20GB`. Additionally, when loading `gpt-j-6B` into a GPU, you
 will need about `~16GB` of VRAM. If you don't have that much RAM or VRAM,
-you can use the smaller `gpt-neo-125m` model instead.
+you can use the smaller `gpt-neo-125M` model instead.
 
 **NOTE2:** The below examples require the `transformers` and `accelerate`
 libraries. You can install them with `pip`:
 ```bash
 python -m pip install transformers accelerate
 ```
 
 [serialize.py](examples/serialize.py)
 ```python
-from transformers import AutoModelForCausalLM
-from tensorizer import TensorSerializer
 import torch
+from tensorizer import TensorSerializer
+from transformers import AutoModelForCausalLM
 
 model_ref = "EleutherAI/gpt-j-6B"
 # For less intensive requirements, swap above with the line below:
-# model_ref = "EleutherAI/gpt-neo-125m"
+# model_ref = "EleutherAI/gpt-neo-125M"
 model_name = model_ref.split("/")[-1]
 # Change this to your S3 bucket.
 s3_bucket = "bucket"
 s3_uri = f"s3://{s3_bucket}/{model_name}.tensors"
 
 model = AutoModelForCausalLM.from_pretrained(
     model_ref,
@@ -121,42 +121,34 @@
 endpoint into the `torch.nn.Module`.
 
 The below example loads the `EleutherAI/gpt-j-6B` model from an S3
 endpoint.
 
 [deserialize.py](examples/deserialize.py)
 ```python
-import torch
-import os
 import time
+import torch
 from tensorizer import TensorDeserializer
 from tensorizer.utils import no_init_or_tensor, convert_bytes, get_mem_usage
-from collections import OrderedDict
-
-# disable missing keys and unexpected key warnings
-os.environ["TRANSFORMERS_VERBOSITY"] = "error"
 
 from transformers import AutoModelForCausalLM, AutoTokenizer, AutoConfig
 
 model_ref = "EleutherAI/gpt-j-6B"
 # To run this at home, swap this with the line below for a smaller example:
-# model_ref = "EleutherAI/gpt-neo-125m"
+# model_ref = "EleutherAI/gpt-neo-125M"
 model_name = model_ref.split("/")[-1]
 # Change this to your S3 bucket.
 s3_bucket = "bucket"
 s3_uri = f"s3://{s3_bucket}/{model_name}.tensors"
 
 config = AutoConfig.from_pretrained(model_ref)
 
 # This ensures that the model is not initialized.
-model = no_init_or_tensor(
-    lambda: AutoModelForCausalLM.from_pretrained(
-        None, config=config, state_dict=OrderedDict()
-    )
-)
+with no_init_or_tensor():
+    model = AutoModelForCausalLM.from_config(config)
 
 before_mem = get_mem_usage()
 
 # Lazy load the tensors from S3 into the model.
 start = time.time()
 deserializer = TensorDeserializer(s3_uri, plaid_mode=True)
 deserializer.load_into_module(model)
@@ -164,27 +156,30 @@
 
 # Brag about how fast we are.
 total_bytes_str = convert_bytes(deserializer.total_tensor_bytes)
 duration = end - start
 per_second = convert_bytes(deserializer.total_tensor_bytes / duration)
 after_mem = get_mem_usage()
 deserializer.close()
-print(f"Deserialized {total_bytes_str} in {end - start:0.2f}s, {per_second}")
+print(f"Deserialized {total_bytes_str} in {end - start:0.2f}s, {per_second}/s")
 print(f"Memory usage before: {before_mem}")
 print(f"Memory usage after: {after_mem}")
 
 # Tokenize and generate
 model.eval()
 tokenizer = AutoTokenizer.from_pretrained(model_ref)
+eos = tokenizer.eos_token_id
 input_ids = tokenizer.encode(
     "¡Hola! Encantado de conocerte. hoy voy a", return_tensors="pt"
 ).to("cuda")
 
 with torch.no_grad():
-    output = model.generate(input_ids, max_new_tokens=50, do_sample=True)
+    output = model.generate(
+        input_ids, max_new_tokens=50, do_sample=True, pad_token_id=eos
+    )
 
 print(f"Output: {tokenizer.decode(output[0], skip_special_tokens=True)}")
 ```
 
 It should produce output similar to the following, with GPT-J-6B:
 ```
 Deserialized model in 6.25 seconds
@@ -201,82 +196,82 @@
 and `hf_main()` serializes
 [HuggingFace Transformers](https://github.com/huggingface/transformers) models.
 
 ## Available Pre-Tensorized Models on the CoreWeave Cloud
 
 The following models are available on the CoreWeave Cloud for free, and can be
 used with the `TensorDeserializer` class. The S3 support defaults to the
-`accel-object.ord1.coreweave.com` endpoint, and the bucket to use `tensorized`.
+`accel-object.ord1.coreweave.com` endpoint, and the bucket to use as `tensorized`.
 
 We name the keys in the S3 bucket after the HuggingFace model identifier, and
 append the `/fp16` suffix for the half-precision version.
 
 For example, the S3 URI for the `EleutherAI/gpt-j-6B` model is:
 `s3://tensorized/EleutherAI/gpt-j-6B/fp16/model.tensors`
 
 The below table shows the available models and their S3 URIs.
 
 ### Large Language Models
 
-| Model                                                                     | Precision | S3 URI  |
-|---------------------------------------------------------------------------|-----------|---------|
-| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-125M/model.tensors` |
-| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-125M/fp16/model.tensors` |
-| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/model.tensors` |
-| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/fp16/model.tensors` |
-| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/model.tensors` |
-| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/fp16/model.tensors` |
-| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)         | `fp32`    | `s3://tensorized/EleutherAI/gpt-j-6B/model.tensors` |
-| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)         | `fp16`    | `s3://tensorized/EleutherAI/gpt-j-6B/fp16/model.tensors` |
-| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neox-20b/model.tensors` |
-| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neox-20b/fp16/model.tensors` |
-| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)     | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m/model.tensors` |
-| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)     | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m/fp16/model.tensors` |
-| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b/model.tensors` |
-| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-1.4b/fp16/model.tensors` |
-| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b/model.tensors` |
-| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-2.8b/fp16/model.tensors` |
-| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b/model.tensors` |
-| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-6.9b/fp16/model.tensors` |
-| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)     | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b/model.tensors` |
-| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)     | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b/fp16/model.tensors` |
-| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/model.tensors` |
-| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-1.4b-deduped](https://huggingface.co/EleutherAI/pythia-1.4b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b-deduped/model.tensors` |
+| Model                                                                                   | Precision | S3 URI                                                              |
+|-----------------------------------------------------------------------------------------|-----------|---------------------------------------------------------------------|
+| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-125M/model.tensors`             |
+| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-125M/fp16/model.tensors`        |
+| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/model.tensors`             |
+| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/fp16/model.tensors`        |
+| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/model.tensors`             |
+| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/fp16/model.tensors`        |
+| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)                       | `fp32`    | `s3://tensorized/EleutherAI/gpt-j-6B/model.tensors`                 |
+| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)                       | `fp16`    | `s3://tensorized/EleutherAI/gpt-j-6B/fp16/model.tensors`            |
+| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neox-20b/model.tensors`             |
+| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neox-20b/fp16/model.tensors`        |
+| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)                   | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m/model.tensors`               |
+| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)                   | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m/fp16/model.tensors`          |
+| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)                 | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b/model.tensors`              |
+| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)                 | `fp16`    | `s3://tensorized/EleutherAI/pythia-1.4b/fp16/model.tensors`         |
+| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)                 | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b/model.tensors`              |
+| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)                 | `fp16`    | `s3://tensorized/EleutherAI/pythia-2.8b/fp16/model.tensors`         |
+| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)                 | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b/model.tensors`              |
+| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)                 | `fp16`    | `s3://tensorized/EleutherAI/pythia-6.9b/fp16/model.tensors`         |
+| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)                   | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b/model.tensors`               |
+| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)                   | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b/fp16/model.tensors`          |
+| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/model.tensors`       |
+| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/fp16/model.tensors`  |
+| [EleutherAI/pythia-1.4b-deduped](https://huggingface.co/EleutherAI/pythia-1.4b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b-deduped/model.tensors`      |
 | [EleutherAI/pythia-1.4b-deduped](https://huggingface.co/EleutherAI/pythia-1.4b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-1.4b-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-2.8b-deduped](https://huggingface.co/EleutherAI/pythia-2.8b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b-deduped/model.tensors` |
+| [EleutherAI/pythia-2.8b-deduped](https://huggingface.co/EleutherAI/pythia-2.8b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b-deduped/model.tensors`      |
 | [EleutherAI/pythia-2.8b-deduped](https://huggingface.co/EleutherAI/pythia-2.8b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-2.8b-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-6.9b-deduped](https://huggingface.co/EleutherAI/pythia-6.9b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b-deduped/model.tensors` |
+| [EleutherAI/pythia-6.9b-deduped](https://huggingface.co/EleutherAI/pythia-6.9b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b-deduped/model.tensors`      |
 | [EleutherAI/pythia-6.9b-deduped](https://huggingface.co/EleutherAI/pythia-6.9b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-6.9b-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/model.tensors` |
-| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/model.tensors` |
-| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/model.tensors` |
-| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/model.tensors` |
-| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/model.tensors` |
-| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/model.tensors` |
-| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/fp16/model.tensors` |
-| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono) | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-mono/model.tensors` |
-| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono) | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-mono/fp16/model.tensors` |
-| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi) | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-multi/model.tensors` |
-| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi) | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-multi/fp16/model.tensors` |
-| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi) | `fp32`    | `s3://tensorized/Salesforce/codegen-2B-multi/model.tensors` |
-| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi) | `fp16`    | `s3://tensorized/Salesforce/codegen-2B-multi/fp16/model.tensors` |
-| [Salesforce/codgen-6B-mono](https://huggingface.co/Salesforce/codgen-6B-mono) | `fp32`    | `s3://tensorized/Salesforce/codgen-6B-mono/model.tensors` |
-| [Salesforce/codgen-6B-mono](https://huggingface.co/Salesforce/codgen-6B-mono) | `fp16`    | `s3://tensorized/Salesforce/codgen-6B-mono/fp16/model.tensors` |
-| [Salesforce/codgen-6B-multi](https://huggingface.co/Salesforce/codgen-6B-multi) | `fp32`    | `s3://tensorized/Salesforce/codgen-6B-multi/model.tensors` |
-| [Salesforce/codgen-6B-multi](https://huggingface.co/Salesforce/codgen-6B-multi) | `fp16`    | `s3://tensorized/Salesforce/codgen-6B-multi/fp16/model.tensors` |
-| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono) | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-mono/model.tensors` |
-| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono) | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-mono/fp16/model.tensors` |
-| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi) | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-multi/model.tensors` |
-| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi) | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-multi/fp16/model.tensors` |
+| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/model.tensors`       |
+| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/fp16/model.tensors`  |
+| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/model.tensors`         |
+| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/model.tensors`         |
+| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/model.tensors`         |
+| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/model.tensors`         |
+| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B)         | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/model.tensors`          |
+| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B)         | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/fp16/model.tensors`     |
+| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono)     | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-mono/model.tensors`        |
+| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono)     | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-mono/fp16/model.tensors`   |
+| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi)   | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-multi/model.tensors`       |
+| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi)   | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-multi/fp16/model.tensors`  |
+| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi)       | `fp32`    | `s3://tensorized/Salesforce/codegen-2B-multi/model.tensors`         |
+| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi)       | `fp16`    | `s3://tensorized/Salesforce/codegen-2B-multi/fp16/model.tensors`    |
+| [Salesforce/codegen-6B-mono](https://huggingface.co/Salesforce/codegen-6B-mono)         | `fp32`    | `s3://tensorized/Salesforce/codegen-6B-mono/model.tensors`          |
+| [Salesforce/codegen-6B-mono](https://huggingface.co/Salesforce/codegen-6B-mono)         | `fp16`    | `s3://tensorized/Salesforce/codegen-6B-mono/fp16/model.tensors`     |
+| [Salesforce/codegen-6B-multi](https://huggingface.co/Salesforce/codegen-6B-multi)       | `fp32`    | `s3://tensorized/Salesforce/codegen-6B-multi/model.tensors`         |
+| [Salesforce/codegen-6B-multi](https://huggingface.co/Salesforce/codegen-6B-multi)       | `fp16`    | `s3://tensorized/Salesforce/codegen-6B-multi/fp16/model.tensors`    |
+| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono)       | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-mono/model.tensors`         |
+| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono)       | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-mono/fp16/model.tensors`    |
+| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi)     | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-multi/model.tensors`        |
+| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi)     | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-multi/fp16/model.tensors`   |
 
 ## S3 Usage Notes
 `tensorizer` uses the `boto3` library to interact with S3. The easiest way
 to use `tensorizer` with S3 is to configure your S3 credentials in
 `~/.s3cfg`.
 
 If you don't want to use `~/.s3cfg`, or wish to use a `.s3cfg` config file
@@ -322,15 +317,15 @@
 endpoint once the object is cached.
 
 **NOTE2:** The cache above does not get invalidated when the object is updated
 in S3. If you update an object in S3, you will need to wait for the cache to
 expire before you can download the updated object. This takes 24 hours since
 the last download.
 
-For this reason, it is recommended to use an unique S3 key for each version
+For this reason, it is recommended to use a unique S3 key for each version
 of a model if you use the `accel-object.ord1.coreweave.com` endpoint.
 
 ## Additional Features
 `tensorizer` has a few additional features that make it more useful than
 just a serialization/deserialization tool.
 
 ### Plaid Mode
```

### Comparing `tensorizer-1.0.1/proto/tensors.proto` & `tensorizer-1.1.0/proto/tensors.proto`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/pyproject.toml` & `tensorizer-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tensorizer"
-version = "1.0.1"
+version = "1.1.0"
 license = { text = "MIT License" }
 keywords = ["tensorizer", "machine learning", "serialization", "tensor", "pytorch"]
 authors = [
   { name="CoreWeave" }
 ]
 description = "A tool for fast PyTorch module, model, and tensor serialization + deserialization."
 readme = "README.md"
@@ -34,8 +34,33 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["tensorizer"]
 
 [tool.setuptools.package-data]
-tensorizer = ["tensors.proto"]
+tensorizer = ["tensors.proto"]
+
+[tool.black]
+line-length = 80
+target-version = ["py38", "py39", "py310", "py311"]
+preview = true
+force-exclude = '''
+(
+  ^/ATTIC
+  | ^/tensors
+  | .*_pb2.py
+)
+'''
+
+[tool.isort]
+profile = "black"
+line_length = 80
+src_paths = ["tensorizer/", "tests/", "examples/"]
+extend_skip_glob = [
+    "ATTIC/*",
+    "*_pb2.py",
+    "tensors/*",
+    "examples/serialize.py",
+    "examples/deserialize.py"
+]
+use_parentheses = true
```

### Comparing `tensorizer-1.0.1/tensorizer/_wide_pipes.py` & `tensorizer-1.1.0/tensorizer/_wide_pipes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import contextlib
 import functools
 import logging
-import threading
 import subprocess
 import sys
+import threading
 
 # =============================================================================
 # From `pipe(7)` manpage:
 #
 # Pipe capacity
 # A pipe has a limited capacity. If the pipe is full, then a write(2) will
 # block or fail, depending on whether the O_NONBLOCK flag is set (see below).
```

### Comparing `tensorizer-1.0.1/tensorizer/protobuf.py` & `tensorizer-1.1.0/tensorizer/protobuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from collections import OrderedDict
+from typing import BinaryIO
+from typing import OrderedDict as OrderedDictType
+from typing import Tuple, Union
+
+import numpy as np
 import torch
 from torch import Tensor
-import numpy as np
-import tensors.tensors_pb2 as tensors_pb
-from tensors.tensors_pb2 import Tensor as TensorPb
-from typing import OrderedDict as OrderedDictType, Tuple, Union, BinaryIO
-from collections import OrderedDict
+
+import tensorizer.tensors_pb2 as tensors_pb
+from tensorizer.tensors_pb2 import Tensor as TensorPb
 
 DtypePbs = {
     torch.float32: tensors_pb.DT_FLOAT32,
     torch.float64: tensors_pb.DT_FLOAT64,
     torch.float16: tensors_pb.DT_FLOAT16,
     torch.bfloat16: tensors_pb.DT_BFLOAT16,
     torch.complex32: tensors_pb.DT_COMPLEX32,
@@ -80,15 +84,15 @@
     if attribute is not None:
         extra_opts = {"attr_type": attribute}
 
     return tensors_pb.Tensor(
         dtype=DtypePbs[t.dtype],
         shape=t.shape,
         data=t.cpu().detach().numpy().tobytes(),
-        **extra_opts
+        **extra_opts,
     )
 
 
 def deserialize_tensor(
     t: tensors_pb.Tensor,
 ) -> Union[Tensor, Tuple[Tensor, "tensors_pb.AttributeType"]]:
     mv = bytearray(t.data)
```

### Comparing `tensorizer-1.0.1/tensorizer/serialization.py` & `tensorizer-1.1.0/tensorizer/serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,39 +7,41 @@
 try:
     import fcntl
     import resource
 except ImportError:
     fcntl = None
     resource = None
 
-from enum import Enum
 import collections.abc
+import ctypes
+import hashlib
 import io
-import os
-import tensorizer.stream_io as stream_io
-import tensorizer.utils as utils
+import logging
 import mmap
-import numpy
+import os
 import struct
+import tempfile
 import time
-import torch
 import typing
-import logging
-import tempfile
-import hashlib
 import zlib
-import ctypes
+from enum import Enum
+
+import numpy
+import torch
+
+import tensorizer.stream_io as stream_io
+import tensorizer.utils as utils
 
 if torch.cuda.is_available():
     cudart = torch.cuda.cudart()
 else:
     cudart = None
 
 from collections import OrderedDict
-from typing import Optional, Tuple, Union, List, Iterator, Dict, Callable, Any
+from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
 lz4 = None
 
 __all__ = ["TensorSerializer", "TensorDeserializer", "TensorType"]
 
 # Setup logger
 logger = logging.getLogger(__name__)
@@ -96,29 +98,33 @@
             torch.float64: numpy.float64,
             torch.complex64: numpy.complex64,
             torch.complex128: numpy.complex128,
         }.get(dtype)
 
         if numpy_dtype is None:
             raise TypeError(
-                "The provided torch.dtype class could not"
-                " be converted to a numpy.dtype"
+                "The provided torch.dtype class could not be converted to a"
+                " numpy.dtype"
             )
         else:
             # Convert it from a dtype class to a dtype object instance
             return numpy.dtype(numpy_dtype)
     else:
         raise TypeError("Could not interpret provided dtype as a numpy.dtype")
 
 
 class TensorDeserializer(collections.abc.Mapping):
     """
     Given a file-like object for read, deserialize tensors to a state_dict or
     a torch.nn.Module.
 
+    See the docs_ for a usage walkthrough.
+
+    .. _docs: https://github.com/coreweave/tensorizer/tree/main#basic-usage
+
     Args:
         file_obj: A file-like object to read from. It can also be a string
             representing a path to a file or an HTTP/HTTPS/S3 URI.
         device: The device to load the tensors to.
         filter_func: A function (tensor_name: str) -> bool that returns True
             if a tensor should be loaded, or False if it should be skipped.
             If None, all tensors are loaded.
@@ -128,26 +134,63 @@
             accessed. If False, all tensors will be loaded into memory up
             front.
         plaid_mode: If True, tensors will be loaded extremely fast into the
             target device. This is only supported on CUDA devices, and the
             buffers are going to be inconsistent due to the extreme
             naughtiness of reusing a backing buffer. This is only recommended
             for use with inference, and not training.
+
+    Examples:
+        Deserializing a pre-serialized_ 16-bit ``transformers`` model from S3::
+
+            from tensorizer import TensorDeserializer, utils
+            from transformers import AutoConfig, AutoModelForCausalLM
+            import torch
+
+            model_ref = "EleutherAI/gpt-neo-125M"
+
+            # Create an empty torch.nn.Module with the right shape
+            config = AutoConfig.from_pretrained(model_ref, dtype=torch.float16)
+            with utils.no_init_or_tensor():
+                model = AutoModelForCausalLM.from_config(config)
+
+            # Public `tensorized` bucket hosted by CoreWeave; see the docs
+            s3_uri = f"s3://tensorized/{model_ref}/fp16/model.tensors"
+
+            deserializer = TensorDeserializer(s3_uri, plaid_mode=True)
+            deserializer.load_into_module(model)
+
+        ## From a private S3 bucket::
+
+            from tensorizer import stream_io
+            s3 = stream_io.open_stream(
+                "s3://some-private-bucket/my-model.tensors",
+                mode="rb",
+                s3_access_key_id=...,
+                s3_secret_access_key=...,
+                s3_endpoint=...,
+            )
+            # Set up `model` as an empty torch.nn.Module in the shape of
+            # my-model.tensors, then:
+            deserializer = TensorDeserializer(s3, plaid_mode=True)
+            deserializer.load_into_module(model)
+
+        .. _pre-serialized: https://github.com/coreweave/tensorizer/tree/main#available-pre-tensorized-models-on-the-coreweave-cloud
     """
 
     def __init__(
         self,
         file_obj: Union[
             io.BufferedIOBase,
             io.RawIOBase,
             typing.BinaryIO,
             str,
             bytes,
             os.PathLike,
-            int
+            int,
         ],
         device: Union[torch.device, str, None] = None,
         filter_func: Optional[Callable[[str], Union[bool, Any]]] = None,
         dtype: Union[numpy.dtype, str, None] = None,
         *,
         lazy_load: bool = False,
         plaid_mode: bool = False,
@@ -407,15 +450,15 @@
         if self._plaid_mode:
             # In plaid_mode, we only have one valid tensor at a time, so
             # we need to make sure that prior tensors are not accessed.
             if self._prior_key is not None and self._prior_key != name:
                 self._cache[self._prior_key] = False
             if self._cache[name] is False:
                 raise RuntimeError(
-                    f"Tensor {name} already overwritten in " "plaid_mode"
+                    f"Tensor {name} already overwritten in plaid_mode"
                 )
             self._prior_key = name
 
         if name in self._cache and self._cache[name] is not None:
             return self._cache[name]
 
         # If we're in lazy_load mode, we populate the cache with the
@@ -748,20 +791,51 @@
 
 
 class TensorSerializer:
     """
     Given a file-like object or path, serialize tensors from a torch.nn.Module
     to it.
 
+    See the docs_ for a usage walkthrough.
+
+    .. _docs: https://github.com/coreweave/tensorizer/tree/main#basic-usage
+
     Args:
         file_obj: A file-like object or path to a file to write to. The path
             can be a S3 URI.
         compress_tensors: If True, compress the tensors using lz4. This
             exists as an internal curiosity as it doesn't seem to make
             much of a difference in practice.
+
+    Example:
+        Serializing a 16-bit HuggingFace model to a private S3 bucket::
+
+            from transformers import AutoModelForCausalLM
+            from tensorizer import TensorSerializer
+            import torch
+
+            model_ref = "EleutherAI/gpt-neo-125M"
+            s3_uri = f"s3://some-private-bucket/{model_ref}.tensors"
+
+            model = AutoModelForCausalLM.from_pretrained(
+                model_ref,
+                revision="float16",
+                torch_dtype=torch.float16,
+                low_cpu_mem_usage=True,
+            )
+
+            serializer = TensorSerializer(s3_uri)
+            serializer.write_module(model)
+            serializer.close()
+
+        This example assumes the credentials for ``some-private-bucket``
+        are configured in `~/.s3cfg`, where they will be auto-detected.
+        To specify credentials manually, use a file-like object from
+        `tensorizer.stream_io.open_stream()` in place of `s3_uri`.
+    ..
     """
 
     def __init__(
         self,
         file_obj: Union[
             io.BufferedIOBase,
             io.RawIOBase,
@@ -870,15 +944,14 @@
             logger.info(f"Comp'd bytes: {self.total_compressed_tensor_bytes}")
             logger.info(f"Ratio: {compression_ratio:.2f}")
 
     def _sync_prologue_state(self):
         """
         This is called after the tensor has been written to the file, and
         ensures that the file is in a consistent state.
-        :return:
         """
         curr = self._file.tell()
 
         # Write our zero-length field, that indicates that this is the last
         # tensor. This will be overwritten if another tensor is written.
         self._file.write(struct.pack("<Q", 0))
         # Write the total number of tensors.
```

### Comparing `tensorizer-1.0.1/tensorizer/stream_io.py` & `tensorizer-1.1.0/tensorizer/stream_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import functools
 import io
 import logging
 import os
+import shutil
 import subprocess
 import sys
 import tempfile
 import typing
 import weakref
+from io import SEEK_CUR, SEEK_END, SEEK_SET
+from typing import Any, Dict, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import boto3
-from io import SEEK_SET, SEEK_CUR, SEEK_END
-from typing import Union, Optional, Dict, Any, Tuple
-import shutil
 
 import tensorizer._wide_pipes as _wide_pipes
 
 __all__ = ["open_stream", "CURLStreamFile"]
 
 logger = logging.getLogger(__name__)
 
@@ -49,30 +49,34 @@
             Tuple[Union[str, bytes, os.PathLike], ...], str, bytes, os.PathLike
         ]
     ] = None
 ) -> _ParsedCredentials:
     """
     Gets S3 credentials from the .s3cfg file.
 
-    :param config_paths: The sequence of potential file paths to check
-        for s3cmd config settings. If not provided or an empty tuple,
-        platform-specific default search locations are used.
-        When specifying a sequence, this argument must be a tuple,
-        because this function is cached, and that requires
-        all arguments to be hashable.
-    :return: A 4-tuple, config_file, s3_endpoint, s3_access_key, s3_secret_key,
+    Args:
+        config_paths: The sequence of potential file paths to check
+            for s3cmd config settings. If not provided or an empty tuple,
+            platform-specific default search locations are used.
+            When specifying a sequence, this argument must be a tuple,
+            because this function is cached, and that requires
+            all arguments to be hashable.
+
+    Returns:
+        A 4-tuple, config_file, s3_endpoint, s3_access_key, s3_secret_key,
         where each element may be None if not found,
         and config_file is the config file path used.
         If config_file is None, no valid config file
         was found, and nothing was parsed.
 
-    If the config_paths argument is not provided or is an empty tuple,
-    platform-specific default search locations are used.
-    This function is cached, and hence config_paths must be a (hashable) tuple
-    when specifying a sequence
+    Note:
+        If the config_paths argument is not provided or is an empty tuple,
+        platform-specific default search locations are used.
+        This function is cached, and hence config_paths must be a
+        (hashable) tuple when specifying a sequence.
     """
     if not config_paths:
         config_paths = _s3_default_config_paths
     elif isinstance(config_paths, (str, bytes, os.PathLike)):
         config_paths = (config_paths,)
 
     import configparser
@@ -170,52 +174,57 @@
         Registers a message to serve as context for possible errors
         encountered later.
         This method serves to keep track of any dubious conditions
         under which the CURLStreamFile was opened for more descriptive
         error messages if those conditions eventually lead to an error,
         while still attempting to connect regardless, in accordance with
         the "easier to ask for forgiveness than permission" principle.
-        :param msg: The message to be registered.
+
+        Args:
+            msg: The message to be registered.
         """
         self._error_context.append(msg)
 
     def _reproduce_and_capture_error(
-            self, expect_code: Optional[int]
+        self, expect_code: Optional[int]
     ) -> Optional[str]:
         """
         Re-attempts the connection with stderr attached to a pipe
         to capture an HTTP error code.
         stderr is not a pipe on the original self._curl Popen object
         because it would get the same `bufsize` as stdout, and waste RAM,
         so this optimizes for the non-error path
         at the slight expense of the error path
 
-        :param expect_code: The error code to expect.
-            If this doesn't match the new error, the original error
-            is considered not to have been reproduced.
-        :return: The cURL error message if the error could be reproduced,
+        Args:
+            expect_code: The error code to expect.
+                If this doesn't match the new error, the original error
+                is considered not to have been reproduced.
+
+        Returns:
+            The cURL error message if the error could be reproduced,
             otherwise None.
         """
         args = [
             curl_path,
             "-I",  # Only read headers
             "-XGET",  # Use a GET request (in case HEAD is not supported)
             "-f",  # Don't return HTML/XML error webpages
             "-s",  # Silence most output
             "-S",  # Keep error messages
-            self._uri
+            self._uri,
         ]
         try:
             result = subprocess.run(
                 args,
                 stdin=subprocess.DEVNULL,
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.PIPE,
                 text=True,
-                timeout=3
+                timeout=3,
             )
 
         except subprocess.TimeoutExpired:
             return None
         if result.returncode == 0 or (
             expect_code and result.returncode != expect_code
         ):
@@ -225,16 +234,18 @@
 
     def _create_read_error_from_context(self) -> IOError:
         return_code = self._curl.poll()
         self._curl.terminate()
         if return_code:
             error = self._reproduce_and_capture_error(expect_code=return_code)
             if error is None:
-                error = f"curl error: ({return_code}), see" \
-                        f" https://curl.se/docs/manpage.html#{return_code}"
+                error = (
+                    f"curl error: ({return_code}), see"
+                    f" https://curl.se/docs/manpage.html#{return_code}"
+                )
         else:
             error = ""
 
         if self._error_context:
             error += "\n" + "\n".join(self._error_context)
 
         error = error.strip()
@@ -424,40 +435,49 @@
     """
     Fill in a potentially incomplete S3 credential pair
     by parsing the s3cmd config file if necessary.
     An empty string ("") is considered a specified credential,
     while None is an unspecified credential.
     Use "" for public buckets.
 
-    :param s3_access_key_id: `s3_access_key_id` if explicitly specified,
-        otherwise None. If None, the s3cmd config file is parsed for the key.
-    :param s3_secret_access_key: `s3_secret_access_key` if explicitly specified,
-        otherwise None. If None, the s3cmd config file is parsed for the key.
-    :param s3_config_path: An explicit path to the s3cmd config file to search,
-        if necessary. If None, platform-specific default paths are used.
-    :return: A `_ParsedCredentials` object with both the
+    Args:
+        s3_access_key_id: `s3_access_key_id` if explicitly specified,
+            otherwise None.
+            If None, the s3cmd config file is parsed for the key.
+        s3_secret_access_key: `s3_secret_access_key` if explicitly specified,
+            otherwise None.
+            If None, the s3cmd config file is parsed for the key.
+        s3_config_path: An explicit path to the s3cmd config file to search,
+            if necessary.
+            If None, platform-specific default paths are used.
+
+    Returns:
+        A `_ParsedCredentials` object with both the
         `s3_access_key` and `s3_secret_key` fields guaranteed to not be None.
-    :raises ValueError: If the credential pair is incomplete and the
-        missing parts could not be found in any s3cmd config file.
-    :raises FileNotFoundError: If `s3_config_path` was explicitly provided,
-        but the file specified does not exist.
+
+    Raises:
+        ValueError: If the credential pair is incomplete and the
+            missing parts could not be found in any s3cmd config file.
+        FileNotFoundError: If `s3_config_path` was explicitly provided,
+            but the file specified does not exist.
     """
     if None not in (s3_access_key_id, s3_secret_access_key):
         # All required credentials were specified; don't parse anything
         return _ParsedCredentials(
             config_file=None,
             s3_endpoint=None,
             s3_access_key=s3_access_key_id,
             s3_secret_key=s3_secret_access_key,
         )
 
     # Try to find default credentials if at least one is not specified
     if s3_config_path is not None and not os.path.exists(s3_config_path):
         raise FileNotFoundError(
-            f"Explicitly specified s3_config_path does not exist: {s3_config_path}"
+            "Explicitly specified s3_config_path does not exist:"
+            f" {s3_config_path}"
         )
     try:
         parsed: _ParsedCredentials = _get_s3cfg_values(s3_config_path)
     except ValueError as parse_error:
         raise ValueError(
             "Attempted to access an S3 bucket,"
             " but credentials were not provided,"
@@ -550,41 +570,89 @@
     path_uri: Union[str, os.PathLike],
     mode: str = "rb",
     s3_access_key_id: Optional[str] = None,
     s3_secret_access_key: Optional[str] = None,
     s3_endpoint: Optional[str] = None,
     s3_config_path: Optional[Union[str, bytes, os.PathLike]] = None,
 ) -> Union[CURLStreamFile, typing.BinaryIO]:
-    """Open a file path, http(s):// URL, or s3:// URI.
-    :param path_uri: File path, http(s):// URL, or s3:// URI to open.
-    :param mode: Mode with which to open the stream.
-        Supported values are:
-        * "rb" for http(s)://,
-        * "rb", "wb[+]", and "ab[+]" for s3://,
-        * All standard binary modes for file paths.
-    :param s3_access_key_id: S3 access key, corresponding to
-        "aws_access_key_id" in boto3.
-        If not specified, an s3:// URI is being opened, and ~/.s3cfg exists,
-        ~/.s3cfg's "access_key" will be parsed as this credential.
-        To specify blank credentials, for a public bucket,
-        pass the empty string ("") rather than None.
-    :param s3_secret_access_key: S3 secret key, corresponding to
-        "aws_secret_access_key" in boto3.
-        If not specified, an s3:// URI is being opened, and ~/.s3cfg exists,
-        ~/.s3cfg's "secret_key" will be parsed as this credential.
-        To specify blank credentials, for a public bucket,
-        pass the empty string ("") rather than None.
-    :param s3_endpoint: S3 endpoint.
-        If not specified and a host_base was found
-        alongside previously parsed credentials, that will be used.
-        Otherwise, object.ord1.coreweave.com is the default.
-    :param s3_config_path: An explicit path to the ~/.s3cfg config file
-        to be parsed if full credentials are not provided.
-        If None, platform-specific default paths are used.
-    :return: An opened file-like object representing the target resource.
+    """
+    Open a file path, http(s):// URL, or s3:// URI.
+
+    Note:
+        The file-like streams returned by this function can be passed directly
+        to `tensorizer.TensorDeserializer` when ``mode="rb"``,
+        and `tensorizer.TensorSerializer` when ``mode="wb"``.
+
+    Args:
+        path_uri: File path, http(s):// URL, or s3:// URI to open.
+        mode: Mode with which to open the stream.
+            Supported values are:
+
+            * "rb" for http(s)://,
+            * "rb", "wb[+]", and "ab[+]" for s3://,
+            * All standard binary modes for file paths.
+
+        s3_access_key_id: S3 access key, corresponding to
+            "aws_access_key_id" in boto3. If not specified and
+            an s3:// URI is being opened, and `~/.s3cfg` exists,
+            `~/.s3cfg`'s "access_key" will be parsed as this credential.
+            To specify blank credentials, for a public bucket,
+            pass the empty string ("") rather than None.
+        s3_secret_access_key: S3 secret key, corresponding to
+            "aws_secret_access_key" in boto3. If not specified and
+            an s3:// URI is being opened, and `~/.s3cfg` exists,
+            `~/.s3cfg`'s "secret_key" will be parsed as this credential.
+            To specify blank credentials, for a public bucket,
+            pass the empty string ("") rather than None.
+        s3_endpoint: S3 endpoint.
+            If not specified and a host_base was found
+            alongside previously parsed credentials, that will be used.
+            Otherwise, ``object.ord1.coreweave.com`` is the default.
+        s3_config_path: An explicit path to the `~/.s3cfg` config file
+            to be parsed if full credentials are not provided.
+            If None, platform-specific default paths are used.
+
+    Returns:
+        An opened file-like object representing the target resource.
+
+    Examples:
+        Opening an S3 stream for writing with manually specified credentials::
+
+            with open_stream(
+                "s3://some-private-bucket/my-model.tensors",
+                mode="wb",
+                s3_access_key_id=...,
+                s3_secret_access_key=...,
+                s3_endpoint=...,
+            ) as stream:
+                ...
+
+        Opening an S3 stream for reading with credentials
+        specified in `~/.s3cfg`::
+
+            # Credentials in ~/.s3cfg are parsed automatically.
+            stream = open_stream(
+                "s3://some-private-bucket/my-model.tensors",
+            )
+
+        Opening an S3 stream for reading with credentials
+        specified in `/etc/secrets/.s3cfg`
+        (e.g., as may be mounted in a Kubernetes pod)::
+
+            stream = open_stream(
+                "s3://some-private-bucket/my-model.tensors",
+                s3_config_path="/etc/secrets/.s3cfg",
+            )
+
+        Opening an http(s):// URI for reading::
+
+            with open_stream(
+                "https://raw.githubusercontent.com/EleutherAI/gpt-neo/master/README.md"
+            ) as stream:
+                print(stream.read(128))
     """
     if isinstance(path_uri, os.PathLike):
         path_uri = os.fspath(path_uri)
 
     scheme, *location = path_uri.split("://", maxsplit=1)
     scheme = scheme.lower() if location else None
```

### Comparing `tensorizer-1.0.1/tensorizer/tensors.proto` & `tensorizer-1.1.0/tensorizer/tensors.proto`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/tensorizer/tensors_pb2.py` & `tensorizer-1.1.0/tensorizer/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/tensorizer.egg-info/PKG-INFO` & `tensorizer-1.1.0/tensorizer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorizer
-Version: 1.0.1
+Version: 1.1.0
 Summary: A tool for fast PyTorch module, model, and tensor serialization + deserialization.
 Author: CoreWeave
 License: MIT License
 Project-URL: Homepage, https://github.com/coreweave/tensorizer
 Keywords: tensorizer,machine learning,serialization,tensor,pytorch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -94,31 +94,31 @@
 The below example serializes the `EleutherAI/gpt-j-6B` model to an S3
 endpoint. It assumes that you have already configured your S3
 credentials in `~/.s3cfg`.
 
 **NOTE:** Loading and serializing `gpt-j-6B` will take a lot of CPU RAM,
 up to `~20GB`. Additionally, when loading `gpt-j-6B` into a GPU, you
 will need about `~16GB` of VRAM. If you don't have that much RAM or VRAM,
-you can use the smaller `gpt-neo-125m` model instead.
+you can use the smaller `gpt-neo-125M` model instead.
 
 **NOTE2:** The below examples require the `transformers` and `accelerate`
 libraries. You can install them with `pip`:
 ```bash
 python -m pip install transformers accelerate
 ```
 
 [serialize.py](examples/serialize.py)
 ```python
-from transformers import AutoModelForCausalLM
-from tensorizer import TensorSerializer
 import torch
+from tensorizer import TensorSerializer
+from transformers import AutoModelForCausalLM
 
 model_ref = "EleutherAI/gpt-j-6B"
 # For less intensive requirements, swap above with the line below:
-# model_ref = "EleutherAI/gpt-neo-125m"
+# model_ref = "EleutherAI/gpt-neo-125M"
 model_name = model_ref.split("/")[-1]
 # Change this to your S3 bucket.
 s3_bucket = "bucket"
 s3_uri = f"s3://{s3_bucket}/{model_name}.tensors"
 
 model = AutoModelForCausalLM.from_pretrained(
     model_ref,
@@ -141,42 +141,34 @@
 endpoint into the `torch.nn.Module`.
 
 The below example loads the `EleutherAI/gpt-j-6B` model from an S3
 endpoint.
 
 [deserialize.py](examples/deserialize.py)
 ```python
-import torch
-import os
 import time
+import torch
 from tensorizer import TensorDeserializer
 from tensorizer.utils import no_init_or_tensor, convert_bytes, get_mem_usage
-from collections import OrderedDict
-
-# disable missing keys and unexpected key warnings
-os.environ["TRANSFORMERS_VERBOSITY"] = "error"
 
 from transformers import AutoModelForCausalLM, AutoTokenizer, AutoConfig
 
 model_ref = "EleutherAI/gpt-j-6B"
 # To run this at home, swap this with the line below for a smaller example:
-# model_ref = "EleutherAI/gpt-neo-125m"
+# model_ref = "EleutherAI/gpt-neo-125M"
 model_name = model_ref.split("/")[-1]
 # Change this to your S3 bucket.
 s3_bucket = "bucket"
 s3_uri = f"s3://{s3_bucket}/{model_name}.tensors"
 
 config = AutoConfig.from_pretrained(model_ref)
 
 # This ensures that the model is not initialized.
-model = no_init_or_tensor(
-    lambda: AutoModelForCausalLM.from_pretrained(
-        None, config=config, state_dict=OrderedDict()
-    )
-)
+with no_init_or_tensor():
+    model = AutoModelForCausalLM.from_config(config)
 
 before_mem = get_mem_usage()
 
 # Lazy load the tensors from S3 into the model.
 start = time.time()
 deserializer = TensorDeserializer(s3_uri, plaid_mode=True)
 deserializer.load_into_module(model)
@@ -184,27 +176,30 @@
 
 # Brag about how fast we are.
 total_bytes_str = convert_bytes(deserializer.total_tensor_bytes)
 duration = end - start
 per_second = convert_bytes(deserializer.total_tensor_bytes / duration)
 after_mem = get_mem_usage()
 deserializer.close()
-print(f"Deserialized {total_bytes_str} in {end - start:0.2f}s, {per_second}")
+print(f"Deserialized {total_bytes_str} in {end - start:0.2f}s, {per_second}/s")
 print(f"Memory usage before: {before_mem}")
 print(f"Memory usage after: {after_mem}")
 
 # Tokenize and generate
 model.eval()
 tokenizer = AutoTokenizer.from_pretrained(model_ref)
+eos = tokenizer.eos_token_id
 input_ids = tokenizer.encode(
     "¡Hola! Encantado de conocerte. hoy voy a", return_tensors="pt"
 ).to("cuda")
 
 with torch.no_grad():
-    output = model.generate(input_ids, max_new_tokens=50, do_sample=True)
+    output = model.generate(
+        input_ids, max_new_tokens=50, do_sample=True, pad_token_id=eos
+    )
 
 print(f"Output: {tokenizer.decode(output[0], skip_special_tokens=True)}")
 ```
 
 It should produce output similar to the following, with GPT-J-6B:
 ```
 Deserialized model in 6.25 seconds
@@ -221,82 +216,82 @@
 and `hf_main()` serializes
 [HuggingFace Transformers](https://github.com/huggingface/transformers) models.
 
 ## Available Pre-Tensorized Models on the CoreWeave Cloud
 
 The following models are available on the CoreWeave Cloud for free, and can be
 used with the `TensorDeserializer` class. The S3 support defaults to the
-`accel-object.ord1.coreweave.com` endpoint, and the bucket to use `tensorized`.
+`accel-object.ord1.coreweave.com` endpoint, and the bucket to use as `tensorized`.
 
 We name the keys in the S3 bucket after the HuggingFace model identifier, and
 append the `/fp16` suffix for the half-precision version.
 
 For example, the S3 URI for the `EleutherAI/gpt-j-6B` model is:
 `s3://tensorized/EleutherAI/gpt-j-6B/fp16/model.tensors`
 
 The below table shows the available models and their S3 URIs.
 
 ### Large Language Models
 
-| Model                                                                     | Precision | S3 URI  |
-|---------------------------------------------------------------------------|-----------|---------|
-| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-125M/model.tensors` |
-| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-125M/fp16/model.tensors` |
-| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/model.tensors` |
-| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/fp16/model.tensors` |
-| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/model.tensors` |
-| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/fp16/model.tensors` |
-| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)         | `fp32`    | `s3://tensorized/EleutherAI/gpt-j-6B/model.tensors` |
-| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)         | `fp16`    | `s3://tensorized/EleutherAI/gpt-j-6B/fp16/model.tensors` |
-| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b) | `fp32`    | `s3://tensorized/EleutherAI/gpt-neox-20b/model.tensors` |
-| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b) | `fp16`    | `s3://tensorized/EleutherAI/gpt-neox-20b/fp16/model.tensors` |
-| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)     | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m/model.tensors` |
-| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)     | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m/fp16/model.tensors` |
-| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b/model.tensors` |
-| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-1.4b/fp16/model.tensors` |
-| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b/model.tensors` |
-| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-2.8b/fp16/model.tensors` |
-| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b/model.tensors` |
-| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-6.9b/fp16/model.tensors` |
-| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)     | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b/model.tensors` |
-| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)     | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b/fp16/model.tensors` |
-| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/model.tensors` |
-| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-1.4b-deduped](https://huggingface.co/EleutherAI/pythia-1.4b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b-deduped/model.tensors` |
+| Model                                                                                   | Precision | S3 URI                                                              |
+|-----------------------------------------------------------------------------------------|-----------|---------------------------------------------------------------------|
+| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-125M/model.tensors`             |
+| [EleutherAI/gpt-neo-125M](https://huggingface.co/EleutherAI/gpt-neo-125M)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-125M/fp16/model.tensors`        |
+| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/model.tensors`             |
+| [EleutherAI/gpt-neo-1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-1.3B/fp16/model.tensors`        |
+| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/model.tensors`             |
+| [EleutherAI/gpt-neo-2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neo-2.7B/fp16/model.tensors`        |
+| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)                       | `fp32`    | `s3://tensorized/EleutherAI/gpt-j-6B/model.tensors`                 |
+| [EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)                       | `fp16`    | `s3://tensorized/EleutherAI/gpt-j-6B/fp16/model.tensors`            |
+| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b)               | `fp32`    | `s3://tensorized/EleutherAI/gpt-neox-20b/model.tensors`             |
+| [EleutherAI/gpt-neox-20b](https://huggingface.co/EleutherAI/gpt-neox-20b)               | `fp16`    | `s3://tensorized/EleutherAI/gpt-neox-20b/fp16/model.tensors`        |
+| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)                   | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m/model.tensors`               |
+| [EleutherAI/pythia-70m](https://huggingface.co/EleutherAI/pythia-70m)                   | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m/fp16/model.tensors`          |
+| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)                 | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b/model.tensors`              |
+| [EleutherAI/pythia-1.4b](https://huggingface.co/EleutherAI/pythia-1.4b)                 | `fp16`    | `s3://tensorized/EleutherAI/pythia-1.4b/fp16/model.tensors`         |
+| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)                 | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b/model.tensors`              |
+| [EleutherAI/pythia-2.8b](https://huggingface.co/EleutherAI/pythia-2.8b)                 | `fp16`    | `s3://tensorized/EleutherAI/pythia-2.8b/fp16/model.tensors`         |
+| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)                 | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b/model.tensors`              |
+| [EleutherAI/pythia-6.9b](https://huggingface.co/EleutherAI/pythia-6.9b)                 | `fp16`    | `s3://tensorized/EleutherAI/pythia-6.9b/fp16/model.tensors`         |
+| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)                   | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b/model.tensors`               |
+| [EleutherAI/pythia-12b](https://huggingface.co/EleutherAI/pythia-12b)                   | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b/fp16/model.tensors`          |
+| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/model.tensors`       |
+| [EleutherAI/pythia-70m-deduped](https://huggingface.co/EleutherAI/pythia-70m-deduped)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-70m-deduped/fp16/model.tensors`  |
+| [EleutherAI/pythia-1.4b-deduped](https://huggingface.co/EleutherAI/pythia-1.4b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-1.4b-deduped/model.tensors`      |
 | [EleutherAI/pythia-1.4b-deduped](https://huggingface.co/EleutherAI/pythia-1.4b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-1.4b-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-2.8b-deduped](https://huggingface.co/EleutherAI/pythia-2.8b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b-deduped/model.tensors` |
+| [EleutherAI/pythia-2.8b-deduped](https://huggingface.co/EleutherAI/pythia-2.8b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-2.8b-deduped/model.tensors`      |
 | [EleutherAI/pythia-2.8b-deduped](https://huggingface.co/EleutherAI/pythia-2.8b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-2.8b-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-6.9b-deduped](https://huggingface.co/EleutherAI/pythia-6.9b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b-deduped/model.tensors` |
+| [EleutherAI/pythia-6.9b-deduped](https://huggingface.co/EleutherAI/pythia-6.9b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-6.9b-deduped/model.tensors`      |
 | [EleutherAI/pythia-6.9b-deduped](https://huggingface.co/EleutherAI/pythia-6.9b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-6.9b-deduped/fp16/model.tensors` |
-| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped) | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/model.tensors` |
-| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped) | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/model.tensors` |
-| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/model.tensors` |
-| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/model.tensors` |
-| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/model.tensors` |
-| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/fp16/model.tensors` |
-| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B) | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/model.tensors` |
-| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B) | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/fp16/model.tensors` |
-| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono) | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-mono/model.tensors` |
-| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono) | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-mono/fp16/model.tensors` |
-| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi) | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-multi/model.tensors` |
-| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi) | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-multi/fp16/model.tensors` |
-| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi) | `fp32`    | `s3://tensorized/Salesforce/codegen-2B-multi/model.tensors` |
-| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi) | `fp16`    | `s3://tensorized/Salesforce/codegen-2B-multi/fp16/model.tensors` |
-| [Salesforce/codgen-6B-mono](https://huggingface.co/Salesforce/codgen-6B-mono) | `fp32`    | `s3://tensorized/Salesforce/codgen-6B-mono/model.tensors` |
-| [Salesforce/codgen-6B-mono](https://huggingface.co/Salesforce/codgen-6B-mono) | `fp16`    | `s3://tensorized/Salesforce/codgen-6B-mono/fp16/model.tensors` |
-| [Salesforce/codgen-6B-multi](https://huggingface.co/Salesforce/codgen-6B-multi) | `fp32`    | `s3://tensorized/Salesforce/codgen-6B-multi/model.tensors` |
-| [Salesforce/codgen-6B-multi](https://huggingface.co/Salesforce/codgen-6B-multi) | `fp16`    | `s3://tensorized/Salesforce/codgen-6B-multi/fp16/model.tensors` |
-| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono) | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-mono/model.tensors` |
-| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono) | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-mono/fp16/model.tensors` |
-| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi) | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-multi/model.tensors` |
-| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi) | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-multi/fp16/model.tensors` |
+| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped)   | `fp32`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/model.tensors`       |
+| [EleutherAI/pythia-12b-deduped](https://huggingface.co/EleutherAI/pythia-12b-deduped)   | `fp16`    | `s3://tensorized/EleutherAI/pythia-12b-deduped/fp16/model.tensors`  |
+| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/model.tensors`         |
+| [KoboldAI/fairseq-dense-125M](https://huggingface.co/KoboldAI/fairseq-dense-125M)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-125M/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/model.tensors`         |
+| [KoboldAI/fairseq-dense-355M](https://huggingface.co/KoboldAI/fairseq-dense-355M)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-355M/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/model.tensors`         |
+| [KoboldAI/fairseq-dense-2.7B](https://huggingface.co/KoboldAI/fairseq-dense-2.7B)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-2.7B/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B)       | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/model.tensors`         |
+| [KoboldAI/fairseq-dense-6.7B](https://huggingface.co/KoboldAI/fairseq-dense-6.7B)       | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-6.7B/fp16/model.tensors`    |
+| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B)         | `fp32`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/model.tensors`          |
+| [KoboldAI/fairseq-dense-13B](https://huggingface.co/KoboldAI/fairseq-dense-13B)         | `fp16`    | `s3://tensorized/KoboldAI/fairseq-dense-13B/fp16/model.tensors`     |
+| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono)     | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-mono/model.tensors`        |
+| [Salesforce/codegen-350M-mono](https://huggingface.co/Salesforce/codegen-350M-mono)     | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-mono/fp16/model.tensors`   |
+| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi)   | `fp32`    | `s3://tensorized/Salesforce/codegen-350M-multi/model.tensors`       |
+| [Salesforce/codegen-350M-multi](https://huggingface.co/Salesforce/codegen-350M-multi)   | `fp16`    | `s3://tensorized/Salesforce/codegen-350M-multi/fp16/model.tensors`  |
+| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi)       | `fp32`    | `s3://tensorized/Salesforce/codegen-2B-multi/model.tensors`         |
+| [Salesforce/codegen-2B-multi](https://huggingface.co/Salesforce/codegen-2B-multi)       | `fp16`    | `s3://tensorized/Salesforce/codegen-2B-multi/fp16/model.tensors`    |
+| [Salesforce/codegen-6B-mono](https://huggingface.co/Salesforce/codegen-6B-mono)         | `fp32`    | `s3://tensorized/Salesforce/codegen-6B-mono/model.tensors`          |
+| [Salesforce/codegen-6B-mono](https://huggingface.co/Salesforce/codegen-6B-mono)         | `fp16`    | `s3://tensorized/Salesforce/codegen-6B-mono/fp16/model.tensors`     |
+| [Salesforce/codegen-6B-multi](https://huggingface.co/Salesforce/codegen-6B-multi)       | `fp32`    | `s3://tensorized/Salesforce/codegen-6B-multi/model.tensors`         |
+| [Salesforce/codegen-6B-multi](https://huggingface.co/Salesforce/codegen-6B-multi)       | `fp16`    | `s3://tensorized/Salesforce/codegen-6B-multi/fp16/model.tensors`    |
+| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono)       | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-mono/model.tensors`         |
+| [Salesforce/codegen-16B-mono](https://huggingface.co/Salesforce/codegen-16B-mono)       | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-mono/fp16/model.tensors`    |
+| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi)     | `fp32`    | `s3://tensorized/Salesforce/codegen-16B-multi/model.tensors`        |
+| [Salesforce/codegen-16B-multi](https://huggingface.co/Salesforce/codegen-16B-multi)     | `fp16`    | `s3://tensorized/Salesforce/codegen-16B-multi/fp16/model.tensors`   |
 
 ## S3 Usage Notes
 `tensorizer` uses the `boto3` library to interact with S3. The easiest way
 to use `tensorizer` with S3 is to configure your S3 credentials in
 `~/.s3cfg`.
 
 If you don't want to use `~/.s3cfg`, or wish to use a `.s3cfg` config file
@@ -342,15 +337,15 @@
 endpoint once the object is cached.
 
 **NOTE2:** The cache above does not get invalidated when the object is updated
 in S3. If you update an object in S3, you will need to wait for the cache to
 expire before you can download the updated object. This takes 24 hours since
 the last download.
 
-For this reason, it is recommended to use an unique S3 key for each version
+For this reason, it is recommended to use a unique S3 key for each version
 of a model if you use the `accel-object.ord1.coreweave.com` endpoint.
 
 ## Additional Features
 `tensorizer` has a few additional features that make it more useful than
 just a serialization/deserialization tool.
 
 ### Plaid Mode
```

### Comparing `tensorizer-1.0.1/tensorizer.egg-info/SOURCES.txt` & `tensorizer-1.1.0/tensorizer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 tensorizer/tensors_pb2.py
 tensorizer/utils.py
 tensorizer.egg-info/PKG-INFO
 tensorizer.egg-info/SOURCES.txt
 tensorizer.egg-info/dependency_links.txt
 tensorizer.egg-info/requires.txt
 tensorizer.egg-info/top_level.txt
+tensors/LICENSE
 tensors/__init__.py
 tensors/go.mod
 tensors/go.sum
 tensors/tensors.pb.go
 tensors/tensors_pb.d.ts
 tensors/tensors_pb.js
 tensors/tensors_pb2.py
```

### Comparing `tensorizer-1.0.1/tensors/__pycache__/tensors_pb2.cpython-310.pyc` & `tensorizer-1.1.0/tensors/__pycache__/tensors_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/tensors/go.sum` & `tensorizer-1.1.0/tensors/go.sum`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/tensors/tensors.pb.go` & `tensorizer-1.1.0/tensors/tensors.pb.go`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/tensors/tensors_pb.d.ts` & `tensorizer-1.1.0/tensors/tensors_pb.d.ts`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/tensors/tensors_pb.js` & `tensorizer-1.1.0/tensors/tensors_pb.js`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/tensors/tensors_pb2.py` & `tensorizer-1.1.0/tensors/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorizer-1.0.1/tests/test_serialization.py` & `tensorizer-1.1.0/tests/test_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 import contextlib
 import gc
 import os
+import re
 import tempfile
 import unittest
-import re
 from typing import Tuple
+
 import torch
 
-os.environ[
-    "TRANSFORMERS_VERBOSITY"
-] = "error"  # disable missing keys and unexpected key warnings
-os.environ[
-    "TOKENIZERS_PARALLELISM"
-] = "false"  # avoids excessive warnings about forking after using a tokenizer
-
-from transformers import AutoModelForCausalLM, AutoTokenizer
-
-from tensorizer import TensorSerializer, TensorDeserializer
-from tensorizer import utils
-from collections import OrderedDict
+os.environ["TOKENIZERS_PARALLELISM"] = (
+    "false"  # avoids excessive warnings about forking after using a tokenizer
+)
+
+from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
+
+from tensorizer import TensorDeserializer, TensorSerializer, utils
 
 model_name = "EleutherAI/gpt-neo-125M"
 num_hellos = 400
 is_cuda_available = torch.cuda.is_available()
 default_device = "cuda" if is_cuda_available else "cpu"
 
 
@@ -41,21 +37,26 @@
 
 
 def check_deserialized(deserialized, model_name: str, allow_subset=False):
     orig_sd = AutoModelForCausalLM.from_pretrained(model_name).state_dict()
     if not allow_subset:
         assert orig_sd.keys() == deserialized.keys()
     for k, v in deserialized.items():
+        # fmt: off
         assert k in orig_sd, \
             f"{k} not in {orig_sd.keys()}"
+
         assert v.size() == orig_sd[k].size(), \
             f"{v.size()} != {orig_sd[k].size()}"
+
         assert v.dtype == orig_sd[k].dtype, \
             f"{v.dtype} != {orig_sd[k].dtype}"
+
         assert torch.all(orig_sd[k].to(v.device) == v)
+        # fmt: on
     del orig_sd
     gc.collect()
 
 
 @contextlib.contextmanager
 def enable_tokenizers_parallelism():
     os.environ["TOKENIZERS_PARALLELISM"] = "true"
@@ -65,32 +66,31 @@
         os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 
 def check_inference(
     deserializer: TensorDeserializer, model_ref: str, device: str
 ):
     # This ensures that the model is not initialized.
-    model = utils.no_init_or_tensor(
-        lambda: AutoModelForCausalLM.from_pretrained(
-            model_ref, state_dict=OrderedDict()
-        )
-    )
+    config = AutoConfig.from_pretrained(model_ref)
+    with utils.no_init_or_tensor():
+        model = AutoModelForCausalLM.from_config(config)
 
     deserializer.load_into_module(model)
 
     # Tokenize and generate
     with enable_tokenizers_parallelism():
         tokenizer = AutoTokenizer.from_pretrained(model_ref)
+        eos = tokenizer.eos_token_id
         input_ids = tokenizer.encode(
             " hello" * num_hellos, return_tensors="pt"
         ).to(device)
 
         with torch.no_grad():
             output = model.generate(
-                input_ids, max_new_tokens=50, do_sample=True
+                input_ids, max_new_tokens=50, do_sample=True, pad_token_id=eos
             )
 
         decoded = tokenizer.decode(output[0], skip_special_tokens=True)
         assert decoded.count("hello") > num_hellos
 
 
 class TestSerialization(unittest.TestCase):
@@ -262,15 +262,16 @@
         ), (
             "The filter_func test cannot continue"
             " because a filter_func used in the test"
             " does not appear in the test model,"
             " or matches all tensor names."
             " Update the pattern and/or custom_check"
             " to use more informative filtering criteria."
-            "\n\nTensors present in the model: " + " ".join(all_keys)
+            "\n\nTensors present in the model: "
+            + " ".join(all_keys)
         )
 
         with self.subTest(msg="Testing regex filter_func"):
             in_file = open(self._serialized_model_path, "rb")
             deserialized = TensorDeserializer(
                 in_file, device=default_device, filter_func=pattern.match
             )
```

### Comparing `tensorizer-1.0.1/tests/test_stream_io.py` & `tensorizer-1.1.0/tests/test_stream_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import contextlib
 import os
 import unittest
-import moto
+
 import boto3
+import moto
+
 from tensorizer import stream_io
 
 NEO_URL = (
     "https://raw.githubusercontent.com/EleutherAI/gpt-neo/master/README.md"
 )
 
 
@@ -74,19 +76,19 @@
 def tear_down_moto(old_environment):
     for key, value in old_environment:
         os.environ[key] = value
 
 
 @contextlib.contextmanager
 def mock_server():
+    import logging
+
     from moto.server import ThreadedMotoServer
 
     # Disable mock server logs
-    import logging
-
     werkzeug_logger = logging.getLogger("werkzeug")
     old_log_level = werkzeug_logger.getEffectiveLevel()
     werkzeug_logger.setLevel(logging.CRITICAL + 1)
 
     server = ThreadedMotoServer(
         ip_address="127.0.0.1", port=5000, verbose=False
     )
```

