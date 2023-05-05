# Comparing `tmp/curated-transformers-0.0.8.tar.gz` & `tmp/curated-transformers-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-0.0.8.tar", last modified: Tue May  2 15:19:14 2023, max compression
+gzip compressed data, was "curated-transformers-0.1.0.tar", last modified: Fri May  5 11:55:56 2023, max compression
```

## Comparing `curated-transformers-0.0.8.tar` & `curated-transformers-0.1.0.tar`

### file list

```diff
@@ -1,106 +1,60 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.819089 curated-transformers-0.0.8/
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1267 2023-05-02 15:19:14.819089 curated-transformers-0.0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      954 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.799089 curated-transformers-0.0.8/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.803089 curated-transformers-0.0.8/curated_transformers/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4050 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/cli/debug_pieces.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4697 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/cli/quantize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4688 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.803089 curated-transformers-0.0.8/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24143 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1206 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19182 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4102 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/output.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pooling.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.807089 curated-transformers-0.0.8/curated_transformers/models/pytorch/
--rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      583 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/activations.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.807089 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/
--rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2364 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      949 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2259 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/attention.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3795 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1739 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4775 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/layer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1240 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/curated_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      890 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10982 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/hf_util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1781 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1882 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/pytorch/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/remove_eos_bos.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4650 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/models/with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17281 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/pipeline/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3207 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4550 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_pooling.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1419 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6139 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3176 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4313 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/models/test_with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.811089 curated-transformers-0.0.8/curated_transformers/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17306 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/pipeline/test_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/pipeline/toy-en-corpus.spacy
--rw-r--r--   0 vsts      (1001) docker     (122)      406 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (122)      794 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/test_torchscript_wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.815089 curated-transformers-0.0.8/curated_transformers/tests/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3369 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2737 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7925 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4819 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/test_xlmr_adapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy-chars.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy.model
--rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/tokenization/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.819089 curated-transformers-0.0.8/curated_transformers/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3612 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/sentencepiece_adapters.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3823 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5890 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/tokenization/wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2711 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/curated_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 15:19:14.803089 curated-transformers-0.0.8/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1267 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4184 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       56 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-02 15:19:14.000000 curated-transformers-0.0.8/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-05-02 15:19:14.819089 curated-transformers-0.0.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-05-02 15:19:04.000000 curated-transformers-0.0.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)      773 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      460 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.113939 curated-transformers-0.1.0/curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      313 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/_compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4688 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.113939 curated-transformers-0.1.0/curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      583 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/activations.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      105 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/albert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2362 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/albert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      949 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/albert/layer_group.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2258 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/attention.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3795 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1738 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4774 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/bert/layer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/curated_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10980 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/hf_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1556 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/output.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/roberta/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/roberta/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1780 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/roberta/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1881 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/models/scalar_weight.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1254 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       94 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tests/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/albert/test_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2969 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/test_hf_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1441 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/models/test_torchscript.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tests/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.117939 curated-transformers-0.1.0/curated_transformers/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/curated_transformers/tokenization/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-05 11:55:56.113939 curated-transformers-0.1.0/curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      773 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       36 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-05 11:55:56.000000 curated-transformers-0.1.0/curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-05 11:55:55.000000 curated-transformers-0.1.0/curated_transformers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)      612 2023-05-05 11:55:56.121939 curated-transformers-0.1.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      204 2023-05-05 11:55:45.000000 curated-transformers-0.1.0/setup.py
```

### Comparing `curated-transformers-0.0.8/LICENSE` & `curated-transformers-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.8/curated_transformers/errors.py` & `curated-transformers-0.1.0/curated_transformers/errors.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/activations.py` & `curated-transformers-0.1.0/curated_transformers/models/activations.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/config.py` & `curated-transformers-0.1.0/curated_transformers/models/albert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/encoder.py` & `curated-transformers-0.1.0/curated_transformers/models/albert/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 import torch
 from torch.nn import Module
 from torch import Tensor
 
-from ....errors import Errors
+from ...errors import Errors
 from ..attention import AttentionMask
 from ..bert.embeddings import BertEmbeddings
-from ...output import PyTorchTransformerOutput
+from ..output import PyTorchTransformerOutput
 from .config import AlbertConfig
 from .layer_group import AlbertLayerGroup
 
 
 class AlbertEncoder(Module):
     def __init__(
         self,
```

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/albert/layer_group.py` & `curated-transformers-0.1.0/curated_transformers/models/albert/layer_group.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/attention.py` & `curated-transformers-0.1.0/curated_transformers/models/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 import math
 import torch
 from torch import Tensor
 from torch.nn import Module
 
-from ...errors import Errors
+from ..errors import Errors
 
 
 class AttentionMask:
     bool_mask: Tensor
     _logit_mask: Optional[Tensor]
 
     def __init__(self, bool_mask: Tensor):
```

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/config.py` & `curated-transformers-0.1.0/curated_transformers/models/bert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/embeddings.py` & `curated-transformers-0.1.0/curated_transformers/models/bert/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/encoder.py` & `curated-transformers-0.1.0/curated_transformers/models/bert/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from torch.nn import Module
 from torch import Tensor
 
 from .config import BertConfig
 from .embeddings import BertEmbeddings
 from .layer import BertEncoderLayer
 from ..attention import AttentionMask
-from ...output import PyTorchTransformerOutput
+from ..output import PyTorchTransformerOutput
 
 
 class BertEncoder(Module):
     def __init__(
         self,
         config: BertConfig,
     ):
```

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/bert/layer.py` & `curated-transformers-0.1.0/curated_transformers/models/bert/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 from torch.nn import Linear, Module
 from torch import Tensor
 
 from .. import GeluNew
 from ..attention import AttentionMask, ScaledDotProductAttention
 from .config import BertAttentionConfig, BertLayerConfig
-from ....errors import Errors
+from ...errors import Errors
 
 
 # https://www.tensorflow.org/text/tutorials/transformer#multi-head_attention
 class BertSelfAttention(Module):
     def __init__(self, config: BertAttentionConfig):
         super().__init__()
```

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/curated_transformer.py` & `curated-transformers-0.1.0/curated_transformers/models/curated_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 from .albert.encoder import AlbertEncoder
 from .bert.encoder import BertEncoder
 from .roberta.encoder import RobertaEncoder
 
 from .attention import AttentionMask
-from ..output import PyTorchTransformerOutput
+from .output import PyTorchTransformerOutput
 
 CuratedEncoderT = TypeVar("CuratedEncoderT", AlbertEncoder, BertEncoder, RobertaEncoder)
 
 
 class CuratedTransformer(Generic[CuratedEncoderT], Module):
     """Simple wrapper for encoders. Currently only used to add a predictable
     prefix (curated_encoder) to encoders."""
```

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/embeddings.py` & `curated-transformers-0.1.0/curated_transformers/models/embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 import torch
 from torch import Tensor
 from torch.nn import Module
 
+
 # https://pytorch.org/tutorials/beginner/transformer_tutorial.html
 class SinusoidalPositionalEmbedding(Module):
     def __init__(self, dim: int, max_len: int, *, normalize=True):
         super().__init__()
 
         position = torch.arange(max_len).unsqueeze(1)
         div_term = torch.exp(torch.arange(0, dim, 2) * (-math.log(10000.0) / dim))
```

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/hf_util.py` & `curated-transformers-0.1.0/curated_transformers/models/hf_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import re
 
 
 from .albert.encoder import AlbertEncoder
 from .bert.encoder import BertEncoder
 from .curated_transformer import CuratedTransformer, CuratedEncoderT
 from .roberta.encoder import RobertaEncoder
-from ..._compat import transformers
-from ...errors import Errors
+from .._compat import transformers
+from ..errors import Errors
 
 SUPPORTED_MODEL_TYPES = ["albert", "bert", "camembert", "roberta", "xlm-roberta"]
 SUPPORTED_CURATED_ENCODERS = (AlbertEncoder, BertEncoder, RobertaEncoder)
 
 
 def _check_supported_hf_models(model_type: str):
     if model_type not in SUPPORTED_MODEL_TYPES:
```

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/config.py` & `curated-transformers-0.1.0/curated_transformers/models/roberta/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/embeddings.py` & `curated-transformers-0.1.0/curated_transformers/models/roberta/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/roberta/encoder.py` & `curated-transformers-0.1.0/curated_transformers/models/roberta/encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import torch
 from torch.nn import Module
 from torch import Tensor
 
 from ..attention import AttentionMask
 from ..bert.layer import BertEncoderLayer
-from ...output import PyTorchTransformerOutput
+from ..output import PyTorchTransformerOutput
 from .embeddings import RobertaEmbeddings
 from .config import RobertaConfig
 
 
 class RobertaEncoder(Module):
     def __init__(self, config: RobertaConfig):
         super().__init__()
```

### Comparing `curated-transformers-0.0.8/curated_transformers/models/pytorch/scalar_weight.py` & `curated-transformers-0.1.0/curated_transformers/models/scalar_weight.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 from torch import Tensor
 from torch.nn import Module
 
-from ...errors import Errors
+from ..errors import Errors
 
 
 # From syntaxdot:
 # https://github.com/tensordot/syntaxdot/blob/22bd3d43ed2d7fcbef8a6217b01684194fae713f/syntaxdot-transformers/src/scalar_weighting.rs#L62
 class ScalarWeight(Module):
     def __init__(self, *, num_layers: int, dropout_prob: float = 0.1):
         super().__init__()
```

### Comparing `curated-transformers-0.0.8/curated_transformers/tests/models/test_hf_model.py` & `curated-transformers-0.1.0/curated_transformers/tests/models/test_hf_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Callable
 from dataclasses import dataclass
 import pytest
-from thinc.api import get_torch_default_device
 from torch.nn import Module
 
 from curated_transformers._compat import has_hf_transformers, transformers
-from curated_transformers.models.architectures import _pytorch_encoder
-from curated_transformers.models.hf_loader import build_hf_transformer_encoder_loader_v1
-from curated_transformers.models.pytorch.albert import AlbertEncoder
-from curated_transformers.models.pytorch.albert.config import AlbertConfig
-from curated_transformers.models.pytorch.attention import AttentionMask
-from curated_transformers.models.pytorch.bert import BertConfig, BertEncoder
-from curated_transformers.models.pytorch.roberta.config import RobertaConfig
-from curated_transformers.models.pytorch.roberta.encoder import RobertaEncoder
+from curated_transformers.models.curated_transformer import CuratedTransformer
+from curated_transformers.models.hf_util import convert_pretrained_model_for_encoder
+from curated_transformers.models.albert import AlbertEncoder
+from curated_transformers.models.albert.config import AlbertConfig
+from curated_transformers.models.attention import AttentionMask
+from curated_transformers.models.bert import BertConfig, BertEncoder
+from curated_transformers.models.roberta.config import RobertaConfig
+from curated_transformers.models.roberta.encoder import RobertaEncoder
+
+from ..conftest import TORCH_DEVICES
 
 from ..util import torch_assertclose
 
 
 @dataclass
 class ModelConfig:
     config: BertConfig
@@ -28,44 +29,37 @@
     ModelConfig(AlbertConfig(vocab_size=30000), AlbertEncoder, "albert-base-v2"),
     ModelConfig(BertConfig(vocab_size=28996), BertEncoder, "bert-base-cased"),
     ModelConfig(RobertaConfig(), RobertaEncoder, "roberta-base"),
     ModelConfig(RobertaConfig(vocab_size=250002), RobertaEncoder, "xlm-roberta-base"),
 ]
 
 
-def encoder_from_config(config: ModelConfig):
+def encoder_from_config(config: ModelConfig, hf_encoder: Module):
     encoder = config.encoder(config.config)
-    model = _pytorch_encoder(encoder)
-    model.init = build_hf_transformer_encoder_loader_v1(name=config.hf_model_name)
-    return model
-
-
-@pytest.mark.slow
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("model_config", TEST_MODELS)
-def test_hf_load_weights(model_config):
-    model = encoder_from_config(model_config)
-    assert model
+    transformer = CuratedTransformer(encoder)
+    transformer.load_state_dict(
+        convert_pretrained_model_for_encoder(transformer, hf_encoder.state_dict())
+    )
+    return transformer
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("model_config", TEST_MODELS)
-def test_model_against_hf_transformers(model_config):
-    torch_device = get_torch_default_device()
-
-    model = encoder_from_config(model_config)
-    model.initialize()
-    encoder = model.shims[0]._model
-    encoder.eval()
+@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
+def test_model_against_hf_transformers(model_config, torch_device):
     hf_encoder = transformers.AutoModel.from_pretrained(model_config.hf_model_name).to(
         torch_device
     )
     hf_encoder.eval()
 
+    encoder = encoder_from_config(model_config, hf_encoder)
+    encoder.to(torch_device)
+    encoder.eval()
+
     hf_tokenizer = transformers.AutoTokenizer.from_pretrained(
         model_config.hf_model_name
     )
     tokenization = hf_tokenizer(
         ["This is a test.", "Let's match outputs"], padding=True, return_tensors="pt"
     ).to(torch_device)
     X = tokenization["input_ids"]
```

