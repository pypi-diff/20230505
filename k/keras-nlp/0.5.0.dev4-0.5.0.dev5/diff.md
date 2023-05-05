# Comparing `tmp/keras-nlp-0.5.0.dev4.tar.gz` & `tmp/keras-nlp-0.5.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nlp-0.5.0.dev4.tar", last modified: Thu May  4 19:46:12 2023, max compression
+gzip compressed data, was "keras-nlp-0.5.0.dev5.tar", last modified: Fri May  5 19:41:39 2023, max compression
```

## Comparing `keras-nlp-0.5.0.dev4.tar` & `keras-nlp-0.5.0.dev5.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/api_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.237939 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/cached_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/cached_multi_head_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/f_net_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/f_net_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_mask_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/multi_segment_packer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_deletion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_swap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/sine_position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/sine_position_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/start_end_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/start_end_packer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/token_and_position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/token_and_position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14352 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_decoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_layer_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.241939 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/bleu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/edit_distance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/perplexity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_l_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_n_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.241939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.245939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.245939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.249939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.253939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/relative_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.257939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.261939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.261939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.265939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.269939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.269939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_transformer_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/task_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.269939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.273939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.277939 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/beam_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/beam_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/contrastive_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/contrastive_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/greedy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/greedy_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/random_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_k_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_k_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_p_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_p_sampler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.277939 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.277939 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/docstring_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/docstring_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24894 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_pair_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/keras_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/keras_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/pipeline_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/tf_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/keras_nlp/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-04 19:46:12.285939 keras-nlp-0.5.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.359506 keras-nlp-0.5.0.dev5/keras_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/api_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.367507 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/cached_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/cached_multi_head_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/f_net_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/f_net_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_head_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_mask_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/multi_segment_packer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_deletion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_swap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/sine_position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/sine_position_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/start_end_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/start_end_packer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/token_and_position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/token_and_position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14352 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_layer_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.367507 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/bleu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/edit_distance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/perplexity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_l_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_n_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.367507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.371507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.371507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.375507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.375507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/relative_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.379507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.379507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.383507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.387508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.391508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.391508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_transformer_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/task_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.391508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.391508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.395508 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/beam_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/beam_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/contrastive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/contrastive_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/greedy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/greedy_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/random_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_k_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_k_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_p_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_p_sampler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.395508 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.395508 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/docstring_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/docstring_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24894 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_pair_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/keras_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/keras_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/pipeline_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/tf_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/keras_nlp/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.359506 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/setup.py
```

### Comparing `keras-nlp-0.5.0.dev4/PKG-INFO` & `keras-nlp-0.5.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.5.0.dev4
+Version: 0.5.0.dev5
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nlp-0.5.0.dev4/README.md` & `keras-nlp-0.5.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/layers/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/models/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/models/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/samplers/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 from keras_nlp.src import layers
 from keras_nlp.src import metrics
 from keras_nlp.src import models
 from keras_nlp.src import samplers
 from keras_nlp.src import tokenizers
 from keras_nlp.src import utils
 
-__version__ = "0.5.0.dev4"
+# This is the global source of truth for the version number.
+__version__ = "0.5.0.dev5"
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/api_export.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/conftest.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,20 @@
     )
     parser.addoption(
         "--mixed_precision",
         action="store_true",
         default=False,
         help="run with mixed precision",
     )
+    parser.addoption(
+        "--docstring_module",
+        action="store",
+        default="",
+        help="restrict docs testing to modules whose name matches this flag",
+    )
 
 
 def pytest_configure(config):
     if config.getoption("--mixed_precision"):
         keras.mixed_precision.set_global_policy("mixed_float16")
     config.addinivalue_line(
         "markers", "large: mark test as being slow or requiring a network"
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/cached_multi_head_attention.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/cached_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/cached_multi_head_attention_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/cached_multi_head_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/f_net_encoder.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/f_net_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/f_net_encoder_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/f_net_encoder_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_head.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_head.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_head_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_head_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_mask_generator.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_mask_generator.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_mask_generator_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_mask_generator_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/multi_segment_packer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/multi_segment_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/multi_segment_packer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/multi_segment_packer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/position_embedding.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/position_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/position_embedding_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/position_embedding_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_deletion.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_deletion.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_deletion_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_deletion_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_swap.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_swap.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_swap_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_swap_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/sine_position_encoding.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/sine_position_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/sine_position_encoding_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/sine_position_encoding_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/start_end_packer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/start_end_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/start_end_packer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/start_end_packer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/token_and_position_embedding.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/token_and_position_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/token_and_position_embedding_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/token_and_position_embedding_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_decoder.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_decoder_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_decoder_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_encoder.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_encoder_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_encoder_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_layer_utils.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_layer_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_layer_utils_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_layer_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/bleu.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/bleu_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/bleu_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/edit_distance.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/edit_distance.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/edit_distance_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/edit_distance_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/perplexity.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/perplexity.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/perplexity_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/perplexity_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_base.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_base.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_l.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_l.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_l_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_l_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_n.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_n.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_n_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_n_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_classifier.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_classifier_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_classifier.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_classifier_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/relative_embedding.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/relative_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_classifier.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_classifier.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_classifier_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 )
 from keras_nlp.src.models.opt.opt_presets import backbone_presets
 from keras_nlp.src.models.task import Task
 from keras_nlp.src.samplers.serialization import get as get_sampler
 from keras_nlp.src.utils.keras_utils import is_xla_compatible
 from keras_nlp.src.utils.python_utils import classproperty
 from keras_nlp.src.utils.tf_utils import tensor_to_string_list
-from keras_nlp.src.utils.tf_utils import truncate_at_token
 
 
 @keras_nlp_export("keras_nlp.models.OPTCausalLM")
 class OPTCausalLM(Task):
     """An end-to-end OPT model for causal langauge modeling.
 
     A causal language model (LM) predicts the next token based on previous
@@ -45,15 +44,15 @@
     This model has a `generate()` method, which generates text based on a
     prompt. The generation strategy used is controlled by an additional
     `sampler` argument on `compile()`. You can recompile the model with
     different `keras_nlp.samplers` objects to control the generation. By
     default, `"top_k"` sampling will be used.
 
     This model can optionally be configured with a `preprocessor` layer, in
-    which case it will automatically apply preprocessing to raw inputs during
+    which case it will automatically apply preprocessing to string inputs during
     `fit()`, `predict()`, `evaluate()` and `generate()`. This is done by default
     when creating the model with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/facebookresearch/fairseq/).
@@ -297,36 +296,31 @@
             self.generate_function = tf.function(
                 self.generate_step, jit_compile=jit_compile
             )
         return self.generate_function
 
     def generate_step(
         self,
-        token_ids,
-        padding_mask,
+        inputs,
         end_token_id=None,
     ):
         """A compilable generation function for a single batch of inputs.
 
         This function represents the inner, XLA-compilable, generation function
-        for a single batch of inputs. It takes in a dense `tf.Tensor` of token
-        ids, and return a dense `tf.Tensor` of token ids, and includes no
-        preprocessing. This function is wrapped by the `generate()` method.
+        for a single batch of inputs. Inputs should have the same structure as
+        model inputs, a dictionary with keys `"token_ids"` and `"padding_mask"`.
 
         Args:
-            token_ids: A dense int Tensor, with shape
-                `(batch_size, max_length)`. The user provided token ids
-                padded to `max_length`.
-            padding_mask: A dense boolean Tensor, with the same shape as
-                `token_ids`. Positions that are True in the `padding_mask`
-                are assumed to be user input and never updated.
+            inputs: A dictionary with two keys `"token_ids"` and
+                `"padding_mask"` and batched tensor values.
             end_token_id: The id of the end token to stop on. If all
                 sequences have produced a new `end_token_id`, generation
                 will stop.
         """
+        token_ids, padding_mask = inputs["token_ids"], inputs["padding_mask"]
         # Create and seed cache with a single forward pass.
         hidden_states, cache = self._build_cache(token_ids)
         # Compute the lengths of all user inputted tokens ids.
         row_lengths = tf.math.reduce_sum(
             tf.cast(padding_mask, tf.int32), axis=-1
         )
         # Start at the first index that has no user inputted id.
@@ -343,117 +337,168 @@
             )
             return (
                 tf.squeeze(logits, axis=1),
                 tf.squeeze(hidden_states, axis=1),
                 cache,
             )
 
-        return self._sampler(
+        token_ids = self._sampler(
             next=next,
             prompt=token_ids,
             cache=cache,
             index=index,
             mask=padding_mask,
             end_token_id=end_token_id,
             hidden_states=hidden_states,
         )
 
+        # Compute an output padding mask with the token ids we updated.
+        if end_token_id is not None:
+            # Build a mask of `end_token_id` locations not in the original
+            # prompt (not in locations where `padding_mask` is True).
+            end_locations = (token_ids == end_token_id) & (~padding_mask)
+            end_locations = tf.cast(end_locations, tf.int32)
+            # Use cumsum to get ones in all locations after end_locations.
+            overflow = tf.math.cumsum(end_locations, exclusive=True)
+            # Our padding mask is the inverse of these overflow locations.
+            padding_mask = ~tf.cast(overflow, tf.bool)
+        else:
+            # Without early stopping, all locations will have been updated.
+            padding_mask = tf.ones_like(token_ids, dtype=tf.bool)
+        return {
+            "token_ids": token_ids,
+            "padding_mask": padding_mask,
+        }
+
+    def _normalize_generate_inputs(
+        self,
+        inputs,
+    ):
+        """Normalize user input to the generate function.
+
+        This function coverts all inputs to tensors, adds a batch dimension if
+        necessary, and returns a iterable "dataset like" object (either an
+        actual `tf.data.Dataset` or a list with a single batch element).
+        """
+        input_is_scalar = False
+
+        if isinstance(inputs, tf.data.Dataset):
+            return inputs, input_is_scalar
+
+        if isinstance(inputs, str) or isinstance(inputs, list):
+            inputs = tf.convert_to_tensor(inputs)
+
+        if isinstance(inputs, tf.Tensor) and inputs.shape.rank == 0:
+            input_is_scalar = True
+            inputs = inputs[tf.newaxis]
+
+        # We avoid coverting to a dataset purely for speed, for a single batch
+        # of input, creating a dataset would add significant overhead.
+        return [inputs], input_is_scalar
+
+    def _normalize_generate_outputs(
+        self,
+        outputs,
+        input_is_scalar,
+    ):
+        """Normalize user output from the generate function.
+
+        This function converts all output to numpy (for integer output), or
+        python strings (for string output). If a batch dimension was added to
+        the input, it is removed from the output (so generate can be string in,
+        string out).
+        """
+
+        def normalize(x):
+            x = tf.concat(x, axis=0)
+            x = tf.squeeze(x, 0) if input_is_scalar else x
+            is_string = x.dtype == tf.string
+            # Convert outputs to a friendly pythonic type. For numerical outputs
+            # that is numpy, for string outputs that is `list` and `str`.
+            return tensor_to_string_list(x) if is_string else x.numpy()
+
+        if isinstance(outputs[0], dict):
+            return {
+                "token_ids": normalize([x["token_ids"] for x in outputs]),
+                "padding_mask": normalize([x["padding_mask"] for x in outputs]),
+            }
+        return normalize([x for x in outputs])
+
     def generate(
         self,
         inputs,
         max_length=None,
     ):
         """Generate text given prompt `inputs`.
 
         This method generates text based on given `inputs`. The sampling method
         used for generation can be set in the `compile` method.
 
-        If `inputs` is a `tf.data.Dataset`, outputs will be generated
+        If `inputs` are a `tf.data.Dataset`, outputs will be generated
         "batch-by-batch" and concatenated. Otherwise, all inputs will be handled
         as a single batch.
 
         If a `preprocessor` is attached to the model, `inputs` should be
         strings and returned sequences will be strings. Otherwise, inputs should
-        be preprocessed into token ids before calling `generate()`, and returned
-        sequences will also be token ids.
+        be preprocessed before calling `generate()`, and returned sequences will
+        be token ids.
 
         Args:
             inputs: a string `tf.Tensor`, a `tf.data.Dataset` of strings, a
                 python string or a list of python strings. If no `preprocessor`
                 is attached to the model, inputs should instead be a nested
                 `tf.Tensor` or `tf.data.Dataset` with keys `"token_ids"` and
                 `"padding_mask"`.
             max_length: Optional. int. The max length of the generated sequence.
-                Will default to the configured `sequence_length` of the
+                Will default to the max configured `sequence_length` of the
                 `preprocessor`. If `preprocessor` is `None`, `inputs` should be
-                padded to the desired max length and this argument is ignored.
+                should be padded to the desired maximum length and this argument
+                will be ignored.
 
         Returns:
             A string or string list if `preprocessor` is set, and a integer
-            tensor of token ids if `preprocessor is None`.
+            tensor of token IDs if `preprocessor is None`.
         """
-        input_is_scalar = False
-
+        # Setup our three main passes.
+        # 1. Optionally preprocessing strings to dense integer tensors.
+        # 2. Generate new tokens via a compiled function on dense tensors.
+        # 3. Optionally postprocess dense integer tensors back to string.
+        generate_function = self.make_generate_function()
+        end_token_id = None
         if self.preprocessor is not None:
+            end_token_id = self.preprocessor.tokenizer.end_token_id
 
-            def preprocess(x):
-                return self.preprocessor(
-                    x,
-                    sequence_length=max_length,
-                    return_labels=False,
-                    # We do not append an end token by default during
-                    # generation, as generating directly in the same sequence is
-                    # the most common workflow. If an end token directly after
-                    # a prompt is desired, it can be added to the prompt string.
-                    add_end_token=False,
-                )
-
-            if not isinstance(inputs, tf.data.Dataset):
-                inputs = tf.convert_to_tensor(inputs)
-                input_is_scalar = inputs.shape.rank == 0
-                inputs = inputs[tf.newaxis] if input_is_scalar else inputs
-                # Wrap a list to avoid the overhead of converting to dataset.
-                inputs = [preprocess(inputs)]
-            else:
+        def preprocess(x):
+            return self.preprocessor.generate_preprocess(
+                x, sequence_length=max_length
+            )
+
+        def generate(x):
+            return generate_function(x, end_token_id=end_token_id)
+
+        def postprocess(x):
+            return self.preprocessor.generate_postprocess(x)
+
+        # Normalize inputs, apply our three passes, and normalize outputs.
+        inputs, input_is_scalar = self._normalize_generate_inputs(inputs)
+
+        if self.preprocessor is not None:
+            if isinstance(inputs, tf.data.Dataset):
                 inputs = inputs.map(preprocess, tf.data.AUTOTUNE)
                 inputs = inputs.prefetch(tf.data.AUTOTUNE)
-        else:
-            if not isinstance(inputs, tf.data.Dataset):
-                # Wrap a list to avoid the overhead of converting to dataset.
-                inputs = [inputs]
+            else:
+                # Fast path for non-dataset, single-batch input.
+                inputs = [preprocess(x) for x in inputs]
 
-        generate_function = self.make_generate_function()
-        outputs = []
-        for batch in inputs:
-            token_ids, padding_mask = batch["token_ids"], batch["padding_mask"]
-            # If `preprocessor` is attached, we can stop after `end_token_id``.
-            end_token_id = None
-            if self.preprocessor is not None:
-                end_token_id = self.preprocessor.tokenizer.end_token_id
-            # Run the compiled generate function.
-            output = generate_function(token_ids, padding_mask, end_token_id)
-
-            if self.preprocessor is not None:
-                # Truncate to ragged by removing tokens after the first
-                # generated `end_token_id`.
-                output = truncate_at_token(output, end_token_id, padding_mask)
-                # Strip start token if added.
-                if self.preprocessor.add_start_token:
-                    output = output[:, 1:]
-                # Detokenize.
-                output = self.preprocessor.tokenizer.detokenize(output)
-            outputs.append(output)
-
-        outputs = tf.concat(outputs, axis=0)
-        outputs = tf.squeeze(outputs, 0) if input_is_scalar else outputs
-        # Convert outputs to a friendly pythonic type. For numerical outputs
-        # that is numpy, for string outputs that is `list` and `str`.
-        if outputs.dtype == tf.string:
-            return tensor_to_string_list(outputs)
-        return outputs.numpy()
+        outputs = [generate(x) for x in inputs]
+
+        if self.preprocessor is not None:
+            outputs = [postprocess(x) for x in outputs]
+
+        return self._normalize_generate_outputs(outputs, input_is_scalar)
 
     @classmethod
     def create_layout_map(cls, mesh):
         """Create a DTensor layout map for an OPTCausalLM.
 
         Given a DTensor mesh describing a list of devices, this method returns a
         DTensor layout map for creating a `keras_nlp.models.OPTCausalLM`
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_tokenizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,124 +8,117 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""OPT Causal LM preprocessor layer."""
+"""RoBERTa tokenizer."""
 
-from absl import logging
+import copy
 
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
-from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
+from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
+
+
+@keras_nlp_export("keras_nlp.models.RobertaTokenizer")
+class RobertaTokenizer(BytePairTokenizer):
+    """A RoBERTa tokenizer using Byte-Pair Encoding subword segmentation.
+
+    This tokenizer class will tokenize raw strings into integer sequences and
+    is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
+    underlying tokenizer, it will check for all special tokens needed by RoBERTa
+    models and provides a `from_preset()` method to automatically download
+    a matching vocabulary for a RoBERTa preset.
+
+    This tokenizer does not provide truncation or padding of inputs. It can be
+    combined with a `keras_nlp.models.RobertaPreprocessor` layer for input
+    packing.
 
+    If input is a batch of strings (rank > 0), the layer will output a
+    `tf.RaggedTensor` where the last dimension of the output is ragged.
 
-@keras_nlp_export("keras_nlp.models.OPTCausalLMPreprocessor")
-class OPTCausalLMPreprocessor(OPTPreprocessor):
-    """OPT Causal LM preprocessor.
-
-    This preprocessing layer is primarily meant to be used with
-    `keras_nlp.models.OPTCausalLM`. By default, it will take in batches of
-    strings, and return outputs in a `(x, y, sample_weight)` format, where the
-    `y` label is the next token id in the `x` sequence. For use with generation,
-    pass `return_labels=False` in which case the output will simply be the
-    encoded string features.
+    If input is a scalar string (rank == 0), the layer will output a dense
+    `tf.Tensor` with static shape `[None]`.
 
     Args:
-        tokenizer: A `keras_nlp.models.OPTTokenizer` instance.
-        sequence_length: The length of the packed inputs.
-        add_start_token: If true, the preprocessor will prepend the tokenizer
-            start token to each input sequence.
-        add_end_token: If true, the preprocessor will append the tokenizer
-            end token to each input sequence.
-
-    Call arguments:
-        x: A string, `tf.Tensor` or list of python strings.
-        y: Label data. Should always be `None` as the layer generates labels.
-        sample_weight: Label weights. Should always be `None` as the layer
-            generates label weights.
-        sequence_length: Pass to override the configured `sequence_length` of
-            the layer.
-        add_start_token: Pass to override the configured value of
-            `add_start_token` on the layer.
-        add_end_token: Pass to override the configured value of
-            `add_end_token` on the layer.
-        return_labels: If `True`, the output `"token_ids"` will be offset by one
-            and returned as labels. If `False` only features will be returned.
+        vocabulary: A dictionary mapping tokens to integer ids, or file path
+            to a json file containing the token to id mapping.
+        merges: A list of merge rules or a string file path, If passing a file
+            path. the file should have one merge rule per line. Every merge
+            rule contains merge entities separated by a space.
 
     Examples:
     ```python
-    # Load the preprocessor from a preset.
-    preprocessor = keras_nlp.models.OPTCausalLMPreprocessor.from_preset(
-        "opt_125m_en"
+    # Unbatched input.
+    tokenizer = keras_nlp.models.RobertaTokenizer.from_preset(
+        "roberta_base_en",
     )
+    tokenizer("The quick brown fox jumped.")
 
-    # Tokenize and pack a single sentence.
-    sentence = tf.constant("League of legends")
-    preprocessor(sentence)
-    # Same output.
-    preprocessor("League of legends")
-
-    # Tokenize a batch of sentences.
-    sentences = tf.constant(["Taco tuesday", "Fish taco please!"])
-    preprocessor(sentences)
-    # Same output.
-    preprocessor(["Taco tuesday", "Fish taco please!"])
-
-    # Map a dataset to preprocess a single sentence.
-    features = tf.constant(
-        [
-            "Avatar 2 is amazing!",
-            "Well, I am not sure.",
-        ]
+    # Batched input.
+    tokenizer(["The quick brown fox jumped.", "The fox slept."])
+
+    # Detokenization.
+    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+
+    # Custom vocabulary.
+    # Note: 'Ġ' is space
+    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
+    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
+    merges += ["Ġ f", "o x", "Ġf ox"]
+    tokenizer = keras_nlp.models.RobertaTokenizer(
+        vocabulary=vocab,
+        merges=merges
     )
-    labels = tf.constant([1, 0])
-    ds = tf.data.Dataset.from_tensor_slices((features, labels))
-    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
-
-    # Map a dataset to preprocess unlabled sentences.
-    ds = tf.data.Dataset.from_tensor_slices(features)
-    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+    tokenizer(["a quick fox", "a fox quick"])
+    ```
     """
 
-    def call(
+    def __init__(
         self,
-        x,
-        y=None,
-        sample_weight=None,
-        sequence_length=None,
-        add_start_token=None,
-        add_end_token=None,
-        return_labels=True,
+        vocabulary,
+        merges,
+        **kwargs,
     ):
-        if y is not None or sample_weight is not None:
-            logging.warning(
-                "`OPTCausalLMPreprocessor` generates `y` and `sample_weight` "
-                "based on your input data, but your data already contains `y` "
-                "or `sample_weight`. Your `y` and `sample_weight` will be "
-                "ignored."
-            )
-        if return_labels:
-            # Tokenize with one extra token to account for the truncation below.
-            sequence_length = (sequence_length or self.sequence_length) + 1
-        x = super().call(
-            x,
-            sequence_length=sequence_length,
-            add_start_token=add_start_token,
-            add_end_token=add_end_token,
+        # Special tokens.
+        start_token = "<s>"
+        pad_token = "<pad>"
+        end_token = "</s>"
+        mask_token = "<mask>"
+
+        super().__init__(
+            vocabulary=vocabulary,
+            merges=merges,
+            unsplittable_tokens=[start_token, pad_token, end_token, mask_token],
+            **kwargs,
         )
-        if return_labels:
-            token_ids, padding_mask = x["token_ids"], x["padding_mask"]
-            # The last token does not have a next token, so we truncate it out.
-            x = {
-                "token_ids": token_ids[..., :-1],
-                "padding_mask": padding_mask[..., :-1],
-            }
-            # Target `y` will be the next token.
-            y = token_ids[..., 1:]
-            sample_weight = padding_mask[..., 1:]
-            return pack_x_y_sample_weight(x, y, sample_weight)
-        else:
-            return x
+
+        # Check whether special tokens are present in the vocabulary.
+        for token in [start_token, pad_token, end_token, mask_token]:
+            if token not in self.get_vocabulary():
+                raise ValueError(
+                    f"Cannot find token `'{token}'` in the provided "
+                    f"`vocabulary`. Please provide `'{token}'` in your "
+                    "`vocabulary` or use a pretrained `vocabulary` name."
+                )
+
+        self.start_token_id = self.token_to_id(start_token)
+        self.pad_token_id = self.token_to_id(pad_token)
+        self.end_token_id = self.token_to_id(end_token)
+        self.mask_token_id = self.token_to_id(mask_token)
+
+    @classproperty
+    def presets(cls):
+        return copy.deepcopy(backbone_presets)
+
+    def get_config(self):
+        config = super().get_config()
+        # In the constructor, we pass the list of special tokens to the
+        # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
+        # delete it from the config here.
+        del config["unsplittable_tokens"]
+        return config
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,24 +105,27 @@
         ds = ds.map(self.preprocessor)
         x, y, sw = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
         self.assertAllEqual(y, [[3, 4, 5, 3, 6, 1, 0, 0]] * 4)
         self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
 
-    def test_call_overrides(self):
+    def test_generate_preprocess(self):
         input_data = " airplane at airport"
-        x, _, _ = self.preprocessor(input_data, add_start_token=False)
-        self.assertAllEqual(x["token_ids"], [3, 4, 5, 3, 6, 1, 0, 0])
-        x, _, _ = self.preprocessor(input_data, add_end_token=False)
+        x = self.preprocessor.generate_preprocess(input_data)
         self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 0, 0])
-        x, _, _ = self.preprocessor(input_data, sequence_length=4)
-        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5])
-        x = self.preprocessor(input_data, return_labels=False)
-        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 1, 0])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0])
+
+    def test_generate_postprocess(self):
+        input_data = {
+            "token_ids": tf.constant([1, 3, 4, 5, 3, 6, 0, 0]),
+            "padding_mask": tf.cast([1, 1, 1, 1, 1, 1, 0, 0], dtype="bool"),
+        }
+        x = self.preprocessor.generate_postprocess(input_data)
+        self.assertAllEqual(x, " airplane at airport")
 
     def test_serialization(self):
         config = keras.utils.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.utils.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,25 +100,32 @@
             loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
             jit_compile=False,
         )
         self.causal_lm.fit(self.preprocessed_dataset)
 
     def test_generate(self):
         # String input.
-        prompt = " airplane"
-        output = self.causal_lm.generate(" airplane")
+        prompt = " airplane at airport"
+        output = self.causal_lm.generate(" airplane at airport")
         self.assertTrue(prompt in output)
         # String tensor input.
         self.assertIsInstance(self.causal_lm.generate(self.raw_batch)[0], str)
         # String dataset input.
         self.assertIsInstance(self.causal_lm.generate(self.raw_dataset)[0], str)
         # Int tensor input.
         self.causal_lm.preprocessor = None
-        self.assertDTypeEqual(
-            self.causal_lm.generate(self.preprocessed_batch), tf.int32
+        outputs = self.causal_lm.generate(self.preprocessed_batch)
+        # Assert prompt is in output in token id space.
+        self.assertAllEqual(
+            outputs["token_ids"][:, :5],
+            self.preprocessed_batch["token_ids"][:, :5],
+        )
+        self.assertAllEqual(
+            outputs["padding_mask"][:, :5],
+            self.preprocessed_batch["padding_mask"][:, :5],
         )
 
     def test_generate_compilation(self):
         # Assert we do not recompile with successive calls.
         self.causal_lm.generate(self.raw_batch)
         first_fn = self.causal_lm.generate_function
         self.causal_lm.generate(self.raw_batch)
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_preprocessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,18 +64,14 @@
 
     Call arguments:
         x: A string, `tf.Tensor` or list of python strings.
         y: Any label data. Will be passed through unaltered.
         sample_weight: Any label weight data. Will be passed through unaltered.
         sequence_length: Pass to override the configured `sequence_length` of
             the layer.
-        add_start_token: Pass to override the configure value of
-            `add_start_token` on the layer.
-        add_end_token: Pass to override the configure value of
-            `add_end_token` on the layer.
 
     Examples:
 
     Directly calling the layer on data.
     ```python
     preprocessor = keras_nlp.models.OPTPreprocessor.from_preset("opt_125m_en")
 
@@ -150,36 +146,29 @@
 
     def call(
         self,
         x,
         y=None,
         sample_weight=None,
         sequence_length=None,
-        add_start_token=None,
-        add_end_token=None,
     ):
         x = convert_inputs_to_list_of_tensor_segments(x)
         if len(x) != 1:
             raise ValueError(
                 "OPT requires each input feature to contain only "
                 f"one segment, but received {len(x)}. If you are using OPT "
                 "for a multi-segment classification task, please refer to "
                 "classification models like BERT or RoBERTa."
             )
-        if sequence_length is None:
-            sequence_length = self.sequence_length
-        if add_start_token is None:
-            add_start_token = self.add_start_token
-        if add_end_token is None:
-            add_end_token = self.add_end_token
+        sequence_length = sequence_length or self.sequence_length
         token_ids, padding_mask = self.packer(
             self.tokenizer(x[0]),
             sequence_length=sequence_length,
-            add_start_value=add_start_token,
-            add_end_value=add_end_token,
+            add_start_value=self.add_start_token,
+            add_end_value=self.add_end_token,
         )
         x = {
             "token_ids": token_ids,
             "padding_mask": padding_mask,
         }
         return pack_x_y_sample_weight(x, y, sample_weight)
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_preprocessor_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,20 +95,16 @@
         x = tf.constant([" airplane at airport"] * 4)
         ds = tf.data.Dataset.from_tensor_slices(x)
         ds = ds.map(self.preprocessor)
         x = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
 
-    def test_call_overrides(self):
+    def test_sequence_length_override(self):
         input_data = " airplane at airport"
-        x = self.preprocessor(input_data, add_start_token=False)
-        self.assertAllEqual(x["token_ids"], [3, 4, 5, 3, 6, 1, 0, 0])
-        x = self.preprocessor(input_data, add_end_token=False)
-        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 0, 0])
         x = self.preprocessor(input_data, sequence_length=4)
         self.assertAllEqual(x["token_ids"], [1, 3, 4, 1])
 
     def test_serialization(self):
         config = keras.utils.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.utils.deserialize_keras_object(config)
         self.assertEqual(
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_classifier.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_classifier_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,117 +8,155 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""RoBERTa tokenizer."""
+"""XLM-RoBERTa tokenizer."""
 
 import copy
 
+import tensorflow as tf
+
 from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
 from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.tf_utils import tensor_to_string_list
 
 
-@keras_nlp_export("keras_nlp.models.RobertaTokenizer")
-class RobertaTokenizer(BytePairTokenizer):
-    """A RoBERTa tokenizer using Byte-Pair Encoding subword segmentation.
+@keras_nlp_export("keras_nlp.models.XLMRobertaTokenizer")
+class XLMRobertaTokenizer(SentencePieceTokenizer):
+    """An XLM-RoBERTa tokenizer using SentencePiece subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
-    is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
-    underlying tokenizer, it will check for all special tokens needed by RoBERTa
-    models and provides a `from_preset()` method to automatically download
-    a matching vocabulary for a RoBERTa preset.
-
-    This tokenizer does not provide truncation or padding of inputs. It can be
-    combined with a `keras_nlp.models.RobertaPreprocessor` layer for input
-    packing.
+    is based on `keras_nlp.tokenizers.SentencePieceTokenizer`. Unlike the
+    underlying tokenizer, it will check for all special tokens needed by
+    XLM-RoBERTa models and provides a `from_preset()` method to automatically
+    download a matching vocabulary for an XLM-RoBERTa preset.
+
+    Note: If you are providing your own custom SentencePiece model, the original
+    fairseq implementation of XLM-RoBERTa re-maps some token indices from the
+    underlying sentencepiece output. To preserve compatibility, we do the same
+    re-mapping here.
 
     If input is a batch of strings (rank > 0), the layer will output a
     `tf.RaggedTensor` where the last dimension of the output is ragged.
 
     If input is a scalar string (rank == 0), the layer will output a dense
     `tf.Tensor` with static shape `[None]`.
 
     Args:
-        vocabulary: A dictionary mapping tokens to integer ids, or file path
-            to a json file containing the token to id mapping.
-        merges: A list of merge rules or a string file path, If passing a file
-            path. the file should have one merge rule per line. Every merge
-            rule contains merge entities separated by a space.
+        proto: Either a `string` path to a SentencePiece proto file or a
+            `bytes` object with a serialized SentencePiece proto. See the
+            [SentencePiece repository](https://github.com/google/sentencepiece)
+            for more details on the format.
 
     Examples:
     ```python
-    # Unbatched input.
-    tokenizer = keras_nlp.models.RobertaTokenizer.from_preset(
-        "roberta_base_en",
+    tokenizer = keras_nlp.models.XLMRobertaTokenizer.from_preset(
+        "xlm_roberta_base_multi",
     )
-    tokenizer("The quick brown fox jumped.")
 
-    # Batched input.
-    tokenizer(["The quick brown fox jumped.", "The fox slept."])
+    # Unbatched inputs.
+    tokenizer("the quick brown fox")
+
+    # Batched inputs.
+    tokenizer(["the quick brown fox", "الأرض كروية"])
 
     # Detokenization.
-    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+    tokenizer.detokenize(tokenizer("the quick brown fox"))
 
-    # Custom vocabulary.
-    # Note: 'Ġ' is space
-    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
-    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
-    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
-    merges += ["Ġ f", "o x", "Ġf ox"]
-    tokenizer = keras_nlp.models.RobertaTokenizer(
-        vocabulary=vocab,
-        merges=merges
+    # Custom vocabulary
+    def train_sentencepiece(ds, vocab_size):
+        bytes_io = io.BytesIO()
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=ds.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=vocab_size,
+            model_type="WORD",
+            unk_id=0,
+            bos_id=1,
+            eos_id=2,
+        )
+        return bytes_io.getvalue()
+
+    ds = tf.data.Dataset.from_tensor_slices(
+        ["the quick brown fox", "the earth is round"]
     )
-    tokenizer(["a quick fox", "a fox quick"])
+    proto = train_sentencepiece(ds, vocab_size=10)
+    tokenizer = keras_nlp.models.XLMRobertaTokenizer(proto=proto)
     ```
     """
 
-    def __init__(
-        self,
-        vocabulary,
-        merges,
-        **kwargs,
-    ):
-        # Special tokens.
-        start_token = "<s>"
-        pad_token = "<pad>"
-        end_token = "</s>"
-        mask_token = "<mask>"
-
-        super().__init__(
-            vocabulary=vocabulary,
-            merges=merges,
-            unsplittable_tokens=[start_token, pad_token, end_token, mask_token],
-            **kwargs,
+    def __init__(self, proto, **kwargs):
+        super().__init__(proto=proto, **kwargs)
+
+        # List of special tokens.
+        self._vocabulary_prefix = ["<s>", "<pad>", "</s>", "<unk>"]
+
+        # IDs of special tokens.
+        self.start_token_id = 0  # <s>
+        self.pad_token_id = 1  # <pad>
+        self.end_token_id = 2  # </s>
+        self.unk_token_id = 3  # <unk>
+        self.mask_token_id = self.vocabulary_size() - 1  # <mask>
+
+    def vocabulary_size(self):
+        """Get the size of the tokenizer vocabulary."""
+        return super().vocabulary_size() + 2
+
+    def get_vocabulary(self):
+        """Get the size of the tokenizer vocabulary."""
+        vocabulary = tensor_to_string_list(
+            self._sentence_piece.id_to_string(
+                tf.range(super().vocabulary_size())
+            )
         )
+        return self._vocabulary_prefix + vocabulary[3:] + ["<mask>"]
+
+    def id_to_token(self, id):
+        """Convert an integer id to a string token."""
+
+        if id == self.mask_token_id:
+            return "<mask>"
+
+        if id < len(self._vocabulary_prefix):
+            return self._vocabulary_prefix[id]
+
+        return tensor_to_string_list(self._sentence_piece.id_to_string(id - 1))
 
-        # Check whether special tokens are present in the vocabulary.
-        for token in [start_token, pad_token, end_token, mask_token]:
-            if token not in self.get_vocabulary():
-                raise ValueError(
-                    f"Cannot find token `'{token}'` in the provided "
-                    f"`vocabulary`. Please provide `'{token}'` in your "
-                    "`vocabulary` or use a pretrained `vocabulary` name."
-                )
-
-        self.start_token_id = self.token_to_id(start_token)
-        self.pad_token_id = self.token_to_id(pad_token)
-        self.end_token_id = self.token_to_id(end_token)
-        self.mask_token_id = self.token_to_id(mask_token)
+    def token_to_id(self, token):
+        """Convert a string token to an integer id."""
+
+        if token in self._vocabulary_prefix:
+            return self._vocabulary_prefix.index(token)
+
+        spm_token_id = self._sentence_piece.string_to_id(token)
+
+        # OOV token
+        spm_unk_token_id = self._sentence_piece.string_to_id("<unk>")
+        if spm_token_id == spm_unk_token_id:
+            return self.unk_token_id
+
+        return int(spm_token_id.numpy()) + 1
+
+    def tokenize(self, inputs):
+        tokens = super().tokenize(inputs)
+
+        # Correct `unk_token_id` (0 -> 3). Note that we do not correct
+        # `start_token_id` and `end_token_id`; they are dealt with in
+        # `XLMRobertaPreprocessor`.
+        tokens = tf.where(tf.equal(tokens, 0), self.unk_token_id - 1, tokens)
+
+        # Shift the tokens IDs right by one.
+        return tf.add(tokens, 1)
+
+    def detokenize(self, ids):
+        ids = tf.ragged.boolean_mask(ids, tf.not_equal(ids, self.mask_token_id))
+        return super().detokenize(ids)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
 
-    def get_config(self):
-        config = super().get_config()
-        # In the constructor, we pass the list of special tokens to the
-        # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
-        # delete it from the config here.
-        del config["unsplittable_tokens"]
-        return config
-
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_layer_norm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_layer_norm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_multi_head_attention.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_transformer_layer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_transformer_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/task.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/task.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/task_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/task_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_decoder.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_encoder.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,156 +7,135 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""XLM-RoBERTa tokenizer."""
-
-import copy
+"""Trainer for SentencePiece Tokenizer."""
+import io
 
 import tensorflow as tf
 
-from keras_nlp.src.api_export import keras_nlp_export
-from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.src.utils.python_utils import classproperty
-from keras_nlp.src.utils.tf_utils import tensor_to_string_list
-
-
-@keras_nlp_export("keras_nlp.models.XLMRobertaTokenizer")
-class XLMRobertaTokenizer(SentencePieceTokenizer):
-    """An XLM-RoBERTa tokenizer using SentencePiece subword segmentation.
-
-    This tokenizer class will tokenize raw strings into integer sequences and
-    is based on `keras_nlp.tokenizers.SentencePieceTokenizer`. Unlike the
-    underlying tokenizer, it will check for all special tokens needed by
-    XLM-RoBERTa models and provides a `from_preset()` method to automatically
-    download a matching vocabulary for an XLM-RoBERTa preset.
-
-    Note: If you are providing your own custom SentencePiece model, the original
-    fairseq implementation of XLM-RoBERTa re-maps some token indices from the
-    underlying sentencepiece output. To preserve compatibility, we do the same
-    re-mapping here.
+try:
+    import sentencepiece as spm
+except ImportError:
+    spm = None
+
+
+def compute_sentence_piece_proto(
+    data,
+    vocabulary_size,
+    model_type="unigram",
+    proto_output_file=None,
+    lowercase=False,
+):
+    r"""A utility to train a SentencePiece vocabulary.
 
-    If input is a batch of strings (rank > 0), the layer will output a
-    `tf.RaggedTensor` where the last dimension of the output is ragged.
+    Trains a SentencePiece vocabulary from an input dataset or a list of
+    filenames.
 
-    If input is a scalar string (rank == 0), the layer will output a dense
-    `tf.Tensor` with static shape `[None]`.
+    If `data` is a list of filenames, the file format is required to be plain
+    text files, and the text will be read in line by line during training.
 
     Args:
-        proto: Either a `string` path to a SentencePiece proto file or a
-            `bytes` object with a serialized SentencePiece proto. See the
-            [SentencePiece repository](https://github.com/google/sentencepiece)
-            for more details on the format.
+        data: A `tf.data.Dataset`, or a list of filenames.
+        vocabulary_size: int. The maximum size of a vocabulary to be trained.
+        model_type: str, defaults to `"unigram"`. The model algorithm must be one
+            of `"unigram"`, `"bpe"`, `"word"` or `"char"`.
+        proto_output_file: str, defaults to `None`. If provided it will be used
+            as model_file which is passed to model_writer.
+            If `None`, the model_file will be `io.BytesIO` object.
+        lowercase: bool, defaults to `False`. If true, the input text will be
+            lowercased before tokenization.
+
+    Returns:
+        A `bytes` object with a serialized SentencePiece proto or
+        `None` if proto_output_file if provided.
 
     Examples:
-    ```python
-    tokenizer = keras_nlp.models.XLMRobertaTokenizer.from_preset(
-        "xlm_roberta_base_multi",
-    )
-
-    # Unbatched inputs.
-    tokenizer("the quick brown fox")
-
-    # Batched inputs.
-    tokenizer(["the quick brown fox", "الأرض كروية"])
-
-    # Detokenization.
-    tokenizer.detokenize(tokenizer("the quick brown fox"))
-
-    # Custom vocabulary
-    def train_sentencepiece(ds, vocab_size):
-        bytes_io = io.BytesIO()
-        sentencepiece.SentencePieceTrainer.train(
-            sentence_iterator=ds.as_numpy_iterator(),
-            model_writer=bytes_io,
-            vocab_size=vocab_size,
-            model_type="WORD",
-            unk_id=0,
-            bos_id=1,
-            eos_id=2,
-        )
-        return bytes_io.getvalue()
 
-    ds = tf.data.Dataset.from_tensor_slices(
-        ["the quick brown fox", "the earth is round"]
-    )
-    proto = train_sentencepiece(ds, vocab_size=10)
-    tokenizer = keras_nlp.models.XLMRobertaTokenizer(proto=proto)
+    Basic Usage (from Dataset).
+    >>> inputs = tf.data.Dataset.from_tensor_slices(["Drifting Along"])
+    >>> proto = keras_nlp.tokenizers.compute_sentence_piece_proto(inputs, vocabulary_size=15)
+    >>> tokenizer = keras_nlp.tokenizers.SentencePieceTokenizer(proto=proto)
+    >>> outputs = inputs.map(tokenizer)
+    >>> for output in outputs:
+    ...     print(output)
+    tf.Tensor([ 4  8 12  5  9 14  5  6 13  4  7 10 11  6 13],
+    shape=(15,), dtype=int32)
+
+    Basic Usage (with files).
+    ``` python
+    with open("test.txt", "w+") as f: f.write("Drifting Along\n")
+    inputs = ["test.txt"]
+    proto = keras_nlp.tokenizers.compute_sentence_piece_proto(
+         inputs, vocabulary_size=15, proto_output_file="model.spm")
+    tokenizer = keras_nlp.tokenizers.SentencePieceTokenizer(proto="model.spm")
+    ds = tf.data.Dataset.from_tensor_slices(["the quick brown fox."])
+    ds = ds.map(tokenizer)
     ```
-    """
-
-    def __init__(self, proto, **kwargs):
-        super().__init__(proto=proto, **kwargs)
 
-        # List of special tokens.
-        self._vocabulary_prefix = ["<s>", "<pad>", "</s>", "<unk>"]
+    Usage with lowercase
+    >>> inputs = tf.data.Dataset.from_tensor_slices(["Drifting Along"])
+    >>> proto = keras_nlp.tokenizers.compute_sentence_piece_proto(
+    ...     inputs, vocabulary_size=15, lowercase=True)
+    >>> tokenizer = keras_nlp.tokenizers.SentencePieceTokenizer(proto=proto)
+    >>> outputs = inputs.map(tokenizer)
+    >>> for output in outputs:
+    ...     print(output)
+    tf.Tensor([ 4  8 12  5  9 14  5  6 13  4  7 10 11  6 13],
+    shape=(15,), dtype=int32)
+    """
 
-        # IDs of special tokens.
-        self.start_token_id = 0  # <s>
-        self.pad_token_id = 1  # <pad>
-        self.end_token_id = 2  # </s>
-        self.unk_token_id = 3  # <unk>
-        self.mask_token_id = self.vocabulary_size() - 1  # <mask>
-
-    def vocabulary_size(self):
-        """Get the size of the tokenizer vocabulary."""
-        return super().vocabulary_size() + 2
-
-    def get_vocabulary(self):
-        """Get the size of the tokenizer vocabulary."""
-        vocabulary = tensor_to_string_list(
-            self._sentence_piece.id_to_string(
-                tf.range(super().vocabulary_size())
-            )
+    if spm is None:
+        raise ImportError(
+            f"{compute_sentence_piece_proto.__name__} requires the "
+            "`sentencepiece` package. Please install it with "
+            "`pip install sentencepiece`."
         )
-        return self._vocabulary_prefix + vocabulary[3:] + ["<mask>"]
-
-    def id_to_token(self, id):
-        """Convert an integer id to a string token."""
-
-        if id == self.mask_token_id:
-            return "<mask>"
 
-        if id < len(self._vocabulary_prefix):
-            return self._vocabulary_prefix[id]
-
-        return tensor_to_string_list(self._sentence_piece.id_to_string(id - 1))
-
-    def token_to_id(self, token):
-        """Convert a string token to an integer id."""
-
-        if token in self._vocabulary_prefix:
-            return self._vocabulary_prefix.index(token)
-
-        spm_token_id = self._sentence_piece.string_to_id(token)
-
-        # OOV token
-        spm_unk_token_id = self._sentence_piece.string_to_id("<unk>")
-        if spm_token_id == spm_unk_token_id:
-            return self.unk_token_id
-
-        return int(spm_token_id.numpy()) + 1
-
-    def tokenize(self, inputs):
-        tokens = super().tokenize(inputs)
-
-        # Correct `unk_token_id` (0 -> 3). Note that we do not correct
-        # `start_token_id` and `end_token_id`; they are dealt with in
-        # `XLMRobertaPreprocessor`.
-        tokens = tf.where(tf.equal(tokens, 0), self.unk_token_id - 1, tokens)
-
-        # Shift the tokens IDs right by one.
-        return tf.add(tokens, 1)
+    if not isinstance(data, (list, tuple, tf.data.Dataset)):
+        raise ValueError(
+            "The `data` argument must be either `tf.data.Dataset` or `tuple` or `list`. "
+            f"Received: type(data)={type(data)}."
+        )
 
-    def detokenize(self, ids):
-        ids = tf.ragged.boolean_mask(ids, tf.not_equal(ids, self.mask_token_id))
-        return super().detokenize(ids)
+    if model_type not in ["unigram", "bpe", "word", "char"]:
+        raise ValueError(
+            "The `model_type` argument must be one of `unigram`, `bpe`, `word`"
+            f"or `char`. Received: model_type={model_type}."
+        )
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
+    model_writer = (
+        open(proto_output_file, "wb") if proto_output_file else io.BytesIO()
+    )
+    is_dataset = isinstance(data, tf.data.Dataset)
+    if is_dataset:
+        spm.SentencePieceTrainer.train(
+            sentence_iterator=data.as_numpy_iterator(),
+            model_writer=model_writer,
+            vocab_size=vocabulary_size,
+            model_type=model_type,
+            normalization_rule_name="nmt_nfkc_cf" if lowercase else "nmt_nfkc",
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
+        )
+    else:
+        spm.SentencePieceTrainer.train(
+            input=data,
+            model_writer=model_writer,
+            vocab_size=vocabulary_size,
+            model_type=model_type,
+            normalization_rule_name="nmt_nfkc_cf" if lowercase else "nmt_nfkc",
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
+        )
+    if proto_output_file:
+        model_writer.close()
+    else:
+        return model_writer.getvalue()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/beam_sampler.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/beam_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/beam_sampler_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/beam_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/contrastive_sampler.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/contrastive_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/contrastive_sampler_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/contrastive_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/greedy_sampler.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/greedy_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/greedy_sampler_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/greedy_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/random_sampler.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/random_sampler_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/random_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/sampler.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/serialization.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/serialization_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/serialization_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_k_sampler.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_k_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_k_sampler_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_k_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_p_sampler.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_p_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_p_sampler_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_p_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/docstring_lib.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/docstring_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/docstring_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/docstring_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,23 +39,31 @@
     for name, module in sys.modules.items():
         if name.startswith(PACKAGE):
             keras_nlp_modules.append(module)
 
     return keras_nlp_modules
 
 
-def test_docstrings():
+@pytest.fixture(scope="session")
+def docstring_module(pytestconfig):
+    return pytestconfig.getoption("docstring_module")
+
+
+def test_docstrings(docstring_module):
     keras_nlp_modules = find_modules()
     # As of this writing, it doesn't seem like pytest support load_tests
     # protocol for unittest:
     #     https://docs.pytest.org/en/7.1.x/how-to/unittest.html
     # So we run the unittest.TestSuite manually and report the results back.
     runner = unittest.TextTestRunner()
     suite = unittest.TestSuite()
     for module in keras_nlp_modules:
+        if docstring_module and docstring_module not in module.__name__:
+            continue
+        print(f"Adding tests for docstrings in {module.__name__}")
         suite.addTest(
             doctest.DocTestSuite(
                 module,
                 test_finder=doctest.DocTestFinder(exclude_empty=False),
                 extraglobs={
                     "tf": tf,
                     "np": np,
@@ -79,25 +87,32 @@
 
 
 @pytest.mark.extra_large
 @pytest.mark.skipif(
     astor is None,
     reason="This test requires `astor`. Please `pip install astor` to run.",
 )
-def test_fenced_docstrings():
+def test_fenced_docstrings(docstring_module):
     """Tests fenced code blocks in docstrings.
 
-    This can only be run manually. Run with:
+    This can only be run manually and will take many minutes. Run with:
     `pytest keras_nlp/tests/doc_tests/docstring_test.py --run_extra_large`
+
+    To restrict the docstring you test, you can pass an additional
+    --docstring_module flag. For example, to run only "bert" module tests:
+    `pytest keras_nlp/tests/doc_tests/docstring_test.py --run_extra_large --docstring_module "models.bert"`
     """
     keras_nlp_modules = find_modules()
 
     runner = unittest.TextTestRunner()
     suite = unittest.TestSuite()
     for module in keras_nlp_modules:
+        if docstring_module and docstring_module not in module.__name__:
+            continue
+        print(f"Adding tests for fenced docstrings in {module.__name__}")
         suite.addTest(
             doctest.DocTestSuite(
                 module,
                 test_finder=doctest.DocTestFinder(
                     exclude_empty=False,
                     parser=fenced_docstring_lib.FencedCellParser(
                         fence_label="python"
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_pair_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_pair_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/keras_utils.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/keras_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/keras_utils_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/keras_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/pipeline_model.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/pipeline_model.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/pipeline_model_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/pipeline_model_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/python_utils.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/python_utils_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/python_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/tf_utils.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/tf_utils_test.py` & `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/tf_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp/tokenizers/__init__.py` & `keras-nlp-0.5.0.dev5/keras_nlp/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp.egg-info/PKG-INFO` & `keras-nlp-0.5.0.dev5/keras_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.5.0.dev4
+Version: 0.5.0.dev5
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nlp-0.5.0.dev4/keras_nlp.egg-info/SOURCES.txt` & `keras-nlp-0.5.0.dev5/keras_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/setup.cfg` & `keras-nlp-0.5.0.dev5/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev4/setup.py` & `keras-nlp-0.5.0.dev5/setup.py`

 * *Files identical despite different names*

