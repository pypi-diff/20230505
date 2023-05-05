# Comparing `tmp/keras-nlp-0.5.0.dev5.tar.gz` & `tmp/keras-nlp-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nlp-0.5.0.dev5.tar", last modified: Fri May  5 19:41:39 2023, max compression
+gzip compressed data, was "keras-nlp-0.5.1.tar", last modified: Fri May  5 21:57:48 2023, max compression
```

## Comparing `keras-nlp-0.5.0.dev5.tar` & `keras-nlp-0.5.1.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.359506 keras-nlp-0.5.0.dev5/keras_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.363506 keras-nlp-0.5.0.dev5/keras_nlp/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/api_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.367507 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/cached_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/cached_multi_head_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/f_net_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/f_net_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_mask_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/multi_segment_packer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_deletion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_swap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/sine_position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/sine_position_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/start_end_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/start_end_packer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/token_and_position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/token_and_position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14352 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_decoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_layer_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.367507 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/bleu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/edit_distance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/perplexity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_l_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_n_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.367507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.371507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.371507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.375507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.375507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/relative_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.379507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.379507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.383507 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.387508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.391508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.391508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_transformer_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/task_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.391508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.391508 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.395508 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/beam_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/beam_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/contrastive_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/contrastive_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/greedy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/greedy_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/random_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_k_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_k_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_p_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_p_sampler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.395508 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.395508 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/docstring_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/docstring_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24894 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_pair_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/keras_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/keras_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/pipeline_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/keras_nlp/src/utils/tf_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/keras_nlp/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-05 19:41:32.000000 keras-nlp-0.5.0.dev5/keras_nlp/tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:41:39.359506 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 19:41:39.000000 keras-nlp-0.5.0.dev5/keras_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-05 19:41:39.399508 keras-nlp-0.5.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-05 19:41:28.000000 keras-nlp-0.5.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.807576 keras-nlp-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-05 21:57:48.811576 keras-nlp-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.771575 keras-nlp-0.5.1/keras_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-05 21:57:43.000000 keras-nlp-0.5.1/keras_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.771575 keras-nlp-0.5.1/keras_nlp/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-05 21:57:43.000000 keras-nlp-0.5.1/keras_nlp/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.771575 keras-nlp-0.5.1/keras_nlp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 21:57:43.000000 keras-nlp-0.5.1/keras_nlp/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.771575 keras-nlp-0.5.1/keras_nlp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-05 21:57:43.000000 keras-nlp-0.5.1/keras_nlp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.771575 keras-nlp-0.5.1/keras_nlp/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-05 21:57:43.000000 keras-nlp-0.5.1/keras_nlp/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.771575 keras-nlp-0.5.1/keras_nlp/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/api_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.779575 keras-nlp-0.5.1/keras_nlp/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/cached_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/cached_multi_head_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/f_net_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/f_net_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/masked_lm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/masked_lm_head_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/masked_lm_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/masked_lm_mask_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/multi_segment_packer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/random_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/random_deletion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/random_swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/random_swap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/sine_position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/sine_position_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/start_end_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/start_end_packer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/token_and_position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/token_and_position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/transformer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14352 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/transformer_decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/transformer_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/transformer_layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/layers/transformer_layer_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.783575 keras-nlp-0.5.1/keras_nlp/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/bleu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/edit_distance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/perplexity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_l_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_n_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.783575 keras-nlp-0.5.1/keras_nlp/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.787576 keras-nlp-0.5.1/keras_nlp/src/models/albert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.787576 keras-nlp-0.5.1/keras_nlp/src/models/bart/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.791576 keras-nlp-0.5.1/keras_nlp/src/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.791576 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/relative_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.795576 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.795576 keras-nlp-0.5.1/keras_nlp/src/models/f_net/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.795576 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.799576 keras-nlp-0.5.1/keras_nlp/src/models/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.799576 keras-nlp-0.5.1/keras_nlp/src/models/roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.803576 keras-nlp-0.5.1/keras_nlp/src/models/t5/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/t5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_transformer_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/task_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.803576 keras-nlp-0.5.1/keras_nlp/src/models/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/whisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/whisper/whisper_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/whisper/whisper_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/whisper/whisper_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/whisper/whisper_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.803576 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.807576 keras-nlp-0.5.1/keras_nlp/src/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/beam_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/beam_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/contrastive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/contrastive_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/greedy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/greedy_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/random_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/top_k_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/top_k_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/top_p_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/samplers/top_p_sampler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.807576 keras-nlp-0.5.1/keras_nlp/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.807576 keras-nlp-0.5.1/keras_nlp/src/tests/doc_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tests/doc_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tests/doc_tests/docstring_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tests/doc_tests/docstring_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.807576 keras-nlp-0.5.1/keras_nlp/src/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24894 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/byte_pair_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/byte_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/byte_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/word_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.807576 keras-nlp-0.5.1/keras_nlp/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/utils/keras_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/utils/keras_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/utils/pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/utils/pipeline_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/keras_nlp/src/utils/tf_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.807576 keras-nlp-0.5.1/keras_nlp/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-05 21:57:43.000000 keras-nlp-0.5.1/keras_nlp/tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:57:48.771575 keras-nlp-0.5.1/keras_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-05 21:57:48.000000 keras-nlp-0.5.1/keras_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-05 21:57:48.000000 keras-nlp-0.5.1/keras_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:57:48.000000 keras-nlp-0.5.1/keras_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-05 21:57:48.000000 keras-nlp-0.5.1/keras_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 21:57:48.000000 keras-nlp-0.5.1/keras_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-05 21:57:48.811576 keras-nlp-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-05 21:57:40.000000 keras-nlp-0.5.1/setup.py
```

### Comparing `keras-nlp-0.5.0.dev5/PKG-INFO` & `keras-nlp-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.5.0.dev5
+Version: 0.5.1
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nlp-0.5.0.dev5/README.md` & `keras-nlp-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/layers/__init__.py` & `keras-nlp-0.5.1/keras_nlp/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/models/__init__.py` & `keras-nlp-0.5.1/keras_nlp/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm import DebertaV3MaskedLM
 from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import DebertaV3MaskedLMPreprocessor
 from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import DebertaV3Preprocessor
 from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 from keras_nlp.src.models.distil_bert.distil_bert_classifier import DistilBertClassifier
 from keras_nlp.src.models.distil_bert.distil_bert_masked_lm import DistilBertMaskedLM
-from keras_nlp.src.models.distil_bert.distil_bert_masked_lm_preprocessor import DistilBertMaskedLMPreprocessor as DistilBertMaskedLMPrerprocessor
+from keras_nlp.src.models.distil_bert.distil_bert_masked_lm_preprocessor import DistilBertMaskedLMPreprocessor
 from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import DistilBertPreprocessor
 from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import DistilBertTokenizer
 from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
 from keras_nlp.src.models.f_net.f_net_classifier import FNetClassifier
 from keras_nlp.src.models.f_net.f_net_masked_lm import FNetMaskedLM
 from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import FNetMaskedLMPreprocessor
 from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
@@ -41,15 +41,15 @@
 from keras_nlp.src.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
 from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
 from keras_nlp.src.models.opt.opt_causal_lm import OPTCausalLM
 from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import OPTCausalLMPreprocessor
 from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
 from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
-from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone as RobertBackbone
+from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.src.models.roberta.roberta_classifier import RobertaClassifier
 from keras_nlp.src.models.roberta.roberta_masked_lm import RobertaMaskedLM
 from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import RobertaMaskedLMPreprocessor
 from keras_nlp.src.models.roberta.roberta_multi_segment_packer import RobertaMultiSegmentPacker
 from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
 from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
```

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/samplers/__init__.py` & `keras-nlp-0.5.1/keras_nlp/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 from keras_nlp.src import metrics
 from keras_nlp.src import models
 from keras_nlp.src import samplers
 from keras_nlp.src import tokenizers
 from keras_nlp.src import utils
 
 # This is the global source of truth for the version number.
-__version__ = "0.5.0.dev5"
+__version__ = "0.5.1"
```

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/api_export.py` & `keras-nlp-0.5.1/keras_nlp/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/conftest.py` & `keras-nlp-0.5.1/keras_nlp/src/conftest.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/cached_multi_head_attention.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/cached_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/cached_multi_head_attention_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/cached_multi_head_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/f_net_encoder.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/f_net_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/f_net_encoder_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/f_net_encoder_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_head.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/masked_lm_head.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_head_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/masked_lm_head_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_mask_generator.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/masked_lm_mask_generator.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/masked_lm_mask_generator_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/masked_lm_mask_generator_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/multi_segment_packer.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/multi_segment_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/multi_segment_packer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/multi_segment_packer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/position_embedding.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/position_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/position_embedding_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/position_embedding_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_deletion.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/random_deletion.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_deletion_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/random_deletion_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_swap.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/random_swap.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/random_swap_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/random_swap_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/sine_position_encoding.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/sine_position_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/sine_position_encoding_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/sine_position_encoding_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/start_end_packer.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/start_end_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/start_end_packer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/start_end_packer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/token_and_position_embedding.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/token_and_position_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/token_and_position_embedding_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/token_and_position_embedding_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_decoder.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_decoder_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/transformer_decoder_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_encoder.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_encoder_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/transformer_encoder_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_layer_utils.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/transformer_layer_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/layers/transformer_layer_utils_test.py` & `keras-nlp-0.5.1/keras_nlp/src/layers/transformer_layer_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/bleu.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/bleu_test.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/bleu_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/edit_distance.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/edit_distance.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/edit_distance_test.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/edit_distance_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/perplexity.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/perplexity.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/perplexity_test.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/perplexity_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_base.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_base.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_l.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_l.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_l_test.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_l_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_n.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_n.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """ROUGE-N metric."""
 
 from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.metrics.rouge_base import RougeBase
 
 
-@keras_nlp_export("keras_nlp.metrics.RogueN")
+@keras_nlp_export("keras_nlp.metrics.RougeN")
 class RougeN(RougeBase):
     """ROUGE-N metric.
 
     This class implements the ROUGE-N variant of the ROUGE metric. The ROUGE-N
     metric is traditionally used for evaluating summarisation systems.
     Succinctly put, ROUGE-N is a score based on the number of matching n-grams
     between the reference text and the hypothesis text.
```

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/metrics/rouge_n_test.py` & `keras-nlp-0.5.1/keras_nlp/src/metrics/rouge_n_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_classifier.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_classifier_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_masked_lm_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/albert/albert_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/albert/albert_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bart/bart_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bart/bart_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_classifier.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_classifier_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_masked_lm_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/bert/bert_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/bert/bert_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/deberta_v3/relative_embedding.py` & `keras-nlp-0.5.1/keras_nlp/src/models/deberta_v3/relative_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_classifier.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from keras_nlp.src.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
 from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
 from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
-@keras_nlp_export("keras_nlp.models.DistilBertMaskedLMPrerprocessor")
+@keras_nlp_export("keras_nlp.models.DistilBertMaskedLMPreprocessor")
 class DistilBertMaskedLMPreprocessor(DistilBertPreprocessor):
     """DistilBERT preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
     task. It is primarily intended for use with the
     `keras_nlp.models.DistilBertMaskedLM` task model. Preprocessing will occur in
     multiple steps.
```

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_classifier.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_classifier_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_masked_lm_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/f_net/f_net_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/f_net/f_net_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_causal_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_causal_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_causal_lm_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_causal_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/opt/opt_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/opt/opt_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from keras_nlp.src.utils.python_utils import classproperty
 
 
 def roberta_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras_nlp_export("keras_nlp.models.RobertBackbone")
+@keras_nlp_export("keras_nlp.models.RobertaBackbone")
 class RobertaBackbone(Backbone):
     """A RoBERTa encoder network.
 
     This network implements a bi-directional Transformer-based encoder as
     described in ["RoBERTa: A Robustly Optimized BERT Pretraining Approach"](https://arxiv.org/abs/1907.11692).
     It includes the embedding lookups and transformer layers, but does not
     include the masked language model head used during pretraining.
```

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_classifier.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_classifier_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_masked_lm_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/roberta/roberta_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/roberta/roberta_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_layer_norm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_layer_norm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_multi_head_attention.py` & `keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/t5/t5_transformer_layer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/t5/t5_transformer_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/task.py` & `keras-nlp-0.5.1/keras_nlp/src/models/task.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/task_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/task_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/whisper/whisper_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/whisper/whisper_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_decoder.py` & `keras-nlp-0.5.1/keras_nlp/src/models/whisper/whisper_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/whisper/whisper_encoder.py` & `keras-nlp-0.5.1/keras_nlp/src/models/whisper/whisper_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/beam_sampler.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/beam_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/beam_sampler_test.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/beam_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/contrastive_sampler.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/contrastive_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/contrastive_sampler_test.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/contrastive_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/greedy_sampler.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/greedy_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/greedy_sampler_test.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/greedy_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/random_sampler.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/random_sampler_test.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/random_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/sampler.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/serialization.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/serialization_test.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/serialization_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_k_sampler.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/top_k_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_k_sampler_test.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/top_k_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_p_sampler.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/top_p_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/samplers/top_p_sampler_test.py` & `keras-nlp-0.5.1/keras_nlp/src/samplers/top_p_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/tests/doc_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/docstring_lib.py` & `keras-nlp-0.5.1/keras_nlp/src/tests/doc_tests/docstring_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/docstring_test.py` & `keras-nlp-0.5.1/keras_nlp/src/tests/doc_tests/docstring_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py` & `keras-nlp-0.5.1/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_pair_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/byte_pair_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/byte_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/byte_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/byte_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 import tensorflow as tf
 
 try:
     import sentencepiece as spm
 except ImportError:
     spm = None
 
+from keras_nlp.src.api_export import keras_nlp_export
 
+
+@keras_nlp_export("keras_nlp.tokenizers.compute_sentence_piece_proto")
 def compute_sentence_piece_proto(
     data,
     vocabulary_size,
     model_type="unigram",
     proto_output_file=None,
     lowercase=False,
 ):
```

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/word_piece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Trainer for WordPiece Tokenizer."""
 
 import tensorflow as tf
 
+from keras_nlp.src.api_export import keras_nlp_export
 from keras_nlp.src.tokenizers.word_piece_tokenizer import pretokenize
 from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
 
 try:
     from tensorflow_text.tools.wordpiece_vocab import (
         wordpiece_tokenizer_learner_lib as learner,
     )
 except ImportError:
     learner = None
 
 
+@keras_nlp_export("keras_nlp.tokenizers.compute_word_piece_vocabulary")
 def compute_word_piece_vocabulary(
     data,
     vocabulary_size,
     vocabulary_output_file=None,
     lowercase=False,
     strip_accents=False,
     split=True,
```

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py` & `keras-nlp-0.5.1/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/__init__.py` & `keras-nlp-0.5.1/keras_nlp/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/keras_utils.py` & `keras-nlp-0.5.1/keras_nlp/src/utils/keras_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/keras_utils_test.py` & `keras-nlp-0.5.1/keras_nlp/src/utils/keras_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/pipeline_model.py` & `keras-nlp-0.5.1/keras_nlp/src/utils/pipeline_model.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/pipeline_model_test.py` & `keras-nlp-0.5.1/keras_nlp/src/utils/pipeline_model_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/python_utils.py` & `keras-nlp-0.5.1/keras_nlp/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/python_utils_test.py` & `keras-nlp-0.5.1/keras_nlp/src/utils/python_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/tf_utils.py` & `keras-nlp-0.5.1/keras_nlp/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/src/utils/tf_utils_test.py` & `keras-nlp-0.5.1/keras_nlp/src/utils/tf_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp/tokenizers/__init__.py` & `keras-nlp-0.5.1/keras_nlp/tokenizers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,10 +4,12 @@
 since your modifications would be overwritten.
 """
 
 
 from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
 from keras_nlp.src.tokenizers.byte_tokenizer import ByteTokenizer
 from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer_trainer import compute_sentence_piece_proto
 from keras_nlp.src.tokenizers.tokenizer import Tokenizer
 from keras_nlp.src.tokenizers.unicode_codepoint_tokenizer import UnicodeCodepointTokenizer
 from keras_nlp.src.tokenizers.word_piece_tokenizer import WordPieceTokenizer
+from keras_nlp.src.tokenizers.word_piece_tokenizer_trainer import compute_word_piece_vocabulary
```

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp.egg-info/PKG-INFO` & `keras-nlp-0.5.1/keras_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.5.0.dev5
+Version: 0.5.1
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nlp-0.5.0.dev5/keras_nlp.egg-info/SOURCES.txt` & `keras-nlp-0.5.1/keras_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/setup.cfg` & `keras-nlp-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev5/setup.py` & `keras-nlp-0.5.1/setup.py`

 * *Files identical despite different names*

