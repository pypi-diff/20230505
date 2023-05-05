# Comparing `tmp/keras-nlp-0.5.0.dev0.tar.gz` & `tmp/keras-nlp-0.5.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nlp-0.5.0.dev0.tar", last modified: Fri Apr 28 17:50:55 2023, max compression
+gzip compressed data, was "keras-nlp-0.5.0.dev4.tar", last modified: Thu May  4 19:46:12 2023, max compression
```

## Comparing `keras-nlp-0.5.0.dev0.tar` & `keras-nlp-0.5.0.dev4.tar`

### file list

```diff
@@ -1,329 +1,299 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.348500 keras-nlp-0.5.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 17:50:55.348500 keras-nlp-0.5.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/bert_pretraining/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/bert_pretraining/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/machine_translation/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/tools/split_sentences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/tools/train_word_piece_vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/utils/scripting_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/integration_tests/basic_usage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/integration_tests/import_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/keras_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/api_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.300500 keras-nlp-0.5.0.dev0/keras_nlp/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/cached_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/cached_multi_head_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/f_net_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/f_net_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_mask_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/multi_segment_packer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/random_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/random_deletion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/random_swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/random_swap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/sine_position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/sine_position_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/start_end_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/start_end_packer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/token_and_position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/token_and_position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_decoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_layer_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.304500 keras-nlp-0.5.0.dev0/keras_nlp/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/bleu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/edit_distance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/perplexity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_l_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_n_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.304500 keras-nlp-0.5.0.dev0/keras_nlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.304500 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.304500 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.308500 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.312500 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/disentangled_attention_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/disentangled_self_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/relative_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.316500 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.320500 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.320500 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.324500 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17266 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.328500 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.328500 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_transformer_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/task_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.332500 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.336500 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.336500 keras-nlp-0.5.0.dev0/keras_nlp/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/beam_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/beam_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/contrastive_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/contrastive_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/greedy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/greedy_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/random_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_k_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_k_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_p_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_p_sampler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.336500 keras-nlp-0.5.0.dev0/keras_nlp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.340499 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/docstring_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/docstring_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/fenced_docstring_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.344499 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24873 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_pair_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_pair_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13541 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.344499 keras-nlp-0.5.0.dev0/keras_nlp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/keras_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/keras_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/pipeline_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/tf_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 17:50:55.348500 keras-nlp-0.5.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.344499 keras-nlp-0.5.0.dev0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.348500 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/checkpoint_conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_albert_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18247 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_bart_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_deberta_v3_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_distilbert_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_f_net_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_gpt2_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_opt_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_roberta_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_xlm_roberta_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/count_preset_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/api_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.237939 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/cached_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/cached_multi_head_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/f_net_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/f_net_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_head_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_mask_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/multi_segment_packer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_deletion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_swap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/sine_position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/sine_position_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/start_end_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/start_end_packer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/token_and_position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/token_and_position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14352 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_layer_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.241939 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/bleu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/edit_distance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/perplexity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_l_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_n_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.241939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.245939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.245939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.249939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.253939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/relative_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.257939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.261939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.261939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.265939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.269939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.269939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_transformer_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/task_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.269939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.273939 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.277939 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/beam_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/beam_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/contrastive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/contrastive_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/greedy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/greedy_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/random_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_k_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_k_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_p_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_p_sampler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.277939 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.277939 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/docstring_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/docstring_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24894 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_pair_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18447 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/keras_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/keras_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/pipeline_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/keras_nlp/src/utils/tf_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.281939 keras-nlp-0.5.0.dev4/keras_nlp/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-04 19:46:04.000000 keras-nlp-0.5.0.dev4/keras_nlp/tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:46:12.229939 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 19:46:12.000000 keras-nlp-0.5.0.dev4/keras_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-04 19:46:12.285939 keras-nlp-0.5.0.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-04 19:46:00.000000 keras-nlp-0.5.0.dev4/setup.py
```

### Comparing `keras-nlp-0.5.0.dev0/PKG-INFO` & `keras-nlp-0.5.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.5.0.dev0
+Version: 0.5.0.dev4
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,14 @@
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extras
-License-File: LICENSE
 
 # KerasNLP: Modular NLP Workflows for Keras
 [![](https://github.com/keras-team/keras-nlp/workflows/Tests/badge.svg?branch=master)](https://github.com/keras-team/keras-nlp/actions?query=workflow%3ATests+branch%3Amaster)
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.5.0+-success.svg)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/keras-team/keras-nlp/issues)
```

### Comparing `keras-nlp-0.5.0.dev0/README.md` & `keras-nlp-0.5.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev0/examples/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/examples/bert_pretraining/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_config.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_presets.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,73 +7,64 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""FNet model preset configurations."""
 
-# TODO(jbischof): remove in favor of presets with load_weights=False
-MODEL_CONFIGS = {
-    "tiny": {
-        "num_layers": 2,
-        "hidden_dim": 128,
-        "dropout": 0.1,
-        "num_heads": 2,
-        "intermediate_dim": 512,
-    },
-    "mini": {
-        "num_layers": 4,
-        "hidden_dim": 256,
-        "dropout": 0.1,
-        "num_heads": 4,
-        "intermediate_dim": 1024,
-    },
-    "small": {
-        "num_layers": 4,
-        "hidden_dim": 512,
-        "dropout": 0.1,
-        "num_heads": 8,
-        "intermediate_dim": 2048,
-    },
-    "medium": {
-        "num_layers": 8,
-        "hidden_dim": 512,
-        "dropout": 0.1,
-        "num_heads": 8,
-        "intermediate_dim": 2048,
-    },
-    "base": {
-        "num_layers": 12,
-        "hidden_dim": 768,
-        "dropout": 0.1,
-        "num_heads": 12,
-        "intermediate_dim": 3072,
-    },
-    "large": {
-        "num_layers": 24,
-        "hidden_dim": 1024,
-        "dropout": 0.1,
-        "num_heads": 16,
-        "intermediate_dim": 4096,
+backbone_presets = {
+    "f_net_base_en": {
+        "metadata": {
+            "description": (
+                "12-layer FNet model where case is maintained. "
+                "Trained on the C4 dataset."
+            ),
+            "params": 82861056,
+            "official_name": "FNet",
+            "path": "f_net",
+            "model_card": "https://github.com/google-research/google-research/blob/master/f_net/README.md",
+        },
+        "config": {
+            "vocabulary_size": 32000,
+            "num_layers": 12,
+            "hidden_dim": 768,
+            "intermediate_dim": 3072,
+            "dropout": 0.1,
+            "max_sequence_length": 512,
+            "num_segments": 4,
+        },
+        "preprocessor_config": {},
+        "weights_url": "https://storage.googleapis.com/keras-nlp/models/f_net_base_en/v1/model.h5",
+        "weights_hash": "35db90842b85a985a0e54c86c00746fe",
+        "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/f_net_base_en/v1/vocab.spm",
+        "spm_proto_hash": "71c5f4610bef1daf116998a113a01f3d",
+    },
+    "f_net_large_en": {
+        "metadata": {
+            "description": (
+                "24-layer FNet model where case is maintained. "
+                "Trained on the C4 dataset."
+            ),
+            "params": 236945408,
+            "official_name": "FNet",
+            "path": "f_net",
+            "model_card": "https://github.com/google-research/google-research/blob/master/f_net/README.md",
+        },
+        "config": {
+            "vocabulary_size": 32000,
+            "num_layers": 24,
+            "hidden_dim": 1024,
+            "intermediate_dim": 4096,
+            "dropout": 0.1,
+            "max_sequence_length": 512,
+            "num_segments": 4,
+        },
+        "preprocessor_config": {},
+        "weights_url": "https://storage.googleapis.com/keras-nlp/models/f_net_large_en/v1/model.h5",
+        "weights_hash": "7ae4a3faa67ff054f8cecffb5619f779",
+        "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/f_net_large_en/v1/vocab.spm",
+        "spm_proto_hash": "71c5f4610bef1daf116998a113a01f3d",
     },
 }
 
-# Currently we have the same set of training parameters for all configurations.
-# We should see if we need to split this for different architecture sizes.
-
-PREPROCESSING_CONFIG = {
-    "max_seq_length": 512,
-    "max_predictions_per_seq": 76,
-    "dupe_factor": 10,
-    "masked_lm_prob": 0.15,
-    "short_seq_prob": 0.1,
-}
-
-TRAINING_CONFIG = {
-    "batch_size": 256,
-    "epochs": 10,
-    "learning_rate": 1e-4,
-    "num_train_steps": 1_000_000,
-    # Percentage of training steps used for learning rate warmup.
-    "warmup_percentage": 0.1,
-}
```

### Comparing `keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_pretrain.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/bleu.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,450 +8,382 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import datetime
-import sys
+"""BLEU metric implementation."""
+
+import collections
+import math
 
 import tensorflow as tf
-from absl import app
-from absl import flags
-from absl import logging
 from tensorflow import keras
 
-import keras_nlp
-from examples.bert_pretraining.bert_config import MODEL_CONFIGS
-from examples.bert_pretraining.bert_config import PREPROCESSING_CONFIG
-from examples.bert_pretraining.bert_config import TRAINING_CONFIG
-
-FLAGS = flags.FLAGS
-
-flags.DEFINE_string(
-    "input_directory",
-    None,
-    "The directory of training data. It can be a local disk path, or the URL "
-    "of Google cloud storage bucket.",
-)
-
-flags.DEFINE_string(
-    "saved_model_output",
-    None,
-    "Output directory to save the model to.",
-)
-
-flags.DEFINE_string(
-    "checkpoint_save_directory",
-    None,
-    "Output directory to save checkpoints to.",
-)
-
-flags.DEFINE_bool(
-    "skip_restore",
-    False,
-    "Skip restoring from checkpoint if True",
-)
-
-flags.DEFINE_bool(
-    "tpu_name",
-    None,
-    "The TPU to connect to. If None, TPU will not be used.",
-)
-
-flags.DEFINE_bool(
-    "enable_cloud_logging",
-    False,
-    "If True, the script will use cloud logging.",
-)
-
-flags.DEFINE_string(
-    "tensorboard_log_path",
-    None,
-    "The path to save tensorboard log to.",
-)
-
-flags.DEFINE_string(
-    "model_size",
-    "tiny",
-    "One of: tiny, mini, small, medium, base, or large.",
-)
-
-flags.DEFINE_string(
-    "vocab_file",
-    None,
-    "The vocabulary file for tokenization.",
-)
-
-flags.DEFINE_integer(
-    "num_train_steps",
-    None,
-    "Override the pre-configured number of train steps..",
-)
-
-
-class MaskedLMHead(keras.layers.Layer):
-    """Masked language model network head for BERT.
-
-    This layer implements a masked language model based on the provided
-    transformer based encoder. It assumes that the encoder network being passed
-    has a "get_embedding_table()" method.
-
-    Example:
-    ```python
-    encoder = keras_nlp.models.BertBackbone(
-        vocabulary_size=30552,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12,
-    )
-    lm_layer = MaskedLMHead(embedding_table=encoder.get_embedding_table())
-    ```
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.utils.tf_utils import tensor_to_list
+
+REPLACE_SUBSTRINGS = [
+    ("<skipped>", ""),
+    ("-\n", ""),
+    ("\n", " "),
+    ("&quot;", '"'),
+    ("&amp;", "&"),
+    ("&lt;", "<"),
+    ("&gt;", ">"),
+]
+
+
+REGEX_PATTERNS = [
+    # language-dependent part (assuming Western languages)
+    (r"([\{-\~\[-\` -\&\(-\+\:-\@\/])", r" \1 "),
+    # tokenize period and comma unless preceded by a digit
+    (r"([^0-9])([\.,])", r"\1 \2 "),
+    # tokenize period and comma unless followed by a digit
+    (r"([\.,])([^0-9])", r" \1 \2"),
+    # tokenize dash when preceded by a digit
+    (r"([0-9])(-)", r"\1 \2 "),
+    # If last character is "." or ",", add space.
+    (r"[\.,]$", r" \0 \1"),
+    # one space only between words
+    (r"\s+", r" "),
+]
+
+
+@keras_nlp_export("keras_nlp.metrics.Bleu")
+class Bleu(keras.metrics.Metric):
+    """BLEU metric.
+
+    This class implements the BLEU metric. BLEU is generally used to evaluate
+    machine translation systems. By default, this implementation replicates
+    SacreBLEU, but user-defined tokenizers can be passed to deal with other
+    languages.
+
+    For BLEU score, we count the number of matching n-grams in the candidate
+    translation and the reference text. We find the "clipped count" of matching
+    n-grams so as to not give a high score to a (reference, prediction) pair
+    with redundant, repeated tokens. Secondly, BLEU score tends to reward
+    shorter predictions more, which is why a brevity penalty is applied to
+    penalise short predictions. For more details, see the following article:
+    https://cloud.google.com/translate/automl/docs/evaluate#bleu.
+
+    Note on input shapes:
+    For unbatched inputs, `y_pred` should be a tensor of shape `()`, and
+    `y_true` should be a tensor of shape `(num_references,)`. For batched
+    inputs, `y_pred` should be a tensor of shape `(batch_size,)`,
+    and `y_true` should be a tensor of shape `(batch_size, num_references)`. In
+    case of batched inputs, `y_true` can also be a ragged tensor of shape
+    `(batch_size, None)` if different samples have different number of
+    references.
 
     Args:
-        embedding_table: The embedding table from encoder network.
-        intermediate_activation: The activation, if any, for the inner dense
-            layer.
-        initializer: The initializer for the dense layer. Defaults to a Glorot
-            uniform initializer.
-        output: The output style for this layer. Can be either 'logits' or
-            'predictions'.
+        tokenizer: callable. A function that takes a string `tf.RaggedTensor`
+            (of any shape), and tokenizes the strings in the tensor. If the
+            tokenizer is not specified, the default tokenizer is used. The
+            default tokenizer replicates the behaviour of SacreBLEU's
+            `"tokenizer_13a"` tokenizer
+            (https://github.com/mjpost/sacrebleu/blob/v2.1.0/sacrebleu/tokenizers/tokenizer_13a.py).
+        max_order: int. The maximum n-gram order to use. For example, if
+            `max_order` is set to 3, unigrams, bigrams, and trigrams will be
+            considered. Defaults to 4.
+        smooth: bool. Whether to apply Lin et al. 2004 smoothing to the BLEU
+            score. Adds 1 to the matched n-gram count (i.e., numerator) and 1
+            to the total n-gram count (i.e., denominator) for every order while
+            calculating precision. Defaults to False.
+        dtype: string or tf.dtypes.Dtype. Precision of metric computation. If
+               not specified, it defaults to tf.float32.
+        name: string. Name of the metric instance.
+        **kwargs: Other keyword arguments.
+
+    References:
+        - [Papineni et al., 2002](https://aclanthology.org/P02-1040/)
+        - [SacreBLEU](https://github.com/mjpost/sacrebleu)
+        - [Lin et al., 2004](https://aclanthology.org/P04-1077/)
     """
 
     def __init__(
         self,
-        embedding_table,
-        intermediate_activation="gelu",
-        initializer="glorot_uniform",
+        tokenizer=None,
+        max_order=4,
+        smooth=False,
+        dtype=None,
+        name="bleu",
         **kwargs,
     ):
-        super().__init__(**kwargs)
-        self.embedding_table = embedding_table
-        self.intermediate_activation = keras.activations.get(
-            intermediate_activation
-        )
-        self.initializer = initializer
-
-    def build(self, input_shape):
-        self._vocab_size, hidden_dim = self.embedding_table.shape
-        self.dense = keras.layers.Dense(
-            hidden_dim,
-            activation=self.intermediate_activation,
-            kernel_initializer=self.initializer,
-            name="transform/dense",
-        )
-        self.layer_norm = keras.layers.LayerNormalization(
-            axis=-1, epsilon=1e-12, name="transform/LayerNorm"
-        )
-        self.bias = self.add_weight(
-            "output_bias/bias",
-            shape=(self._vocab_size,),
-            initializer="zeros",
-            trainable=True,
-        )
+        super().__init__(name=name, dtype=dtype, **kwargs)
 
-        super().build(input_shape)
+        if not tf.as_dtype(self.dtype).is_floating:
+            raise ValueError(
+                "`dtype` must be a floating point type. "
+                f"Received: dtype={dtype}"
+            )
 
-    def call(self, sequence_data, masked_positions):
-        masked_lm_input = self._gather_indexes(sequence_data, masked_positions)
-        lm_data = self.dense(masked_lm_input)
-        lm_data = self.layer_norm(lm_data)
-        lm_data = tf.matmul(lm_data, self.embedding_table, transpose_b=True)
-        logits = tf.nn.bias_add(lm_data, self.bias)
-        masked_positions_length = (
-            masked_positions.shape.as_list()[1] or tf.shape(masked_positions)[1]
+        self.tokenizer = tokenizer
+        self.max_order = max_order
+        self.smooth = smooth
+
+        self._matches = self.add_weight(
+            shape=(self.max_order,),
+            name="bleu_matches",
+            initializer="zeros",
+            dtype=self.dtype,
         )
-        return tf.reshape(
-            logits, [-1, masked_positions_length, self._vocab_size]
+        self._possible_matches = self.add_weight(
+            shape=(self.max_order,),
+            name="bleu_possible_matches",
+            initializer="zeros",
+            dtype=self.dtype,
+        )
+        self._translation_length = self.add_weight(
+            name="bleu_translation_length",
+            initializer="zeros",
+            dtype=self.dtype,
+        )
+        self._reference_length = self.add_weight(
+            name="bleu_reference_length",
+            initializer="zeros",
+            dtype=self.dtype,
+        )
+        self._bleu = self.add_weight(
+            name="bleu",
+            initializer="zeros",
+            dtype=self.dtype,
         )
 
-    def _gather_indexes(self, sequence_tensor, positions):
-        """Gathers the vectors at the specific positions, for performance.
-
-        Args:
-            sequence_tensor: Sequence output of shape
-                (`batch_size`, `seq_length`, `hidden_dim`) where `hidden_dim`
-                is number of hidden units.
-            positions: Positions ids of tokens in sequence to mask for
-                pretraining of with dimension (batch_size, num_predictions)
-                where `num_predictions` is maximum number of tokens to mask out
-                and predict per each sequence.
-
-        Returns:
-            Masked out sequence tensor of shape (batch_size * num_predictions,
-            `hidden_dim`).
+    def _tokenizer(self, inputs):
+        """
+        Tokenizes the input strings. By default, replicates the behaviour of
+        SacreBLEU's default tokenizer, namely, `tokenizer_13a`.
         """
-        sequence_shape = tf.shape(sequence_tensor)
-        batch_size, seq_length = sequence_shape[0], sequence_shape[1]
-        width = sequence_tensor.shape.as_list()[2] or sequence_shape[2]
+        if self.tokenizer:
+            return self.tokenizer(inputs)
 
-        flat_offsets = tf.reshape(
-            tf.range(0, batch_size, dtype=tf.int32) * seq_length, [-1, 1]
-        )
-        flat_positions = tf.reshape(positions + flat_offsets, [-1])
-        flat_sequence_tensor = tf.reshape(
-            sequence_tensor, [batch_size * seq_length, width]
-        )
-        output_tensor = tf.gather(flat_sequence_tensor, flat_positions)
+        for pattern, replacement in REPLACE_SUBSTRINGS + REGEX_PATTERNS:
+            inputs = tf.strings.regex_replace(
+                input=inputs,
+                pattern=pattern,
+                rewrite=replacement,
+                replace_global=True,
+                name=None,
+            )
+        inputs = tf.strings.split(inputs)
+        return inputs
 
-        return output_tensor
+    def _get_ngrams(self, segment, max_order):
+        """Extracts all n-grams up to a given maximum order from an input segment.
 
+        Uses Python ops. Inspired from
+        https://github.com/tensorflow/nmt/blob/master/nmt/scripts/bleu.py.
 
-class BertPretrainingModel(keras.Model):
-    """MaskedLM + NSP model with Bert encoder."""
+        Args:
+            segment: list. Text segment from which n-grams will be
+                extracted.
+            max_order: int. Maximum length in tokens of the n-grams returned
+                by this method.
+        """
+        ngram_counts = collections.Counter()
+        for order in range(1, max_order + 1):
+            for i in range(0, len(segment) - order + 1):
+                ngram = tuple(segment[i : i + order])
+                ngram_counts[ngram] += 1
+        return ngram_counts
 
-    def __init__(self, encoder, **kwargs):
-        super().__init__(**kwargs)
-        self.encoder = encoder
-        # TODO(jbischof): replace with keras_nlp.layers.MaskedLMHead (Issue #166)
-        self.masked_lm_head = MaskedLMHead(
-            embedding_table=encoder.token_embedding.embeddings,
-            initializer=keras.initializers.TruncatedNormal(stddev=0.02),
-            name="mlm_layer",
-        )
-        self.next_sentence_head = keras.layers.Dense(
-            encoder.num_segments,
-            kernel_initializer=keras.initializers.TruncatedNormal(stddev=0.02),
-            name="nsp_layer",
-        )
+    def _corpus_bleu(
+        self,
+        reference_corpus,
+        translation_corpus,
+        matches_by_order,
+        possible_matches_by_order,
+        translation_length,
+        reference_length,
+        max_order=4,
+        smooth=False,
+    ):
+        """Corpus BLEU implementation using Python ops.
 
-    def call(self, data):
-        encoder_output = self.encoder(
-            {
-                "token_ids": data["token_ids"],
-                "segment_ids": data["segment_ids"],
-                "padding_mask": data["padding_mask"],
-            }
-        )
-        sequence_output, pooled_output = (
-            encoder_output["sequence_output"],
-            encoder_output["pooled_output"],
-        )
-        lm_preds = self.masked_lm_head(
-            sequence_output, data["masked_lm_positions"]
-        )
-        nsp_preds = self.next_sentence_head(pooled_output)
-        return {"mlm": lm_preds, "nsp": nsp_preds}
+        Computes BLEU score of translated segments against one or more
+        references. Inspired from
+        https://github.com/tensorflow/nmt/blob/master/nmt/scripts/bleu.py.
+
+        Args:
+            reference_corpus: list of lists of references for each
+                translation. Each reference should be tokenized into a list
+                of tokens.
+            translation_corpus: list of translations to score. Each
+                translation should be tokenized into a list of tokens.
+            matches_by_order: list of floats containing the initial number
+                of matches for each order.
+            possible_matches_by_order: list of floats containing the initial
+                number of possible matches for each order.
+            translation_length: float. Initial number of tokens in all the
+                translations.
+            reference_length: float. Initial number of tokens in all the
+                references.
+            max_order: int. Maximum n-gram order to use when computing
+                BLEU score.
+            smooth: boolean. Whether or not to apply Lin et al. 2004
+                smoothing.
+        """
+        for references, translation in zip(
+            reference_corpus, translation_corpus
+        ):
+            reference_length += min(len(r) for r in references)
+            translation_length += len(translation)
+
+            merged_ref_ngram_counts = collections.Counter()
+            for reference in references:
+                merged_ref_ngram_counts |= self._get_ngrams(
+                    reference, max_order
+                )
+            translation_ngram_counts = self._get_ngrams(translation, max_order)
+            overlap = translation_ngram_counts & merged_ref_ngram_counts
+            for ngram in overlap:
+                matches_by_order[len(ngram) - 1] += overlap[ngram]
+            for order in range(1, max_order + 1):
+                possible_matches = len(translation) - order + 1
+                if possible_matches > 0:
+                    possible_matches_by_order[order - 1] += possible_matches
+
+        precisions = [0] * max_order
+        for i in range(0, max_order):
+            if smooth:
+                precisions[i] = (matches_by_order[i] + 1.0) / (
+                    possible_matches_by_order[i] + 1.0
+                )
+            else:
+                if possible_matches_by_order[i] > 0:
+                    precisions[i] = (
+                        float(matches_by_order[i])
+                        / possible_matches_by_order[i]
+                    )
+                else:
+                    precisions[i] = 0.0
+
+        if min(precisions) > 0:
+            p_log_sum = sum((1.0 / max_order) * math.log(p) for p in precisions)
+            geo_mean = math.exp(p_log_sum)
+        else:
+            geo_mean = 0
 
+        ratio = float(translation_length) / reference_length
 
-class LinearDecayWithWarmup(keras.optimizers.schedules.LearningRateSchedule):
-    """
-    A learning rate schedule with linear warmup and decay.
+        if ratio > 1.0:
+            bp = 1.0
+        else:
+            bp = math.exp(1 - 1.0 / ratio)
 
-    This schedule implements a linear warmup for the first `num_warmup_steps`
-    and a linear ramp down until `num_train_steps`.
-    """
+        bleu = geo_mean * bp
 
-    def __init__(self, learning_rate, num_warmup_steps, num_train_steps):
-        self.learning_rate = learning_rate
-        self.warmup_steps = num_warmup_steps
-        self.train_steps = num_train_steps
-
-    def __call__(self, step):
-        peak_lr = tf.cast(self.learning_rate, dtype=tf.float32)
-        warmup = tf.cast(self.warmup_steps, dtype=tf.float32)
-        training = tf.cast(self.train_steps, dtype=tf.float32)
-        step = tf.cast(step, dtype=tf.float32)
-
-        is_warmup = step < warmup
-
-        # Linear Warmup will be implemented if current step is less than
-        # `num_warmup_steps` else Linear Decay will be implemented.
-        return tf.cond(
-            is_warmup,
-            lambda: peak_lr * (step / warmup),
-            lambda: tf.math.maximum(
-                0.0, peak_lr * (training - step) / (training - warmup)
-            ),
-        )
+        return (
+            bleu,
+            matches_by_order,
+            possible_matches_by_order,
+            translation_length,
+            reference_length,
+        )
+
+    def _calculate_bleu_score(self, references, translation):
+        references = tensor_to_list(references)
+        translation = tensor_to_list(translation)
+
+        matches = self._matches.numpy()
+        possible_matches = self._possible_matches.numpy()
+        translation_length = self._translation_length.numpy()
+        reference_length = self._reference_length.numpy()
+
+        (
+            bleu_score,
+            matches,
+            possible_matches,
+            translation_length,
+            reference_length,
+        ) = self._corpus_bleu(
+            reference_corpus=references,
+            translation_corpus=translation,
+            matches_by_order=matches,
+            possible_matches_by_order=possible_matches,
+            translation_length=translation_length,
+            reference_length=reference_length,
+            max_order=self.max_order,
+            smooth=self.smooth,
+        )
+        return (
+            tf.constant(bleu_score, dtype=self.dtype),
+            tf.constant(matches, dtype=self.dtype),
+            tf.constant(possible_matches, dtype=self.dtype),
+            tf.constant(translation_length, dtype=self.dtype),
+            tf.constant(reference_length, dtype=self.dtype),
+        )
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        def validate_and_fix_rank(inputs, tensor_name, base_rank=0):
+            if not isinstance(inputs, (tf.Tensor, tf.RaggedTensor)):
+                inputs = tf.convert_to_tensor(inputs)
+
+            if inputs.shape.rank == base_rank:
+                return inputs[tf.newaxis]
+            elif inputs.shape.rank == base_rank + 1:
+                return inputs
+            elif inputs.shape.rank == base_rank + 2:
+                if tf.shape(inputs)[-1] != 1:
+                    raise ValueError(
+                        f"{tensor_name} is of rank {input.shape.rank}. The "
+                        f"last dimension must be of size 1."
+                    )
+                return tf.squeeze(inputs, axis=-1)
+            else:
+                raise ValueError(
+                    f"{tensor_name} must be of rank {base_rank}, {base_rank+1} "
+                    f"or {base_rank+2}. Found rank: {inputs.shape.rank}"
+                )
+
+        y_true = validate_and_fix_rank(y_true, "y_true", 1)
+        y_pred = validate_and_fix_rank(y_pred, "y_pred", 0)
+
+        # Tokenize the inputs.
+        y_true = self._tokenizer(y_true)
+        y_pred = self._tokenizer(y_pred)
+
+        (
+            bleu_score,
+            matches,
+            possible_matches,
+            translation_length,
+            reference_length,
+        ) = tf.py_function(
+            func=self._calculate_bleu_score,
+            inp=[y_true, y_pred],
+            Tout=[self.dtype, self.dtype, self.dtype, self.dtype, self.dtype],
+        )
+
+        self._matches.assign(matches)
+        self._possible_matches.assign(possible_matches)
+        self._translation_length.assign(translation_length)
+        self._reference_length.assign(reference_length)
+        self._bleu.assign(bleu_score)
+
+    def result(self):
+        return self._bleu
+
+    def reset_state(self):
+        self._matches.assign(
+            tf.zeros(shape=(self.max_order,), dtype=self.dtype)
+        )
+        self._possible_matches.assign(
+            tf.zeros(shape=(self.max_order,), dtype=self.dtype)
+        )
+        self._translation_length.assign(0.0)
+        self._reference_length.assign(0.0)
+        self._bleu.assign(0.0)
 
     def get_config(self):
-        return {
-            "learning_rate": self.learning_rate,
-            "num_warmup_steps": self.warmup_steps,
-            "num_train_steps": self.train_steps,
-        }
-
-
-def decode_record(record):
-    """Decodes a record to a TensorFlow example."""
-    seq_length = PREPROCESSING_CONFIG["max_seq_length"]
-    lm_length = PREPROCESSING_CONFIG["max_predictions_per_seq"]
-    name_to_features = {
-        "token_ids": tf.io.FixedLenFeature([seq_length], tf.int64),
-        "padding_mask": tf.io.FixedLenFeature([seq_length], tf.int64),
-        "segment_ids": tf.io.FixedLenFeature([seq_length], tf.int64),
-        "masked_lm_positions": tf.io.FixedLenFeature([lm_length], tf.int64),
-        "masked_lm_ids": tf.io.FixedLenFeature([lm_length], tf.int64),
-        "masked_lm_weights": tf.io.FixedLenFeature([lm_length], tf.float32),
-        "next_sentence_labels": tf.io.FixedLenFeature([1], tf.int64),
-    }
-    # tf.Example only supports tf.int64, but the TPU only supports tf.int32.
-    # So cast all int64 to int32.
-    example = tf.io.parse_single_example(record, name_to_features)
-    for name in list(example.keys()):
-        value = example[name]
-        if value.dtype == tf.int64:
-            value = tf.cast(value, tf.int32)
-        example[name] = value
-
-    inputs = {
-        "token_ids": example["token_ids"],
-        "padding_mask": example["padding_mask"],
-        "segment_ids": example["segment_ids"],
-        "masked_lm_positions": example["masked_lm_positions"],
-    }
-    labels = {
-        "mlm": example["masked_lm_ids"],
-        "nsp": example["next_sentence_labels"],
-    }
-    sample_weights = {"mlm": example["masked_lm_weights"], "nsp": tf.ones((1,))}
-    sample = (inputs, labels, sample_weights)
-    return sample
-
-
-def get_checkpoint_callback():
-    if tf.io.gfile.exists(FLAGS.checkpoint_save_directory):
-        if not tf.io.gfile.isdir(FLAGS.checkpoint_save_directory):
-            raise ValueError(
-                "`checkpoint_save_directory` should be a directory, "
-                f"but {FLAGS.checkpoint_save_directory} is not a "
-                "directory. Please set `checkpoint_save_directory` as "
-                "a directory."
-            )
+        config = super().get_config()
+        config.update(
+            {
+                "tokenizer": self.tokenizer,
+                "max_order": self.max_order,
+                "smooth": self.smooth,
+            }
+        )
+        return config
 
-        elif FLAGS.skip_restore:
-            # Clear up the directory if users want to skip restoring.
-            tf.io.gfile.rmtree(FLAGS.checkpoint_save_directory)
-    checkpoint_path = FLAGS.checkpoint_save_directory
-    return keras.callbacks.BackupAndRestore(
-        backup_dir=checkpoint_path,
-    )
-
-
-def get_tensorboard_callback():
-    timestamp = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
-    log_dir = FLAGS.tensorboard_log_path + timestamp
-    return keras.callbacks.TensorBoard(log_dir=log_dir, histogram_freq=1)
-
-
-def main(_):
-    if FLAGS.enable_cloud_logging:
-        # If the job is on cloud, we will use cloud logging.
-        import google.cloud.logging
-
-        keras.utils.disable_interactive_logging()
-        client = google.cloud.logging.Client()
-        client.setup_logging()
-
-    logging.info(f"Reading input data from {FLAGS.input_directory}")
-    if not tf.io.gfile.isdir(FLAGS.input_directory):
-        raise ValueError(
-            "`input_directory` should be a directory, "
-            f"but {FLAGS.input_directory} is not a directory. Please "
-            "set `input_directory` flag as a directory."
-        )
-    files = tf.io.gfile.listdir(FLAGS.input_directory)
-    input_filenames = [FLAGS.input_directory + "/" + file for file in files]
-
-    if not input_filenames:
-        logging.info("No input files found. Check `input_directory` flag.")
-        sys.exit(1)
-
-    vocab = []
-    with tf.io.gfile.GFile(FLAGS.vocab_file) as vocab_file:
-        for line in vocab_file:
-            vocab.append(line.strip())
-
-    model_config = MODEL_CONFIGS[FLAGS.model_size]
-
-    if FLAGS.tpu_name is None:
-        # Use default strategy if not using TPU.
-        strategy = tf.distribute.get_strategy()
-    else:
-        # Connect to TPU and create TPU strategy.
-        resolver = tf.distribute.cluster_resolver.TPUClusterResolver.connect(
-            tpu=FLAGS.tpu_name
-        )
-        strategy = tf.distribute.TPUStrategy(resolver)
-
-    # Decode and batch data.
-    dataset = tf.data.TFRecordDataset(input_filenames)
-    dataset = dataset.map(
-        lambda record: decode_record(record),
-        num_parallel_calls=tf.data.experimental.AUTOTUNE,
-    )
-    dataset = dataset.batch(TRAINING_CONFIG["batch_size"], drop_remainder=True)
-    dataset = dataset.repeat()
-
-    with strategy.scope():
-        # Create a Bert model the input config.
-        encoder = keras_nlp.models.BertBackbone(
-            vocabulary_size=len(vocab), **model_config
-        )
-        # Make sure model has been called.
-        encoder(encoder.inputs)
-        encoder.summary()
-
-        # Allow overriding train steps from the command line for quick testing.
-        if FLAGS.num_train_steps is not None:
-            num_train_steps = FLAGS.num_train_steps
-        else:
-            num_train_steps = TRAINING_CONFIG["num_train_steps"]
-        num_warmup_steps = int(
-            num_train_steps * TRAINING_CONFIG["warmup_percentage"]
-        )
-        learning_rate_schedule = LinearDecayWithWarmup(
-            learning_rate=TRAINING_CONFIG["learning_rate"],
-            num_warmup_steps=num_warmup_steps,
-            num_train_steps=num_train_steps,
-        )
-        optimizer = keras.optimizers.Adam(learning_rate=learning_rate_schedule)
-
-        lm_loss = keras.losses.SparseCategoricalCrossentropy(
-            from_logits=True,
-            name="lm_loss",
-        )
-        nsp_loss = keras.losses.SparseCategoricalCrossentropy(
-            from_logits=True,
-            name="nsp_loss",
-        )
-
-        lm_accuracy = keras.metrics.SparseCategoricalAccuracy(name="accuracy")
-        nsp_accuracy = keras.metrics.SparseCategoricalAccuracy(name="accuracy")
-
-        pretraining_model = BertPretrainingModel(encoder)
-        pretraining_model.compile(
-            optimizer=optimizer,
-            loss={"mlm": lm_loss, "nsp": nsp_loss},
-            weighted_metrics={"mlm": lm_accuracy, "nsp": nsp_accuracy},
-        )
-
-    epochs = TRAINING_CONFIG["epochs"]
-    steps_per_epoch = num_train_steps // epochs
-
-    callbacks = []
-    if FLAGS.checkpoint_save_directory:
-        callbacks.append(get_checkpoint_callback())
-    if FLAGS.tensorboard_log_path:
-        callbacks.append(get_tensorboard_callback())
-
-    pretraining_model.fit(
-        dataset,
-        epochs=epochs,
-        steps_per_epoch=steps_per_epoch,
-        callbacks=callbacks,
-    )
-
-    model_path = FLAGS.saved_model_output
-    logging.info(f"Saving to {FLAGS.saved_model_output}")
-    encoder.save(model_path)
-
-
-if __name__ == "__main__":
-    flags.mark_flag_as_required("input_directory")
-    flags.mark_flag_as_required("vocab_file")
-    flags.mark_flag_as_required("saved_model_output")
-    app.run(main)
```

### Comparing `keras-nlp-0.5.0.dev0/examples/machine_translation/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/examples/tools/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/examples/utils/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/integration_tests/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Copyright 2021 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/integration_tests/import_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import tensorflow as tf
+# sentencepiece is segfaulting on tf-nightly if tensorflow is imported first.
+# This is a temporary fix to restore our nightly testing to green, while we look
+# for a longer term solution.
+try:
+    import sentencepiece
+except ImportError:
+    pass
 
-import keras_nlp
+from keras_nlp.src import layers
+from keras_nlp.src import metrics
+from keras_nlp.src import models
+from keras_nlp.src import samplers
+from keras_nlp.src import tokenizers
+from keras_nlp.src import utils
 
+__version__ = "0.5.0.dev4"
 
-class ImportTest(tf.test.TestCase):
-    def test_version(self):
-        self.assertIsNotNone(keras_nlp.__version__)
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/api_export.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/api_export.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,7 +42,8 @@
     class keras_nlp_export:
         def __init__(self, path):
             pass
 
         def __call__(self, symbol):
             maybe_register_serializable(symbol)
             return symbol
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/conftest.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,7 +109,8 @@
             item.add_marker(skip_keras_saving_test)
         if "large" in item.keywords:
             item.add_marker(skip_large)
         if "extra_large" in item.keywords:
             item.add_marker(skip_extra_large)
         if "tpu" in item.keywords:
             item.add_marker(skip_tpu)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/cached_multi_head_attention.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/cached_multi_head_attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Cached MHA layer based on `keras.layers.MultiHeadAttention`."""
 
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.layers.CachedMultiHeadAttention")
 class CachedMultiHeadAttention(keras.layers.MultiHeadAttention):
     """MutliHeadAttention layer with cache support.
 
     In autoregressive decoding, it's a common practice to cache the key/value in
@@ -94,7 +94,8 @@
         attention_scores = self._dropout_layer(attention_scores)
 
         attention_output = tf.einsum(
             self._combine_equation, attention_scores, value
         )
         attention_output = self._output_dense(attention_output)
         return attention_output, cache
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/cached_multi_head_attention_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/cached_multi_head_attention_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Tests for CachedMultiHeadAttention."""
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
-from keras_nlp.layers.cached_multi_head_attention import (
+from keras_nlp.src.layers.cached_multi_head_attention import (
     CachedMultiHeadAttention,
 )
 
 
 class CachedMultiHeadAttentionTest(tf.test.TestCase, parameterized.TestCase):
     def test_valid_call(self):
         layer = CachedMultiHeadAttention(num_heads=2, key_dim=4)
@@ -75,7 +75,8 @@
         call = call if eager else tf.function(call)
         output, cache = call(outputs, cache)
 
         no_loop_outputs, _ = layer(x, x, attention_mask=mask)
         _, no_loop_cache = layer(x, x, cache=cache, attention_mask=mask)
         self.assertAllClose(output, no_loop_outputs)
         self.assertAllClose(cache, no_loop_cache)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/f_net_encoder.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/f_net_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 
 """FNet encoder block implementation based on `keras.layers.Layer`."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.utils.keras_utils import clone_initializer
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.utils.keras_utils import clone_initializer
 
 
 @keras_nlp_export("keras_nlp.layers.FNetEncoder")
 class FNetEncoder(keras.layers.Layer):
     """FNet encoder.
 
     This class follows the architecture of FNet encoder layer in the
@@ -170,7 +170,8 @@
                 ),
                 "bias_initializer": keras.initializers.serialize(
                     self.bias_initializer
                 ),
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/f_net_encoder_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/f_net_encoder_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.layers import f_net_encoder
+from keras_nlp.src.layers import f_net_encoder
 
 
 class FNetEncoderTest(tf.test.TestCase, parameterized.TestCase):
     def test_valid_call(self):
         encoder = f_net_encoder.FNetEncoder(intermediate_dim=4)
         model = keras.Sequential(
             [
@@ -137,7 +137,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         loaded_model = keras.models.load_model(path)
 
         model_output = model(data)
         loaded_model_output = loaded_model(data)
         self.assertAllClose(model_output, loaded_model_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_head.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Masked Language Model (MaskedLM) head."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.layers.MaskedLMHead")
 class MaskedLMHead(keras.layers.Layer):
     """Masked Language Model (MaskedLM) head.
 
     This layer takes two inputs:
@@ -210,7 +210,8 @@
                 ),
                 "bias_initializer": keras.initializers.serialize(
                     self.bias_initializer
                 ),
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_head_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_head_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.layers import masked_lm_head
+from keras_nlp.src.layers import masked_lm_head
 
 
 class MaskedLMHeadTest(tf.test.TestCase, parameterized.TestCase):
     def test_valid_call(self):
         head = masked_lm_head.MaskedLMHead(
             vocabulary_size=100,
             activation="softmax",
@@ -180,7 +180,8 @@
         # Don't save traces in the tf format, we check compilation elsewhere.
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
 
         restored_output = restored_model((token_data, position_data))
         self.assertAllClose(model_output, restored_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_mask_generator.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_mask_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.utils.tf_utils import assert_tf_text_installed
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
@@ -220,7 +220,8 @@
                 "unselectable_token_ids": self.unselectable_token_ids,
                 "mask_token_id": self.mask_token_id,
                 "mask_token_rate": self.mask_token_rate,
                 "random_token_rate": self.random_token_rate,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_mask_generator_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/masked_lm_mask_generator_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
-from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
+from keras_nlp.src.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
 
 
 class MaskedLMMaskGeneratorTest(tf.test.TestCase):
     def setUp(self):
         super().setUp()
         self.VOCAB = [
             "[UNK]",
@@ -261,7 +261,8 @@
         )
         batch_first = ds.batch(8).map(masked_lm_masker)
         batch_second = ds.map(masked_lm_masker).batch(8)
         self.assertEqual(
             batch_first.take(1).get_single_element()["token_ids"].shape,
             batch_second.take(1).get_single_element()["token_ids"].shape,
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/multi_segment_packer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/multi_segment_packer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 
 """BERT token packing layer."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.utils.tf_utils import assert_tf_text_installed
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
@@ -227,7 +227,8 @@
         segment_ids = segment_ids.to_tensor(shape=shape)
         # Remove the batch dim if added.
         if rank_1:
             token_ids = tf.squeeze(token_ids, 0)
             segment_ids = tf.squeeze(segment_ids, 0)
 
         return (token_ids, segment_ids)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/multi_segment_packer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/multi_segment_packer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
+from keras_nlp.src.layers.multi_segment_packer import MultiSegmentPacker
 
 
 class MultiSegmentPackerTest(tf.test.TestCase, parameterized.TestCase):
     def test_trim_single_input_ints(self):
         input_data = tf.range(3, 10)
         packer = MultiSegmentPacker(8, start_value=1, end_value=2)
         output = packer(input_data)
@@ -182,7 +182,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model((seq1, seq2)),
             restored_model((seq1, seq2)),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/position_embedding.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/position_embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Position embedding implementation based on `keras.layers.Layer`."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.layers.PositionEmbedding")
 class PositionEmbedding(keras.layers.Layer):
     """A layer which learns a position embedding for inputs sequences.
 
     This class assumes that in the input tensor, the last dimension corresponds
@@ -129,7 +129,8 @@
         position_embeddings = tf.slice(
             self.position_embeddings,
             (start_index, 0),
             (sequence_length, feature_length),
         )
         # then broadcast to add the missing dimensions to match "shape"
         return tf.broadcast_to(position_embeddings, shape)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/position_embedding_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/position_embedding_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.layers import position_embedding
+from keras_nlp.src.layers import position_embedding
 
 
 def custom_init(shape, dtype=None):
     count = 1
     for length in shape:
         count *= length
     return tf.reshape(tf.range(count, dtype=dtype), shape)
@@ -317,7 +317,8 @@
         model_output = model.predict(data)
         loaded_model_output = loaded_model.predict(data)
         self.assertAllClose(model_output, loaded_model_output)
 
 
 if __name__ == "__main__":
     tf.test.main()
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/random_deletion.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_deletion.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import random
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.layers.RandomDeletion")
 class RandomDeletion(keras.layers.Layer):
     """Augments input by randomly deleting tokens.
 
     This layer comes in handy when you need to generate new data using deletion
@@ -268,7 +268,8 @@
                 "seed": self.seed,
                 "skip_list": self.skip_list,
                 "skip_fn": self.skip_fn,
                 "skip_py_fn": self.skip_py_fn,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/random_deletion_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_deletion_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for RandomDeletion Layer."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers.random_deletion import RandomDeletion
+from keras_nlp.src.layers.random_deletion import RandomDeletion
 
 
 class RandomDeletionTest(tf.test.TestCase):
     def test_shape_and_output_from_word_deletion(self):
         keras.utils.set_random_seed(1337)
         inputs = ["Hey I like", "Keras and Tensorflow"]
         split = tf.strings.split(inputs)
@@ -191,7 +191,8 @@
         inputs = tf.keras.Input(dtype="string", shape=())
         outputs = augmenter(tf.strings.split(inputs))
         model = tf.keras.Model(inputs, outputs)
         model_output = model(input_data)
         self.assertAllEqual(
             model_output, [[b"I", b"like"], [b"and", b"Tensorflow"]]
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/random_swap.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_swap.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import random
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.layers.RandomSwap")
 class RandomSwap(keras.layers.Layer):
     """Augments input by randomly swapping words.
 
     This layer comes in handy when you need to generate new data using swap
@@ -264,7 +264,8 @@
                 "seed": self.seed,
                 "skip_list": self.skip_list,
                 "skip_fn": self.skip_fn,
                 "skip_py_fn": self.skip_py_fn,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/random_swap_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/random_swap_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for RandomSwaps Layer."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers.random_swap import RandomSwap
+from keras_nlp.src.layers.random_swap import RandomSwap
 
 
 class RandomSwapTest(tf.test.TestCase):
     def test_shape_and_output_from_word_swap(self):
         keras.utils.set_random_seed(1337)
         inputs = ["Hey I like", "Keras and Tensorflow"]
         split = tf.strings.split(inputs)
@@ -208,7 +208,8 @@
         model = tf.keras.Model(inputs, outputs)
         model_output = model(input_data)
         exp_output = [
             [b"like", b"I", b"Hey"],
             [b"Tensorflow", b"Keras", b"and"],
         ]
         self.assertAllEqual(model_output, exp_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/sine_position_encoding.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/sine_position_encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Sinusoidal position embedding layer."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.layers.SinePositionEncoding")
 class SinePositionEncoding(keras.layers.Layer):
     """Sinusoidal positional encoding layer.
 
     This layer calculates the position encoding as a mix of sine and cosine
@@ -114,7 +114,8 @@
         config = super().get_config()
         config.update(
             {
                 "max_wavelength": self.max_wavelength,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/sine_position_encoding_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/sine_position_encoding_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for Sinusoidal Positional encoding."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers import sine_position_encoding
+from keras_nlp.src.layers import sine_position_encoding
 
 
 class SinePositionEncodingTest(tf.test.TestCase):
     def test_valid_call(self):
         pos_encoding = sine_position_encoding.SinePositionEncoding()
         model = keras.Sequential(
             [
@@ -184,7 +184,8 @@
         seq_length = 100
         hidden_size = 32
         inputs = keras.Input(shape=(seq_length, hidden_size))
         outputs = pos_encoding(inputs)
 
         # output dtype for this layer should be tf.float16.
         self.assertEqual(outputs.dtype, tf.float16)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/start_end_packer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/start_end_packer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Start End Packer implementation based on `keras.layers.Layer`."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.layers.StartEndPacker")
 class StartEndPacker(keras.layers.Layer):
     """Adds start and end tokens to a sequence and pads to a fixed length.
 
     This layer is useful when tokenizing inputs for tasks like translation,
@@ -178,7 +178,8 @@
                 "start_value": self.start_value,
                 "end_value": self.end_value,
                 "pad_value": self.pad_value,
                 "return_padding_mask": self.return_padding_mask,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/start_end_packer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/start_end_packer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """Tests for Start End Packer layer."""
 
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers.start_end_packer import StartEndPacker
+from keras_nlp.src.layers.start_end_packer import StartEndPacker
 
 
 class StartEndPackerTest(tf.test.TestCase):
     def test_dense_input(self):
         input_data = tf.constant([5, 6, 7])
         start_end_packer = StartEndPacker(sequence_length=5)
         output = start_end_packer(input_data)
@@ -149,7 +149,8 @@
             "sequence_length": 512,
             "start_value": 10,
             "end_value": 20,
             "pad_value": 100,
         }
 
         self.assertEqual(config, {**config, **expected_config_subset})
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/token_and_position_embedding.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/token_and_position_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Creates an Embedding Layer and adds Positional Embeddings"""
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.position_embedding import PositionEmbedding
-from keras_nlp.utils.keras_utils import clone_initializer
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.position_embedding import PositionEmbedding
+from keras_nlp.src.utils.keras_utils import clone_initializer
 
 
 @keras_nlp_export("keras_nlp.layers.TokenAndPositionEmbedding")
 class TokenAndPositionEmbedding(keras.layers.Layer):
     """A layer which sums a token and position embedding.
 
     Token and position embeddings are ways of representing words and their order
@@ -126,7 +126,8 @@
             start_index=start_index,
         )
         outputs = embedded_tokens + embedded_positions
         return outputs
 
     def compute_mask(self, inputs, mask=None):
         return self.token_embedding.compute_mask(inputs, mask=mask)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/token_and_position_embedding_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/token_and_position_embedding_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.layers.token_and_position_embedding import (
+from keras_nlp.src.layers.token_and_position_embedding import (
     TokenAndPositionEmbedding,
 )
 
 
 class TokenAndPositionEmbeddingTest(tf.test.TestCase, parameterized.TestCase):
     def test_get_config_and_from_config(self):
         token_and_position_embed = TokenAndPositionEmbedding(
@@ -154,7 +154,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         loaded_model = keras.models.load_model(path)
 
         model_output = model.predict(data)
         loaded_model_output = loaded_model.predict(data)
         self.assertAllClose(model_output, loaded_model_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_decoder.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 # limitations under the License.
 
 """Transformer decoder block implementation based on `keras.layers.Layer`."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.cached_multi_head_attention import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.cached_multi_head_attention import (
     CachedMultiHeadAttention,
 )
-from keras_nlp.utils.keras_utils import clone_initializer
+from keras_nlp.src.utils.keras_utils import clone_initializer
 
-from keras_nlp.layers.transformer_layer_utils import (  # isort:skip
+from keras_nlp.src.layers.transformer_layer_utils import (  # isort:skip
     compute_causal_mask,
     merge_padding_and_attention_mask,
 )
 
 
 @keras_nlp_export("keras_nlp.layers.TransformerDecoder")
 class TransformerDecoder(keras.layers.Layer):
@@ -360,7 +360,8 @@
                 ),
                 "normalize_first": self.normalize_first,
                 "build_input_shape": self._input_shape,
                 "has_cross_attention": self._has_cross_attention,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_decoder_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_decoder_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
-from keras_nlp.layers import transformer_decoder
+from keras_nlp.src.layers import transformer_decoder
 
 
 class TransformerDecoderTest(tf.test.TestCase, parameterized.TestCase):
     @parameterized.named_parameters(
         ("without_norm_first", False),
         ("with_norm_first", True),
     )
@@ -369,7 +369,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         loaded_model = keras.models.load_model(path)
 
         model_output = model(decoder_sequence)
         loaded_model_output = loaded_model(decoder_sequence)
         self.assertAllClose(model_output, loaded_model_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_encoder.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Transformer encoder block implementation based on `keras.layers.Layer`."""
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.utils.keras_utils import clone_initializer
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.utils.keras_utils import clone_initializer
 
-from keras_nlp.layers.transformer_layer_utils import (  # isort:skip
+from keras_nlp.src.layers.transformer_layer_utils import (  # isort:skip
     merge_padding_and_attention_mask,
 )
 
 
 @keras_nlp_export("keras_nlp.layers.TransformerEncoder")
 class TransformerEncoder(keras.layers.Layer):
     """Transformer encoder.
@@ -230,7 +230,8 @@
                     self.bias_initializer
                 ),
                 "normalize_first": self.normalize_first,
                 "build_input_shape": self._input_shape,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_encoder_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_encoder_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.layers import transformer_encoder
+from keras_nlp.src.layers import transformer_encoder
 
 
 class TransformerEncoderTest(tf.test.TestCase, parameterized.TestCase):
     @parameterized.named_parameters(
         ("without_norm_first", False),
         ("with_norm_first", True),
     )
@@ -179,7 +179,8 @@
         # Don't save traces in the tf format, we check compilation elsewhere.
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
 
         loaded_model = keras.models.load_model(path)
         loaded_model_output = loaded_model(data)
         self.assertAllClose(model_output, loaded_model_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_layer_utils.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_layer_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,7 +99,8 @@
     if attention_mask is not None:
         attention_mask = tf.cast(attention_mask, dtype=tf.int32)
         if mask is None:
             return attention_mask
         else:
             return tf.minimum(mask, attention_mask)
     return mask
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_layer_utils_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/layers/transformer_layer_utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
-import keras_nlp.layers.transformer_layer_utils as utils
+import keras_nlp.src.layers.transformer_layer_utils as utils
 
 
 class TransformerEncoderTest(tf.test.TestCase):
     def test_compute_causal_mask(self):
         mask = utils.compute_causal_mask(1, 2, 2)
         self.assertTrue((mask.numpy() == [[1, 0], [1, 1]]).all())
 
@@ -55,7 +55,8 @@
             attention_mask = tf.convert_to_tensor([[0, 0, 1], [1, 0, 0]])
             inputs = tf.random.uniform(shape=[1, 3, 2])
             utils.merge_padding_and_attention_mask(
                 inputs,
                 padding_mask,
                 attention_mask,
             )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from keras_nlp.metrics.bleu import Bleu
-from keras_nlp.metrics.edit_distance import EditDistance
-from keras_nlp.metrics.perplexity import Perplexity
-from keras_nlp.metrics.rouge_l import RougeL
-from keras_nlp.metrics.rouge_n import RougeN
+from keras_nlp.src.metrics.bleu import Bleu
+from keras_nlp.src.metrics.edit_distance import EditDistance
+from keras_nlp.src.metrics.perplexity import Perplexity
+from keras_nlp.src.metrics.rouge_l import RougeL
+from keras_nlp.src.metrics.rouge_n import RougeN
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/bleu_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/bleu_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 
 """Tests for Bleu."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.metrics.bleu import Bleu
-from keras_nlp.tokenizers.byte_tokenizer import ByteTokenizer
+from keras_nlp.src.metrics.bleu import Bleu
+from keras_nlp.src.tokenizers.byte_tokenizer import ByteTokenizer
 
 
 class BleuTest(tf.test.TestCase):
     def test_initialization(self):
         bleu = Bleu()
         result = bleu.result()
 
@@ -262,7 +262,8 @@
         config = bleu.get_config()
         expected_config_subset = {
             "tokenizer": byte_tokenizer,
             "max_order": 8,
             "smooth": True,
         }
         self.assertEqual(config, {**config, **expected_config_subset})
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/edit_distance.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/edit_distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Edit Distance metric."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.metrics.EditDistance")
 class EditDistance(keras.metrics.Metric):
     """Edit Distance metric.
 
     This class implements the edit distance metric, sometimes called
@@ -221,7 +221,8 @@
         else:
             self._number_of_samples.assign(0.0)
 
     def get_config(self):
         config = super().get_config()
         config.update({"normalize": self.normalize})
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/edit_distance_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/edit_distance_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Tests for EditDistance."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.metrics.edit_distance import EditDistance
+from keras_nlp.src.metrics.edit_distance import EditDistance
 
 
 class EditDistanceTest(tf.test.TestCase):
     def test_initialization(self):
         edit_distance = EditDistance()
         result = edit_distance.result()
 
@@ -294,7 +294,8 @@
         )
 
         config = rouge.get_config()
         expected_config_subset = {
             "normalize": False,
         }
         self.assertEqual(config, {**config, **expected_config_subset})
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/perplexity.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/perplexity.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Perplexity metric."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.metrics.Perplexity")
 class Perplexity(keras.metrics.Metric):
     """Perplexity metric.
 
     This class implements the perplexity metric. In short, this class calculates
@@ -178,7 +178,8 @@
         config.update(
             {
                 "from_logits": self.from_logits,
                 "mask_token_id": self.mask_token_id,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/perplexity_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/perplexity_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for Perplexity."""
 
 import tensorflow as tf
 
-from keras_nlp.metrics.perplexity import Perplexity
+from keras_nlp.src.metrics.perplexity import Perplexity
 
 
 class PerplexityTest(tf.test.TestCase):
     def test_vars_after_initializing_class(self):
         perplexity = Perplexity()
         self.assertEqual(perplexity.result().numpy(), 0.0)
 
@@ -349,7 +349,8 @@
         expected_config = {
             "from_logits": True,
             "mask_token_id": 0,
             "dtype": tf.float32,
             "name": "perplexity_test",
         }
         self.assertEqual(config, expected_config)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_base.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 import types
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.utils.tf_utils import tensor_to_string_list
+from keras_nlp.src.utils.tf_utils import tensor_to_string_list
 
 try:
     from rouge_score import rouge_scorer
 except ImportError:
     rouge_scorer = None
 
 
@@ -219,7 +219,8 @@
         config.update(
             {
                 "variant": self.variant,
                 "use_stemmer": self.use_stemmer,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_l.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_l.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ROUGE-L metric."""
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.metrics.rouge_base import RougeBase
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.metrics.rouge_base import RougeBase
 
 
 @keras_nlp_export("keras_nlp.metrics.RougeL")
 class RougeL(RougeBase):
     """ROUGE-L metric.
 
     This class implements the ROUGE-L variant of the ROUGE metric. The ROUGE-L
@@ -127,7 +127,8 @@
             **kwargs,
         )
 
     def get_config(self):
         config = super().get_config()
         del config["variant"]
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_l_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_l_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Tests for RougeL."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.metrics.rouge_l import RougeL
+from keras_nlp.src.metrics.rouge_l import RougeL
 
 
 class RougeLTest(tf.test.TestCase):
     def setUp(self):
         super().setUp()
 
         def assertDictAlmostEqual(d1, d2, delta=1e-3, typecast_to_numpy=True):
@@ -222,7 +222,8 @@
         )
 
         config = rouge.get_config()
         expected_config_subset = {
             "use_stemmer": True,
         }
         self.assertEqual(config, {**config, **expected_config_subset})
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_n.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_n.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ROUGE-N metric."""
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.metrics.rouge_base import RougeBase
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.metrics.rouge_base import RougeBase
 
 
 @keras_nlp_export("keras_nlp.metrics.RogueN")
 class RougeN(RougeBase):
     """ROUGE-N metric.
 
     This class implements the ROUGE-N variant of the ROUGE metric. The ROUGE-N
@@ -161,7 +161,8 @@
 
         config.update(
             {
                 "order": self.order,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_n_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/metrics/rouge_n_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Tests for RougeN."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.metrics.rouge_n import RougeN
+from keras_nlp.src.metrics.rouge_n import RougeN
 
 
 class RougeNTest(tf.test.TestCase):
     def setUp(self):
         super().setUp()
 
         def assertDictAlmostEqual(d1, d2, delta=1e-3, typecast_to_numpy=True):
@@ -248,7 +248,8 @@
         config = rouge.get_config()
         expected_config_subset = {
             "order": 5,
             "use_stemmer": True,
         }
 
         self.assertEqual(config, {**config, **expected_config_subset})
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,97 +8,98 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.models.albert.albert_classifier import AlbertClassifier
-from keras_nlp.models.albert.albert_masked_lm import AlbertMaskedLM
-from keras_nlp.models.albert.albert_masked_lm_preprocessor import (
+from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
+from keras_nlp.src.models.albert.albert_classifier import AlbertClassifier
+from keras_nlp.src.models.albert.albert_masked_lm import AlbertMaskedLM
+from keras_nlp.src.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
 )
-from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
-from keras_nlp.models.bert.bert_backbone import BertBackbone
-from keras_nlp.models.bert.bert_classifier import BertClassifier
-from keras_nlp.models.bert.bert_masked_lm import BertMaskedLM
-from keras_nlp.models.bert.bert_masked_lm_preprocessor import (
+from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
+from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.bert.bert_backbone import BertBackbone
+from keras_nlp.src.models.bert.bert_classifier import BertClassifier
+from keras_nlp.src.models.bert.bert_masked_lm import BertMaskedLM
+from keras_nlp.src.models.bert.bert_masked_lm_preprocessor import (
     BertMaskedLMPreprocessor,
 )
-from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
-from keras_nlp.models.deberta_v3.deberta_v3_classifier import (
+from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
+from keras_nlp.src.models.deberta_v3.deberta_v3_classifier import (
     DebertaV3Classifier,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_masked_lm import DebertaV3MaskedLM
-from keras_nlp.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm import DebertaV3MaskedLM
+from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
     DebertaV3MaskedLMPreprocessor,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
-from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
-from keras_nlp.models.distil_bert.distil_bert_classifier import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
+from keras_nlp.src.models.distil_bert.distil_bert_classifier import (
     DistilBertClassifier,
 )
-from keras_nlp.models.distil_bert.distil_bert_masked_lm import (
+from keras_nlp.src.models.distil_bert.distil_bert_masked_lm import (
     DistilBertMaskedLM,
 )
-from keras_nlp.models.distil_bert.distil_bert_masked_lm_preprocessor import (
+from keras_nlp.src.models.distil_bert.distil_bert_masked_lm_preprocessor import (
     DistilBertMaskedLMPreprocessor,
 )
-from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
+from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
+from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
-from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
-from keras_nlp.models.f_net.f_net_classifier import FNetClassifier
-from keras_nlp.models.f_net.f_net_masked_lm import FNetMaskedLM
-from keras_nlp.models.f_net.f_net_masked_lm_preprocessor import (
+from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.src.models.f_net.f_net_classifier import FNetClassifier
+from keras_nlp.src.models.f_net.f_net_masked_lm import FNetMaskedLM
+from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import (
     FNetMaskedLMPreprocessor,
 )
-from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
-from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
-from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
-from keras_nlp.models.gpt2.gpt2_causal_lm import GPT2CausalLM
-from keras_nlp.models.gpt2.gpt2_causal_lm_preprocessor import (
+from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.gpt2.gpt2_backbone import GPT2Backbone
+from keras_nlp.src.models.gpt2.gpt2_causal_lm import GPT2CausalLM
+from keras_nlp.src.models.gpt2.gpt2_causal_lm_preprocessor import (
     GPT2CausalLMPreprocessor,
 )
-from keras_nlp.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
-from keras_nlp.models.opt.opt_backbone import OPTBackbone
-from keras_nlp.models.opt.opt_causal_lm import OPTCausalLM
-from keras_nlp.models.opt.opt_causal_lm_preprocessor import (
+from keras_nlp.src.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
+from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
+from keras_nlp.src.models.opt.opt_causal_lm import OPTCausalLM
+from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
     OPTCausalLMPreprocessor,
 )
-from keras_nlp.models.opt.opt_preprocessor import OPTPreprocessor
-from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
-from keras_nlp.models.roberta.roberta_classifier import RobertaClassifier
-from keras_nlp.models.roberta.roberta_masked_lm import RobertaMaskedLM
-from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
+from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
+from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.src.models.roberta.roberta_classifier import RobertaClassifier
+from keras_nlp.src.models.roberta.roberta_masked_lm import RobertaMaskedLM
+from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import (
     RobertaMaskedLMPreprocessor,
 )
-from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
-from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
-from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
-from keras_nlp.models.xlm_roberta.xlm_roberta_classifier import (
+from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_classifier import (
     XLMRobertaClassifier,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm import (
     XLMRobertaMaskedLM,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
     XLMRobertaMaskedLMPreprocessor,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
     XLMRobertaPreprocessor,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 """ALBERT backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.position_embedding import PositionEmbedding
-from keras_nlp.layers.transformer_encoder import TransformerEncoder
-from keras_nlp.models.albert.albert_presets import backbone_presets
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.position_embedding import PositionEmbedding
+from keras_nlp.src.layers.transformer_encoder import TransformerEncoder
+from keras_nlp.src.models.albert.albert_presets import backbone_presets
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 def albert_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.AlbertBackbone")
@@ -275,7 +275,8 @@
     @property
     def token_embedding(self):
         return self.get_layer("token_embedding")
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_backbone_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
+from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
 
 
 class AlbertBackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.backbone = AlbertBackbone(
             vocabulary_size=10,
             num_layers=2,
@@ -134,7 +134,8 @@
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
         self.backbone.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_classifier.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # limitations under the License.
 """ALBERT classification model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.models.albert.albert_backbone import albert_kernel_initializer
-from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.models.albert.albert_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
+from keras_nlp.src.models.albert.albert_backbone import albert_kernel_initializer
+from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
+from keras_nlp.src.models.albert.albert_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.AlbertClassifier")
 class AlbertClassifier(Task):
     """An end-to-end ALBERT model for classification tasks
 
     This model attaches a classification head to a `keras_nlp.model.AlbertBackbone`
@@ -213,7 +213,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return AlbertPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy({**backbone_presets})
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_classifier_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_classifier_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.models.albert.albert_classifier import AlbertClassifier
-from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
+from keras_nlp.src.models.albert.albert_classifier import AlbertClassifier
+from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
+from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
 
 
 class AlbertClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         # Setup model
 
         bytes_io = io.BytesIO()
@@ -137,7 +137,8 @@
 
         # Check we got the real object back
         self.assertIsInstance(restored_model, AlbertClassifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 """ALBERT masked LM model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_head import MaskedLMHead
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.models.albert.albert_backbone import albert_kernel_initializer
-from keras_nlp.models.albert.albert_masked_lm_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_head import MaskedLMHead
+from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
+from keras_nlp.src.models.albert.albert_backbone import albert_kernel_initializer
+from keras_nlp.src.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
 )
-from keras_nlp.models.albert.albert_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.albert.albert_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.AlbertMaskedLM")
 class AlbertMaskedLM(Task):
     """An end-to-end ALBERT model for the masked language modeling task.
 
     This model will train ALBERT on a masked language modeling task.
@@ -146,7 +146,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return AlbertMaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ALBERT masked language model preprocessor layer."""
 
 from absl import logging
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
-from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
+from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 @keras_nlp_export("keras_nlp.models.AlbertMaskedLMPreprocessor")
 class AlbertMaskedLMPreprocessor(AlbertPreprocessor):
     """ALBERT preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
@@ -178,7 +178,8 @@
             "segment_ids": segment_ids,
             "padding_mask": padding_mask,
             "mask_positions": masker_outputs["mask_positions"],
         }
         y = masker_outputs["mask_ids"]
         sample_weight = masker_outputs["mask_weights"]
         return pack_x_y_sample_weight(x, y, sample_weight)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_masked_lm_preprocessor import (
+from keras_nlp.src.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
 )
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
 
 
 class AlbertMaskedLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
@@ -168,7 +168,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         outputs = model(input_data)[0]["token_ids"]
         restored_outputs = restored_model(input_data)[0]["token_ids"]
         self.assertAllEqual(outputs, restored_outputs)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_masked_lm_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.models.albert.albert_masked_lm import AlbertMaskedLM
-from keras_nlp.models.albert.albert_masked_lm_preprocessor import (
+from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
+from keras_nlp.src.models.albert.albert_masked_lm import AlbertMaskedLM
+from keras_nlp.src.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
 )
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
 
 
 class AlbertMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         # Setup model.
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round", "an eagle flew"]
@@ -137,7 +137,8 @@
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, AlbertMaskedLM)
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output, atol=0.01, rtol=0.01)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ALBERT preprocessor layer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
-from keras_nlp.models.albert.albert_presets import backbone_presets
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.multi_segment_packer import MultiSegmentPacker
+from keras_nlp.src.models.albert.albert_presets import backbone_presets
+from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.AlbertPreprocessor")
 class AlbertPreprocessor(Preprocessor):
     """An ALBERT preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -189,7 +189,8 @@
     @classproperty
     def tokenizer_cls(cls):
         return AlbertTokenizer
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_preprocessor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
+from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
 
 
 class AlbertPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -181,7 +181,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_presets.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,7 +132,8 @@
         "preprocessor_config": {},
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/albert_extra_extra_large_en_uncased/v1/model.h5",
         "weights_hash": "a835177b692fb6a82139f94c66db2f22",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/albert_extra_extra_large_en_uncased/v1/vocab.spm",
         "spm_proto_hash": "73e62ff8e90f951f24c8b907913039a5",
     },
 }
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_presets_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.models.albert.albert_classifier import AlbertClassifier
-from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.albert.albert_backbone import AlbertBackbone
+from keras_nlp.src.models.albert.albert_classifier import AlbertClassifier
+from keras_nlp.src.models.albert.albert_preprocessor import AlbertPreprocessor
+from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
 
 
 @pytest.mark.large
 class AlbertPresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
     A smoke test for ALBERT presets we run continuously.
     This only tests the smallest weights we have available. Run with:
@@ -190,7 +190,8 @@
             tokenizer = AlbertTokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
 
     def test_load_preprocessors(self):
         for preset in AlbertPreprocessor.presets:
             preprocessor = AlbertPreprocessor.from_preset(preset)
             preprocessor("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ALBERT tokenizer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.albert.albert_presets import backbone_presets
-from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.albert.albert_presets import backbone_presets
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.AlbertTokenizer")
 class AlbertTokenizer(SentencePieceTokenizer):
     """ALBERT tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -108,7 +108,8 @@
         self.sep_token_id = self.token_to_id(sep_token)
         self.pad_token_id = self.token_to_id(pad_token)
         self.mask_token_id = self.token_to_id(mask_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/albert/albert_tokenizer_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.src.models.albert.albert_tokenizer import AlbertTokenizer
 
 
 class AlbertTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -109,7 +109,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/backbone.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 """Base class for Backbone models."""
 
 import os
 
 from tensorflow import keras
 
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class Backbone(keras.Model):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -122,7 +122,8 @@
         if cls.from_preset.__doc__ is None:
             cls.from_preset.__func__.__doc__ = Backbone.from_preset.__doc__
             format_docstring(
                 model_name=cls.__name__,
                 example_preset_name=next(iter(cls.presets), ""),
                 preset_names='", "'.join(cls.presets),
             )(cls.from_preset.__func__)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 """BART backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers.position_embedding import PositionEmbedding
-from keras_nlp.layers.transformer_decoder import TransformerDecoder
-from keras_nlp.layers.transformer_encoder import TransformerEncoder
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.models.bart.bart_presets import backbone_presets
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.layers.position_embedding import PositionEmbedding
+from keras_nlp.src.layers.transformer_decoder import TransformerDecoder
+from keras_nlp.src.layers.transformer_encoder import TransformerEncoder
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.models.bart.bart_presets import backbone_presets
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 def bart_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
@@ -258,7 +258,8 @@
     @property
     def token_embedding(self):
         return self.get_layer("token_embedding")
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_backbone_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bart.bart_backbone import BartBackbone
+from keras_nlp.src.models.bart.bart_backbone import BartBackbone
 
 
 class BartBackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.model = BartBackbone(
             vocabulary_size=1000,
             num_layers=2,
@@ -140,7 +140,8 @@
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.model.compile()
         self.model.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 """BART preprocessor layer."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
-from keras_nlp.models.bart.bart_presets import backbone_presets
-from keras_nlp.models.bart.bart_tokenizer import BartTokenizer
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.layers.multi_segment_packer import MultiSegmentPacker
+from keras_nlp.src.models.bart.bart_presets import backbone_presets
+from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class BartPreprocessor(Preprocessor):
     """A BART preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -302,7 +302,8 @@
 
         return cls(
             tokenizer=tokenizer,
             encoder_sequence_length=encoder_sequence_length,
             decoder_sequence_length=decoder_sequence_length,
             **kwargs,
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_preprocessor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bart.bart_preprocessor import BartPreprocessor
-from keras_nlp.models.bart.bart_tokenizer import BartTokenizer
+from keras_nlp.src.models.bart.bart_preprocessor import BartPreprocessor
+from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
 
 
 class BartPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         vocab = {
             "<s>": 0,
             "<pad>": 1,
@@ -196,7 +196,8 @@
         model_output = model(input_data)
         restored_model_output = restored_model(input_data)
 
         self.assertAllClose(
             model_output,
             restored_model_output,
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_presets.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,7 +67,8 @@
         "weights_hash": "6bfe7e591af8c5699ce6f9f18753af9a",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/bart_large_en/v1/vocab.json",
         "vocabulary_hash": "cf410ee085c5c69c957bb1f6d8456596",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/bart_large_en/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
 }
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_presets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.bart.bart_backbone import BartBackbone
-from keras_nlp.models.bart.bart_tokenizer import BartTokenizer
+from keras_nlp.src.models.bart.bart_backbone import BartBackbone
+from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
 
 
 @pytest.mark.large
 class BartPresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
     A smoke test for BART presets we run continuously.
 
@@ -133,7 +133,8 @@
             }
             model(input_data)
 
     def test_load_tokenizers(self):
         for preset in BartTokenizer.presets:
             tokenizer = BartTokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 
 """BART Seq2Seq LM preprocessor layer."""
 
 from absl import logging
 from tensorflow import keras
 
-from keras_nlp.models.bart.bart_preprocessor import BartPreprocessor
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.models.bart.bart_preprocessor import BartPreprocessor
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class BartSeq2SeqLMPreprocessor(BartPreprocessor):
     """BART Seq2Seq LM preprocessor.
 
     This layer is used as preprocessor for seq2seq tasks using the BART model.
@@ -181,7 +181,8 @@
             "decoder_padding_mask": decoder_padding_mask[..., :-1],
         }
         # Target `y` will be the decoder input sequence shifted one step to the
         # left (i.e., the next token).
         y = decoder_token_ids[..., 1:]
         sample_weight = decoder_padding_mask[..., 1:]
         return pack_x_y_sample_weight(x, y, sample_weight)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bart.bart_seq_2_seq_lm_preprocessor import (
+from keras_nlp.src.models.bart.bart_seq_2_seq_lm_preprocessor import (
     BartSeq2SeqLMPreprocessor,
 )
-from keras_nlp.models.bart.bart_tokenizer import BartTokenizer
+from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
 
 
 class BartSeq2SeqLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         vocab = {
             "<s>": 0,
             "<pad>": 1,
@@ -155,7 +155,8 @@
         model_output = model(input_data)
         restored_model_output = restored_model(input_data)
 
         self.assertAllClose(
             model_output,
             restored_model_output,
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 """BART tokenizer."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.models.bart.bart_presets import backbone_presets
-from keras_nlp.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.bart.bart_presets import backbone_presets
+from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class BartTokenizer(BytePairTokenizer):
     """A BART tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -117,7 +117,8 @@
     def get_config(self):
         config = super().get_config()
         # In the constructor, we pass the list of special tokens to the
         # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
         # delete it from the config here.
         del config["unsplittable_tokens"]
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bart/bart_tokenizer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bart.bart_tokenizer import BartTokenizer
+from keras_nlp.src.models.bart.bart_tokenizer import BartTokenizer
 
 
 class BartTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         vocab = {
             "<s>": 0,
             "<pad>": 1,
@@ -91,7 +91,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 """BERT backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.position_embedding import PositionEmbedding
-from keras_nlp.layers.transformer_encoder import TransformerEncoder
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.models.bert.bert_presets import backbone_presets
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.position_embedding import PositionEmbedding
+from keras_nlp.src.layers.transformer_encoder import TransformerEncoder
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.models.bert.bert_presets import backbone_presets
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 def bert_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.BertBackbone")
@@ -221,7 +221,8 @@
     @property
     def token_embedding(self):
         return self.get_layer("token_embedding")
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_backbone_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bert.bert_backbone import BertBackbone
+from keras_nlp.src.models.bert.bert_backbone import BertBackbone
 
 
 class BertBackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.backbone = BertBackbone(
             vocabulary_size=10,
             num_layers=2,
@@ -116,7 +116,8 @@
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
         self.backbone.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_classifier.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 # limitations under the License.
 """BERT classification model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.bert.bert_backbone import BertBackbone
-from keras_nlp.models.bert.bert_backbone import bert_kernel_initializer
-from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.models.bert.bert_presets import backbone_presets
-from keras_nlp.models.bert.bert_presets import classifier_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.bert.bert_backbone import BertBackbone
+from keras_nlp.src.models.bert.bert_backbone import bert_kernel_initializer
+from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
+from keras_nlp.src.models.bert.bert_presets import backbone_presets
+from keras_nlp.src.models.bert.bert_presets import classifier_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.BertClassifier")
 class BertClassifier(Task):
     """An end-to-end BERT model for classification tasks.
 
     This model attaches a classification head to a
@@ -197,7 +197,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return BertPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy({**backbone_presets, **classifier_presets})
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_classifier_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_classifier_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bert.bert_backbone import BertBackbone
-from keras_nlp.models.bert.bert_classifier import BertClassifier
-from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.bert.bert_backbone import BertBackbone
+from keras_nlp.src.models.bert.bert_classifier import BertClassifier
+from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 
 
 class BertClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         # Setup model.
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["the", "quick", "brown", "fox", "."]
@@ -112,7 +112,8 @@
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, BertClassifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 # limitations under the License.
 """BERT masked LM model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_head import MaskedLMHead
-from keras_nlp.models.bert.bert_backbone import BertBackbone
-from keras_nlp.models.bert.bert_backbone import bert_kernel_initializer
-from keras_nlp.models.bert.bert_masked_lm_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_head import MaskedLMHead
+from keras_nlp.src.models.bert.bert_backbone import BertBackbone
+from keras_nlp.src.models.bert.bert_backbone import bert_kernel_initializer
+from keras_nlp.src.models.bert.bert_masked_lm_preprocessor import (
     BertMaskedLMPreprocessor,
 )
-from keras_nlp.models.bert.bert_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.bert.bert_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.BertMaskedLM")
 class BertMaskedLM(Task):
     """An end-to-end BERT model for the masked language modeling task.
 
     This model will train BERT on a masked language modeling task.
@@ -147,7 +147,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return BertMaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """BERT masked language model preprocessor layer."""
 
 from absl import logging
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
-from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
+from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 @keras_nlp_export("keras_nlp.models.BertMaskedLMPreprocessor")
 class BertMaskedLMPreprocessor(BertPreprocessor):
     """BERT preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
@@ -183,7 +183,8 @@
             "padding_mask": padding_mask,
             "segment_ids": segment_ids,
             "mask_positions": masker_outputs["mask_positions"],
         }
         y = masker_outputs["mask_ids"]
         sample_weight = masker_outputs["mask_weights"]
         return pack_x_y_sample_weight(x, y, sample_weight)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bert.bert_masked_lm_preprocessor import (
+from keras_nlp.src.models.bert.bert_masked_lm_preprocessor import (
     BertMaskedLMPreprocessor,
 )
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 
 
 class BertMaskedLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
         self.vocab += ["the", "quick", "brown", "fox"]
@@ -152,7 +152,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         outputs = model(input_data)[0]["token_ids"]
         restored_outputs = restored_model(input_data)[0]["token_ids"]
         self.assertAllEqual(outputs, restored_outputs)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_masked_lm_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bert.bert_backbone import BertBackbone
-from keras_nlp.models.bert.bert_masked_lm import BertMaskedLM
-from keras_nlp.models.bert.bert_masked_lm_preprocessor import (
+from keras_nlp.src.models.bert.bert_backbone import BertBackbone
+from keras_nlp.src.models.bert.bert_masked_lm import BertMaskedLM
+from keras_nlp.src.models.bert.bert_masked_lm_preprocessor import (
     BertMaskedLMPreprocessor,
 )
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 
 
 class BertMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         # Setup model.
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["the", "quick", "brown", "fox", "."]
@@ -112,7 +112,8 @@
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, BertMaskedLM)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output, atol=0.01, rtol=0.01)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """BERT preprocessor layer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
-from keras_nlp.models.bert.bert_presets import backbone_presets
-from keras_nlp.models.bert.bert_presets import classifier_presets
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.multi_segment_packer import MultiSegmentPacker
+from keras_nlp.src.models.bert.bert_presets import backbone_presets
+from keras_nlp.src.models.bert.bert_presets import classifier_presets
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 PRESET_NAMES = ", ".join(list(backbone_presets) + list(classifier_presets))
 
 
 @keras_nlp_export("keras_nlp.models.BertPreprocessor")
 class BertPreprocessor(Preprocessor):
     """A BERT preprocessing layer which tokenizes and packs inputs.
@@ -170,7 +170,8 @@
     @classproperty
     def tokenizer_cls(cls):
         return BertTokenizer
 
     @classproperty
     def presets(cls):
         return copy.deepcopy({**backbone_presets, **classifier_presets})
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_preprocessor_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 
 
 class BertPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
         self.vocab += ["the", "quick", "brown", "fox"]
@@ -135,7 +135,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_presets.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,7 +310,8 @@
         },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/bert_tiny_en_uncased_sst2/v1/model.h5",
         "weights_hash": "1f9c2d59f9e229e08f3fbd44239cfb0b",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/bert_tiny_en_uncased_sst2/v1/vocab.txt",
         "vocabulary_hash": "64800d5d8528ce344256daf115d4965e",
     }
 }
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_presets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.bert.bert_backbone import BertBackbone
-from keras_nlp.models.bert.bert_classifier import BertClassifier
-from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.bert.bert_backbone import BertBackbone
+from keras_nlp.src.models.bert.bert_classifier import BertClassifier
+from keras_nlp.src.models.bert.bert_preprocessor import BertPreprocessor
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 
 
 @pytest.mark.large
 class BertPresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
     A smoke test for BERT presets we run continuously.
 
@@ -238,7 +238,8 @@
             tokenizer = BertTokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
 
     def test_load_preprocessors(self):
         for preset in BertPreprocessor.presets:
             preprocessor = BertPreprocessor.from_preset(preset)
             preprocessor("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """BERT tokenizer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.bert.bert_presets import backbone_presets
-from keras_nlp.models.bert.bert_presets import classifier_presets
-from keras_nlp.tokenizers.word_piece_tokenizer import WordPieceTokenizer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.bert.bert_presets import backbone_presets
+from keras_nlp.src.models.bert.bert_presets import classifier_presets
+from keras_nlp.src.tokenizers.word_piece_tokenizer import WordPieceTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 PRESET_NAMES = ", ".join(list(backbone_presets) + list(classifier_presets))
 
 
 @keras_nlp_export("keras_nlp.models.BertTokenizer")
 class BertTokenizer(WordPieceTokenizer):
     """A BERT tokenizer using WordPiece subword segmentation.
@@ -102,7 +102,8 @@
         self.sep_token_id = self.token_to_id(sep_token)
         self.pad_token_id = self.token_to_id(pad_token)
         self.mask_token_id = self.token_to_id(mask_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy({**backbone_presets, **classifier_presets})
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/bert/bert_tokenizer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.src.models.bert.bert_tokenizer import BertTokenizer
 
 
 class BertTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
         self.vocab += ["the", "quick", "brown", "fox"]
@@ -82,7 +82,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 """DeBERTa backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
-from keras_nlp.models.deberta_v3.disentangled_attention_encoder import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
+from keras_nlp.src.models.deberta_v3.disentangled_attention_encoder import (
     DisentangledAttentionEncoder,
 )
-from keras_nlp.models.deberta_v3.relative_embedding import RelativeEmbedding
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.deberta_v3.relative_embedding import RelativeEmbedding
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 def deberta_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3Backbone")
@@ -207,7 +207,8 @@
     @property
     def token_embedding(self):
         return self.get_layer("token_embedding")
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
+from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
 
 
 class DebertaV3BackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.backbone = DebertaV3Backbone(
             vocabulary_size=10,
             num_layers=2,
@@ -118,7 +118,8 @@
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
         self.backbone.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 """DeBERTa classification model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
+from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import (
     deberta_kernel_initializer,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3Classifier")
 class DebertaV3Classifier(Task):
     """An end-to-end DeBERTa model for classification tasks.
 
     This model attaches a classification head to a
@@ -229,7 +229,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return DebertaV3Preprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
-from keras_nlp.models.deberta_v3.deberta_v3_classifier import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
+from keras_nlp.src.models.deberta_v3.deberta_v3_classifier import (
     DebertaV3Classifier,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 
 
 class DebertaV3ClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -135,7 +135,8 @@
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, DebertaV3Classifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 # limitations under the License.
 """DeBERTaV3 masked lm model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_head import MaskedLMHead
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_head import MaskedLMHead
+from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
+from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import (
     deberta_kernel_initializer,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
     DebertaV3MaskedLMPreprocessor,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3MaskedLM")
 class DebertaV3MaskedLM(Task):
     """An end-to-end DeBERTaV3 model for the masked language modeling task.
 
     This model will train DeBERTaV3 on a masked language modeling task.
@@ -153,7 +153,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return DebertaV3MaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """DeBERTa masked language model preprocessor layer."""
 
 from absl import logging
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
-from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
+from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3MaskedLMPreprocessor")
 class DebertaV3MaskedLMPreprocessor(DebertaV3Preprocessor):
     """DeBERTa preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
@@ -174,7 +174,8 @@
             "token_ids": masker_outputs["token_ids"],
             "padding_mask": padding_mask,
             "mask_positions": masker_outputs["mask_positions"],
         }
         y = masker_outputs["mask_ids"]
         sample_weight = masker_outputs["mask_weights"]
         return pack_x_y_sample_weight(x, y, sample_weight)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
     DebertaV3MaskedLMPreprocessor,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 
 
 class DebertaV3PreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -165,7 +165,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         outputs = model(input_data)[0]["token_ids"]
         restored_outputs = restored_model(input_data)[0]["token_ids"]
         self.assertAllEqual(outputs, restored_outputs)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
-from keras_nlp.models.deberta_v3.deberta_v3_masked_lm import DebertaV3MaskedLM
-from keras_nlp.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
+from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm import DebertaV3MaskedLM
+from keras_nlp.src.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
     DebertaV3MaskedLMPreprocessor,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 
 
 class DebertaV3MaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round", "an eagle flew"]
@@ -126,7 +126,8 @@
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, DebertaV3MaskedLM)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output, atol=0.01, rtol=0.01)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """DeBERTa preprocessor layer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
-from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.multi_segment_packer import MultiSegmentPacker
+from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3Preprocessor")
 class DebertaV3Preprocessor(Preprocessor):
     """A DeBERTa preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -186,7 +186,8 @@
     @classproperty
     def tokenizer_cls(cls):
         return DebertaV3Tokenizer
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 
 
 class DebertaV3PreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -160,7 +160,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,7 +146,8 @@
         "preprocessor_config": {},
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_base_multi/v1/model.h5",
         "weights_hash": "26e5a824b26afd2ee336835bd337bbeb",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_base_multi/v1/vocab.spm",
         "spm_proto_hash": "b4ca07289eac48600b29529119d565e2",
     },
 }
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
-from keras_nlp.models.deberta_v3.deberta_v3_classifier import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
+from keras_nlp.src.models.deberta_v3.deberta_v3_classifier import (
     DebertaV3Classifier,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
+from keras_nlp.src.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 
 
 @pytest.mark.large
 class DebertaV3PresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
     A smoke test for DeBERTa presets we run continuously.
 
@@ -196,7 +196,8 @@
             tokenizer = DebertaV3Tokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
 
     def test_load_preprocessors(self):
         for preset in DebertaV3Preprocessor.presets:
             preprocessor = DebertaV3Preprocessor.from_preset(preset)
             preprocessor("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 """DeBERTa tokenizer."""
 
 import copy
 
 import tensorflow as tf
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
-from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.deberta_v3.deberta_v3_presets import backbone_presets
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DebertaV3Tokenizer")
 class DebertaV3Tokenizer(SentencePieceTokenizer):
     """DeBERTa tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -148,7 +148,8 @@
     def detokenize(self, ids):
         ids = tf.ragged.boolean_mask(ids, tf.not_equal(ids, self.mask_token_id))
         return super().detokenize(ids)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.src.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 
 
 class DebertaV3TokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -121,7 +121,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/disentangled_attention_encoder.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Disentangled attention encoder block implementation based on `keras.layers.Layer`."""
 
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.disentangled_self_attention import (
+from keras_nlp.src.models.deberta_v3.disentangled_self_attention import (
     DisentangledSelfAttention,
 )
-from keras_nlp.utils.keras_utils import clone_initializer
+from keras_nlp.src.utils.keras_utils import clone_initializer
 
-from keras_nlp.layers.transformer_layer_utils import (  # isort:skip
+from keras_nlp.src.layers.transformer_layer_utils import (  # isort:skip
     merge_padding_and_attention_mask,
 )
 
 
 class DisentangledAttentionEncoder(keras.layers.Layer):
     """Disentangled attention encoder.
 
@@ -210,7 +210,8 @@
                 "bias_initializer": keras.initializers.serialize(
                     self.bias_initializer
                 ),
                 "build_input_shape": self._input_shape,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/disentangled_self_attention.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/disentangled_self_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Disentangled self-attention layer."""
 
 import math
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.utils.keras_utils import clone_initializer
+from keras_nlp.src.utils.keras_utils import clone_initializer
 
 
 class DisentangledSelfAttention(keras.layers.Layer):
     """DisentangledSelfAttention layer.
 
     This is an implementation of disentangled self-attention as described in the
     paper ["DeBERTaV3: Improving DeBERTa using ELECTRA-Style Pre-Training with Gradient-Disentangled Embedding Sharing"](https://arxiv.org/abs/2111.09543).
@@ -370,7 +370,8 @@
                 ),
                 "bias_initializer": keras.initializers.serialize(
                     self._bias_initializer
                 ),
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/relative_embedding.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/deberta_v3/relative_embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,7 +83,8 @@
                 "layer_norm_epsilon": self.layer_norm_epsilon,
                 "kernel_initializer": keras.initializers.serialize(
                     self.kernel_initializer
                 ),
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 """DistilBERT backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.token_and_position_embedding import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.token_and_position_embedding import (
     TokenAndPositionEmbedding,
 )
-from keras_nlp.layers.transformer_encoder import TransformerEncoder
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.layers.transformer_encoder import TransformerEncoder
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 def distilbert_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertBackbone")
@@ -184,7 +184,8 @@
     @property
     def token_embedding(self):
         return self.get_layer("token_and_position_embedding").token_embedding
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 
 
 class DistilBertTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.backbone = DistilBertBackbone(
             vocabulary_size=10,
             num_layers=2,
@@ -111,7 +111,8 @@
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
         self.backbone.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_classifier.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 """DistilBERT classification model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
-from keras_nlp.models.distil_bert.distil_bert_backbone import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import (
     distilbert_kernel_initializer,
 )
-from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
+from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
-from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertClassifier")
 class DistilBertClassifier(Task):
     """An end-to-end DistilBERT model for classification tasks.
 
     This model attaches a classification head to a
@@ -214,7 +214,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return DistilBertPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_classifier_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
-from keras_nlp.models.distil_bert.distil_bert_classifier import (
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
+from keras_nlp.src.models.distil_bert.distil_bert_classifier import (
     DistilBertClassifier,
 )
-from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
+from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
+from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 
 
 class DistilBertClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         # Setup model
@@ -119,7 +119,8 @@
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, DistilBertClassifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 # limitations under the License.
 """DistilBERT masked lm model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_head import MaskedLMHead
-from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
-from keras_nlp.models.distil_bert.distil_bert_backbone import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_head import MaskedLMHead
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import (
     distilbert_kernel_initializer,
 )
-from keras_nlp.models.distil_bert.distil_bert_masked_lm_preprocessor import (
+from keras_nlp.src.models.distil_bert.distil_bert_masked_lm_preprocessor import (
     DistilBertMaskedLMPreprocessor,
 )
-from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertMaskedLM")
 class DistilBertMaskedLM(Task):
     """An end-to-end DistilBERT model for the masked language modeling task.
 
     This model will train DistilBERT on a masked language modeling task.
@@ -151,7 +151,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return DistilBertMaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """DistilBERT masked language model preprocessor layer."""
 
 from absl import logging
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
-from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
+from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertMaskedLMPrerprocessor")
 class DistilBertMaskedLMPreprocessor(DistilBertPreprocessor):
     """DistilBERT preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
@@ -179,7 +179,8 @@
             "token_ids": masker_outputs["token_ids"],
             "padding_mask": padding_mask,
             "mask_positions": masker_outputs["mask_positions"],
         }
         y = masker_outputs["mask_ids"]
         sample_weight = masker_outputs["mask_weights"]
         return pack_x_y_sample_weight(x, y, sample_weight)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,138 +1,139 @@
-# Copyright 2022 The KerasNLP Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""Tests for DistilBERT masked language model preprocessor layer."""
-
-import os
-
-import pytest
-import tensorflow as tf
-from absl.testing import parameterized
-from tensorflow import keras
-
-from keras_nlp.models.distil_bert.distil_bert_masked_lm_preprocessor import (
-    DistilBertMaskedLMPreprocessor,
-)
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
-    DistilBertTokenizer,
-)
-
-
-class DistilBertMaskedLMPreprocessorTest(
-    tf.test.TestCase, parameterized.TestCase
-):
-    def setUp(self):
-        self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
-        self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
-        self.vocab += ["the", "quick", "brown", "fox"]
-
-        self.preprocessor = DistilBertMaskedLMPreprocessor(
-            tokenizer=DistilBertTokenizer(
-                vocabulary=self.vocab,
-            ),
-            # Simplify out testing by masking every available token.
-            mask_selection_rate=1.0,
-            mask_token_rate=1.0,
-            random_token_rate=0.0,
-            mask_selection_length=5,
-            sequence_length=8,
-        )
-
-    def test_preprocess_strings(self):
-        input_data = " THE QUICK BROWN FOX."
-
-        x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [2, 4, 4, 4, 4, 4, 3, 0])
-        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
-        self.assertAllEqual(x["mask_positions"], [1, 2, 3, 4, 5])
-        self.assertAllEqual(y, [5, 6, 7, 8, 1])
-        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0, 1.0])
-
-    def test_preprocess_list_of_strings(self):
-        input_data = [" THE QUICK BROWN FOX."] * 4
-
-        x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[2, 4, 4, 4, 4, 4, 3, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4, 5]] * 4)
-        self.assertAllEqual(y, [[5, 6, 7, 8, 1]] * 4)
-        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0, 1.0]] * 4)
-
-    def test_preprocess_dataset(self):
-        sentences = tf.constant([" THE QUICK BROWN FOX."] * 4)
-        ds = tf.data.Dataset.from_tensor_slices(sentences)
-        ds = ds.map(self.preprocessor)
-        x, y, sw = ds.batch(4).take(1).get_single_element()
-        self.assertAllEqual(x["token_ids"], [[2, 4, 4, 4, 4, 4, 3, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4, 5]] * 4)
-        self.assertAllEqual(y, [[5, 6, 7, 8, 1]] * 4)
-        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0, 1.0]] * 4)
-
-    def test_mask_multiple_sentences(self):
-        sentence_one = tf.constant(" THE QUICK")
-        sentence_two = tf.constant(" BROWN FOX.")
-
-        x, y, sw = self.preprocessor((sentence_one, sentence_two))
-        self.assertAllEqual(x["token_ids"], [2, 4, 4, 3, 4, 4, 4, 3])
-        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1])
-        self.assertAllEqual(x["mask_positions"], [1, 2, 4, 5, 6])
-        self.assertAllEqual(y, [5, 6, 7, 8, 1])
-        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0, 1.0])
-
-    def test_no_masking_zero_rate(self):
-        no_mask_preprocessor = DistilBertMaskedLMPreprocessor(
-            self.preprocessor.tokenizer,
-            mask_selection_rate=0.0,
-            mask_selection_length=5,
-            sequence_length=8,
-        )
-        input_data = " THE QUICK BROWN FOX."
-
-        x, y, sw = no_mask_preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [2, 5, 6, 7, 8, 1, 3, 0])
-        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
-        self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0, 0])
-        self.assertAllEqual(y, [0, 0, 0, 0, 0])
-        self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0, 0.0])
-
-    def test_serialization(self):
-        config = keras.utils.serialize_keras_object(self.preprocessor)
-        new_preprocessor = keras.utils.deserialize_keras_object(config)
-        self.assertEqual(
-            new_preprocessor.get_config(),
-            self.preprocessor.get_config(),
-        )
-
-    @parameterized.named_parameters(
-        ("tf_format", "tf", "model"),
-        ("keras_format", "keras_v3", "model.keras"),
-    )
-    @pytest.mark.large
-    def test_saved_model(self, save_format, filename):
-        input_data = tf.constant([" THE QUICK BROWN FOX."])
-
-        inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
-        model = keras.Model(inputs, outputs)
-
+# Copyright 2022 The KerasNLP Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""Tests for DistilBERT masked language model preprocessor layer."""
+
+import os
+
+import pytest
+import tensorflow as tf
+from absl.testing import parameterized
+from tensorflow import keras
+
+from keras_nlp.src.models.distil_bert.distil_bert_masked_lm_preprocessor import (
+    DistilBertMaskedLMPreprocessor,
+)
+from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
+    DistilBertTokenizer,
+)
+
+
+class DistilBertMaskedLMPreprocessorTest(
+    tf.test.TestCase, parameterized.TestCase
+):
+    def setUp(self):
+        self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
+        self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
+        self.vocab += ["the", "quick", "brown", "fox"]
+
+        self.preprocessor = DistilBertMaskedLMPreprocessor(
+            tokenizer=DistilBertTokenizer(
+                vocabulary=self.vocab,
+            ),
+            # Simplify out testing by masking every available token.
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=5,
+            sequence_length=8,
+        )
+
+    def test_preprocess_strings(self):
+        input_data = " THE QUICK BROWN FOX."
+
+        x, y, sw = self.preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [2, 4, 4, 4, 4, 4, 3, 0])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
+        self.assertAllEqual(x["mask_positions"], [1, 2, 3, 4, 5])
+        self.assertAllEqual(y, [5, 6, 7, 8, 1])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0, 1.0])
+
+    def test_preprocess_list_of_strings(self):
+        input_data = [" THE QUICK BROWN FOX."] * 4
+
+        x, y, sw = self.preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [[2, 4, 4, 4, 4, 4, 3, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4, 5]] * 4)
+        self.assertAllEqual(y, [[5, 6, 7, 8, 1]] * 4)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0, 1.0]] * 4)
+
+    def test_preprocess_dataset(self):
+        sentences = tf.constant([" THE QUICK BROWN FOX."] * 4)
+        ds = tf.data.Dataset.from_tensor_slices(sentences)
+        ds = ds.map(self.preprocessor)
+        x, y, sw = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(x["token_ids"], [[2, 4, 4, 4, 4, 4, 3, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4, 5]] * 4)
+        self.assertAllEqual(y, [[5, 6, 7, 8, 1]] * 4)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0, 1.0]] * 4)
+
+    def test_mask_multiple_sentences(self):
+        sentence_one = tf.constant(" THE QUICK")
+        sentence_two = tf.constant(" BROWN FOX.")
+
+        x, y, sw = self.preprocessor((sentence_one, sentence_two))
+        self.assertAllEqual(x["token_ids"], [2, 4, 4, 3, 4, 4, 4, 3])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1])
+        self.assertAllEqual(x["mask_positions"], [1, 2, 4, 5, 6])
+        self.assertAllEqual(y, [5, 6, 7, 8, 1])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0, 1.0])
+
+    def test_no_masking_zero_rate(self):
+        no_mask_preprocessor = DistilBertMaskedLMPreprocessor(
+            self.preprocessor.tokenizer,
+            mask_selection_rate=0.0,
+            mask_selection_length=5,
+            sequence_length=8,
+        )
+        input_data = " THE QUICK BROWN FOX."
+
+        x, y, sw = no_mask_preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [2, 5, 6, 7, 8, 1, 3, 0])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
+        self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0, 0])
+        self.assertAllEqual(y, [0, 0, 0, 0, 0])
+        self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0, 0.0])
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
+
+    @parameterized.named_parameters(
+        ("tf_format", "tf", "model"),
+        ("keras_format", "keras_v3", "model.keras"),
+    )
+    @pytest.mark.large
+    def test_saved_model(self, save_format, filename):
+        input_data = tf.constant([" THE QUICK BROWN FOX."])
+
+        inputs = keras.Input(dtype="string", shape=())
+        outputs = self.preprocessor(inputs)
+        model = keras.Model(inputs, outputs)
+
         path = os.path.join(self.get_temp_dir(), filename)
         # Don't save traces in the tf format, we check compilation elsewhere.
-        kwargs = {"save_traces": False} if save_format == "tf" else {}
-        model.save(path, save_format=save_format, **kwargs)
-
-        restored_model = keras.models.load_model(path)
-        outputs = model(input_data)[0]["token_ids"]
-        restored_outputs = restored_model(input_data)[0]["token_ids"]
-        self.assertAllEqual(outputs, restored_outputs)
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
+
+        restored_model = keras.models.load_model(path)
+        outputs = model(input_data)[0]["token_ids"]
+        restored_outputs = restored_model(input_data)[0]["token_ids"]
+        self.assertAllEqual(outputs, restored_outputs)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
-from keras_nlp.models.distil_bert.distil_bert_masked_lm import (
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
+from keras_nlp.src.models.distil_bert.distil_bert_masked_lm import (
     DistilBertMaskedLM,
 )
-from keras_nlp.models.distil_bert.distil_bert_masked_lm_preprocessor import (
+from keras_nlp.src.models.distil_bert.distil_bert_masked_lm_preprocessor import (
     DistilBertMaskedLMPreprocessor,
 )
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
+from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 
 
 class DistilBertMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         # Setup model.
@@ -106,7 +106,8 @@
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, DistilBertMaskedLM)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output, atol=0.01, rtol=0.01)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """DistilBERT preprocessor layers."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
-from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.multi_segment_packer import MultiSegmentPacker
+from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
+from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertPreprocessor")
 class DistilBertPreprocessor(Preprocessor):
     """A DistilBERT preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -157,7 +157,8 @@
     @classproperty
     def tokenizer_cls(cls):
         return DistilBertTokenizer
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
+from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
+from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 
 
 class DistilBertPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
@@ -125,7 +125,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_presets.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,7 +96,8 @@
         },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/distil_bert_base_multi/v1/model.h5",
         "weights_hash": "c0f11095e2a6455bd3b1a6d14800a7fa",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/distil_bert_base_multi/v1/vocab.txt",
         "vocabulary_hash": "d9d865138d17f1958502ed060ecfeeb6",
     },
 }
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_presets_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
-from keras_nlp.models.distil_bert.distil_bert_classifier import (
+from keras_nlp.src.models.distil_bert.distil_bert_backbone import DistilBertBackbone
+from keras_nlp.src.models.distil_bert.distil_bert_classifier import (
     DistilBertClassifier,
 )
-from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
+from keras_nlp.src.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
+from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 
 
 @pytest.mark.large
 class DistilBertPresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
@@ -187,7 +187,8 @@
             tokenizer = DistilBertTokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
 
     def test_load_preprocessors(self):
         for preset in DistilBertPreprocessor.presets:
             preprocessor = DistilBertPreprocessor.from_preset(preset)
             preprocessor("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """DistilBERT tokenizer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
-from keras_nlp.tokenizers.word_piece_tokenizer import WordPieceTokenizer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.distil_bert.distil_bert_presets import backbone_presets
+from keras_nlp.src.tokenizers.word_piece_tokenizer import WordPieceTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.DistilBertTokenizer")
 class DistilBertTokenizer(WordPieceTokenizer):
     """A DistilBERT tokenizer using WordPiece subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -100,7 +100,8 @@
         self.sep_token_id = self.token_to_id(sep_token)
         self.pad_token_id = self.token_to_id(pad_token)
         self.mask_token_id = self.token_to_id(mask_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
+from keras_nlp.src.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 
 
 class DistilBertTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
@@ -84,7 +84,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 """FNet backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.f_net_encoder import FNetEncoder
-from keras_nlp.layers.position_embedding import PositionEmbedding
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.models.f_net.f_net_presets import backbone_presets
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.f_net_encoder import FNetEncoder
+from keras_nlp.src.layers.position_embedding import PositionEmbedding
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 def f_net_kernel_initializer(stddev=0.02):
     return keras.initializers.RandomNormal(stddev=stddev)
 
 
 def f_net_bias_initializer(stddev=0.02):
@@ -223,7 +223,8 @@
     @property
     def token_embedding(self):
         return self.get_layer("token_embedding")
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_backbone_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
 
 
 class FNetBackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.backbone = FNetBackbone(
             vocabulary_size=10,
             num_layers=2,
@@ -109,7 +109,8 @@
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
         self.backbone.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_classifier.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_classifier.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,170 +1,171 @@
-# Copyright 2022 The KerasNLP Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""FNet classification model."""
-
-import copy
-
-from tensorflow import keras
-
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
-from keras_nlp.models.f_net.f_net_backbone import f_net_kernel_initializer
-from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
-from keras_nlp.models.f_net.f_net_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
-
-
-@keras_nlp_export("keras_nlp.models.FNetClassifier")
-class FNetClassifier(Task):
-    """An end-to-end f_net model for classification tasks.
-
-    This model attaches a classification head to a
-    `keras_nlp.model.FNetBackbone` instance, mapping from the backbone outputs
-    to logits suitable for a classification task. For usage of this model with
-    pre-trained weights, use the `from_preset()` constructor.
-
-    This model can optionally be configured with a `preprocessor` layer, in
-    which case it will automatically apply preprocessing to raw inputs during
-    `fit()`, `predict()`, and `evaluate()`. This is done by default when
-    creating the model with `from_preset()`.
-
-    Disclaimer: Pre-trained models are provided on an "as is" basis, without
-    warranties or conditions of any kind.
-
-    Args:
-        backbone: A `keras_nlp.models.FNetBackbone` instance.
-        num_classes: int. Number of classes to predict.
-        preprocessor: A `keras_nlp.models.FNetPreprocessor` or `None`. If
-            `None`, this model will not apply preprocessing, and inputs should
-            be preprocessed before calling the model.
-        activation: Optional `str` or callable, defaults to `None`. The
-            activation function to use on the model outputs. Set
-            `activation="softmax"` to return output probabilities.
-        hidden_dim: int. The size of the pooler layer.
-        dropout: float. The dropout probability value, applied after the dense
-            layer.
-
-    Examples:
-
-    Raw string data.
-    ```python
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
-    labels = [0, 3]
-
-    # Pretrained classifier.
-    classifier = keras_nlp.models.FNetClassifier.from_preset(
-        "f_net_base_en",
-        num_classes=4,
-    )
-    classifier.fit(x=features, y=labels, batch_size=2)
-    classifier.predict(x=features, batch_size=2)
-
-    # Re-compile (e.g., with a new learning rate).
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-        optimizer=keras.optimizers.Adam(5e-5),
-        jit_compile=True,
-    )
-    # Access backbone programatically (e.g., to change `trainable`).
-    classifier.backbone.trainable = False
-    # Fit again.
-    classifier.fit(x=features, y=labels, batch_size=2)
-    ```
-
-    Preprocessed integer data.
-    ```python
-    features = {
-        "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
-        "segment_ids": tf.constant(
-            [[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
-        ),
-    }
-    labels = [0, 3]
-
-    # Pretrained classifier without preprocessing.
-    classifier = keras_nlp.models.FNetClassifier.from_preset(
-        "f_net_base_en",
-        num_classes=4,
-        preprocessor=None,
-    )
-    classifier.fit(x=features, y=labels, batch_size=2)
-    ```
-    """
-
-    def __init__(
-        self,
-        backbone,
-        num_classes,
-        preprocessor=None,
-        activation=None,
-        dropout=0.1,
-        **kwargs,
-    ):
-        inputs = backbone.input
-        pooled = backbone(inputs)["pooled_output"]
-        pooled = keras.layers.Dropout(dropout)(pooled)
-        outputs = keras.layers.Dense(
-            num_classes,
-            kernel_initializer=f_net_kernel_initializer(),
-            activation=activation,
-            name="logits",
-        )(pooled)
-        # Instantiate using Functional API Model constructor
-        super().__init__(
-            inputs=inputs,
-            outputs=outputs,
-            include_preprocessing=preprocessor is not None,
-            **kwargs,
-        )
-        # All references to `self` below this line
-        self.backbone = backbone
-        self.preprocessor = preprocessor
-        self.num_classes = num_classes
-        self.activation = keras.activations.get(activation)
-        self.dropout = dropout
-
-        self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(
-                from_logits=activation is None
-            ),
-            optimizer=keras.optimizers.Adam(5e-5),
-            metrics=keras.metrics.SparseCategoricalAccuracy(),
-            jit_compile=is_xla_compatible(self),
-        )
-
-    def get_config(self):
-        config = super().get_config()
-        config.update(
-            {
-                "num_classes": self.num_classes,
-                "dropout": self.dropout,
-                "activation": keras.activations.serialize(self.activation),
-            }
-        )
-        return config
-
-    @classproperty
-    def backbone_cls(cls):
-        return FNetBackbone
-
-    @classproperty
-    def preprocessor_cls(cls):
-        return FNetPreprocessor
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
+# Copyright 2022 The KerasNLP Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""FNet classification model."""
+
+import copy
+
+from tensorflow import keras
+
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.src.models.f_net.f_net_backbone import f_net_kernel_initializer
+from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
+from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
+
+
+@keras_nlp_export("keras_nlp.models.FNetClassifier")
+class FNetClassifier(Task):
+    """An end-to-end f_net model for classification tasks.
+
+    This model attaches a classification head to a
+    `keras_nlp.model.FNetBackbone` instance, mapping from the backbone outputs
+    to logits suitable for a classification task. For usage of this model with
+    pre-trained weights, use the `from_preset()` constructor.
+
+    This model can optionally be configured with a `preprocessor` layer, in
+    which case it will automatically apply preprocessing to raw inputs during
+    `fit()`, `predict()`, and `evaluate()`. This is done by default when
+    creating the model with `from_preset()`.
+
+    Disclaimer: Pre-trained models are provided on an "as is" basis, without
+    warranties or conditions of any kind.
+
+    Args:
+        backbone: A `keras_nlp.models.FNetBackbone` instance.
+        num_classes: int. Number of classes to predict.
+        preprocessor: A `keras_nlp.models.FNetPreprocessor` or `None`. If
+            `None`, this model will not apply preprocessing, and inputs should
+            be preprocessed before calling the model.
+        activation: Optional `str` or callable, defaults to `None`. The
+            activation function to use on the model outputs. Set
+            `activation="softmax"` to return output probabilities.
+        hidden_dim: int. The size of the pooler layer.
+        dropout: float. The dropout probability value, applied after the dense
+            layer.
+
+    Examples:
+
+    Raw string data.
+    ```python
+    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    labels = [0, 3]
+
+    # Pretrained classifier.
+    classifier = keras_nlp.models.FNetClassifier.from_preset(
+        "f_net_base_en",
+        num_classes=4,
+    )
+    classifier.fit(x=features, y=labels, batch_size=2)
+    classifier.predict(x=features, batch_size=2)
+
+    # Re-compile (e.g., with a new learning rate).
+    classifier.compile(
+        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
+    )
+    # Access backbone programatically (e.g., to change `trainable`).
+    classifier.backbone.trainable = False
+    # Fit again.
+    classifier.fit(x=features, y=labels, batch_size=2)
+    ```
+
+    Preprocessed integer data.
+    ```python
+    features = {
+        "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
+        "segment_ids": tf.constant(
+            [[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
+        ),
+    }
+    labels = [0, 3]
+
+    # Pretrained classifier without preprocessing.
+    classifier = keras_nlp.models.FNetClassifier.from_preset(
+        "f_net_base_en",
+        num_classes=4,
+        preprocessor=None,
+    )
+    classifier.fit(x=features, y=labels, batch_size=2)
+    ```
+    """
+
+    def __init__(
+        self,
+        backbone,
+        num_classes,
+        preprocessor=None,
+        activation=None,
+        dropout=0.1,
+        **kwargs,
+    ):
+        inputs = backbone.input
+        pooled = backbone(inputs)["pooled_output"]
+        pooled = keras.layers.Dropout(dropout)(pooled)
+        outputs = keras.layers.Dense(
+            num_classes,
+            kernel_initializer=f_net_kernel_initializer(),
+            activation=activation,
+            name="logits",
+        )(pooled)
+        # Instantiate using Functional API Model constructor
+        super().__init__(
+            inputs=inputs,
+            outputs=outputs,
+            include_preprocessing=preprocessor is not None,
+            **kwargs,
+        )
+        # All references to `self` below this line
+        self.backbone = backbone
+        self.preprocessor = preprocessor
+        self.num_classes = num_classes
+        self.activation = keras.activations.get(activation)
+        self.dropout = dropout
+
+        self.compile(
+            loss=keras.losses.SparseCategoricalCrossentropy(
+                from_logits=activation is None
+            ),
+            optimizer=keras.optimizers.Adam(5e-5),
+            metrics=keras.metrics.SparseCategoricalAccuracy(),
+            jit_compile=is_xla_compatible(self),
+        )
+
+    def get_config(self):
+        config = super().get_config()
+        config.update(
+            {
+                "num_classes": self.num_classes,
+                "dropout": self.dropout,
+                "activation": keras.activations.serialize(self.activation),
+            }
+        )
+        return config
+
+    @classproperty
+    def backbone_cls(cls):
+        return FNetBackbone
+
+    @classproperty
+    def preprocessor_cls(cls):
+        return FNetPreprocessor
+
+    @classproperty
+    def presets(cls):
+        return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_classifier_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,140 +1,137 @@
-# Copyright 2023 The KerasNLP Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Tests for FNet classification model."""
-
-import io
-import os
-
-import pytest
-import sentencepiece
-import tensorflow as tf
-from absl.testing import parameterized
-from tensorflow import keras
-
-from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
-from keras_nlp.models.f_net.f_net_classifier import FNetClassifier
-from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
-from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
-
-
-class FNetClassifierTest(tf.test.TestCase, parameterized.TestCase):
-    def setUp(self):
-        # Setup Model
-        bytes_io = io.BytesIO()
-        vocab_data = tf.data.Dataset.from_tensor_slices(
-            ["the quick brown fox", "the earth is round"]
-        )
-
-        sentencepiece.SentencePieceTrainer.train(
-            sentence_iterator=vocab_data.as_numpy_iterator(),
-            model_writer=bytes_io,
-            vocab_size=12,
-            model_type="WORD",
-            pad_id=3,
-            unk_id=0,
-            bos_id=4,
-            eos_id=5,
-            pad_piece="<pad>",
-            unk_piece="<unk>",
-            bos_piece="[CLS]",
-            eos_piece="[SEP]",
-            user_defined_symbols="[MASK]",
-        )
-
-        self.proto = bytes_io.getvalue()
-
-        self.preprocessor = FNetPreprocessor(
-            tokenizer=FNetTokenizer(proto=self.proto),
-            sequence_length=8,
-        )
-        self.backbone = FNetBackbone(
-            vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
-            num_layers=2,
-            hidden_dim=2,
-            intermediate_dim=4,
-            max_sequence_length=self.preprocessor.packer.sequence_length,
-        )
-        self.classifier = FNetClassifier(
-            self.backbone,
-            num_classes=4,
-            preprocessor=self.preprocessor,
-            # Check we handle serialization correctly.
-            activation=keras.activations.softmax,
-        )
-
-        # Setup data.
-        self.raw_batch = tf.constant(
-            [
-                "the quick brown fox.",
-                "the slow brown fox.",
-            ]
-        )
-        self.preprocessed_batch = self.preprocessor(self.raw_batch)
-        self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, tf.ones((2,)))
-        ).batch(2)
-        self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
-
-    def test_valid_call_classifier(self):
-        self.classifier(self.preprocessed_batch)
-
-    def test_classifier_predict(self):
-        preds1 = self.classifier.predict(self.raw_batch)
-        self.classifier.preprocessor = None
-        preds2 = self.classifier.predict(self.preprocessed_batch)
-        # Assert predictions match.
-        self.assertAllClose(preds1, preds2)
-        # Assert valid softmax output.
-        self.assertAllClose(tf.reduce_sum(preds2, axis=-1), [1.0, 1.0])
-
-    def test_fnet_classifier_fit(self):
-        self.classifier.fit(self.raw_dataset)
-        self.classifier.preprocessor = None
-        self.classifier.fit(self.preprocessed_dataset)
-
-    def test_classifier_fit_no_xla(self):
-        self.classifier.preprocessor = None
-        self.classifier.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
-            jit_compile=False,
-        )
-        self.classifier.fit(self.preprocessed_dataset)
-
-    def test_serialization(self):
-        config = keras.utils.serialize_keras_object(self.classifier)
-        new_classifier = keras.utils.deserialize_keras_object(config)
-        self.assertEqual(
-            new_classifier.get_config(),
-            self.classifier.get_config(),
-        )
-
-    @parameterized.named_parameters(
-        ("tf_format", "tf", "model"),
-        ("keras_format", "keras_v3", "model.keras"),
-    )
-    @pytest.mark.large
-    def test_saved_model(self, save_format, filename):
-        model_output = self.classifier.predict(self.raw_batch)
-        path = os.path.join(self.get_temp_dir(), filename)
-        # Don't save traces in the tf format, we check compilation elsewhere.
-        kwargs = {"save_traces": False} if save_format == "tf" else {}
-        self.classifier.save(path, save_format=save_format, **kwargs)
-        restored_model = keras.models.load_model(path)
-
-        # Check we got the real object back.
-        self.assertIsInstance(restored_model, FNetClassifier)
-
-        # Check that output matches.
-        restored_output = restored_model.predict(self.raw_batch)
-        self.assertAllClose(model_output, restored_output)
+# Copyright 2023 The KerasNLP Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""Tests for XLM-RoBERTa classification model."""
+
+import io
+import os
+
+import pytest
+import sentencepiece
+import tensorflow as tf
+from absl.testing import parameterized
+from tensorflow import keras
+
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_classifier import (
+    XLMRobertaClassifier,
+)
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
+    XLMRobertaPreprocessor,
+)
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
+    XLMRobertaTokenizer,
+)
+
+
+class XLMRobertaClassifierTest(tf.test.TestCase, parameterized.TestCase):
+    def setUp(self):
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=10,
+            model_type="WORD",
+            unk_id=0,
+            bos_id=1,
+            eos_id=2,
+        )
+        self.preprocessor = XLMRobertaPreprocessor(
+            tokenizer=XLMRobertaTokenizer(proto=bytes_io.getvalue()),
+            sequence_length=5,
+        )
+        self.backbone = XLMRobertaBackbone(
+            vocabulary_size=10,
+            num_layers=2,
+            num_heads=2,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=self.preprocessor.packer.sequence_length,
+        )
+        self.classifier = XLMRobertaClassifier(
+            self.backbone,
+            num_classes=4,
+            preprocessor=self.preprocessor,
+            # Check we handle serialization correctly.
+            activation=keras.activations.softmax,
+            hidden_dim=4,
+        )
+
+        self.raw_batch = tf.constant(
+            [
+                "the quick brown fox.",
+                "the slow brown fox.",
+            ]
+        )
+        self.preprocessed_batch = self.preprocessor(self.raw_batch)
+        self.raw_dataset = tf.data.Dataset.from_tensor_slices(
+            (self.raw_batch, tf.ones((2,)))
+        ).batch(2)
+        self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
+
+    def test_valid_call_classifier(self):
+        self.classifier(self.preprocessed_batch)
+
+    def test_classifier_predict(self):
+        preds1 = self.classifier.predict(self.raw_batch)
+        self.classifier.preprocessor = None
+        preds2 = self.classifier.predict(self.preprocessed_batch)
+        # Assert predictions match.
+        self.assertAllClose(preds1, preds2)
+        # Assert valid softmax output.
+        self.assertAllClose(tf.reduce_sum(preds2, axis=-1), [1.0, 1.0])
+
+    def test_classifier_fit(self):
+        self.classifier.fit(self.raw_dataset)
+        self.classifier.preprocessor = None
+        self.classifier.fit(self.preprocessed_dataset)
+
+    def test_classifier_fit_no_xla(self):
+        self.classifier.preprocessor = None
+        self.classifier.compile(
+            loss="sparse_categorical_crossentropy",
+            jit_compile=False,
+        )
+        self.classifier.fit(self.preprocessed_dataset)
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.classifier)
+        new_classifier = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_classifier.get_config(),
+            self.classifier.get_config(),
+        )
+
+    @parameterized.named_parameters(
+        ("tf_format", "tf", "model"),
+        ("keras_format", "keras_v3", "model.keras"),
+    )
+    @pytest.mark.large  # Saving is slow, so mark these large.
+    def test_saving_model(self, save_format, filename):
+        model_output = self.classifier.predict(self.raw_batch)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.classifier.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
+
+        # Check we got the real object back.
+        self.assertIsInstance(restored_model, XLMRobertaClassifier)
+
+        # Check that output matches.
+        restored_output = restored_model.predict(self.raw_batch)
+        self.assertAllClose(model_output, restored_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_head import MaskedLMHead
-from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
-from keras_nlp.models.f_net.f_net_backbone import f_net_kernel_initializer
-from keras_nlp.models.f_net.f_net_masked_lm_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_head import MaskedLMHead
+from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.src.models.f_net.f_net_backbone import f_net_kernel_initializer
+from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import (
     FNetMaskedLMPreprocessor,
 )
-from keras_nlp.models.f_net.f_net_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.FNetMaskedLM")
 class FNetMaskedLM(Task):
     """An end-to-end FNet model for the masked language modeling task.
 
     This model will train FNet on a masked language modeling task.
@@ -145,7 +145,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return FNetMaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from absl import logging
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
-from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
+from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 @keras_nlp_export("keras_nlp.models.FNetMaskedLMPreprocessor")
 class FNetMaskedLMPreprocessor(FNetPreprocessor):
     """FNet preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
@@ -178,7 +178,8 @@
             "token_ids": masker_outputs["token_ids"],
             "segment_ids": segment_ids,
             "mask_positions": masker_outputs["mask_positions"],
         }
         y = masker_outputs["mask_ids"]
         sample_weight = masker_outputs["mask_weights"]
         return pack_x_y_sample_weight(x, y, sample_weight)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.f_net.f_net_masked_lm_preprocessor import (
+from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import (
     FNetMaskedLMPreprocessor,
 )
-from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 
 
 class FNetMaskedLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -146,7 +146,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         outputs = model(input_data)[0]["token_ids"]
         restored_outputs = restored_model(input_data)[0]["token_ids"]
         self.assertAllEqual(outputs, restored_outputs)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_masked_lm_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
-from keras_nlp.models.f_net.f_net_masked_lm import FNetMaskedLM
-from keras_nlp.models.f_net.f_net_masked_lm_preprocessor import (
+from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.src.models.f_net.f_net_masked_lm import FNetMaskedLM
+from keras_nlp.src.models.f_net.f_net_masked_lm_preprocessor import (
     FNetMaskedLMPreprocessor,
 )
-from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 
 
 class FNetMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         # Setup Model.
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
@@ -124,7 +124,8 @@
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, FNetMaskedLM)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output, atol=0.01, rtol=0.01)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """FNet preprocessor layer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
-from keras_nlp.models.f_net.f_net_presets import backbone_presets
-from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.multi_segment_packer import MultiSegmentPacker
+from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.FNetPreprocessor")
 class FNetPreprocessor(Preprocessor):
     """An FNet preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -159,7 +159,8 @@
     @classproperty
     def tokenizer_cls(cls):
         return FNetTokenizer
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_preprocessor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
-from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 
 
 class FNetPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -163,7 +163,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_presets_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
-from keras_nlp.models.f_net.f_net_classifier import FNetClassifier
-from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
-from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.src.models.f_net.f_net_classifier import FNetClassifier
+from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 
 
 @pytest.mark.large
 class FNetPresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
     A smoke test for FNet presets we run continuously.
 
@@ -177,7 +177,8 @@
             tokenizer = FNetTokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
 
     def test_load_preprocessors(self):
         for preset in FNetPreprocessor.presets:
             preprocessor = FNetPreprocessor.from_preset(preset)
             preprocessor("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """FNet tokenizer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.f_net.f_net_presets import backbone_presets
-from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.f_net.f_net_presets import backbone_presets
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.FNetTokenizer")
 class FNetTokenizer(SentencePieceTokenizer):
     """FNet tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -84,7 +84,8 @@
         self.sep_token_id = self.token_to_id(sep_token)
         self.pad_token_id = self.token_to_id(pad_token)
         self.mask_token_id = self.token_to_id(mask_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_tokenizer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 
 
 class FNetTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -109,7 +109,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_backbone.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,173 +8,164 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""GPT-2 backbone model."""
+"""RoBERTa backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.position_embedding import PositionEmbedding
-from keras_nlp.layers.transformer_decoder import TransformerDecoder
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.models.gpt2.gpt2_presets import backbone_presets
-from keras_nlp.utils.python_utils import classproperty
-
-
-def _gpt_2_kernel_initializer(stddev=0.02):
-    return keras.initializers.RandomNormal(stddev=stddev)
-
-
-@keras_nlp_export("keras_nlp.models.GPT2Backbone")
-class GPT2Backbone(Backbone):
-    """GPT-2 core network with hyperparameters.
-
-    This network implements a Transformer-based decoder network,
-    Generative Pretrained Transformer-2 (GPT-2), as described in
-    ["Language Models are Unsupervised Multitask Learners"](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf).
-    It includes the embedding lookups and transformer layers.
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.token_and_position_embedding import (
+    TokenAndPositionEmbedding,
+)
+from keras_nlp.src.layers.transformer_encoder import TransformerEncoder
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
+from keras_nlp.src.utils.python_utils import classproperty
+
+
+def roberta_kernel_initializer(stddev=0.02):
+    return keras.initializers.TruncatedNormal(stddev=stddev)
+
+
+@keras_nlp_export("keras_nlp.models.RobertBackbone")
+class RobertaBackbone(Backbone):
+    """A RoBERTa encoder network.
+
+    This network implements a bi-directional Transformer-based encoder as
+    described in ["RoBERTa: A Robustly Optimized BERT Pretraining Approach"](https://arxiv.org/abs/1907.11692).
+    It includes the embedding lookups and transformer layers, but does not
+    include the masked language model head used during pretraining.
 
     The default constructor gives a fully customizable, randomly initialized
-    GPT-2 model with any number of layers, heads, and embedding
-    dimensions. To load preset architectures and weights, use the `from_preset`
+    RoBERTa encoder with any number of layers, heads, and embedding
+    dimensions. To load preset architectures and weights, use the `from_preset()`
     constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
-    [here](https://github.com/openai/gpt-2).
+    [here](https://github.com/facebookresearch/fairseq).
 
     Args:
         vocabulary_size: int. The size of the token vocabulary.
         num_layers: int. The number of transformer layers.
         num_heads: int. The number of attention heads for each transformer.
             The hidden size must be divisible by the number of attention heads.
-        hidden_dim: int. The size of the transformer encoding and pooler layers.
+        hidden_dim: int. The size of the transformer encoding layer.
         intermediate_dim: int. The output dimension of the first Dense layer in
             a two-layer feedforward network for each transformer.
         dropout: float. Dropout probability for the Transformer encoder.
-        max_sequence_length: int. The maximum sequence length that this encoder
-            can consume. If None, `max_sequence_length` uses the value from
-            sequence length. This determines the variable shape for positional
-            embeddings.
+        max_sequence_length: int. The maximum sequence length this encoder can
+            consume. The sequence length of the input must be less than
+            `max_sequence_length` default value. This determines the variable
+            shape for positional embeddings.
 
-    Example usage:
+    Examples:
     ```python
     input_data = {
         "token_ids": tf.ones(shape=(1, 12), dtype=tf.int64),
         "padding_mask": tf.constant(
-            [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)
-        ),
+            [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)),
     }
 
-    # Pretrained GPT-2 decoder.
-    model = keras_nlp.models.GPT2Backbone.from_preset("gpt2_base_en")
+    # Pretrained RoBERTa encoder
+    model = keras_nlp.models.RobertaBackbone.from_preset("roberta_base_en")
     model(input_data)
 
-    # Randomly initialized GPT-2 decoder with custom config.
-    model = keras_nlp.models.GPT2Backbone(
-        vocabulary_size=50257,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=1024,
+    # Randomly initialized RoBERTa model with custom config
+    model = keras_nlp.models.RobertaBackbone(
+        vocabulary_size=50265,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
     )
     model(input_data)
     ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
         num_heads,
         hidden_dim,
         intermediate_dim,
         dropout=0.1,
-        max_sequence_length=1024,
+        max_sequence_length=512,
         **kwargs,
     ):
         # Inputs
-        token_ids = keras.Input(shape=(None,), dtype="int32", name="token_ids")
+        token_id_input = keras.Input(
+            shape=(None,), dtype=tf.int32, name="token_ids"
+        )
         padding_mask = keras.Input(
-            shape=(None,), dtype="int32", name="padding_mask"
+            shape=(None,), dtype=tf.int32, name="padding_mask"
         )
 
-        # Embed tokens, positions.
-        token_embedding = keras.layers.Embedding(
-            input_dim=vocabulary_size,
-            output_dim=hidden_dim,
-            embeddings_initializer=_gpt_2_kernel_initializer(stddev=0.01),
-            name="token_embedding",
-        )(token_ids)
-
-        # Can't use `TokenAndPositionEmbedding` layer here because of different
-        # initializers.
-        position_embedding = PositionEmbedding(
-            initializer=_gpt_2_kernel_initializer(stddev=0.02),
+        # Embed tokens and positions.
+        embedding_layer = TokenAndPositionEmbedding(
+            vocabulary_size=vocabulary_size,
             sequence_length=max_sequence_length,
-            name="position_embedding",
-        )(token_embedding)
-
-        # Sum and apply dropout to embeddings.
-        x = keras.layers.Add(name="embeddings_add")(
-            (token_embedding, position_embedding)
+            embedding_dim=hidden_dim,
+            embeddings_initializer=roberta_kernel_initializer(),
+            name="embeddings",
         )
+        embedding = embedding_layer(token_id_input)
+
+        # Sum, normalize and apply dropout to embeddings.
+        x = keras.layers.LayerNormalization(
+            name="embeddings_layer_norm",
+            axis=-1,
+            epsilon=1e-5,  # Original paper uses this epsilon value
+            dtype=tf.float32,
+        )(embedding)
         x = keras.layers.Dropout(
             dropout,
             name="embeddings_dropout",
         )(x)
 
-        # Apply successive transformer decoder blocks.
+        # Apply successive transformer encoder blocks.
         for i in range(num_layers):
-            x = TransformerDecoder(
-                intermediate_dim=intermediate_dim,
+            x = TransformerEncoder(
                 num_heads=num_heads,
+                intermediate_dim=intermediate_dim,
+                activation="gelu",
                 dropout=dropout,
-                layer_norm_epsilon=1e-05,
-                activation=lambda x: keras.activations.gelu(
-                    x, approximate=True
-                ),
-                kernel_initializer=_gpt_2_kernel_initializer(stddev=0.02),
-                normalize_first=True,
+                layer_norm_epsilon=1e-5,
+                kernel_initializer=roberta_kernel_initializer(),
                 name=f"transformer_layer_{i}",
-            )(x, decoder_padding_mask=padding_mask)
-
-        sequence_output = keras.layers.LayerNormalization(
-            name="layer_norm",
-            axis=-1,
-            epsilon=1e-05,
-            dtype=tf.float32,
-        )(x)
+            )(x, padding_mask=padding_mask)
 
         # Instantiate using Functional API Model constructor
         super().__init__(
             inputs={
-                "token_ids": token_ids,
+                "token_ids": token_id_input,
                 "padding_mask": padding_mask,
             },
-            outputs=sequence_output,
+            outputs=x,
             **kwargs,
         )
         # All references to `self` below this line
         self.vocabulary_size = vocabulary_size
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.hidden_dim = hidden_dim
         self.intermediate_dim = intermediate_dim
         self.dropout = dropout
         self.max_sequence_length = max_sequence_length
+        self.start_token_index = 0
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "vocabulary_size": self.vocabulary_size,
                 "num_layers": self.num_layers,
@@ -185,12 +176,13 @@
                 "max_sequence_length": self.max_sequence_length,
             }
         )
         return config
 
     @property
     def token_embedding(self):
-        return self.get_layer("token_embedding")
+        return self.get_layer("embeddings").token_embedding
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,63 +7,66 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for GPT-2 backbone models."""
+
+"""Tests for XLM-RoBERTa backbone models."""
 
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
 
 
-class GPT2Test(tf.test.TestCase, parameterized.TestCase):
+class XLMRobertaBackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = GPT2Backbone(
+        self.backbone = XLMRobertaBackbone(
             vocabulary_size=10,
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
         )
         self.input_batch = {
             "token_ids": tf.ones((2, 5), dtype="int32"),
-            "segment_ids": tf.ones((2, 5), dtype="int32"),
             "padding_mask": tf.ones((2, 5), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_call(self):
+    def test_valid_call_xlm_roberta(self):
         self.backbone(self.input_batch)
 
     def test_token_embedding(self):
         output = self.backbone.token_embedding(self.input_batch["token_ids"])
         self.assertEqual(output.shape, (2, 5, 2))
 
     def test_name(self):
         # Check default name passed through
-        self.assertRegexpMatches(self.backbone.name, "gpt2_backbone")
+        self.assertRegexpMatches(self.backbone.name, "xlm_roberta_backbone")
 
-    def test_variable_sequence_length(self):
+    def test_variable_sequence_length_call_xlm_roberta(self):
         for seq_length in (2, 3, 4):
             input_data = {
                 "token_ids": tf.ones((2, seq_length), dtype="int32"),
                 "padding_mask": tf.ones((2, seq_length), dtype="int32"),
             }
-            self.backbone(input_data)
+            output = self.backbone(input_data)
+            self.assertAllEqual(
+                tf.shape(output), [2, seq_length, self.backbone.hidden_dim]
+            )
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
     def test_serialization(self):
         new_backbone = keras.utils.deserialize_keras_object(
@@ -71,48 +74,49 @@
         )
         self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
-    @pytest.mark.large
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         model_output = self.backbone(self.input_batch)
         path = os.path.join(self.get_temp_dir(), filename)
         # Don't save traces in the tf format, we check compilation elsewhere.
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         self.backbone.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, GPT2Backbone)
+        self.assertIsInstance(restored_model, XLMRobertaBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(model_output, restored_output)
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
-class GPT2BackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
+class XLMRobertaBackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.model = GPT2Backbone(
-                vocabulary_size=10,
+            self.backbone = XLMRobertaBackbone(
+                vocabulary_size=1000,
                 num_layers=2,
                 num_heads=2,
-                hidden_dim=2,
-                intermediate_dim=4,
-                max_sequence_length=5,
+                hidden_dim=64,
+                intermediate_dim=128,
+                max_sequence_length=128,
             )
         self.input_batch = {
-            "token_ids": tf.ones((2, 5), dtype="int32"),
-            "padding_mask": tf.ones((2, 5), dtype="int32"),
+            "token_ids": tf.ones((8, 128), dtype="int32"),
+            "padding_mask": tf.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
-        self.model.compile()
-        self.model.predict(self.input_dataset)
+        self.backbone.compile()
+        self.backbone.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,45 +14,45 @@
 """GPT2 Causal LM (Language Model)."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
-from keras_nlp.models.gpt2.gpt2_causal_lm_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.gpt2.gpt2_backbone import GPT2Backbone
+from keras_nlp.src.models.gpt2.gpt2_causal_lm_preprocessor import (
     GPT2CausalLMPreprocessor,
 )
-from keras_nlp.models.gpt2.gpt2_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.samplers.serialization import get as get_sampler
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.tf_utils import tensor_to_string_list
-from keras_nlp.utils.tf_utils import truncate_at_token
+from keras_nlp.src.models.gpt2.gpt2_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.samplers.serialization import get as get_sampler
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.tf_utils import tensor_to_string_list
 
 
 @keras_nlp_export("keras_nlp.models.GPT2CausalLM")
 class GPT2CausalLM(Task):
     """An end-to-end GPT2 model for causal langauge modeling.
 
     A causal language model (LM) predicts the next token based on previous
-    tokens the next token based on previous tokens, which is the way GPT2 gets
-    pretrained. You can finetune `GPT2CausalLM` to generate text similar to
-    the custom dataset.
+    tokens. This task setup can be used to train the model unsupervised on
+    plain text input, or to autoregressively generate plain text similar to
+    the data used for training. This task can be used for pre-training or
+    fine-tuning a GPT-2 model, simply by calling `fit()`.
 
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
     [here](https://github.com/openai/gpt-2).
@@ -301,36 +301,31 @@
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
@@ -347,24 +342,96 @@
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
 
@@ -392,66 +459,81 @@
                 should be padded to the desired maximum length and this argument
                 will be ignored.
 
         Returns:
             A string or string list if `preprocessor` is set, and a integer
             tensor of token IDs if `preprocessor is None`.
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
+
+        outputs = [generate(x) for x in inputs]
+
+        if self.preprocessor is not None:
+            outputs = [postprocess(x) for x in outputs]
+
+        return self._normalize_generate_outputs(outputs, input_is_scalar)
+
+    @classmethod
+    def create_layout_map(cls, mesh):
+        """Create a DTensor layout map for an GPT2CausalLM.
+
+        Given a DTensor mesh describing a list of devices, this method returns a
+        DTensor layout map for creating a `keras_nlp.models.GPT2CausalLM`
+        instance. This mapping describes how to distribute all model weights
+        across multiple devices. For an overview of DTensor concepts, see
+        [this guide](https://www.tensorflow.org/guide/dtensor_overview).
+
+        Args:
+            mesh: A 2D `tf.experimental.dtensor.Mesh` describing the arrangement
+                of devices for running distributed computation. The
+                first dimension in the mesh is expected to be for data parallel
+                distribution, and the second for model parallel distribution.
+
+        Returns:
+            A `tf.keras.dtensor.experimental.LayoutMap` which contains the
+            proper layout to weights mapping for the model parallel setting.
+
+        Examples:
+        ```python
+        keras.backend.experimental.enable_tf_random_generator()
+        keras.utils.set_random_seed(1337)
+
+        # Update both dimensions below for a multi-device setting.
+        mesh = tf.experimental.dtensor.create_mesh([("batch", 1), ("model", 1)])
+        layout_map = keras_nlp.models.GPT2CausalLM.create_layout_map(mesh)
+
+        with layout_map.scope():
+            gpt2_lm = keras_nlp.models.GPT2CausalLM.from_preset("gpt2_base_en")
+        ```
+        """
+        # As this task has no new variables, we just re-use the backbone method.
+        return cls.backbone_cls.create_layout_map(mesh)
 
-        generate_function = self.make_generate_function()
-        outputs = []
-        for batch in inputs:
-            token_ids, padding_mask = batch["token_ids"], batch["padding_mask"]
-            # If `preprocessor` is attached, we can stop after end_token_id.
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
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""GPT2 Causal LM preprocessor layer."""
+"""OPT Causal LM preprocessor layer."""
 
 from absl import logging
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
-@keras_nlp_export("keras_nlp.models.GPT2CausalLMPreprocessor")
-class GPT2CausalLMPreprocessor(GPT2Preprocessor):
-    """GPT2 Causal LM preprocessor.
+@keras_nlp_export("keras_nlp.models.OPTCausalLMPreprocessor")
+class OPTCausalLMPreprocessor(OPTPreprocessor):
+    """OPT Causal LM preprocessor.
 
     This preprocessing layer is primarily meant to be used with
-    `keras_nlp.models.GPT2CausalLM`. By default, it will take in batches of
+    `keras_nlp.models.OPTCausalLM`. By default, it will take in batches of
     strings, and return outputs in a `(x, y, sample_weight)` format, where the
     `y` label is the next token id in the `x` sequence. For use with generation,
     pass `return_labels=False` in which case the output will simply be the
     encoded string features.
 
     Args:
-        tokenizer: A `keras_nlp.models.GPT2Tokenizer` instance.
+        tokenizer: A `keras_nlp.models.OPTTokenizer` instance.
         sequence_length: The length of the packed inputs.
-        add_start_token: If true, the preprocessor will append the tokenizer
+        add_start_token: If true, the preprocessor will prepend the tokenizer
             start token to each input sequence.
         add_end_token: If true, the preprocessor will append the tokenizer
             end token to each input sequence.
 
     Call arguments:
-        x: A string `tf.Tensor` or list of python strings.
+        x: A string, `tf.Tensor` or list of python strings.
         y: Label data. Should always be `None` as the layer generates labels.
         sample_weight: Label weights. Should always be `None` as the layer
             generates label weights.
         sequence_length: Pass to override the configured `sequence_length` of
             the layer.
         add_start_token: Pass to override the configured value of
             `add_start_token` on the layer.
@@ -53,16 +53,16 @@
             `add_end_token` on the layer.
         return_labels: If `True`, the output `"token_ids"` will be offset by one
             and returned as labels. If `False` only features will be returned.
 
     Examples:
     ```python
     # Load the preprocessor from a preset.
-    preprocessor = keras_nlp.models.GPT2CausalLMPreprocessor.from_preset(
-        "gpt2_base_en"
+    preprocessor = keras_nlp.models.OPTCausalLMPreprocessor.from_preset(
+        "opt_125m_en"
     )
 
     # Tokenize and pack a single sentence.
     sentence = tf.constant("League of legends")
     preprocessor(sentence)
     # Same output.
     preprocessor("League of legends")
@@ -97,15 +97,15 @@
         sequence_length=None,
         add_start_token=None,
         add_end_token=None,
         return_labels=True,
     ):
         if y is not None or sample_weight is not None:
             logging.warning(
-                "`GPT2CausalLMPreprocessor` generates `y` and `sample_weight` "
+                "`OPTCausalLMPreprocessor` generates `y` and `sample_weight` "
                 "based on your input data, but your data already contains `y` "
                 "or `sample_weight`. Your `y` and `sample_weight` will be "
                 "ignored."
             )
         if return_labels:
             # Tokenize with one extra token to account for the truncation below.
             sequence_length = (sequence_length or self.sequence_length) + 1
@@ -124,7 +124,8 @@
             }
             # Target `y` will be the next token.
             y = token_ids[..., 1:]
             sample_weight = padding_mask[..., 1:]
             return pack_x_y_sample_weight(x, y, sample_weight)
         else:
             return x
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,126 +1,153 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for GPT2 causal LM preprocessor layer."""
+"""Tests for XLM-RoBERTa masked language model preprocessor layer."""
 
+import io
 import os
 
 import pytest
+import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.gpt2.gpt2_causal_lm_preprocessor import (
-    GPT2CausalLMPreprocessor,
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
+    XLMRobertaMaskedLMPreprocessor,
+)
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
+    XLMRobertaTokenizer,
 )
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 
 
-class GPT2CausalLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
+class XLMRobertaMaskedLMPreprocessorTest(
+    tf.test.TestCase, parameterized.TestCase
+):
     def setUp(self):
-        self.vocab = {
-            "!": 0,
-            "air": 1,
-            "Ġair": 2,
-            "plane": 3,
-            "Ġat": 4,
-            "port": 5,
-            "<|endoftext|>": 6,
-        }
-
-        self.merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
-        self.merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
-        self.merges += ["Ġai r", "Ġa i", "pla ne"]
-
-        self.preprocessor = GPT2CausalLMPreprocessor(
-            tokenizer=GPT2Tokenizer(
-                vocabulary=self.vocab,
-                merges=self.merges,
-            ),
-            sequence_length=8,
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=12,
+            model_type="WORD",
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
+            bos_piece="<s>",
+            eos_piece="</s>",
+            user_defined_symbols="[MASK]",
+        )
+        self.proto = bytes_io.getvalue()
+
+        self.tokenizer = XLMRobertaTokenizer(proto=self.proto)
+        self.preprocessor = XLMRobertaMaskedLMPreprocessor(
+            tokenizer=self.tokenizer,
+            # Simplify out testing by masking every available token.
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=5,
+            sequence_length=12,
         )
 
-    def test_strings(self):
-        input_data = "airplane at airport"
+    def test_preprocess_strings(self):
+        input_data = " brown fox quick"
 
         x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
-        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
-        self.assertAllEqual(y, [1, 3, 4, 2, 5, 6, 0, 0])
-        self.assertAllEqual(sw, [1, 1, 1, 1, 1, 1, 0, 0])
+        self.assertAllEqual(
+            x["token_ids"], [0, 13, 13, 13, 2, 1, 1, 1, 1, 1, 1, 1]
+        )
+        self.assertAllEqual(
+            x["padding_mask"], [1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(x["mask_positions"], [1, 2, 3, 0, 0])
+        self.assertAllEqual(y, [7, 9, 11, 0, 0])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 0.0, 0.0])
 
-    def test_list_of_strings(self):
-        input_data = ["airplane at airport"] * 4
+    def test_preprocess_list_of_strings(self):
+        input_data = [" brown fox quick"] * 13
 
         x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
-
-    def test_no_start_end_token(self):
-        input_data = ["airplane at airport"] * 4
-
-        preprocessor = GPT2CausalLMPreprocessor(
-            tokenizer=GPT2Tokenizer(
-                vocabulary=self.vocab,
-                merges=self.merges,
-            ),
-            sequence_length=8,
-            add_start_token=False,
-            add_end_token=False,
-        )
-        x, y, sw = preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 2, 5, 0, 0, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
-        self.assertAllEqual(y, [[3, 4, 2, 5, 0, 0, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 0, 0, 0, 0]] * 4)
-
-    def test_labeled_batch(self):
-        x = tf.constant(["airplane at airport"] * 4)
-        y = tf.constant([1] * 4)  # Ignored.
-        sw = tf.constant([1.0] * 4)  # Ignored.
-        x, y, sw = self.preprocessor(x, y, sw)
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
-
-    def test_dataset(self):
-        x = tf.constant(["airplane at airport"] * 4)
-        ds = tf.data.Dataset.from_tensor_slices(x)
+        self.assertAllEqual(
+            x["token_ids"], [[0, 13, 13, 13, 2, 1, 1, 1, 1, 1, 1, 1]] * 13
+        )
+        self.assertAllEqual(
+            x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]] * 13
+        )
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 0, 0]] * 13)
+        self.assertAllEqual(y, [[7, 9, 11, 0, 0]] * 13)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 0.0, 0.0]] * 13)
+
+    def test_preprocess_dataset(self):
+        sentences = tf.constant([" brown fox quick"] * 13)
+        ds = tf.data.Dataset.from_tensor_slices(sentences)
         ds = ds.map(self.preprocessor)
-        x, y, sw = ds.batch(4).take(1).get_single_element()
-        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
-        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
-
-    def test_call_overrides(self):
-        input_data = "airplane at airport"
-        x, _, _ = self.preprocessor(input_data, add_start_token=False)
-        self.assertAllEqual(x["token_ids"], [1, 3, 4, 2, 5, 6, 0, 0])
-        x, _, _ = self.preprocessor(input_data, add_end_token=False)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 0, 0])
-        x, _, _ = self.preprocessor(input_data, sequence_length=4)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4])
-        x = self.preprocessor(input_data, return_labels=False)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
+        x, y, sw = ds.batch(13).take(1).get_single_element()
+        self.assertAllEqual(
+            x["token_ids"], [[0, 13, 13, 13, 2, 1, 1, 1, 1, 1, 1, 1]] * 13
+        )
+        self.assertAllEqual(
+            x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]] * 13
+        )
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 0, 0]] * 13)
+        self.assertAllEqual(y, [[7, 9, 11, 0, 0]] * 13)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 0.0, 0.0]] * 13)
+
+    def test_mask_multiple_sentences(self):
+        sentence_one = tf.constant(" airplane")
+        sentence_two = tf.constant(" round")
+
+        x, y, sw = self.preprocessor((sentence_one, sentence_two))
+        self.assertAllEqual(
+            x["token_ids"], [0, 2, 2, 2, 13, 2, 1, 1, 1, 1, 1, 1]
+        )
+        self.assertAllEqual(
+            x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(x["mask_positions"], [4, 0, 0, 0, 0])
+        self.assertAllEqual(y, [12, 0, 0, 0, 0])
+        self.assertAllEqual(sw, [1.0, 0.0, 0.0, 0.0, 0.0])
+
+    def test_no_masking_zero_rate(self):
+        no_mask_preprocessor = XLMRobertaMaskedLMPreprocessor(
+            self.preprocessor.tokenizer,
+            mask_selection_rate=0.0,
+            mask_selection_length=5,
+            sequence_length=12,
+        )
+        input_data = " quick brown fox"
+
+        x, y, sw = no_mask_preprocessor(input_data)
+        self.assertAllEqual(
+            x["token_ids"], [0, 11, 7, 9, 2, 1, 1, 1, 1, 1, 1, 1]
+        )
+        self.assertAllEqual(
+            x["padding_mask"], [1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0, 0])
+        self.assertAllEqual(y, [0, 0, 0, 0, 0])
+        self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0, 0.0])
 
     def test_serialization(self):
         config = keras.utils.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.utils.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
@@ -128,23 +155,21 @@
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        input_data = tf.constant(["airplane at airport"])
+        input_data = tf.constant([" quick brown fox"])
 
         inputs = keras.Input(dtype="string", shape=())
-        outputs, y, sw = self.preprocessor(inputs)
+        outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        # Don't save traces in the tf format, we check compilation elsewhere.
-        kwargs = {"save_traces": False} if save_format == "tf" else {}
-        model.save(path, save_format=save_format, **kwargs)
+        model.save(path, save_format=save_format)
 
         restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
+        outputs = model(input_data)[0]["token_ids"]
+        restored_outputs = restored_model(input_data)[0]["token_ids"]
+        self.assertAllEqual(outputs, restored_outputs)
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,58 +7,68 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for GPT2 causal LM model."""
+"""Tests for OPT causal LM model."""
 
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
-from keras_nlp.models.gpt2.gpt2_causal_lm import GPT2CausalLM
-from keras_nlp.models.gpt2.gpt2_causal_lm_preprocessor import (
-    GPT2CausalLMPreprocessor,
+from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
+from keras_nlp.src.models.opt.opt_causal_lm import OPTCausalLM
+from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
+    OPTCausalLMPreprocessor,
 )
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 
 
-class GPT2CausalLMTest(tf.test.TestCase, parameterized.TestCase):
+class OPTCausalLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
+        # For DTensor.
+        keras.backend.experimental.enable_tf_random_generator()
+        keras.utils.set_random_seed(1337)
+
         self.vocab = {
-            "!": 0,
-            "air": 1,
+            "<pad>": 0,
+            "</s>": 1,
             "Ġair": 2,
             "plane": 3,
             "Ġat": 4,
             "port": 5,
-            "<|endoftext|>": 6,
+            "Ġkoh": 6,
+            "li": 7,
+            "Ġis": 8,
+            "Ġthe": 9,
+            "Ġbest": 10,
         }
-        self.merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
-        self.merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
-        self.merges += ["Ġai r", "Ġa i", "pla ne"]
-        self.preprocessor = GPT2CausalLMPreprocessor(
-            GPT2Tokenizer(vocabulary=self.vocab, merges=self.merges),
+        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
+        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
+        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
+        merges += ["pla ne"]
+        self.merges = merges
+        self.preprocessor = OPTCausalLMPreprocessor(
+            OPTTokenizer(vocabulary=self.vocab, merges=self.merges),
             sequence_length=8,
         )
-        self.backbone = GPT2Backbone(
+        self.backbone = OPTBackbone(
             vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
             hidden_dim=64,
             intermediate_dim=128,
             max_sequence_length=self.preprocessor.packer.sequence_length,
         )
-        self.causal_lm = GPT2CausalLM(
+        self.causal_lm = OPTCausalLM(
             backbone=self.backbone,
             preprocessor=self.preprocessor,
         )
 
         self.raw_batch = tf.constant(
             [
                 " airplane at airport",
@@ -137,13 +147,24 @@
         path = os.path.join(self.get_temp_dir(), filename)
         # Don't save traces in the tf format, we check compilation elsewhere.
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         self.causal_lm.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, GPT2CausalLM)
+        self.assertIsInstance(restored_model, OPTCausalLM)
 
         # Check that output matches.
         keras.utils.set_random_seed(42)
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
+
+    def test_create_layout_map(self):
+        mesh = tf.experimental.dtensor.create_mesh([("batch", 1), ("model", 1)])
+        with OPTCausalLM.create_layout_map(mesh).scope():
+            OPTCausalLM(backbone=self.backbone)
+        # Using DTensor enables the mlir bridge as a side effect. Eventually
+        # this will be default, but for now we have compile errors with the
+        # bridge elsewhere and must disable. See
+        # https://github.com/keras-team/keras-nlp/issues/1001
+        tf.config.experimental.disable_mlir_bridge()
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """GPT2 preprocessor layer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.start_end_packer import StartEndPacker
-from keras_nlp.models.gpt2.gpt2_presets import backbone_presets
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.start_end_packer import StartEndPacker
+from keras_nlp.src.models.gpt2.gpt2_presets import backbone_presets
+from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.GPT2Preprocessor")
 class GPT2Preprocessor(Preprocessor):
     """GPT2 preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do 2 things:
 
-    - Tokenize the input using the `tokenizer`.
+    - Tokenize the inputs using the `tokenizer`.
     - Construct a dictionary with keys `"token_ids"`, `"padding_mask"`, that can
         be passed directly to a `keras_nlp.models.GPT2Backbone`.
 
     This layer can be used directly with `tf.data.Dataset.map` to preprocess
     string data in the `(x, y, sample_weight)` format used by
     `keras.Model.fit`.
 
@@ -53,29 +53,25 @@
     mainly used for generation tasks. For tasks having multi-segment inputs
     like "glue/mnli", please use a model designed for classification purposes
     such as BERT or RoBERTa.
 
     Args:
         tokenizer: A `keras_nlp.models.GPT2Tokenizer` instance.
         sequence_length: The length of the packed inputs.
-        add_start_token: If true, the preprocessor will append the tokenizer
+        add_start_token: If true, the preprocessor will prepend the tokenizer
             start token to each input sequence.
         add_end_token: If true, the preprocessor will append the tokenizer
             end token to each input sequence.
 
     Call arguments:
-        x: A string `tf.Tensor` or list of python strings.
+        x: A string, `tf.Tensor` or list of python strings.
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
     preprocessor = keras_nlp.models.GPT2Preprocessor.from_preset("gpt2_base_en")
 
@@ -150,43 +146,37 @@
 
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
                 "GPT2 requires each input feature to contain only "
                 f"one segment, but received {len(x)}. If you are using GPT2 "
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
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
 
     @classproperty
     def tokenizer_cls(cls):
         return GPT2Tokenizer
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
+from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 
 
 class GPT2PreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
             "!": 0,
             "air": 1,
@@ -93,20 +93,16 @@
         x = tf.constant(["airplane at airport"] * 4)
         ds = tf.data.Dataset.from_tensor_slices(x)
         ds = ds.map(self.preprocessor)
         x = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
         self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
 
-    def test_call_overrides(self):
+    def test_sequence_length_override(self):
         input_data = "airplane at airport"
-        x = self.preprocessor(input_data, add_start_token=False)
-        self.assertAllEqual(x["token_ids"], [1, 3, 4, 2, 5, 6, 0, 0])
-        x = self.preprocessor(input_data, add_end_token=False)
-        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 0, 0])
         x = self.preprocessor(input_data, sequence_length=4)
         self.assertAllEqual(x["token_ids"], [6, 1, 3, 6])
 
     def test_serialization(self):
         config = keras.utils.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.utils.deserialize_keras_object(config)
         self.assertEqual(
@@ -132,7 +128,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_presets.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,7 +151,8 @@
         "weights_hash": "09d86ca6e1b4213886b720a1392f2a70",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_base_en_news/v1/vocab.json",
         "vocabulary_hash": "dffec25a898b1f5e569bec4dffd7e5c0",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_base_en_news/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
 }
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_presets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.gpt2.gpt2_backbone import GPT2Backbone
+from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 
 
 @pytest.mark.large
 class GPT2PresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
     A smoke test for GPT-2 presets we run continuously.
 
@@ -103,7 +103,8 @@
             }
             model(input_data)
 
     def test_load_tokenizers(self):
         for preset in GPT2Tokenizer.presets:
             tokenizer = GPT2Tokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """GPT-2 preprocessing layers."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.gpt2.gpt2_presets import backbone_presets
-from keras_nlp.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.gpt2.gpt2_presets import backbone_presets
+from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.GPT2Tokenizer")
 class GPT2Tokenizer(BytePairTokenizer):
     """A GPT-2 tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -105,7 +105,8 @@
     def get_config(self):
         config = super().get_config()
         # In the constructor, we pass the list of special tokens to the
         # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
         # delete it from the config here.
         del config["unsplittable_tokens"]
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 
 
 class GPT2TokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
             "<|endoftext|>": 0,
             "Ġair": 1,
@@ -117,7 +117,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_backbone_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,112 +7,118 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for OPT backbone models."""
+
+"""Test for RoBERTa backbone models."""
 
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.opt.opt_backbone import OPTBackbone
+from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
 
 
-class OPTTest(tf.test.TestCase, parameterized.TestCase):
+class RobertaBackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = OPTBackbone(
+        self.backbone = RobertaBackbone(
             vocabulary_size=10,
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
         )
+        self.batch_size = 8
         self.input_batch = {
             "token_ids": tf.ones((2, 5), dtype="int32"),
             "padding_mask": tf.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_valid_call_opt(self):
+    def test_valid_call_roberta(self):
         self.backbone(self.input_batch)
 
     def test_token_embedding(self):
         output = self.backbone.token_embedding(self.input_batch["token_ids"])
         self.assertEqual(output.shape, (2, 5, 2))
 
     def test_name(self):
-        # Check default name passed through
-        self.assertRegexpMatches(self.backbone.name, "opt_backbone")
-
-    def test_variable_sequence_length_call_opt(self):
-        for seq_length in (2, 3, 4):
-            input_data = {
-                "token_ids": tf.ones((2, seq_length), dtype="int32"),
-                "padding_mask": tf.ones((2, seq_length), dtype="int32"),
-            }
-            self.backbone(input_data)
+        self.assertRegexpMatches(self.backbone.name, "roberta_backbone")
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
     def test_serialization(self):
         new_backbone = keras.utils.deserialize_keras_object(
             keras.utils.serialize_keras_object(self.backbone)
         )
         self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
+    def test_variable_sequence_length_call_roberta(self):
+        for seq_length in (2, 3, 4):
+            input_data = {
+                "token_ids": tf.ones((2, seq_length), dtype="int32"),
+                "padding_mask": tf.ones((2, seq_length), dtype="int32"),
+            }
+            output = self.backbone(input_data)
+            self.assertAllEqual(
+                tf.shape(output),
+                [2, seq_length, self.backbone.hidden_dim],
+            )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         model_output = self.backbone(self.input_batch)
         path = os.path.join(self.get_temp_dir(), filename)
         # Don't save traces in the tf format, we check compilation elsewhere.
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         self.backbone.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, OPTBackbone)
+        self.assertIsInstance(restored_model, RobertaBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(model_output, restored_output)
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
-class OPTBackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
+class RobertaBackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.backbone = OPTBackbone(
+            self.backbone = RobertaBackbone(
                 vocabulary_size=1000,
                 num_layers=2,
                 num_heads=2,
-                hidden_dim=32,
+                hidden_dim=64,
                 intermediate_dim=128,
                 max_sequence_length=128,
             )
         self.input_batch = {
             "token_ids": tf.ones((8, 128), dtype="int32"),
             "padding_mask": tf.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
         self.backbone.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,36 +14,37 @@
 """OPT Causal LM (Language Model)."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.opt.opt_backbone import OPTBackbone
-from keras_nlp.models.opt.opt_causal_lm_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
+from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
     OPTCausalLMPreprocessor,
 )
-from keras_nlp.models.opt.opt_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.samplers.serialization import get as get_sampler
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.tf_utils import tensor_to_string_list
-from keras_nlp.utils.tf_utils import truncate_at_token
+from keras_nlp.src.models.opt.opt_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.samplers.serialization import get as get_sampler
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.tf_utils import tensor_to_string_list
+from keras_nlp.src.utils.tf_utils import truncate_at_token
 
 
 @keras_nlp_export("keras_nlp.models.OPTCausalLM")
 class OPTCausalLM(Task):
     """An end-to-end OPT model for causal langauge modeling.
 
     A causal language model (LM) predicts the next token based on previous
-    tokens the next token based on previous tokens, which is the way OPT gets
-    pretrained. You can finetune `OPTCausalLM` to generate text similar to
-    the custom dataset.
+    tokens. This task setup can be used to train the model unsupervised on
+    plain text input, or to autoregressively generate plain text similar to
+    the data used for training. This task can be used for pre-training or
+    fine-tuning a GPT-2 model, simply by calling `fit()`.
 
     This model has a `generate()` method, which generates text based on a
     prompt. The generation strategy used is controlled by an additional
     `sampler` argument on `compile()`. You can recompile the model with
     different `keras_nlp.samplers` objects to control the generation. By
     default, `"top_k"` sampling will be used.
 
@@ -445,7 +446,44 @@
         outputs = tf.concat(outputs, axis=0)
         outputs = tf.squeeze(outputs, 0) if input_is_scalar else outputs
         # Convert outputs to a friendly pythonic type. For numerical outputs
         # that is numpy, for string outputs that is `list` and `str`.
         if outputs.dtype == tf.string:
             return tensor_to_string_list(outputs)
         return outputs.numpy()
+
+    @classmethod
+    def create_layout_map(cls, mesh):
+        """Create a DTensor layout map for an OPTCausalLM.
+
+        Given a DTensor mesh describing a list of devices, this method returns a
+        DTensor layout map for creating a `keras_nlp.models.OPTCausalLM`
+        instance. This mapping describes how to distribute all model weights
+        across multiple devices. For an overview of DTensor concepts, see
+        [this guide](https://www.tensorflow.org/guide/dtensor_overview).
+
+        Args:
+            mesh: A 2D `tf.experimental.dtensor.Mesh` describing the arrangement
+                of devices for running distributed computation. The
+                first dimension in the mesh is expected to be for data parallel
+                distribution, and the second for model parallel distribution.
+
+        Returns:
+            A `tf.keras.dtensor.experimental.LayoutMap` which contains the
+            proper layout to weights mapping for the model parallel setting.
+
+        Examples:
+        ```python
+        keras.backend.experimental.enable_tf_random_generator()
+        keras.utils.set_random_seed(1337)
+
+        # Update both dimensions below for a multi-device setting.
+        mesh = tf.experimental.dtensor.create_mesh([("batch", 1), ("model", 1)])
+        layout_map = keras_nlp.models.OPTCausalLM.create_layout_map(mesh)
+
+        with layout_map.scope():
+            opt_lm = keras_nlp.models.OPTCausalLM.from_preset("opt_125m_en")
+        ```
+        """
+        # As this task has no new variables, we just re-use the backbone method.
+        return cls.backbone_cls.create_layout_map(mesh)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_tokenizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,123 +8,117 @@
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
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.opt.opt_preprocessor import OPTPreprocessor
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
+from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
-@keras_nlp_export("keras_nlp.models.OPTCausalLMPreprocessor")
-class OPTCausalLMPreprocessor(OPTPreprocessor):
-    """OPT Causal LM preprocessor.
+@keras_nlp_export("keras_nlp.models.RobertaTokenizer")
+class RobertaTokenizer(BytePairTokenizer):
+    """A RoBERTa tokenizer using Byte-Pair Encoding subword segmentation.
 
-    This preprocessing layer is primarily meant to be used with
-    `keras_nlp.models.OPTCausalLM`. By default, it will take in batches of
-    strings, and return outputs in a `(x, y, sample_weight)` format, where the
-    `y` label is the next token id in the `x` sequence. For use with generation,
-    pass `return_labels=False` in which case the output will simply be the
-    encoded string features.
+    This tokenizer class will tokenize raw strings into integer sequences and
+    is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
+    underlying tokenizer, it will check for all special tokens needed by RoBERTa
+    models and provides a `from_preset()` method to automatically download
+    a matching vocabulary for a RoBERTa preset.
+
+    This tokenizer does not provide truncation or padding of inputs. It can be
+    combined with a `keras_nlp.models.RobertaPreprocessor` layer for input
+    packing.
+
+    If input is a batch of strings (rank > 0), the layer will output a
+    `tf.RaggedTensor` where the last dimension of the output is ragged.
+
+    If input is a scalar string (rank == 0), the layer will output a dense
+    `tf.Tensor` with static shape `[None]`.
 
     Args:
-        tokenizer: A `keras_nlp.models.OPTTokenizer` instance.
-        sequence_length: The length of the packed inputs.
-        add_start_token: If true, the preprocessor will append the tokenizer
-            start token to each input sequence.
-        add_end_token: If true, the preprocessor will append the tokenizer
-            end token to each input sequence.
-
-    Call arguments:
-        x: A string `tf.Tensor` or list of python strings.
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
+
+    # Batched input.
+    tokenizer(["The quick brown fox jumped.", "The fox slept."])
 
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
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.opt.opt_causal_lm_preprocessor import (
+from keras_nlp.src.models.opt.opt_causal_lm_preprocessor import (
     OPTCausalLMPreprocessor,
 )
-from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 
 
 class OPTCausalLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
             "<pad>": 0,
             "</s>": 1,
@@ -146,7 +146,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """OPT preprocessor layer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.start_end_packer import StartEndPacker
-from keras_nlp.models.opt.opt_presets import backbone_presets
-from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.start_end_packer import StartEndPacker
+from keras_nlp.src.models.opt.opt_presets import backbone_presets
+from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.OPTPreprocessor")
 class OPTPreprocessor(Preprocessor):
     """OPT preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do 2 things:
@@ -59,15 +59,15 @@
         sequence_length: The length of the packed inputs.
         add_start_token: If true, the preprocessor will append the tokenizer
             start token to each input sequence.
         add_end_token: If true, the preprocessor will append the tokenizer
             end token to each input sequence.
 
     Call arguments:
-        x: A string `tf.Tensor` or list of python strings.
+        x: A string, `tf.Tensor` or list of python strings.
         y: Any label data. Will be passed through unaltered.
         sample_weight: Any label weight data. Will be passed through unaltered.
         sequence_length: Pass to override the configured `sequence_length` of
             the layer.
         add_start_token: Pass to override the configure value of
             `add_start_token` on the layer.
         add_end_token: Pass to override the configure value of
@@ -186,7 +186,8 @@
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
 
     @classproperty
     def tokenizer_cls(cls):
         return OPTTokenizer
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_preprocessor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.opt.opt_preprocessor import OPTPreprocessor
-from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.src.models.opt.opt_preprocessor import OPTPreprocessor
+from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 
 
 class OPTPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
             "<pad>": 0,
             "</s>": 1,
@@ -134,7 +134,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_presets.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,7 +126,8 @@
         "weights_hash": "543120fbe601b70e6ec04cc909781e21",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/opt_6.7b_en/v1/vocab.json",
         "vocabulary_hash": "cf410ee085c5c69c957bb1f6d8456596",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/opt_6.7b_en/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
 }
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_presets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.opt.opt_backbone import OPTBackbone
-from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
+from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 
 
 @pytest.mark.large
 class OPTPresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
     A smoke test for GPT-2 presets we run continuously.
 
@@ -103,7 +103,8 @@
             }
             model(input_data)
 
     def test_load_tokenizers(self):
         for preset in OPTTokenizer.presets:
             tokenizer = OPTTokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """OPT tokenizer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.opt.opt_presets import backbone_presets
-from keras_nlp.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.opt.opt_presets import backbone_presets
+from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.OPTTokenizer")
 class OPTTokenizer(BytePairTokenizer):
     """An OPT tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -122,7 +122,8 @@
     def get_config(self):
         config = super().get_config()
         # In the constructor, we pass the list of special tokens to the
         # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
         # delete it from the config here.
         del config["unsplittable_tokens"]
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_tokenizer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.src.models.opt.opt_tokenizer import OPTTokenizer
 
 
 class OPTTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
             "<pad>": 0,
             "</s>": 1,
@@ -101,7 +101,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from tensorflow import keras
 
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class Preprocessor(keras.layers.Layer):
     """Base class for model preprocessors."""
 
     def __init__(self, *args, **kwargs):
@@ -129,7 +129,8 @@
         if cls.from_preset.__doc__ is None:
             cls.from_preset.__func__.__doc__ = Preprocessor.from_preset.__doc__
             format_docstring(
                 preprocessor_name=cls.__name__,
                 example_preset_name=next(iter(cls.presets), ""),
                 preset_names='", "'.join(cls.presets),
             )(cls.from_preset.__func__)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,180 +8,164 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""RoBERTa backbone model."""
-
-import copy
+"""GPT2 Causal LM preprocessor layer."""
 
 import tensorflow as tf
-from tensorflow import keras
+from absl import logging
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.token_and_position_embedding import (
-    TokenAndPositionEmbedding,
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
+from keras_nlp.src.utils.keras_utils import (
+    convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.layers.transformer_encoder import TransformerEncoder
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.utils.python_utils import classproperty
-
-
-def roberta_kernel_initializer(stddev=0.02):
-    return keras.initializers.TruncatedNormal(stddev=stddev)
-
-
-@keras_nlp_export("keras_nlp.models.RobertBackbone")
-class RobertaBackbone(Backbone):
-    """A RoBERTa encoder network.
-
-    This network implements a bi-directional Transformer-based encoder as
-    described in ["RoBERTa: A Robustly Optimized BERT Pretraining Approach"](https://arxiv.org/abs/1907.11692).
-    It includes the embedding lookups and transformer layers, but does not
-    include the masked language model head used during pretraining.
-
-    The default constructor gives a fully customizable, randomly initialized
-    RoBERTa encoder with any number of layers, heads, and embedding
-    dimensions. To load preset architectures and weights, use the `from_preset()`
-    constructor.
-
-    Disclaimer: Pre-trained models are provided on an "as is" basis, without
-    warranties or conditions of any kind. The underlying model is provided by a
-    third party and subject to a separate license, available
-    [here](https://github.com/facebookresearch/fairseq).
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+
+
+@keras_nlp_export("keras_nlp.models.GPT2CausalLMPreprocessor")
+class GPT2CausalLMPreprocessor(GPT2Preprocessor):
+    """GPT2 Causal LM preprocessor.
+
+    This preprocessing layer is meant for use with
+    `keras_nlp.models.GPT2CausalLM`. By default, it will take in batches of
+    strings, and return outputs in a `(x, y, sample_weight)` format, where the
+    `y` label is the next token id in the `x` sequence.
+
+    For use with generation, the layer also exposes two methods
+    `generate_preprocess()` and `generate_postprocess()`. When this preprocessor
+    is attached to a `keras_nlp.models.GPT2CausalLM` instance, these methods
+    will be called implicitly in `generate()`. They can also be called
+    standalone (e.g. to precompute preprocessing inputs for generation in a
+    separate process).
 
     Args:
-        vocabulary_size: int. The size of the token vocabulary.
-        num_layers: int. The number of transformer layers.
-        num_heads: int. The number of attention heads for each transformer.
-            The hidden size must be divisible by the number of attention heads.
-        hidden_dim: int. The size of the transformer encoding layer.
-        intermediate_dim: int. The output dimension of the first Dense layer in
-            a two-layer feedforward network for each transformer.
-        dropout: float. Dropout probability for the Transformer encoder.
-        max_sequence_length: int. The maximum sequence length this encoder can
-            consume. The sequence length of the input must be less than
-            `max_sequence_length` default value. This determines the variable
-            shape for positional embeddings.
+        tokenizer: A `keras_nlp.models.GPT2Tokenizer` instance.
+        sequence_length: The length of the packed inputs.
+        add_start_token: If true, the preprocessor will prepend the tokenizer
+            start token to each input sequence.
+        add_end_token: If true, the preprocessor will append the tokenizer
+            end token to each input sequence.
+
+    Call arguments:
+        x: A string, `tf.Tensor` or list of python strings.
+        y: Label data. Should always be `None` as the layer generates labels.
+        sample_weight: Label weights. Should always be `None` as the layer
+            generates label weights.
+        sequence_length: Pass to override the configured `sequence_length` of
+            the layer.
 
     Examples:
     ```python
-    input_data = {
-        "token_ids": tf.ones(shape=(1, 12), dtype=tf.int64),
-        "padding_mask": tf.constant(
-            [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)),
-    }
-
-    # Pretrained RoBERTa encoder
-    model = keras_nlp.models.RobertaBackbone.from_preset("roberta_base_en")
-    model(input_data)
-
-    # Randomly initialized RoBERTa model with custom config
-    model = keras_nlp.models.RobertaBackbone(
-        vocabulary_size=50265,
-        num_layers=4,
-        num_heads=4,
-        hidden_dim=256,
-        intermediate_dim=512,
-        max_sequence_length=128,
+    # Load the preprocessor from a preset.
+    preprocessor = keras_nlp.models.GPT2CausalLMPreprocessor.from_preset(
+        "gpt2_base_en"
     )
-    model(input_data)
-    ```
+
+    # Tokenize and pack a single sentence.
+    sentence = tf.constant("League of legends")
+    preprocessor(sentence)
+    # Same output.
+    preprocessor("League of legends")
+
+    # Tokenize a batch of sentences.
+    sentences = tf.constant(["Taco tuesday", "Fish taco please!"])
+    preprocessor(sentences)
+    # Same output.
+    preprocessor(["Taco tuesday", "Fish taco please!"])
+
+    # Map a dataset to preprocess a single sentence.
+    features = tf.constant(
+        [
+            "Avatar 2 is amazing!",
+            "Well, I am not sure.",
+        ]
+    )
+    labels = tf.constant([1, 0])
+    ds = tf.data.Dataset.from_tensor_slices((features, labels))
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+
+    # Map a dataset to preprocess unlabled sentences.
+    ds = tf.data.Dataset.from_tensor_slices(features)
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
     """
 
-    def __init__(
+    def call(
         self,
-        vocabulary_size,
-        num_layers,
-        num_heads,
-        hidden_dim,
-        intermediate_dim,
-        dropout=0.1,
-        max_sequence_length=512,
-        **kwargs,
+        x,
+        y=None,
+        sample_weight=None,
+        sequence_length=None,
     ):
-        # Inputs
-        token_id_input = keras.Input(
-            shape=(None,), dtype=tf.int32, name="token_ids"
-        )
-        padding_mask = keras.Input(
-            shape=(None,), dtype=tf.int32, name="padding_mask"
+        if y is not None or sample_weight is not None:
+            logging.warning(
+                "`GPT2CausalLMPreprocessor` generates `y` and `sample_weight` "
+                "based on your input data, but your data already contains `y` "
+                "or `sample_weight`. Your `y` and `sample_weight` will be "
+                "ignored."
+            )
+        sequence_length = sequence_length or self.sequence_length
+
+        x = convert_inputs_to_list_of_tensor_segments(x)[0]
+        x = self.tokenizer(x)
+        # Pad with one extra token to account for the truncation below.
+        token_ids, padding_mask = self.packer(
+            x,
+            sequence_length=sequence_length + 1,
+            add_start_value=self.add_start_token,
+            add_end_value=self.add_end_token,
         )
+        # The last token does not have a next token, so we truncate it out.
+        x = {
+            "token_ids": token_ids[..., :-1],
+            "padding_mask": padding_mask[..., :-1],
+        }
+        # Target `y` will be the next token.
+        y, sample_weight = token_ids[..., 1:], padding_mask[..., 1:]
+        return pack_x_y_sample_weight(x, y, sample_weight)
 
-        # Embed tokens and positions.
-        embedding_layer = TokenAndPositionEmbedding(
-            vocabulary_size=vocabulary_size,
-            sequence_length=max_sequence_length,
-            embedding_dim=hidden_dim,
-            embeddings_initializer=roberta_kernel_initializer(),
-            name="embeddings",
-        )
-        embedding = embedding_layer(token_id_input)
+    def generate_preprocess(
+        self,
+        x,
+        sequence_length=None,
+    ):
+        """Covert strings to integer token input for generation.
 
-        # Sum, normalize and apply dropout to embeddings.
-        x = keras.layers.LayerNormalization(
-            name="embeddings_layer_norm",
-            axis=-1,
-            epsilon=1e-5,  # Original paper uses this epsilon value
-            dtype=tf.float32,
-        )(embedding)
-        x = keras.layers.Dropout(
-            dropout,
-            name="embeddings_dropout",
-        )(x)
-
-        # Apply successive transformer encoder blocks.
-        for i in range(num_layers):
-            x = TransformerEncoder(
-                num_heads=num_heads,
-                intermediate_dim=intermediate_dim,
-                activation="gelu",
-                dropout=dropout,
-                layer_norm_epsilon=1e-5,
-                kernel_initializer=roberta_kernel_initializer(),
-                name=f"transformer_layer_{i}",
-            )(x, padding_mask=padding_mask)
-
-        # Instantiate using Functional API Model constructor
-        super().__init__(
-            inputs={
-                "token_ids": token_id_input,
-                "padding_mask": padding_mask,
-            },
-            outputs=x,
-            **kwargs,
+        Similar to calling the layer for training, this method takes in strings
+        or tensor strings, tokenizes and packs the input, and computes a padding
+        mask masking all inputs not filled in with a padded value.
+
+        Unlike calling the the layer for training, this method does not compute
+        labels and will never append a `tokenizer.end_token_id` to the end of
+        the sequence (as generation is expected to continue at the end of the
+        inputted prompt).
+        """
+        x = convert_inputs_to_list_of_tensor_segments(x)[0]
+        x = self.tokenizer(x)
+        token_ids, padding_mask = self.packer(
+            x, sequence_length=sequence_length, add_end_value=False
         )
-        # All references to `self` below this line
-        self.vocabulary_size = vocabulary_size
-        self.num_layers = num_layers
-        self.num_heads = num_heads
-        self.hidden_dim = hidden_dim
-        self.intermediate_dim = intermediate_dim
-        self.dropout = dropout
-        self.max_sequence_length = max_sequence_length
-        self.start_token_index = 0
-
-    def get_config(self):
-        config = super().get_config()
-        config.update(
-            {
-                "vocabulary_size": self.vocabulary_size,
-                "num_layers": self.num_layers,
-                "num_heads": self.num_heads,
-                "hidden_dim": self.hidden_dim,
-                "intermediate_dim": self.intermediate_dim,
-                "dropout": self.dropout,
-                "max_sequence_length": self.max_sequence_length,
-            }
-        )
-        return config
+        return {
+            "token_ids": token_ids,
+            "padding_mask": padding_mask,
+        }
+
+    def generate_postprocess(
+        self,
+        x,
+    ):
+        """Covert integer token output to strings for generation.
+
+        This method reverses `generate_preprocess()`, by first removing all
+        padding and start/end tokens, and then converting the interger sequence
+        back to a string.
+        """
+        token_ids, padding_mask = x["token_ids"], x["padding_mask"]
+        # Strip any special tokens during detokenization (e.g. the start and
+        # end markers). In the future we could make this configurable.
+        padding_mask = padding_mask & (token_ids != self.tokenizer.end_token_id)
+        token_ids = tf.ragged.boolean_mask(token_ids, padding_mask)
+        return self.tokenizer.detokenize(token_ids)
 
-    @property
-    def token_embedding(self):
-        return self.get_layer("embeddings").token_embedding
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/opt/opt_backbone_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,117 +7,134 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""Test for RoBERTa backbone models."""
+"""Test for OPT backbone models."""
 
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.src.models.opt.opt_backbone import OPTBackbone
 
 
-class RobertaBackboneTest(tf.test.TestCase, parameterized.TestCase):
+class OPTTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = RobertaBackbone(
+        # For DTensor.
+        keras.backend.experimental.enable_tf_random_generator()
+        keras.utils.set_random_seed(1337)
+
+        self.backbone = OPTBackbone(
             vocabulary_size=10,
             num_layers=2,
             num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=5,
         )
-        self.batch_size = 8
         self.input_batch = {
             "token_ids": tf.ones((2, 5), dtype="int32"),
             "padding_mask": tf.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_valid_call_roberta(self):
+    def test_valid_call_opt(self):
         self.backbone(self.input_batch)
 
     def test_token_embedding(self):
         output = self.backbone.token_embedding(self.input_batch["token_ids"])
         self.assertEqual(output.shape, (2, 5, 2))
 
     def test_name(self):
-        self.assertRegexpMatches(self.backbone.name, "roberta_backbone")
+        # Check default name passed through
+        self.assertRegexpMatches(self.backbone.name, "opt_backbone")
+
+    def test_variable_sequence_length_call_opt(self):
+        for seq_length in (2, 3, 4):
+            input_data = {
+                "token_ids": tf.ones((2, seq_length), dtype="int32"),
+                "padding_mask": tf.ones((2, seq_length), dtype="int32"),
+            }
+            self.backbone(input_data)
 
     def test_predict(self):
         self.backbone.predict(self.input_batch)
         self.backbone.predict(self.input_dataset)
 
     def test_serialization(self):
         new_backbone = keras.utils.deserialize_keras_object(
             keras.utils.serialize_keras_object(self.backbone)
         )
         self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
-    def test_variable_sequence_length_call_roberta(self):
-        for seq_length in (2, 3, 4):
-            input_data = {
-                "token_ids": tf.ones((2, seq_length), dtype="int32"),
-                "padding_mask": tf.ones((2, seq_length), dtype="int32"),
-            }
-            output = self.backbone(input_data)
-            self.assertAllEqual(
-                tf.shape(output),
-                [2, seq_length, self.backbone.hidden_dim],
-            )
-
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         model_output = self.backbone(self.input_batch)
         path = os.path.join(self.get_temp_dir(), filename)
         # Don't save traces in the tf format, we check compilation elsewhere.
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         self.backbone.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, RobertaBackbone)
+        self.assertIsInstance(restored_model, OPTBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(model_output, restored_output)
 
+    def test_create_layout_map(self):
+        mesh = tf.experimental.dtensor.create_mesh([("batch", 1), ("model", 1)])
+        with OPTBackbone.create_layout_map(mesh).scope():
+            OPTBackbone(
+                vocabulary_size=10,
+                num_layers=2,
+                num_heads=2,
+                hidden_dim=2,
+                intermediate_dim=4,
+                max_sequence_length=5,
+            )
+        # Using DTensor enables the mlir bridge as a side effect. Eventually
+        # this will be default, but for now we have compile errors with the
+        # bridge elsewhere and must disable. See
+        # https://github.com/keras-team/keras-nlp/issues/1001
+        tf.config.experimental.disable_mlir_bridge()
+
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
-class RobertaBackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
+class OPTBackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.backbone = RobertaBackbone(
+            self.backbone = OPTBackbone(
                 vocabulary_size=1000,
                 num_layers=2,
                 num_heads=2,
-                hidden_dim=64,
+                hidden_dim=32,
                 intermediate_dim=128,
                 max_sequence_length=128,
             )
         self.input_batch = {
             "token_ids": tf.ones((8, 128), dtype="int32"),
             "padding_mask": tf.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
         self.backbone.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_classifier.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # limitations under the License.
 """RoBERTa classification model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
-from keras_nlp.models.roberta.roberta_backbone import roberta_kernel_initializer
-from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
-from keras_nlp.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
+from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
+from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.RobertaClassifier")
 class RobertaClassifier(Task):
     """An end-to-end RoBERTa model for classification tasks.
 
     This model attaches a classification head to a
@@ -209,7 +209,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return RobertaPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_classifier_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_classifier_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
-from keras_nlp.models.roberta.roberta_classifier import RobertaClassifier
-from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
-from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.src.models.roberta.roberta_classifier import RobertaClassifier
+from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 
 
 class RobertaClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
             "<s>": 0,
             "<pad>": 1,
@@ -131,7 +131,8 @@
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, RobertaClassifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 # limitations under the License.
 """RoBERTa masked lm model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_head import MaskedLMHead
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
-from keras_nlp.models.roberta.roberta_backbone import roberta_kernel_initializer
-from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_head import MaskedLMHead
+from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
+from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import (
     RobertaMaskedLMPreprocessor,
 )
-from keras_nlp.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.models.task import Task
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.RobertaMaskedLM")
 class RobertaMaskedLM(Task):
     """An end-to-end RoBERTa model for the masked language modeling task.
 
     This model will train RoBERTa on a masked language modeling task.
@@ -150,7 +150,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return RobertaMaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """RoBERTa masked language model preprocessor layer."""
 
 from absl import logging
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
-from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
+from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 @keras_nlp_export("keras_nlp.models.RobertaMaskedLMPreprocessor")
 class RobertaMaskedLMPreprocessor(RobertaPreprocessor):
     """RoBERTa preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
@@ -180,7 +180,8 @@
             "token_ids": masker_outputs["token_ids"],
             "padding_mask": padding_mask,
             "mask_positions": masker_outputs["mask_positions"],
         }
         y = masker_outputs["mask_ids"]
         sample_weight = masker_outputs["mask_weights"]
         return pack_x_y_sample_weight(x, y, sample_weight)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
+from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import (
     RobertaMaskedLMPreprocessor,
 )
-from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 
 
 class RobertaMaskedLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         vocab = {
             "<s>": 0,
             "<pad>": 1,
@@ -166,7 +166,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         outputs = model(input_data)[0]["token_ids"]
         restored_outputs = restored_model(input_data)[0]["token_ids"]
         self.assertAllEqual(outputs, restored_outputs)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_masked_lm_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
-from keras_nlp.models.roberta.roberta_masked_lm import RobertaMaskedLM
-from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
+from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.src.models.roberta.roberta_masked_lm import RobertaMaskedLM
+from keras_nlp.src.models.roberta.roberta_masked_lm_preprocessor import (
     RobertaMaskedLMPreprocessor,
 )
-from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 
 
 class RobertaMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
             "<s>": 0,
             "<pad>": 1,
@@ -129,7 +129,8 @@
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, RobertaMaskedLM)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output, atol=0.01, rtol=0.01)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_multi_segment_packer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_multi_segment_packer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.utils.tf_utils import assert_tf_text_installed
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
@@ -140,7 +140,8 @@
             shape=shape, default_value=self.pad_value
         )
         # Remove the batch dim if added.
         if rank_1:
             token_ids = tf.squeeze(token_ids, 0)
 
         return token_ids
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """RoBERTa preprocessor layer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.models.roberta.roberta_multi_segment_packer import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.models.roberta.roberta_multi_segment_packer import (
     RobertaMultiSegmentPacker,
 )
-from keras_nlp.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.models.roberta.roberta_presets import backbone_presets
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.RobertaPreprocessor")
 class RobertaPreprocessor(Preprocessor):
     """A RoBERTa preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -176,7 +176,8 @@
     @classproperty
     def tokenizer_cls(cls):
         return RobertaTokenizer
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_preprocessor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
-from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 
 
 class RobertaPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         vocab = {
             "<s>": 0,
             "<pad>": 1,
@@ -166,7 +166,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_presets.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,7 +67,8 @@
         "weights_hash": "1978b864c317a697fe62a894d3664f14",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/roberta_large_en/v1/vocab.json",
         "vocabulary_hash": "be4d3c6f3f5495426b2c03b334334354",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/roberta_large_en/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
 }
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_presets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
-from keras_nlp.models.roberta.roberta_classifier import RobertaClassifier
-from keras_nlp.models.roberta.roberta_masked_lm import RobertaMaskedLM
-from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
-from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.src.models.roberta.roberta_classifier import RobertaClassifier
+from keras_nlp.src.models.roberta.roberta_masked_lm import RobertaMaskedLM
+from keras_nlp.src.models.roberta.roberta_preprocessor import RobertaPreprocessor
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 
 
 @pytest.mark.large
 class RobertaPresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
     A smoke test for RoBERTa presets we run continuously.
 
@@ -243,7 +243,8 @@
             tokenizer = RobertaTokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
 
     def test_load_preprocessors(self):
         for preset in RobertaPreprocessor.presets:
             preprocessor = RobertaPreprocessor.from_preset(preset)
             preprocessor("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_tokenizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,116 +8,89 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""RoBERTa tokenizer."""
+"""T5 tokenizer."""
 
-import copy
+from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.roberta.roberta_presets import backbone_presets
-from keras_nlp.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
 
 
-@keras_nlp_export("keras_nlp.models.RobertaTokenizer")
-class RobertaTokenizer(BytePairTokenizer):
-    """A RoBERTa tokenizer using Byte-Pair Encoding subword segmentation.
+@keras.utils.register_keras_serializable(package="keras_nlp")
+class T5Tokenizer(SentencePieceTokenizer):
+    """T5 tokenizer layer based on SentencePiece.
 
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
+    T5 models and provides a `from_preset()` method to automatically
+    download a matching vocabulary for a T5 preset.
 
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
+        proto: Either a `string` path to a SentencePiece proto file, or a
+            `bytes` object with a serialized SentencePiece proto. See the
+            [SentencePiece repository](https://github.com/google/sentencepiece)
+            for more details on the format.
 
     Examples:
+
     ```python
-    # Unbatched input.
-    tokenizer = keras_nlp.models.RobertaTokenizer.from_preset(
-        "roberta_base_en",
+    bytes_io = io.BytesIO()
+    ds = tf.data.Dataset.from_tensor_slices(["The quick brown fox jumped."])
+    sentencepiece.SentencePieceTrainer.train(
+        sentence_iterator=ds.as_numpy_iterator(),
+        model_writer=bytes_io,
+        vocab_size=8,
+        model_type="WORD",
+        bos_id=-1,
+        pad_id=0,
+        eos_id=1,
+        unk_id=2,
+        pad_piece="<pad>",
+        eos_piece="</s>",
+        unk_piece="<unk>",
+    )
+    tokenizer = keras_nlp.models.T5Tokenizer(
+        proto=bytes_io.getvalue(),
     )
     tokenizer("The quick brown fox jumped.")
 
-    # Batched input.
-    tokenizer(["The quick brown fox jumped.", "The fox slept."])
+    # Batched inputs.
+    tokenizer(["the quick brown fox", "the earth is round"])
+
+    # Unbatched inputs.
+    tokenizer("the quick brown fox")
 
     # Detokenization.
     tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
-
-    # Custom vocabulary.
-    # Note: 'Ġ' is space
-    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
-    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
-    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
-    merges += ["Ġ f", "o x", "Ġf ox"]
-    tokenizer = keras_nlp.models.RobertaTokenizer(
-        vocabulary=vocab,
-        merges=merges
-    )
-    tokenizer(["a quick fox", "a fox quick"])
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
-        )
+    def __init__(self, proto, **kwargs):
+        super().__init__(proto=proto, **kwargs)
 
-        # Check whether special tokens are present in the vocabulary.
-        for token in [start_token, pad_token, end_token, mask_token]:
+        # Check for necessary special tokens.
+        end_token = "</s>"
+        pad_token = "<pad>"
+        for token in [pad_token]:
             if token not in self.get_vocabulary():
                 raise ValueError(
                     f"Cannot find token `'{token}'` in the provided "
                     f"`vocabulary`. Please provide `'{token}'` in your "
                     "`vocabulary` or use a pretrained `vocabulary` name."
                 )
 
-        self.start_token_id = self.token_to_id(start_token)
         self.pad_token_id = self.token_to_id(pad_token)
         self.end_token_id = self.token_to_id(end_token)
-        self.mask_token_id = self.token_to_id(mask_token)
+        # T5 uses the same start token as end token, i.e., "<\s>".
+        self.start_token_id = self.end_token_id
 
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
-
-    def get_config(self):
-        config = super().get_config()
-        # In the constructor, we pass the list of special tokens to the
-        # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
-        # delete it from the config here.
-        del config["unsplittable_tokens"]
-        return config
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/roberta/roberta_tokenizer_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.src.models.roberta.roberta_tokenizer import RobertaTokenizer
 
 
 class RobertaTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         vocab = {
             "<s>": 0,
             "<pad>": 1,
@@ -102,7 +102,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # limitations under the License.
 
 """T5 backbone model."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers.transformer_layer_utils import compute_causal_mask
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.models.t5.t5_layer_norm import T5LayerNorm
-from keras_nlp.models.t5.t5_transformer_layer import T5TransformerLayer
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.layers.transformer_layer_utils import compute_causal_mask
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.models.t5.t5_layer_norm import T5LayerNorm
+from keras_nlp.src.models.t5.t5_transformer_layer import T5TransformerLayer
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class T5Backbone(Backbone):
     """T5 encoder-decoder backbone model.
 
     T5 is a LLM pretrained on a mix of unsupervised and supervised tasks,
@@ -233,7 +233,8 @@
     @property
     def token_embedding(self):
         return self.get_layer("token_embedding")
 
     @classproperty
     def presets(cls):
         return {}
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_backbone_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.t5.t5_backbone import T5Backbone
+from keras_nlp.src.models.t5.t5_backbone import T5Backbone
 
 
 class T5Test(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.backbone = T5Backbone(
             vocabulary_size=4,
             num_layers=2,
@@ -138,7 +138,8 @@
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
         outputs = self.backbone.predict(self.input_dataset)
         self.assertIn("encoder_sequence_output", outputs)
         self.assertIn("decoder_sequence_output", outputs)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_layer_norm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_layer_norm.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,7 +27,8 @@
 
     def call(self, hidden_states):
         variance = tf.math.reduce_mean(
             tf.math.square(hidden_states), axis=-1, keepdims=True
         )
         hidden_states = hidden_states * tf.math.rsqrt(variance + self.epsilon)
         return self.weight * hidden_states
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_multi_head_attention.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_multi_head_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,7 +318,8 @@
 
         attention_output = tf.matmul(
             weights, value_states
         )  # (batch_size, num_heads, query_length, dim_per_head)
 
         attention_output = self.output_projector(unshape(attention_output))
         return (attention_output, position_bias)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_tokenizer_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.t5.t5_tokenizer import T5Tokenizer
+from keras_nlp.src.models.t5.t5_tokenizer import T5Tokenizer
 
 
 class T5TokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
@@ -108,7 +108,8 @@
         model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_transformer_layer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/t5/t5_transformer_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from tensorflow import keras
 
-from keras_nlp.models.t5.t5_layer_norm import T5LayerNorm
-from keras_nlp.models.t5.t5_multi_head_attention import T5MultiHeadAttention
+from keras_nlp.src.models.t5.t5_layer_norm import T5LayerNorm
+from keras_nlp.src.models.t5.t5_multi_head_attention import T5MultiHeadAttention
 
 
 class T5TransformerLayer(keras.layers.Layer):
     def __init__(
         self,
         is_decoder,
         hidden_dim,
@@ -129,7 +129,8 @@
             x = self.input_projector(x)
         x = self.dropout_layer(x, training=training)
         x = self.output_projector(x)
         x = self.dropout_layer(x, training=training)
         x = x + residual
 
         return x, position_bias
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/task.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 """Base class for Task models."""
 
 import os
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.utils.keras_utils import print_msg
-from keras_nlp.utils.keras_utils import print_row
-from keras_nlp.utils.pipeline_model import PipelineModel
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.utils.keras_utils import print_msg
+from keras_nlp.src.utils.keras_utils import print_row
+from keras_nlp.src.utils.pipeline_model import PipelineModel
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class Task(PipelineModel):
     """Base class for Task models."""
 
     def __init__(self, *args, **kwargs):
@@ -266,7 +266,8 @@
 
         super().summary(
             line_length=line_length,
             positions=positions,
             print_fn=print_fn,
             **kwargs,
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/task_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/task_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.keras.losses import SparseCategoricalCrossentropy
 
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.models.task import Task
-from keras_nlp.tokenizers.tokenizer import Tokenizer
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.tokenizers.tokenizer import Tokenizer
 
 
 class SimpleTokenizer(Tokenizer):
     def vocabulary_size(self):
         return 10
 
 
@@ -74,7 +74,8 @@
         with self.assertRaises(ValueError):
             model.compile(loss=SparseCategoricalCrossentropy(from_logits=True))
 
         # Non-standard activations should not throw.
         model = SimpleTask(activation="tanh")
         model.compile(loss=SparseCategoricalCrossentropy(from_logits=True))
         model.compile(loss=SparseCategoricalCrossentropy(from_logits=False))
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 # limitations under the License.
 """Whisper backbone model."""
 
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers.position_embedding import PositionEmbedding
-from keras_nlp.layers.token_and_position_embedding import (
+from keras_nlp.src.layers.position_embedding import PositionEmbedding
+from keras_nlp.src.layers.token_and_position_embedding import (
     TokenAndPositionEmbedding,
 )
-from keras_nlp.models.backbone import Backbone
-from keras_nlp.models.whisper.whisper_decoder import WhisperDecoder
-from keras_nlp.models.whisper.whisper_encoder import WhisperEncoder
+from keras_nlp.src.models.backbone import Backbone
+from keras_nlp.src.models.whisper.whisper_decoder import WhisperDecoder
+from keras_nlp.src.models.whisper.whisper_encoder import WhisperEncoder
 
 # We hardcode the number of mel-frequency filters:
 # https://github.com/openai/whisper/blob/v20230124/whisper/audio.py#L101-L102.
 # TODO: If needed, we can make it configurable.
 NUM_MELS = 80
 
 
@@ -286,7 +286,8 @@
         return config
 
     @property
     def token_embedding(self):
         return self.get_layer(
             "decoder_token_and_position_embedding"
         ).token_embedding
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_backbone_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.whisper.whisper_backbone import NUM_MELS
-from keras_nlp.models.whisper.whisper_backbone import WhisperBackbone
+from keras_nlp.src.models.whisper.whisper_backbone import NUM_MELS
+from keras_nlp.src.models.whisper.whisper_backbone import WhisperBackbone
 
 
 class WhisperBackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.backbone = WhisperBackbone(
             vocabulary_size=10,
             num_layers=2,
@@ -160,7 +160,8 @@
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
         self.backbone.compile()
         self.backbone.predict(self.input_dataset)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_decoder.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Whisper decoder block."""
 
 from tensorflow import keras
 
-from keras_nlp.layers.transformer_decoder import TransformerDecoder
+from keras_nlp.src.layers.transformer_decoder import TransformerDecoder
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class WhisperDecoder(TransformerDecoder):
     """A Whisper decoder.
 
     Inherits from `keras_nlp.layers.TransformerDecoder`, and overrides the
@@ -30,7 +30,8 @@
         super()._build(input_shape, has_cross_attention)
 
         # Since there is no exposed option for this in MHA, we will reach into
         # the internals of the layer for now.
         self._self_attention_layer._key_dense.bias_axes = None
         if has_cross_attention:
             self._cross_attention_layer._key_dense.bias_axes = None
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_encoder.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/whisper/whisper_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Whisper encoder block."""
 
 from tensorflow import keras
 
-from keras_nlp.layers.transformer_encoder import TransformerEncoder
+from keras_nlp.src.layers.transformer_encoder import TransformerEncoder
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class WhisperEncoder(TransformerEncoder):
     """A Whisper encoder.
 
     Inherits from `keras_nlp.layers.TransformerEncoder`, and overrides the
@@ -28,7 +28,8 @@
 
     def _build(self, input_shape):
         super()._build(input_shape)
 
         # Since there is no exposed option for this in MHA, we will reach into
         # the internals of the layer for now.
         self._self_attention_layer._key_dense.bias_axes = None
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """XLM-RoBERTa backbone model."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.roberta import roberta_backbone
-from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.roberta import roberta_backbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.XLMRobertaBackbone")
 class XLMRobertaBackbone(roberta_backbone.RobertaBackbone):
     """An XLM-RoBERTa encoder network.
 
     This class implements a bi-directional Transformer-based encoder as
@@ -81,7 +81,8 @@
     model(input_data)
     ```
     """
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,114 +8,128 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for XLM-RoBERTa backbone models."""
+"""Tests for XLM-RoBERTa tokenizer."""
 
+import io
 import os
 
 import pytest
+import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
+    XLMRobertaTokenizer,
+)
 
 
-class XLMRobertaBackboneTest(tf.test.TestCase, parameterized.TestCase):
+class XLMRobertaTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = XLMRobertaBackbone(
-            vocabulary_size=10,
-            num_layers=2,
-            num_heads=2,
-            hidden_dim=2,
-            intermediate_dim=4,
-            max_sequence_length=5,
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round"]
         )
-        self.input_batch = {
-            "token_ids": tf.ones((2, 5), dtype="int32"),
-            "padding_mask": tf.ones((2, 5), dtype="int32"),
-        }
-        self.input_dataset = tf.data.Dataset.from_tensor_slices(
-            self.input_batch
-        ).batch(2)
-
-    def test_valid_call_xlm_roberta(self):
-        self.backbone(self.input_batch)
-
-    def test_token_embedding(self):
-        output = self.backbone.token_embedding(self.input_batch["token_ids"])
-        self.assertEqual(output.shape, (2, 5, 2))
-
-    def test_name(self):
-        # Check default name passed through
-        self.assertRegexpMatches(self.backbone.name, "xlm_roberta_backbone")
-
-    def test_variable_sequence_length_call_xlm_roberta(self):
-        for seq_length in (2, 3, 4):
-            input_data = {
-                "token_ids": tf.ones((2, seq_length), dtype="int32"),
-                "padding_mask": tf.ones((2, seq_length), dtype="int32"),
-            }
-            output = self.backbone(input_data)
-            self.assertAllEqual(
-                tf.shape(output), [2, seq_length, self.backbone.hidden_dim]
-            )
-
-    def test_predict(self):
-        self.backbone.predict(self.input_batch)
-        self.backbone.predict(self.input_dataset)
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=10,
+            model_type="WORD",
+            unk_id=0,
+            bos_id=1,
+            eos_id=2,
+        )
+        self.proto = bytes_io.getvalue()
+
+        self.tokenizer = XLMRobertaTokenizer(proto=self.proto)
+
+    def test_tokenize(self):
+        input_data = "the quick brown fox"
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [4, 9, 5, 7])
+
+    def test_tokenize_batch(self):
+        input_data = tf.constant(["the quick brown fox", "the earth is round"])
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [[4, 9, 5, 7], [4, 6, 8, 10]])
+
+    def test_unk_token(self):
+        input_data = "the quick brown fox running"
+
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [4, 9, 5, 7, 3])
+
+    def test_detokenize(self):
+        input_data = tf.constant([[4, 9, 5, 7]])
+        output = self.tokenizer.detokenize(input_data)
+        self.assertEqual(output, tf.constant(["brown round earth is"]))
+
+    def test_vocabulary(self):
+        vocabulary = self.tokenizer.get_vocabulary()
+        self.assertAllEqual(
+            vocabulary,
+            [
+                "<s>",
+                "<pad>",
+                "</s>",
+                "<unk>",
+                "▁the",
+                "▁brown",
+                "▁earth",
+                "▁fox",
+                "▁is",
+                "▁quick",
+                "▁round",
+                "<mask>",
+            ],
+        )
+        self.assertEqual(self.tokenizer.vocabulary_size(), 12)
+
+    def test_id_to_token(self):
+        print(self.tokenizer.id_to_token(9))
+        self.assertEqual(self.tokenizer.id_to_token(9), "▁quick")
+        self.assertEqual(self.tokenizer.id_to_token(5), "▁brown")
+
+    def test_token_to_id(self):
+        self.assertEqual(self.tokenizer.token_to_id("▁the"), 4)
+        self.assertEqual(self.tokenizer.token_to_id("▁round"), 10)
+        # Test any random OOV token.
+        self.assertEqual(self.tokenizer.token_to_id("<oov-token>"), 3)
+        # Test a special token.
+        self.assertEqual(self.tokenizer.token_to_id("<pad>"), 1)
 
     def test_serialization(self):
-        new_backbone = keras.utils.deserialize_keras_object(
-            keras.utils.serialize_keras_object(self.backbone)
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
         )
-        self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
-        model_output = self.backbone(self.input_batch)
+        input_data = tf.constant(["the quick brown fox"])
+
+        inputs = keras.Input(dtype="string", shape=())
+        outputs = self.tokenizer(inputs)
+        model = keras.Model(inputs, outputs)
+
         path = os.path.join(self.get_temp_dir(), filename)
         # Don't save traces in the tf format, we check compilation elsewhere.
         kwargs = {"save_traces": False} if save_format == "tf" else {}
-        self.backbone.save(path, save_format=save_format, **kwargs)
-        restored_model = keras.models.load_model(path)
-
-        # Check we got the real object back.
-        self.assertIsInstance(restored_model, XLMRobertaBackbone)
-
-        # Check that output matches.
-        restored_output = restored_model(self.input_batch)
-        self.assertAllClose(model_output, restored_output)
+        model.save(path, save_format=save_format, **kwargs)
 
+        restored_model = keras.models.load_model(path)
+        self.assertAllEqual(
+            model(input_data),
+            restored_model(input_data),
+        )
 
-@pytest.mark.tpu
-@pytest.mark.usefixtures("tpu_test_class")
-class XLMRobertaBackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
-    def setUp(self):
-        with self.tpu_strategy.scope():
-            self.backbone = XLMRobertaBackbone(
-                vocabulary_size=1000,
-                num_layers=2,
-                num_heads=2,
-                hidden_dim=64,
-                intermediate_dim=128,
-                max_sequence_length=128,
-            )
-        self.input_batch = {
-            "token_ids": tf.ones((8, 128), dtype="int32"),
-            "padding_mask": tf.ones((8, 128), dtype="int32"),
-        }
-        self.input_dataset = tf.data.Dataset.from_tensor_slices(
-            self.input_batch
-        ).batch(2)
-
-    def test_predict(self):
-        self.backbone.compile()
-        self.backbone.predict(self.input_dataset)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # limitations under the License.
 """XLM-RoBERTa classification model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.roberta.roberta_backbone import roberta_kernel_initializer
-from keras_nlp.models.task import Task
-from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
-from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
     XLMRobertaPreprocessor,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.XLMRobertaClassifier")
 class XLMRobertaClassifier(Task):
     """An end-to-end XLM-RoBERTa model for classification tasks.
 
     This model attaches a classification head to a
@@ -224,7 +224,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return XLMRobertaPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/f_net/f_net_classifier_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,73 +7,77 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for XLM-RoBERTa classification model."""
+"""Tests for FNet classification model."""
 
 import io
 import os
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
-from keras_nlp.models.xlm_roberta.xlm_roberta_classifier import (
-    XLMRobertaClassifier,
-)
-from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
-    XLMRobertaPreprocessor,
-)
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
-    XLMRobertaTokenizer,
-)
+from keras_nlp.src.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.src.models.f_net.f_net_classifier import FNetClassifier
+from keras_nlp.src.models.f_net.f_net_preprocessor import FNetPreprocessor
+from keras_nlp.src.models.f_net.f_net_tokenizer import FNetTokenizer
 
 
-class XLMRobertaClassifierTest(tf.test.TestCase, parameterized.TestCase):
+class FNetClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
+        # Setup Model
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
+
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
-            vocab_size=10,
+            vocab_size=12,
             model_type="WORD",
+            pad_id=3,
             unk_id=0,
-            bos_id=1,
-            eos_id=2,
-        )
-        self.preprocessor = XLMRobertaPreprocessor(
-            tokenizer=XLMRobertaTokenizer(proto=bytes_io.getvalue()),
-            sequence_length=5,
+            bos_id=4,
+            eos_id=5,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
+            bos_piece="[CLS]",
+            eos_piece="[SEP]",
+            user_defined_symbols="[MASK]",
+        )
+
+        self.proto = bytes_io.getvalue()
+
+        self.preprocessor = FNetPreprocessor(
+            tokenizer=FNetTokenizer(proto=self.proto),
+            sequence_length=8,
         )
-        self.backbone = XLMRobertaBackbone(
-            vocabulary_size=10,
+        self.backbone = FNetBackbone(
+            vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
-            num_heads=2,
             hidden_dim=2,
             intermediate_dim=4,
             max_sequence_length=self.preprocessor.packer.sequence_length,
         )
-        self.classifier = XLMRobertaClassifier(
+        self.classifier = FNetClassifier(
             self.backbone,
             num_classes=4,
             preprocessor=self.preprocessor,
             # Check we handle serialization correctly.
             activation=keras.activations.softmax,
-            hidden_dim=4,
         )
 
+        # Setup data.
         self.raw_batch = tf.constant(
             [
                 "the quick brown fox.",
                 "the slow brown fox.",
             ]
         )
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
@@ -90,23 +94,23 @@
         self.classifier.preprocessor = None
         preds2 = self.classifier.predict(self.preprocessed_batch)
         # Assert predictions match.
         self.assertAllClose(preds1, preds2)
         # Assert valid softmax output.
         self.assertAllClose(tf.reduce_sum(preds2, axis=-1), [1.0, 1.0])
 
-    def test_classifier_fit(self):
+    def test_fnet_classifier_fit(self):
         self.classifier.fit(self.raw_dataset)
         self.classifier.preprocessor = None
         self.classifier.fit(self.preprocessed_dataset)
 
     def test_classifier_fit_no_xla(self):
         self.classifier.preprocessor = None
         self.classifier.compile(
-            loss="sparse_categorical_crossentropy",
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
             jit_compile=False,
         )
         self.classifier.fit(self.preprocessed_dataset)
 
     def test_serialization(self):
         config = keras.utils.serialize_keras_object(self.classifier)
         new_classifier = keras.utils.deserialize_keras_object(config)
@@ -115,22 +119,23 @@
             self.classifier.get_config(),
         )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
-    @pytest.mark.large  # Saving is slow, so mark these large.
-    def test_saving_model(self, save_format, filename):
+    @pytest.mark.large
+    def test_saved_model(self, save_format, filename):
         model_output = self.classifier.predict(self.raw_batch)
         path = os.path.join(self.get_temp_dir(), filename)
         # Don't save traces in the tf format, we check compilation elsewhere.
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         self.classifier.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, XLMRobertaClassifier)
+        self.assertIsInstance(restored_model, FNetClassifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 # limitations under the License.
 """XLM-RoBERTa masked lm model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_head import MaskedLMHead
-from keras_nlp.models.roberta.roberta_backbone import roberta_kernel_initializer
-from keras_nlp.models.task import Task
-from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
-from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_head import MaskedLMHead
+from keras_nlp.src.models.roberta.roberta_backbone import roberta_kernel_initializer
+from keras_nlp.src.models.task import Task
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
     XLMRobertaMaskedLMPreprocessor,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.utils.keras_utils import is_xla_compatible
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
+from keras_nlp.src.utils.keras_utils import is_xla_compatible
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.XLMRobertaMaskedLM")
 class XLMRobertaMaskedLM(Task):
     """An end-to-end XLM-RoBERTa model for the masked language modeling task.
 
     This model will train XLM-RoBERTa on a masked language modeling task.
@@ -153,7 +153,8 @@
     @classproperty
     def preprocessor_cls(cls):
         return XLMRobertaMaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """XLM-RoBERTa masked language model preprocessor layer."""
 
 from absl import logging
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
-from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
     XLMRobertaPreprocessor,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 @keras_nlp_export("keras_nlp.models.XLMRobertaMaskedLMPreprocessor")
 class XLMRobertaMaskedLMPreprocessor(XLMRobertaPreprocessor):
     """XLM-RoBERTa preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
@@ -180,7 +180,8 @@
             "token_ids": masker_outputs["token_ids"],
             "padding_mask": padding_mask,
             "mask_positions": masker_outputs["mask_positions"],
         }
         y = masker_outputs["mask_ids"]
         sample_weight = masker_outputs["mask_weights"]
         return pack_x_y_sample_weight(x, y, sample_weight)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,153 +1,129 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for XLM-RoBERTa masked language model preprocessor layer."""
+"""Tests for GPT2 causal LM preprocessor layer."""
 
-import io
 import os
 
 import pytest
-import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
-    XLMRobertaMaskedLMPreprocessor,
-)
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
-    XLMRobertaTokenizer,
+from keras_nlp.src.models.gpt2.gpt2_causal_lm_preprocessor import (
+    GPT2CausalLMPreprocessor,
 )
+from keras_nlp.src.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 
 
-class XLMRobertaMaskedLMPreprocessorTest(
-    tf.test.TestCase, parameterized.TestCase
-):
+class GPT2CausalLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        bytes_io = io.BytesIO()
-        vocab_data = tf.data.Dataset.from_tensor_slices(
-            ["the quick brown fox", "the earth is round"]
-        )
-        sentencepiece.SentencePieceTrainer.train(
-            sentence_iterator=vocab_data.as_numpy_iterator(),
-            model_writer=bytes_io,
-            vocab_size=12,
-            model_type="WORD",
-            pad_id=0,
-            unk_id=1,
-            bos_id=2,
-            eos_id=3,
-            pad_piece="<pad>",
-            unk_piece="<unk>",
-            bos_piece="<s>",
-            eos_piece="</s>",
-            user_defined_symbols="[MASK]",
-        )
-        self.proto = bytes_io.getvalue()
-
-        self.tokenizer = XLMRobertaTokenizer(proto=self.proto)
-        self.preprocessor = XLMRobertaMaskedLMPreprocessor(
-            tokenizer=self.tokenizer,
-            # Simplify out testing by masking every available token.
-            mask_selection_rate=1.0,
-            mask_token_rate=1.0,
-            random_token_rate=0.0,
-            mask_selection_length=5,
-            sequence_length=12,
+        self.vocab = {
+            "!": 0,
+            "air": 1,
+            "Ġair": 2,
+            "plane": 3,
+            "Ġat": 4,
+            "port": 5,
+            "<|endoftext|>": 6,
+        }
+
+        self.merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
+        self.merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
+        self.merges += ["Ġai r", "Ġa i", "pla ne"]
+
+        self.preprocessor = GPT2CausalLMPreprocessor(
+            tokenizer=GPT2Tokenizer(
+                vocabulary=self.vocab,
+                merges=self.merges,
+            ),
+            sequence_length=8,
         )
 
-    def test_preprocess_strings(self):
-        input_data = " brown fox quick"
+    def test_strings(self):
+        input_data = "airplane at airport"
 
         x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(
-            x["token_ids"], [0, 13, 13, 13, 2, 1, 1, 1, 1, 1, 1, 1]
-        )
-        self.assertAllEqual(
-            x["padding_mask"], [1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]
-        )
-        self.assertAllEqual(x["mask_positions"], [1, 2, 3, 0, 0])
-        self.assertAllEqual(y, [7, 9, 11, 0, 0])
-        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 0.0, 0.0])
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
+        self.assertAllEqual(y, [1, 3, 4, 2, 5, 6, 0, 0])
+        self.assertAllEqual(sw, [1, 1, 1, 1, 1, 1, 0, 0])
 
-    def test_preprocess_list_of_strings(self):
-        input_data = [" brown fox quick"] * 13
+    def test_list_of_strings(self):
+        input_data = ["airplane at airport"] * 4
 
         x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(
-            x["token_ids"], [[0, 13, 13, 13, 2, 1, 1, 1, 1, 1, 1, 1]] * 13
-        )
-        self.assertAllEqual(
-            x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]] * 13
-        )
-        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 0, 0]] * 13)
-        self.assertAllEqual(y, [[7, 9, 11, 0, 0]] * 13)
-        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 0.0, 0.0]] * 13)
-
-    def test_preprocess_dataset(self):
-        sentences = tf.constant([" brown fox quick"] * 13)
-        ds = tf.data.Dataset.from_tensor_slices(sentences)
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
+        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
+
+    def test_no_start_end_token(self):
+        input_data = ["airplane at airport"] * 4
+
+        preprocessor = GPT2CausalLMPreprocessor(
+            tokenizer=GPT2Tokenizer(
+                vocabulary=self.vocab,
+                merges=self.merges,
+            ),
+            sequence_length=8,
+            add_start_token=False,
+            add_end_token=False,
+        )
+        x, y, sw = preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 2, 5, 0, 0, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
+        self.assertAllEqual(y, [[3, 4, 2, 5, 0, 0, 0, 0]] * 4)
+        self.assertAllEqual(sw, [[1, 1, 1, 1, 0, 0, 0, 0]] * 4)
+
+    def test_labeled_batch(self):
+        x = tf.constant(["airplane at airport"] * 4)
+        y = tf.constant([1] * 4)  # Ignored.
+        sw = tf.constant([1.0] * 4)  # Ignored.
+        x, y, sw = self.preprocessor(x, y, sw)
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
+        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
+
+    def test_dataset(self):
+        x = tf.constant(["airplane at airport"] * 4)
+        ds = tf.data.Dataset.from_tensor_slices(x)
         ds = ds.map(self.preprocessor)
-        x, y, sw = ds.batch(13).take(1).get_single_element()
-        self.assertAllEqual(
-            x["token_ids"], [[0, 13, 13, 13, 2, 1, 1, 1, 1, 1, 1, 1]] * 13
-        )
-        self.assertAllEqual(
-            x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]] * 13
-        )
-        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 0, 0]] * 13)
-        self.assertAllEqual(y, [[7, 9, 11, 0, 0]] * 13)
-        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 0.0, 0.0]] * 13)
-
-    def test_mask_multiple_sentences(self):
-        sentence_one = tf.constant(" airplane")
-        sentence_two = tf.constant(" round")
-
-        x, y, sw = self.preprocessor((sentence_one, sentence_two))
-        self.assertAllEqual(
-            x["token_ids"], [0, 2, 2, 2, 13, 2, 1, 1, 1, 1, 1, 1]
-        )
-        self.assertAllEqual(
-            x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
-        )
-        self.assertAllEqual(x["mask_positions"], [4, 0, 0, 0, 0])
-        self.assertAllEqual(y, [12, 0, 0, 0, 0])
-        self.assertAllEqual(sw, [1.0, 0.0, 0.0, 0.0, 0.0])
-
-    def test_no_masking_zero_rate(self):
-        no_mask_preprocessor = XLMRobertaMaskedLMPreprocessor(
-            self.preprocessor.tokenizer,
-            mask_selection_rate=0.0,
-            mask_selection_length=5,
-            sequence_length=12,
-        )
-        input_data = " quick brown fox"
-
-        x, y, sw = no_mask_preprocessor(input_data)
-        self.assertAllEqual(
-            x["token_ids"], [0, 11, 7, 9, 2, 1, 1, 1, 1, 1, 1, 1]
-        )
-        self.assertAllEqual(
-            x["padding_mask"], [1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0]
-        )
-        self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0, 0])
-        self.assertAllEqual(y, [0, 0, 0, 0, 0])
-        self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0, 0.0])
+        x, y, sw = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
+        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
+
+    def test_generate_preprocess(self):
+        input_data = "airplane at airport"
+        x = self.preprocessor.generate_preprocess(input_data)
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 0, 0])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0])
+
+    def test_generate_postprocess(self):
+        input_data = {
+            "token_ids": tf.constant([6, 1, 3, 4, 2, 5, 0, 0]),
+            "padding_mask": tf.cast([1, 1, 1, 1, 1, 1, 0, 0], dtype="bool"),
+        }
+        x = self.preprocessor.generate_postprocess(input_data)
+        self.assertAllEqual(x, "airplane at airport")
 
     def test_serialization(self):
         config = keras.utils.serialize_keras_object(self.preprocessor)
         new_preprocessor = keras.utils.deserialize_keras_object(config)
         self.assertEqual(
             new_preprocessor.get_config(),
             self.preprocessor.get_config(),
@@ -155,20 +131,24 @@
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        input_data = tf.constant([" quick brown fox"])
+        input_data = tf.constant(["airplane at airport"])
 
         inputs = keras.Input(dtype="string", shape=())
-        outputs = self.preprocessor(inputs)
+        outputs, y, sw = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
-        outputs = model(input_data)[0]["token_ids"]
-        restored_outputs = restored_model(input_data)[0]["token_ids"]
-        self.assertAllEqual(outputs, restored_outputs)
+        self.assertAllEqual(
+            model(input_data)["token_ids"],
+            restored_model(input_data)["token_ids"],
+        )
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
-from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm import (
     XLMRobertaMaskedLM,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
     XLMRobertaMaskedLMPreprocessor,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
 
 
 class XLMRobertaMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
@@ -128,7 +128,8 @@
         # Check we got the real object back.
         self.assertIsInstance(restored_model, XLMRobertaMaskedLM)
 
         model_output = self.masked_lm(self.preprocessed_batch)
         restored_output = restored_model(self.preprocessed_batch)
 
         self.assertAllClose(model_output, restored_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """XLM-RoBERTa preprocessor layer."""
 
 import copy
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.models.roberta.roberta_preprocessor import (
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.preprocessor import Preprocessor
+from keras_nlp.src.models.roberta.roberta_preprocessor import (
     RobertaMultiSegmentPacker,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
-from keras_nlp.utils.keras_utils import (
+from keras_nlp.src.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.python_utils import classproperty
 
 
 @keras_nlp_export("keras_nlp.models.XLMRobertaPreprocessor")
 class XLMRobertaPreprocessor(Preprocessor):
     """An XLM-RoBERTa preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
@@ -190,7 +190,8 @@
     @classproperty
     def tokenizer_cls(cls):
         return XLMRobertaTokenizer
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
     XLMRobertaPreprocessor,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
 
 
 class XLMRobertaPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
@@ -156,7 +156,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,7 +63,8 @@
         "preprocessor_config": {},
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/xlm_roberta_large_multi/v1/model.h5",
         "weights_hash": "276211827174b71751f2ce3a89da503a",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/xlm_roberta_large_multi/v1/vocab.spm",
         "spm_proto_hash": "bf25eb5120ad92ef5c7d8596b5dc4046",
     },
 }
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # limitations under the License.
 """Tests for loading pretrained model presets."""
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
-from keras_nlp.models.xlm_roberta.xlm_roberta_classifier import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_classifier import (
     XLMRobertaClassifier,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_preprocessor import (
     XLMRobertaPreprocessor,
 )
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
 
 
 @pytest.mark.large
 class XLMRobertaPresetSmokeTest(tf.test.TestCase, parameterized.TestCase):
     """
@@ -190,7 +190,8 @@
             tokenizer = XLMRobertaTokenizer.from_preset(preset)
             tokenizer("The quick brown fox.")
 
     def test_load_preprocessors(self):
         for preset in XLMRobertaPreprocessor.presets:
             preprocessor = XLMRobertaPreprocessor.from_preset(preset)
             preprocessor("The quick brown fox.")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 """XLM-RoBERTa tokenizer."""
 
 import copy
 
 import tensorflow as tf
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.tf_utils import tensor_to_string_list
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.models.xlm_roberta.xlm_roberta_presets import backbone_presets
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.tf_utils import tensor_to_string_list
 
 
 @keras_nlp_export("keras_nlp.models.XLMRobertaTokenizer")
 class XLMRobertaTokenizer(SentencePieceTokenizer):
     """An XLM-RoBERTa tokenizer using SentencePiece subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
@@ -155,7 +155,8 @@
     def detokenize(self, ids):
         ids = tf.ragged.boolean_mask(ids, tf.not_equal(ids, self.mask_token_id))
         return super().detokenize(ids)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from tensorflow import keras
 
-from keras_nlp.samplers.beam_sampler import BeamSampler
-from keras_nlp.samplers.contrastive_sampler import ContrastiveSampler
-from keras_nlp.samplers.greedy_sampler import GreedySampler
-from keras_nlp.samplers.random_sampler import RandomSampler
-from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.serialization import deserialize
-from keras_nlp.samplers.serialization import get
-from keras_nlp.samplers.serialization import serialize
-from keras_nlp.samplers.top_k_sampler import TopKSampler
-from keras_nlp.samplers.top_p_sampler import TopPSampler
+from keras_nlp.src.samplers.beam_sampler import BeamSampler
+from keras_nlp.src.samplers.contrastive_sampler import ContrastiveSampler
+from keras_nlp.src.samplers.greedy_sampler import GreedySampler
+from keras_nlp.src.samplers.random_sampler import RandomSampler
+from keras_nlp.src.samplers.sampler import Sampler
+from keras_nlp.src.samplers.serialization import deserialize
+from keras_nlp.src.samplers.serialization import get
+from keras_nlp.src.samplers.serialization import serialize
+from keras_nlp.src.samplers.top_k_sampler import TopKSampler
+from keras_nlp.src.samplers.top_p_sampler import TopPSampler
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/beam_sampler.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/beam_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 """Beam Sampler."""
 
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import call_args_docstring
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.samplers.sampler import Sampler
+from keras_nlp.src.samplers.sampler import call_args_docstring
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @format_docstring(call_args=call_args_docstring)
 @keras_nlp_export("keras_nlp.samplers.BeamSampler")
 class BeamSampler(Sampler):
     """Beam Sampler class.
 
@@ -229,7 +229,8 @@
         config.update(
             {
                 "num_beams": self.num_beams,
                 "return_all_beams": self.return_all_beams,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/beam_sampler_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/beam_sampler_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for Beam sampler."""
 
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.samplers.beam_sampler import BeamSampler
+from keras_nlp.src.samplers.beam_sampler import BeamSampler
 
 
 class BeamSamplerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         super().setUp()
         # Use a simple alphabet of lowercase characters to [0, 26).
         self.int_lookup = {i: chr(i + ord("a")) for i in range(26)}
@@ -121,7 +121,8 @@
 
         @tf.function(jit_compile=jit_compile)
         def generate(prompt, cache):
             return self.sampler(self.next, prompt=prompt, cache=cache)
 
         output = generate(prompt, cache)
         self.assertEqual(self.join_as_string(output), ["sequentially"])
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/contrastive_sampler.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/contrastive_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 """Contrastive Sampler."""
 
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import call_args_docstring
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.samplers.sampler import Sampler
+from keras_nlp.src.samplers.sampler import call_args_docstring
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @format_docstring(call_args=call_args_docstring)
 @keras_nlp_export("keras_nlp.samplers.ContrastiveSampler")
 class ContrastiveSampler(Sampler):
     """Contrastive Sampler class.
 
@@ -238,7 +238,8 @@
             {
                 "k": self.k,
                 "alpha": self.alpha,
                 "seed": self.seed,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/contrastive_sampler_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/contrastive_sampler_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for Contrastive Sampler."""
 
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.samplers.contrastive_sampler import ContrastiveSampler
+from keras_nlp.src.samplers.contrastive_sampler import ContrastiveSampler
 
 
 class ContrastiveSamplerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         super().setUp()
         # Use a simple alphabet of lowercase characters to [0, 26).
         self.int_lookup = {i: chr(i + ord("a")) for i in range(26)}
@@ -181,7 +181,8 @@
                 cache=cache,
                 index=1,
                 hidden_states=self.hidden_states,
             )
 
         output = generate(prompt, cache)
         self.assertEqual(self.join_as_string(output), ["sequentially"])
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/greedy_sampler.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/greedy_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Greedy Sampler."""
 
 import tensorflow as tf
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import call_args_docstring
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.samplers.sampler import Sampler
+from keras_nlp.src.samplers.sampler import call_args_docstring
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @format_docstring(call_args=call_args_docstring)
 @keras_nlp_export("keras_nlp.samplers.GreedySampler")
 class GreedySampler(Sampler):
     """Greedy sampler class.
 
@@ -59,7 +59,8 @@
         self,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
     def get_next_token(self, probabilities):
         return tf.argmax(probabilities, axis=-1)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/greedy_sampler_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/greedy_sampler_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for Greedy sampler."""
 
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.samplers.greedy_sampler import GreedySampler
+from keras_nlp.src.samplers.greedy_sampler import GreedySampler
 
 
 class GreedySamplerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         super().setUp()
         # Use a simple alphabet of lowercase characters to [0, 26).
         self.int_lookup = {i: chr(i + ord("a")) for i in range(26)}
@@ -114,7 +114,8 @@
 
         @tf.function(jit_compile=jit_compile)
         def generate(prompt, cache):
             return self.sampler(self.next, prompt=prompt, cache=cache)
 
         output = generate(prompt, cache)
         self.assertEqual(self.join_as_string(output), ["sequentially"])
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/random_sampler.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/random_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Random Sampler."""
 
 import tensorflow as tf
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import call_args_docstring
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.samplers.sampler import Sampler
+from keras_nlp.src.samplers.sampler import call_args_docstring
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @format_docstring(call_args=call_args_docstring)
 @keras_nlp_export("keras_nlp.samplers.RandomSampler")
 class RandomSampler(Sampler):
     """Random Sampler class.
 
@@ -78,7 +78,8 @@
         config = super().get_config()
         config.update(
             {
                 "seed": self.seed,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/random_sampler_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/random_sampler_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Tests for Random sampler."""
 
 import numpy as np
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.samplers.random_sampler import RandomSampler
+from keras_nlp.src.samplers.random_sampler import RandomSampler
 
 
 class RandomSamplerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         super().setUp()
         # Use a simple alphabet of lowercase characters to [0, 25].
         self.int_lookup = {i: chr(i + ord("a")) for i in range(26)}
@@ -109,7 +109,8 @@
 
         @tf.function(jit_compile=jit_compile)
         def generate(prompt, cache):
             return self.sampler(self.next, prompt=prompt, cache=cache)
 
         output = generate(prompt, cache)
         self.assertEqual(self.join_as_string(output), ["sequentially"])
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/sampler.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,37 +13,39 @@
 # limitations under the License.
 """Base sampler class."""
 
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.utils.python_utils import format_docstring
 
 call_args_docstring = """next: A function which takes in the
             `prompt, cache, index` of the current generation loop, and outputs
             a tuple `(logits, cache, hidden_states)` with `logits` being the
             logits of next token, `cache` for next iteration, and
             `hidden_states` being the representation of the token.
         prompt: A 2D integer tensor with shape `(batch_size, max_length)`. This
             tensor will be iteratively updated column by column with new sampled
             values, starting at `index`.
         cache: Optional. A tensor or nested structure of tensors that will be
             updated by each call to `next`. This can be used to cache
             computations from early iterations of the generative loop.
-        index: Optional. The first index to start sampling at.
+        index: Optional. The first index of `prompt` to start sampling at.
+            Usually this is set as the length of the shortest non-padding
+            sequence in `prompt`.
         mask: Optional. A 2D integer tensor with the same shape as `prompt`.
             Locations which are `True` in the mask are never updated during
-            sampling. Often this will mark all ids in `prompt` which were
-            present in the original input.
+            sampling. Usually used to mark all locations in the dense prompt
+            tensor which were present in a user input.
         end_token_id: Optional. The token marking the end of the sequence. If
             specified, sampling will stop as soon as all sequences in the prompt
             produce a `end_token_id` in a location where `mask` is `False`.
-    """
+"""
 
 
 @format_docstring(call_args=call_args_docstring)
 @keras_nlp_export("keras_nlp.samplers.Sampler")
 class Sampler:
     """Base sampler class.
 
@@ -56,16 +58,16 @@
         {{call_args}}
 
     This base class can be extended to implement different auto-regressive
     sampling methods. Subclasses can either:
 
     - Override the `get_next_token()` method, which computes the next token
       based on a probability distribution over all possible vocab entries.
-    - Override `__call__`, if the sampling method need additional cache beyond
-      the next tokens probability distribution to sample a sequence.
+    - Override `__call__`, if the sampling method needs additional information
+      beyond the next tokens probability distribution to sample a sequence.
 
     Please check available subclass samplers for examples.
 
     Examples:
 
     ```python
     # Use a simple alphabet of lowercase characters with ids in range [0, 25].
@@ -160,7 +162,8 @@
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
 
     def get_config(self):
         return {"temperature": self.temperature}
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/serialization.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/serialization.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.samplers.beam_sampler import BeamSampler
-from keras_nlp.samplers.contrastive_sampler import ContrastiveSampler
-from keras_nlp.samplers.greedy_sampler import GreedySampler
-from keras_nlp.samplers.random_sampler import RandomSampler
-from keras_nlp.samplers.top_k_sampler import TopKSampler
-from keras_nlp.samplers.top_p_sampler import TopPSampler
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.samplers.beam_sampler import BeamSampler
+from keras_nlp.src.samplers.contrastive_sampler import ContrastiveSampler
+from keras_nlp.src.samplers.greedy_sampler import GreedySampler
+from keras_nlp.src.samplers.random_sampler import RandomSampler
+from keras_nlp.src.samplers.top_k_sampler import TopKSampler
+from keras_nlp.src.samplers.top_p_sampler import TopPSampler
 
 
 @keras_nlp_export("keras_nlp.samplers.serialize")
 def serialize(sampler):
     return keras.utils.serialize_keras_object(sampler)
 
 
@@ -91,7 +91,8 @@
         return deserialize(identifier)
     elif callable(identifier):
         return identifier
     else:
         raise ValueError(
             "Could not interpret sampler identifier: " + str(identifier)
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/serialization_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/serialization_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for Sampler classes."""
 
 import tensorflow as tf
 
-from keras_nlp.samplers.serialization import deserialize
-from keras_nlp.samplers.serialization import get
-from keras_nlp.samplers.serialization import serialize
-from keras_nlp.samplers.top_k_sampler import TopKSampler
+from keras_nlp.src.samplers.serialization import deserialize
+from keras_nlp.src.samplers.serialization import get
+from keras_nlp.src.samplers.serialization import serialize
+from keras_nlp.src.samplers.top_k_sampler import TopKSampler
 
 
 class SerializationTest(tf.test.TestCase):
     def test_serialization(self):
         sampler = TopKSampler(k=5)
         restored = deserialize(serialize(sampler))
         self.assertDictEqual(sampler.get_config(), restored.get_config())
@@ -42,7 +42,8 @@
             serialize(original_sampler),
         )
 
         # Test identifier is already a sampler instance.
         original_sampler = TopKSampler(k=7)
         restored_sampler = get(original_sampler)
         self.assertEqual(original_sampler, restored_sampler)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_k_sampler.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_k_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Top-k Sampler."""
 
 import tensorflow as tf
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import call_args_docstring
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.samplers.sampler import Sampler
+from keras_nlp.src.samplers.sampler import call_args_docstring
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @format_docstring(call_args=call_args_docstring)
 @keras_nlp_export("keras_nlp.samplers.TopKSampler")
 class TopKSampler(Sampler):
     """Top-K Sampler class.
 
@@ -88,7 +88,8 @@
         config.update(
             {
                 "k": self.k,
                 "seed": self.seed,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_k_sampler_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_k_sampler_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for Top-K sampler."""
 
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.samplers.top_k_sampler import TopKSampler
+from keras_nlp.src.samplers.top_k_sampler import TopKSampler
 
 
 class TopKSamplerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         super().setUp()
         # Use a simple alphabet of lowercase characters to [0, 26).
         self.int_lookup = {i: chr(i + ord("a")) for i in range(26)}
@@ -114,7 +114,8 @@
 
         @tf.function(jit_compile=jit_compile)
         def generate(prompt, cache):
             return self.sampler(self.next, prompt=prompt, cache=cache)
 
         output = generate(prompt, cache)
         self.assertEqual(self.join_as_string(output), ["sequentially"])
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_p_sampler.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_p_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Top-p Sampler."""
 
 import tensorflow as tf
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import call_args_docstring
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.samplers.sampler import Sampler
+from keras_nlp.src.samplers.sampler import call_args_docstring
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 @format_docstring(call_args=call_args_docstring)
 @keras_nlp_export("keras_nlp.samplers.TopPSampler")
 class TopPSampler(Sampler):
     """Top-P Sampler class.
 
@@ -113,7 +113,8 @@
             {
                 "p": self.p,
                 "k": self.k,
                 "seed": self.seed,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_p_sampler_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/samplers/top_p_sampler_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Tests for Top-P sampler."""
 
 import numpy as np
 import tensorflow as tf
 from absl.testing import parameterized
 
-from keras_nlp.samplers.top_p_sampler import TopPSampler
+from keras_nlp.src.samplers.top_p_sampler import TopPSampler
 
 
 class TopPSamplerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         super().setUp()
         # Use a simple alphabet of lowercase characters to [0, 26).
         self.int_lookup = {i: chr(i + ord("a")) for i in range(26)}
@@ -148,7 +148,8 @@
 
         @tf.function(jit_compile=jit_compile)
         def generate(prompt, cache):
             return self.sampler(self.next, prompt=prompt, cache=cache)
 
         output = generate(prompt, cache)
         self.assertEqual(self.join_as_string(output), ["sequentially"])
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/docstring_lib.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/docstring_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,7 +215,8 @@
                     "\n\nCAUTION: tf_doctest doesn't work if *some* of the "
                     '*float output* is hidden with a "...".'
                 )
 
         got.append(self.MESSAGE)
         got = "\n".join(got)
         return super().output_difference(example, got, optionflags)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/docstring_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/docstring_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 import numpy as np
 import pytest
 import sentencepiece
 import tensorflow as tf
 from tensorflow import keras
 
-import keras_nlp
-from keras_nlp.tests.doc_tests import docstring_lib
-from keras_nlp.tests.doc_tests import fenced_docstring_lib
-from keras_nlp.tests.doc_tests.fenced_docstring_lib import (
+import keras_nlp.src as keras_nlp
+from keras_nlp.src.tests.doc_tests import docstring_lib
+from keras_nlp.src.tests.doc_tests import fenced_docstring_lib
+from keras_nlp.src.tests.doc_tests.fenced_docstring_lib import (
     astor,  # For checking conditional import.
 )
 
 PACKAGE = "keras_nlp."
 
 
 def find_modules():
@@ -124,7 +124,8 @@
                 ),
             )
         )
     result = runner.run(suite)
     if not result.wasSuccessful():
         print(result)
     assert result.wasSuccessful()
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/fenced_docstring_lib.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,7 +198,8 @@
         source,
         filename="dummy.py",
         mode="exec",
         flags=flags,
         dont_inherit=dont_inherit,
         optimize=optimize,
     )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/__init__.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from keras_nlp.tokenizers.byte_pair_tokenizer import BytePairTokenizer
-from keras_nlp.tokenizers.byte_tokenizer import ByteTokenizer
-from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.tokenizers.sentence_piece_tokenizer_trainer import (
+from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
+from keras_nlp.src.tokenizers.byte_tokenizer import ByteTokenizer
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer_trainer import (
     compute_sentence_piece_proto,
 )
-from keras_nlp.tokenizers.tokenizer import Tokenizer
-from keras_nlp.tokenizers.unicode_codepoint_tokenizer import (
+from keras_nlp.src.tokenizers.tokenizer import Tokenizer
+from keras_nlp.src.tokenizers.unicode_codepoint_tokenizer import (
     UnicodeCodepointTokenizer,
 )
-from keras_nlp.tokenizers.word_piece_tokenizer import WordPieceTokenizer
-from keras_nlp.tokenizers.word_piece_tokenizer_trainer import (
+from keras_nlp.src.tokenizers.word_piece_tokenizer import WordPieceTokenizer
+from keras_nlp.src.tokenizers.word_piece_tokenizer_trainer import (
     compute_word_piece_vocabulary,
 )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_pair_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_pair_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 from typing import Iterable
 from typing import List
 
 import regex as re
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.tokenizers import tokenizer
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.python_utils import format_docstring
-from keras_nlp.utils.tf_utils import assert_tf_text_installed
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.tokenizers import tokenizer
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.python_utils import format_docstring
+from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 # As python and TF handles special spaces differently, we need to
@@ -674,7 +674,8 @@
                 BytePairTokenizer.from_preset.__doc__
             )
             format_docstring(
                 model_name=cls.__name__,
                 example_preset_name=next(iter(cls.presets), ""),
                 preset_names='", "'.join(cls.presets),
             )(cls.from_preset.__func__)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_pair_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.tokenizers.byte_pair_tokenizer import BytePairTokenizer
+from keras_nlp.src.tokenizers.byte_pair_tokenizer import BytePairTokenizer
 
 VOCAB_PATH = keras.utils.get_file(
     None,
     "https://storage.googleapis.com/keras-nlp/models/roberta_base/vocab.json",
 )
 MERGE_PATH = keras.utils.get_file(
     None,
@@ -186,7 +186,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 
 """Byte Tokenizer."""
 
 import numpy as np
 import tensorflow as tf
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.tokenizers import tokenizer
-from keras_nlp.utils.tf_utils import assert_tf_text_installed
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.tokenizers import tokenizer
+from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
@@ -266,7 +266,8 @@
                 "sequence_length": self.sequence_length,
                 "normalization_form": self.normalization_form,
                 "errors": self.errors,
                 "replacement_char": self.replacement_char,
             }
         )
         return config
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/byte_tokenizer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.tokenizers.byte_tokenizer import ByteTokenizer
+from keras_nlp.src.tokenizers.byte_tokenizer import ByteTokenizer
 
 
 class ByteTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def test_tokenize(self):
         input_data = tf.constant(["hello", "fun", "▀▁▂▃"])
         tokenizer = ByteTokenizer()
         call_output = tokenizer(input_data)
@@ -265,7 +265,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 import binascii
 import os
 from typing import List
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.tokenizers import tokenizer
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.python_utils import format_docstring
-from keras_nlp.utils.tf_utils import assert_tf_text_installed
-from keras_nlp.utils.tf_utils import tensor_to_string_list
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.tokenizers import tokenizer
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.python_utils import format_docstring
+from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
+from keras_nlp.src.utils.tf_utils import tensor_to_string_list
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
@@ -288,7 +288,8 @@
                 SentencePieceTokenizer.from_preset.__doc__
             )
             format_docstring(
                 model_name=cls.__name__,
                 example_preset_name=next(iter(cls.presets), ""),
                 preset_names='", "'.join(cls.presets),
             )(cls.from_preset.__func__)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
 
 
 class SentencePieceTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         super().setUp()
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
@@ -205,7 +205,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,7 +134,8 @@
             bos_id=2,
             eos_id=3,
         )
     if proto_output_file:
         model_writer.close()
     else:
         return model_writer.getvalue()
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """Tests for SentencePiece Tokenizer Trainer."""
 
 import os
 import re
 
 import tensorflow as tf
 
-from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
-from keras_nlp.tokenizers.sentence_piece_tokenizer_trainer import (
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.src.tokenizers.sentence_piece_tokenizer_trainer import (
     compute_sentence_piece_proto,
 )
 
 
 class SentencePieceTokenizerTrainerTest(tf.test.TestCase):
     def test_dataset_input(self):
         test_text = ["Ninjas and Samurais"]
@@ -92,7 +92,8 @@
         )
         tokenizer = SentencePieceTokenizer(
             proto=os.path.join(self.get_temp_dir(), "model.spm")
         )
         output = inputs.map(tokenizer).take(1).get_single_element()
         expected_output = [4, 8, 12, 5, 9, 14, 5, 6, 13, 4, 7, 10, 11, 6, 13]
         self.assertAllEqual(expected_output, output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.src.api_export import keras_nlp_export
 
 
 @keras_nlp_export("keras_nlp.tokenizers.Tokenizer")
 class Tokenizer(keras.layers.Layer):
     """A base class for tokenizer layers.
 
     Tokenizers in the KerasNLP library should all subclass this layer.
@@ -138,7 +138,8 @@
             return self._tokenize_without_call(*args, **kwargs)
         elif mode == "detokenize":
             return self._detokenize_without_call(*args, **kwargs)
         else:
             raise ValueError(
                 f"Unsupported tokenizer mode. Received: mode={mode}"
             )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/tokenizer_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.tokenizers.tokenizer import Tokenizer
+from keras_nlp.src.tokenizers.tokenizer import Tokenizer
 
 
 class SimpleTokenizer(Tokenizer):
     __test__ = False  # for pytest
 
     def tokenize(self, inputs):
         return tf.strings.split(inputs).to_tensor()
@@ -53,7 +53,8 @@
         # There appears to be a bug with shape inference for ragged reduce_join.
         # The second dimension should be removed.
         self.assertAllEqual(model_output, [["the quick brown fox"]])
 
     def test_missing_tokenize_raises(self):
         with self.assertRaises(NotImplementedError):
             Tokenizer()(["the quick brown fox"])
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.tokenizers import tokenizer
-from keras_nlp.utils.tf_utils import assert_tf_text_installed
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.tokenizers import tokenizer
+from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
@@ -323,7 +323,8 @@
         encoded_string = tf.strings.unicode_encode(
             inputs,
             errors=self.errors,
             replacement_char=self.replacement_char,
             output_encoding=self.output_encoding,
         )
         return encoded_string
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.tokenizers.unicode_codepoint_tokenizer import (
+from keras_nlp.src.tokenizers.unicode_codepoint_tokenizer import (
     UnicodeCodepointTokenizer,
 )
 
 
 class UnicodeCodepointTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def test_tokenize(self):
         input_data = tf.constant(["ninja", "samurai", "▀▁▂▃"])
@@ -367,7 +367,8 @@
         kwargs = {"save_traces": False} if save_format == "tf" else {}
         model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 import os
 from typing import Iterable
 from typing import List
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.api_export import keras_nlp_export
-from keras_nlp.tokenizers import tokenizer
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.python_utils import format_docstring
-from keras_nlp.utils.tf_utils import assert_tf_text_installed
+from keras_nlp.src.api_export import keras_nlp_export
+from keras_nlp.src.tokenizers import tokenizer
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.python_utils import format_docstring
+from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 # Matches whitespace and control characters.
@@ -496,7 +496,8 @@
                 WordPieceTokenizer.from_preset.__doc__
             )
             format_docstring(
                 model_name=cls.__name__,
                 example_preset_name=next(iter(cls.presets), ""),
                 preset_names='", "'.join(cls.presets),
             )(cls.from_preset.__func__)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.tokenizers.word_piece_tokenizer import WordPieceTokenizer
+from keras_nlp.src.tokenizers.word_piece_tokenizer import WordPieceTokenizer
 
 
 class WordPieceTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def test_tokenize(self):
         input_data = ["the quick brown fox."]
         vocab_data = ["[UNK]", "the", "qu", "##ick", "br", "##own", "fox", "."]
         tokenizer = WordPieceTokenizer(vocabulary=vocab_data)
@@ -243,7 +243,8 @@
         with self.assertRaises(ValueError):
             WordPieceTokenizer(
                 vocabulary=vocab_data,
             )
 
         with self.assertRaises(ValueError):
             WordPieceTokenizer(vocabulary=vocab_data, oov_token=None)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Trainer for WordPiece Tokenizer."""
 
 import tensorflow as tf
 
-from keras_nlp.tokenizers.word_piece_tokenizer import pretokenize
-from keras_nlp.utils.tf_utils import assert_tf_text_installed
+from keras_nlp.src.tokenizers.word_piece_tokenizer import pretokenize
+from keras_nlp.src.utils.tf_utils import assert_tf_text_installed
 
 try:
     from tensorflow_text.tools.wordpiece_vocab import (
         wordpiece_tokenizer_learner_lib as learner,
     )
 except ImportError:
     learner = None
@@ -170,7 +170,8 @@
     if vocabulary_output_file is not None:
         vocab_text = "".join([line + "\n" for line in vocab])
         # Write vocab to file.
         with open(vocabulary_output_file, "w") as vocab_file:
             vocab_file.write(vocab_text)
     else:
         return vocab
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Tests for WordPiece Tokenizer Trainer."""
 
 import os
 
 import tensorflow as tf
 
-from keras_nlp.tokenizers.word_piece_tokenizer_trainer import (
+from keras_nlp.src.tokenizers.word_piece_tokenizer_trainer import (
     compute_word_piece_vocabulary,
 )
 
 
 class WordPieceTokenizerTrainerTest(tf.test.TestCase):
     def test_dataset_input(self):
         test_text = ["baa maa caa saa aaa"]
@@ -198,7 +198,8 @@
     def test_suffix_indicator(self):
         test_text = tf.data.Dataset.from_tensor_slices(["baa maa caa saa aaa"])
         test_output = ["a", "b", "c", "m", "s", "@@aa", "@@a", "@@b"]
         vocab = compute_word_piece_vocabulary(
             test_text, 8, suffix_indicator="@@", reserved_tokens=[]
         )
         self.assertAllEqual(vocab, test_output)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/utils/keras_utils.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/keras_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import platform
 import sys
 
 import tensorflow as tf
 from absl import logging
 from tensorflow import keras
 
-from keras_nlp.utils.tf_utils import is_tensor_type
+from keras_nlp.src.utils.tf_utils import is_tensor_type
 
 
 def clone_initializer(initializer):
     """Clones an initializer to ensure a new seed.
 
     As of tensorflow 2.10, we need to clone user passed initializers when
     invoking them twice to avoid creating the same randomized initialization.
@@ -166,7 +166,8 @@
             # Pad out to the next position
             if nested_level:
                 line += " " * (positions[col] - len(line) - nested_level)
             else:
                 line += " " * (positions[col] - len(line))
         line += "|" * nested_level
         print_fn(line)
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/utils/keras_utils_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/keras_utils_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.utils.keras_utils import clone_initializer
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.keras_utils import clone_initializer
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
 
 
 class CloneInitializerTest(tf.test.TestCase):
     def test_config_equality(self):
         initializer = keras.initializers.VarianceScaling(
             scale=2.0,
             mode="fan_out",
@@ -61,7 +61,8 @@
 
     def test_pack_triplet(self):
         x = tf.constant([1, 2])
         y = tf.constant([3, 4])
         sw = tf.constant([5, 6])
         data = pack_x_y_sample_weight(x, y, sw)
         self.assertAllEqual(data, (x, y, sw))
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/utils/pipeline_model.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/pipeline_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 import functools
 import math
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.tf_utils import is_tensor_type
+from keras_nlp.src.utils.keras_utils import pack_x_y_sample_weight
+from keras_nlp.src.utils.tf_utils import is_tensor_type
 
 
 def _convert_inputs_to_dataset(
     x=None,
     y=None,
     sample_weight=None,
     batch_size=None,
@@ -282,7 +282,8 @@
         if self.include_preprocessing:
             data = self.preprocess_samples(x)
             x, _, _ = tf.keras.utils.unpack_x_y_sample_weight(data)
         return super().predict_on_batch(
             x=x,
             **kwargs,
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/utils/pipeline_model_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/pipeline_model_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.utils.pipeline_model import PipelineModel
+from keras_nlp.src.utils.pipeline_model import PipelineModel
 
 
 class NoopPipeline(PipelineModel):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.dense = keras.layers.Dense(1)
 
@@ -583,7 +583,8 @@
             model.fit(x=tf.constant(["test"]), y=tf.constant(0))
         with self.assertRaisesRegex(ValueError, "must have a batch dimension"):
             model.fit(
                 x=tf.constant(["test"]), y=tf.constant([0]), sample_weight=0.0
             )
         with self.assertRaisesRegex(ValueError, "must have a batch dimension"):
             model.fit(x="test")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/utils/python_utils.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/python_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,7 +40,8 @@
         # to swap all double and single brackets in the source docstring.
         doc = "{".join(part.replace("{", "{{") for part in doc.split("{{"))
         doc = "}".join(part.replace("}", "}}") for part in doc.split("}}"))
         obj.__doc__ = doc.format(**replacements)
         return obj
 
     return decorate
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/utils/python_utils_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/python_utils_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
-from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.python_utils import format_docstring
+from keras_nlp.src.utils.python_utils import classproperty
+from keras_nlp.src.utils.python_utils import format_docstring
 
 
 class ClassPropertyTest(tf.test.TestCase):
     def test_class_property(self):
         class Foo:
             @classproperty
             def bar(cls):
@@ -79,7 +79,8 @@
             """Use `{}` to create a dictionary, {{nickname}}."""
             return "function"
 
         self.assertAllEqual(bar(), "function")
         self.assertAllEqual(
             bar.__doc__, "Use `{}` to create a dictionary, dumdum."
         )
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/utils/tf_utils.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/tf_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,7 +84,8 @@
 
 
 def is_tensor_type(x):
     if pd is None:
         return isinstance(x, (tf.Tensor, np.ndarray))
     else:
         return isinstance(x, (tf.Tensor, np.ndarray, pd.Series, pd.DataFrame))
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp/utils/tf_utils_test.py` & `keras-nlp-0.5.0.dev4/keras_nlp/src/utils/tf_utils_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
-from keras_nlp.utils.tf_utils import tensor_to_list
-from keras_nlp.utils.tf_utils import tensor_to_string_list
+from keras_nlp.src.utils.tf_utils import tensor_to_list
+from keras_nlp.src.utils.tf_utils import tensor_to_string_list
 
 
 class TensorToListTest(tf.test.TestCase):
     def test_ragged_input(self):
         input_data = tf.ragged.constant([[1, 2], [4, 5, 6]])
         list_output = tensor_to_list(input_data)
         self.assertAllEqual(list_output, [[1, 2], [4, 5, 6]])
@@ -46,7 +46,8 @@
         detokenize_output = tensor_to_string_list(input_data)
         self.assertAllEqual(detokenize_output, [["▀▁▂▃", "samurai"]])
 
     def test_detokenize_to_strings_for_scalar(self):
         input_data = tf.constant("▀▁▂▃")
         detokenize_output = tensor_to_string_list(input_data)
         self.assertEqual(detokenize_output, "▀▁▂▃")
+
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp.egg-info/PKG-INFO` & `keras-nlp-0.5.0.dev4/keras_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.5.0.dev0
+Version: 0.5.0.dev4
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,14 @@
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extras
-License-File: LICENSE
 
 # KerasNLP: Modular NLP Workflows for Keras
 [![](https://github.com/keras-team/keras-nlp/workflows/Tests/badge.svg?branch=master)](https://github.com/keras-team/keras-nlp/actions?query=workflow%3ATests+branch%3Amaster)
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.5.0+-success.svg)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/keras-team/keras-nlp/issues)
```

### Comparing `keras-nlp-0.5.0.dev0/keras_nlp.egg-info/SOURCES.txt` & `keras-nlp-0.5.0.dev4/keras_nlp.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,297 +1,269 @@
-LICENSE
 README.md
-pyproject.toml
 setup.cfg
 setup.py
-examples/__init__.py
-examples/bert_pretraining/__init__.py
-examples/bert_pretraining/bert_config.py
-examples/bert_pretraining/bert_create_pretraining_data.py
-examples/bert_pretraining/bert_pretrain.py
-examples/machine_translation/__init__.py
-examples/machine_translation/data.py
-examples/machine_translation/inference.py
-examples/machine_translation/model.py
-examples/machine_translation/train.py
-examples/tools/__init__.py
-examples/tools/split_sentences.py
-examples/tools/train_word_piece_vocab.py
-examples/utils/__init__.py
-examples/utils/data_utils.py
-examples/utils/scripting_utils.py
-integration_tests/__init__.py
-integration_tests/basic_usage_test.py
-integration_tests/import_test.py
 keras_nlp/__init__.py
-keras_nlp/api_export.py
-keras_nlp/conftest.py
 keras_nlp.egg-info/PKG-INFO
 keras_nlp.egg-info/SOURCES.txt
 keras_nlp.egg-info/dependency_links.txt
 keras_nlp.egg-info/requires.txt
 keras_nlp.egg-info/top_level.txt
 keras_nlp/layers/__init__.py
-keras_nlp/layers/cached_multi_head_attention.py
-keras_nlp/layers/cached_multi_head_attention_test.py
-keras_nlp/layers/f_net_encoder.py
-keras_nlp/layers/f_net_encoder_test.py
-keras_nlp/layers/masked_lm_head.py
-keras_nlp/layers/masked_lm_head_test.py
-keras_nlp/layers/masked_lm_mask_generator.py
-keras_nlp/layers/masked_lm_mask_generator_test.py
-keras_nlp/layers/multi_segment_packer.py
-keras_nlp/layers/multi_segment_packer_test.py
-keras_nlp/layers/position_embedding.py
-keras_nlp/layers/position_embedding_test.py
-keras_nlp/layers/random_deletion.py
-keras_nlp/layers/random_deletion_test.py
-keras_nlp/layers/random_swap.py
-keras_nlp/layers/random_swap_test.py
-keras_nlp/layers/sine_position_encoding.py
-keras_nlp/layers/sine_position_encoding_test.py
-keras_nlp/layers/start_end_packer.py
-keras_nlp/layers/start_end_packer_test.py
-keras_nlp/layers/token_and_position_embedding.py
-keras_nlp/layers/token_and_position_embedding_test.py
-keras_nlp/layers/transformer_decoder.py
-keras_nlp/layers/transformer_decoder_test.py
-keras_nlp/layers/transformer_encoder.py
-keras_nlp/layers/transformer_encoder_test.py
-keras_nlp/layers/transformer_layer_utils.py
-keras_nlp/layers/transformer_layer_utils_test.py
 keras_nlp/metrics/__init__.py
-keras_nlp/metrics/bleu.py
-keras_nlp/metrics/bleu_test.py
-keras_nlp/metrics/edit_distance.py
-keras_nlp/metrics/edit_distance_test.py
-keras_nlp/metrics/perplexity.py
-keras_nlp/metrics/perplexity_test.py
-keras_nlp/metrics/rouge_base.py
-keras_nlp/metrics/rouge_l.py
-keras_nlp/metrics/rouge_l_test.py
-keras_nlp/metrics/rouge_n.py
-keras_nlp/metrics/rouge_n_test.py
 keras_nlp/models/__init__.py
-keras_nlp/models/backbone.py
-keras_nlp/models/preprocessor.py
-keras_nlp/models/task.py
-keras_nlp/models/task_test.py
-keras_nlp/models/albert/__init__.py
-keras_nlp/models/albert/albert_backbone.py
-keras_nlp/models/albert/albert_backbone_test.py
-keras_nlp/models/albert/albert_classifier.py
-keras_nlp/models/albert/albert_classifier_test.py
-keras_nlp/models/albert/albert_masked_lm.py
-keras_nlp/models/albert/albert_masked_lm_preprocessor.py
-keras_nlp/models/albert/albert_masked_lm_preprocessor_test.py
-keras_nlp/models/albert/albert_masked_lm_test.py
-keras_nlp/models/albert/albert_preprocessor.py
-keras_nlp/models/albert/albert_preprocessor_test.py
-keras_nlp/models/albert/albert_presets.py
-keras_nlp/models/albert/albert_presets_test.py
-keras_nlp/models/albert/albert_tokenizer.py
-keras_nlp/models/albert/albert_tokenizer_test.py
-keras_nlp/models/bart/__init__.py
-keras_nlp/models/bart/bart_backbone.py
-keras_nlp/models/bart/bart_backbone_test.py
-keras_nlp/models/bart/bart_preprocessor.py
-keras_nlp/models/bart/bart_preprocessor_test.py
-keras_nlp/models/bart/bart_presets.py
-keras_nlp/models/bart/bart_presets_test.py
-keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor.py
-keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
-keras_nlp/models/bart/bart_tokenizer.py
-keras_nlp/models/bart/bart_tokenizer_test.py
-keras_nlp/models/bert/__init__.py
-keras_nlp/models/bert/bert_backbone.py
-keras_nlp/models/bert/bert_backbone_test.py
-keras_nlp/models/bert/bert_classifier.py
-keras_nlp/models/bert/bert_classifier_test.py
-keras_nlp/models/bert/bert_masked_lm.py
-keras_nlp/models/bert/bert_masked_lm_preprocessor.py
-keras_nlp/models/bert/bert_masked_lm_preprocessor_test.py
-keras_nlp/models/bert/bert_masked_lm_test.py
-keras_nlp/models/bert/bert_preprocessor.py
-keras_nlp/models/bert/bert_preprocessor_test.py
-keras_nlp/models/bert/bert_presets.py
-keras_nlp/models/bert/bert_presets_test.py
-keras_nlp/models/bert/bert_tokenizer.py
-keras_nlp/models/bert/bert_tokenizer_test.py
-keras_nlp/models/deberta_v3/__init__.py
-keras_nlp/models/deberta_v3/deberta_v3_backbone.py
-keras_nlp/models/deberta_v3/deberta_v3_backbone_test.py
-keras_nlp/models/deberta_v3/deberta_v3_classifier.py
-keras_nlp/models/deberta_v3/deberta_v3_classifier_test.py
-keras_nlp/models/deberta_v3/deberta_v3_masked_lm.py
-keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
-keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
-keras_nlp/models/deberta_v3/deberta_v3_masked_lm_test.py
-keras_nlp/models/deberta_v3/deberta_v3_preprocessor.py
-keras_nlp/models/deberta_v3/deberta_v3_preprocessor_test.py
-keras_nlp/models/deberta_v3/deberta_v3_presets.py
-keras_nlp/models/deberta_v3/deberta_v3_presets_test.py
-keras_nlp/models/deberta_v3/deberta_v3_tokenizer.py
-keras_nlp/models/deberta_v3/deberta_v3_tokenizer_test.py
-keras_nlp/models/deberta_v3/disentangled_attention_encoder.py
-keras_nlp/models/deberta_v3/disentangled_self_attention.py
-keras_nlp/models/deberta_v3/relative_embedding.py
-keras_nlp/models/distil_bert/__init__.py
-keras_nlp/models/distil_bert/distil_bert_backbone.py
-keras_nlp/models/distil_bert/distil_bert_backbone_test.py
-keras_nlp/models/distil_bert/distil_bert_classifier.py
-keras_nlp/models/distil_bert/distil_bert_classifier_test.py
-keras_nlp/models/distil_bert/distil_bert_masked_lm.py
-keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor.py
-keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
-keras_nlp/models/distil_bert/distil_bert_masked_lm_test.py
-keras_nlp/models/distil_bert/distil_bert_preprocessor.py
-keras_nlp/models/distil_bert/distil_bert_preprocessor_test.py
-keras_nlp/models/distil_bert/distil_bert_presets.py
-keras_nlp/models/distil_bert/distil_bert_presets_test.py
-keras_nlp/models/distil_bert/distil_bert_tokenizer.py
-keras_nlp/models/distil_bert/distil_bert_tokenizer_test.py
-keras_nlp/models/f_net/__init__.py
-keras_nlp/models/f_net/f_net_backbone.py
-keras_nlp/models/f_net/f_net_backbone_test.py
-keras_nlp/models/f_net/f_net_classifier.py
-keras_nlp/models/f_net/f_net_classifier_test.py
-keras_nlp/models/f_net/f_net_masked_lm.py
-keras_nlp/models/f_net/f_net_masked_lm_preprocessor.py
-keras_nlp/models/f_net/f_net_masked_lm_preprocessor_test.py
-keras_nlp/models/f_net/f_net_masked_lm_test.py
-keras_nlp/models/f_net/f_net_preprocessor.py
-keras_nlp/models/f_net/f_net_preprocessor_test.py
-keras_nlp/models/f_net/f_net_presets.py
-keras_nlp/models/f_net/f_net_presets_test.py
-keras_nlp/models/f_net/f_net_tokenizer.py
-keras_nlp/models/f_net/f_net_tokenizer_test.py
-keras_nlp/models/gpt2/__init__.py
-keras_nlp/models/gpt2/gpt2_backbone.py
-keras_nlp/models/gpt2/gpt2_backbone_test.py
-keras_nlp/models/gpt2/gpt2_causal_lm.py
-keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor.py
-keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor_test.py
-keras_nlp/models/gpt2/gpt2_causal_lm_test.py
-keras_nlp/models/gpt2/gpt2_preprocessor.py
-keras_nlp/models/gpt2/gpt2_preprocessor_test.py
-keras_nlp/models/gpt2/gpt2_presets.py
-keras_nlp/models/gpt2/gpt2_presets_test.py
-keras_nlp/models/gpt2/gpt2_tokenizer.py
-keras_nlp/models/gpt2/gpt2_tokenizer_test.py
-keras_nlp/models/opt/__init__.py
-keras_nlp/models/opt/opt_backbone.py
-keras_nlp/models/opt/opt_backbone_test.py
-keras_nlp/models/opt/opt_causal_lm.py
-keras_nlp/models/opt/opt_causal_lm_preprocessor.py
-keras_nlp/models/opt/opt_causal_lm_preprocessor_test.py
-keras_nlp/models/opt/opt_causal_lm_test.py
-keras_nlp/models/opt/opt_preprocessor.py
-keras_nlp/models/opt/opt_preprocessor_test.py
-keras_nlp/models/opt/opt_presets.py
-keras_nlp/models/opt/opt_presets_test.py
-keras_nlp/models/opt/opt_tokenizer.py
-keras_nlp/models/opt/opt_tokenizer_test.py
-keras_nlp/models/roberta/__init__.py
-keras_nlp/models/roberta/roberta_backbone.py
-keras_nlp/models/roberta/roberta_backbone_test.py
-keras_nlp/models/roberta/roberta_classifier.py
-keras_nlp/models/roberta/roberta_classifier_test.py
-keras_nlp/models/roberta/roberta_masked_lm.py
-keras_nlp/models/roberta/roberta_masked_lm_preprocessor.py
-keras_nlp/models/roberta/roberta_masked_lm_preprocessor_test.py
-keras_nlp/models/roberta/roberta_masked_lm_test.py
-keras_nlp/models/roberta/roberta_multi_segment_packer.py
-keras_nlp/models/roberta/roberta_preprocessor.py
-keras_nlp/models/roberta/roberta_preprocessor_test.py
-keras_nlp/models/roberta/roberta_presets.py
-keras_nlp/models/roberta/roberta_presets_test.py
-keras_nlp/models/roberta/roberta_tokenizer.py
-keras_nlp/models/roberta/roberta_tokenizer_test.py
-keras_nlp/models/t5/__init__.py
-keras_nlp/models/t5/t5_backbone.py
-keras_nlp/models/t5/t5_backbone_test.py
-keras_nlp/models/t5/t5_layer_norm.py
-keras_nlp/models/t5/t5_multi_head_attention.py
-keras_nlp/models/t5/t5_tokenizer.py
-keras_nlp/models/t5/t5_tokenizer_test.py
-keras_nlp/models/t5/t5_transformer_layer.py
-keras_nlp/models/whisper/__init__.py
-keras_nlp/models/whisper/whisper_backbone.py
-keras_nlp/models/whisper/whisper_backbone_test.py
-keras_nlp/models/whisper/whisper_decoder.py
-keras_nlp/models/whisper/whisper_encoder.py
-keras_nlp/models/xlm_roberta/__init__.py
-keras_nlp/models/xlm_roberta/xlm_roberta_backbone.py
-keras_nlp/models/xlm_roberta/xlm_roberta_backbone_test.py
-keras_nlp/models/xlm_roberta/xlm_roberta_classifier.py
-keras_nlp/models/xlm_roberta/xlm_roberta_classifier_test.py
-keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm.py
-keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
-keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
-keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_test.py
-keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor.py
-keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor_test.py
-keras_nlp/models/xlm_roberta/xlm_roberta_presets.py
-keras_nlp/models/xlm_roberta/xlm_roberta_presets_test.py
-keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer.py
-keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer_test.py
 keras_nlp/samplers/__init__.py
-keras_nlp/samplers/beam_sampler.py
-keras_nlp/samplers/beam_sampler_test.py
-keras_nlp/samplers/contrastive_sampler.py
-keras_nlp/samplers/contrastive_sampler_test.py
-keras_nlp/samplers/greedy_sampler.py
-keras_nlp/samplers/greedy_sampler_test.py
-keras_nlp/samplers/random_sampler.py
-keras_nlp/samplers/random_sampler_test.py
-keras_nlp/samplers/sampler.py
-keras_nlp/samplers/serialization.py
-keras_nlp/samplers/serialization_test.py
-keras_nlp/samplers/top_k_sampler.py
-keras_nlp/samplers/top_k_sampler_test.py
-keras_nlp/samplers/top_p_sampler.py
-keras_nlp/samplers/top_p_sampler_test.py
-keras_nlp/tests/__init__.py
-keras_nlp/tests/doc_tests/__init__.py
-keras_nlp/tests/doc_tests/docstring_lib.py
-keras_nlp/tests/doc_tests/docstring_test.py
-keras_nlp/tests/doc_tests/fenced_docstring_lib.py
-keras_nlp/tokenizers/__init__.py
-keras_nlp/tokenizers/byte_pair_tokenizer.py
-keras_nlp/tokenizers/byte_pair_tokenizer_test.py
-keras_nlp/tokenizers/byte_tokenizer.py
-keras_nlp/tokenizers/byte_tokenizer_test.py
-keras_nlp/tokenizers/sentence_piece_tokenizer.py
-keras_nlp/tokenizers/sentence_piece_tokenizer_test.py
-keras_nlp/tokenizers/sentence_piece_tokenizer_trainer.py
-keras_nlp/tokenizers/sentence_piece_tokenizer_trainer_test.py
-keras_nlp/tokenizers/tokenizer.py
-keras_nlp/tokenizers/tokenizer_test.py
-keras_nlp/tokenizers/unicode_codepoint_tokenizer.py
-keras_nlp/tokenizers/unicode_codepoint_tokenizer_test.py
-keras_nlp/tokenizers/word_piece_tokenizer.py
-keras_nlp/tokenizers/word_piece_tokenizer_test.py
-keras_nlp/tokenizers/word_piece_tokenizer_trainer.py
-keras_nlp/tokenizers/word_piece_tokenizer_trainer_test.py
-keras_nlp/utils/__init__.py
-keras_nlp/utils/keras_utils.py
-keras_nlp/utils/keras_utils_test.py
-keras_nlp/utils/pipeline_model.py
-keras_nlp/utils/pipeline_model_test.py
-keras_nlp/utils/python_utils.py
-keras_nlp/utils/python_utils_test.py
-keras_nlp/utils/tf_utils.py
-keras_nlp/utils/tf_utils_test.py
-tools/__init__.py
-tools/count_preset_params.py
-tools/checkpoint_conversion/__init__.py
-tools/checkpoint_conversion/checkpoint_conversion_utils.py
-tools/checkpoint_conversion/convert_albert_checkpoints.py
-tools/checkpoint_conversion/convert_bart_checkpoints.py
-tools/checkpoint_conversion/convert_deberta_v3_checkpoints.py
-tools/checkpoint_conversion/convert_distilbert_checkpoints.py
-tools/checkpoint_conversion/convert_f_net_checkpoints.py
-tools/checkpoint_conversion/convert_gpt2_checkpoints.py
-tools/checkpoint_conversion/convert_opt_checkpoints.py
-tools/checkpoint_conversion/convert_roberta_checkpoints.py
-tools/checkpoint_conversion/convert_xlm_roberta_checkpoints.py
+keras_nlp/src/__init__.py
+keras_nlp/src/api_export.py
+keras_nlp/src/conftest.py
+keras_nlp/src/layers/__init__.py
+keras_nlp/src/layers/cached_multi_head_attention.py
+keras_nlp/src/layers/cached_multi_head_attention_test.py
+keras_nlp/src/layers/f_net_encoder.py
+keras_nlp/src/layers/f_net_encoder_test.py
+keras_nlp/src/layers/masked_lm_head.py
+keras_nlp/src/layers/masked_lm_head_test.py
+keras_nlp/src/layers/masked_lm_mask_generator.py
+keras_nlp/src/layers/masked_lm_mask_generator_test.py
+keras_nlp/src/layers/multi_segment_packer.py
+keras_nlp/src/layers/multi_segment_packer_test.py
+keras_nlp/src/layers/position_embedding.py
+keras_nlp/src/layers/position_embedding_test.py
+keras_nlp/src/layers/random_deletion.py
+keras_nlp/src/layers/random_deletion_test.py
+keras_nlp/src/layers/random_swap.py
+keras_nlp/src/layers/random_swap_test.py
+keras_nlp/src/layers/sine_position_encoding.py
+keras_nlp/src/layers/sine_position_encoding_test.py
+keras_nlp/src/layers/start_end_packer.py
+keras_nlp/src/layers/start_end_packer_test.py
+keras_nlp/src/layers/token_and_position_embedding.py
+keras_nlp/src/layers/token_and_position_embedding_test.py
+keras_nlp/src/layers/transformer_decoder.py
+keras_nlp/src/layers/transformer_decoder_test.py
+keras_nlp/src/layers/transformer_encoder.py
+keras_nlp/src/layers/transformer_encoder_test.py
+keras_nlp/src/layers/transformer_layer_utils.py
+keras_nlp/src/layers/transformer_layer_utils_test.py
+keras_nlp/src/metrics/__init__.py
+keras_nlp/src/metrics/bleu.py
+keras_nlp/src/metrics/bleu_test.py
+keras_nlp/src/metrics/edit_distance.py
+keras_nlp/src/metrics/edit_distance_test.py
+keras_nlp/src/metrics/perplexity.py
+keras_nlp/src/metrics/perplexity_test.py
+keras_nlp/src/metrics/rouge_base.py
+keras_nlp/src/metrics/rouge_l.py
+keras_nlp/src/metrics/rouge_l_test.py
+keras_nlp/src/metrics/rouge_n.py
+keras_nlp/src/metrics/rouge_n_test.py
+keras_nlp/src/models/__init__.py
+keras_nlp/src/models/backbone.py
+keras_nlp/src/models/preprocessor.py
+keras_nlp/src/models/task.py
+keras_nlp/src/models/task_test.py
+keras_nlp/src/models/albert/__init__.py
+keras_nlp/src/models/albert/albert_backbone.py
+keras_nlp/src/models/albert/albert_backbone_test.py
+keras_nlp/src/models/albert/albert_classifier.py
+keras_nlp/src/models/albert/albert_classifier_test.py
+keras_nlp/src/models/albert/albert_masked_lm.py
+keras_nlp/src/models/albert/albert_masked_lm_preprocessor.py
+keras_nlp/src/models/albert/albert_masked_lm_preprocessor_test.py
+keras_nlp/src/models/albert/albert_masked_lm_test.py
+keras_nlp/src/models/albert/albert_preprocessor.py
+keras_nlp/src/models/albert/albert_preprocessor_test.py
+keras_nlp/src/models/albert/albert_presets.py
+keras_nlp/src/models/albert/albert_presets_test.py
+keras_nlp/src/models/albert/albert_tokenizer.py
+keras_nlp/src/models/albert/albert_tokenizer_test.py
+keras_nlp/src/models/bart/__init__.py
+keras_nlp/src/models/bart/bart_backbone.py
+keras_nlp/src/models/bart/bart_backbone_test.py
+keras_nlp/src/models/bart/bart_preprocessor.py
+keras_nlp/src/models/bart/bart_preprocessor_test.py
+keras_nlp/src/models/bart/bart_presets.py
+keras_nlp/src/models/bart/bart_presets_test.py
+keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor.py
+keras_nlp/src/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
+keras_nlp/src/models/bart/bart_tokenizer.py
+keras_nlp/src/models/bart/bart_tokenizer_test.py
+keras_nlp/src/models/bert/__init__.py
+keras_nlp/src/models/bert/bert_backbone.py
+keras_nlp/src/models/bert/bert_backbone_test.py
+keras_nlp/src/models/bert/bert_classifier.py
+keras_nlp/src/models/bert/bert_classifier_test.py
+keras_nlp/src/models/bert/bert_masked_lm.py
+keras_nlp/src/models/bert/bert_masked_lm_preprocessor.py
+keras_nlp/src/models/bert/bert_masked_lm_preprocessor_test.py
+keras_nlp/src/models/bert/bert_masked_lm_test.py
+keras_nlp/src/models/bert/bert_preprocessor.py
+keras_nlp/src/models/bert/bert_preprocessor_test.py
+keras_nlp/src/models/bert/bert_presets.py
+keras_nlp/src/models/bert/bert_presets_test.py
+keras_nlp/src/models/bert/bert_tokenizer.py
+keras_nlp/src/models/bert/bert_tokenizer_test.py
+keras_nlp/src/models/deberta_v3/__init__.py
+keras_nlp/src/models/deberta_v3/deberta_v3_backbone.py
+keras_nlp/src/models/deberta_v3/deberta_v3_backbone_test.py
+keras_nlp/src/models/deberta_v3/deberta_v3_classifier.py
+keras_nlp/src/models/deberta_v3/deberta_v3_classifier_test.py
+keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm.py
+keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
+keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
+keras_nlp/src/models/deberta_v3/deberta_v3_masked_lm_test.py
+keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor.py
+keras_nlp/src/models/deberta_v3/deberta_v3_preprocessor_test.py
+keras_nlp/src/models/deberta_v3/deberta_v3_presets.py
+keras_nlp/src/models/deberta_v3/deberta_v3_presets_test.py
+keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer.py
+keras_nlp/src/models/deberta_v3/deberta_v3_tokenizer_test.py
+keras_nlp/src/models/deberta_v3/disentangled_attention_encoder.py
+keras_nlp/src/models/deberta_v3/disentangled_self_attention.py
+keras_nlp/src/models/deberta_v3/relative_embedding.py
+keras_nlp/src/models/distil_bert/__init__.py
+keras_nlp/src/models/distil_bert/distil_bert_backbone.py
+keras_nlp/src/models/distil_bert/distil_bert_backbone_test.py
+keras_nlp/src/models/distil_bert/distil_bert_classifier.py
+keras_nlp/src/models/distil_bert/distil_bert_classifier_test.py
+keras_nlp/src/models/distil_bert/distil_bert_masked_lm.py
+keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor.py
+keras_nlp/src/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
+keras_nlp/src/models/distil_bert/distil_bert_masked_lm_test.py
+keras_nlp/src/models/distil_bert/distil_bert_preprocessor.py
+keras_nlp/src/models/distil_bert/distil_bert_preprocessor_test.py
+keras_nlp/src/models/distil_bert/distil_bert_presets.py
+keras_nlp/src/models/distil_bert/distil_bert_presets_test.py
+keras_nlp/src/models/distil_bert/distil_bert_tokenizer.py
+keras_nlp/src/models/distil_bert/distil_bert_tokenizer_test.py
+keras_nlp/src/models/f_net/__init__.py
+keras_nlp/src/models/f_net/f_net_backbone.py
+keras_nlp/src/models/f_net/f_net_backbone_test.py
+keras_nlp/src/models/f_net/f_net_classifier.py
+keras_nlp/src/models/f_net/f_net_classifier_test.py
+keras_nlp/src/models/f_net/f_net_masked_lm.py
+keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor.py
+keras_nlp/src/models/f_net/f_net_masked_lm_preprocessor_test.py
+keras_nlp/src/models/f_net/f_net_masked_lm_test.py
+keras_nlp/src/models/f_net/f_net_preprocessor.py
+keras_nlp/src/models/f_net/f_net_preprocessor_test.py
+keras_nlp/src/models/f_net/f_net_presets.py
+keras_nlp/src/models/f_net/f_net_presets_test.py
+keras_nlp/src/models/f_net/f_net_tokenizer.py
+keras_nlp/src/models/f_net/f_net_tokenizer_test.py
+keras_nlp/src/models/gpt2/__init__.py
+keras_nlp/src/models/gpt2/gpt2_backbone.py
+keras_nlp/src/models/gpt2/gpt2_backbone_test.py
+keras_nlp/src/models/gpt2/gpt2_causal_lm.py
+keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor.py
+keras_nlp/src/models/gpt2/gpt2_causal_lm_preprocessor_test.py
+keras_nlp/src/models/gpt2/gpt2_causal_lm_test.py
+keras_nlp/src/models/gpt2/gpt2_preprocessor.py
+keras_nlp/src/models/gpt2/gpt2_preprocessor_test.py
+keras_nlp/src/models/gpt2/gpt2_presets.py
+keras_nlp/src/models/gpt2/gpt2_presets_test.py
+keras_nlp/src/models/gpt2/gpt2_tokenizer.py
+keras_nlp/src/models/gpt2/gpt2_tokenizer_test.py
+keras_nlp/src/models/opt/__init__.py
+keras_nlp/src/models/opt/opt_backbone.py
+keras_nlp/src/models/opt/opt_backbone_test.py
+keras_nlp/src/models/opt/opt_causal_lm.py
+keras_nlp/src/models/opt/opt_causal_lm_preprocessor.py
+keras_nlp/src/models/opt/opt_causal_lm_preprocessor_test.py
+keras_nlp/src/models/opt/opt_causal_lm_test.py
+keras_nlp/src/models/opt/opt_preprocessor.py
+keras_nlp/src/models/opt/opt_preprocessor_test.py
+keras_nlp/src/models/opt/opt_presets.py
+keras_nlp/src/models/opt/opt_presets_test.py
+keras_nlp/src/models/opt/opt_tokenizer.py
+keras_nlp/src/models/opt/opt_tokenizer_test.py
+keras_nlp/src/models/roberta/__init__.py
+keras_nlp/src/models/roberta/roberta_backbone.py
+keras_nlp/src/models/roberta/roberta_backbone_test.py
+keras_nlp/src/models/roberta/roberta_classifier.py
+keras_nlp/src/models/roberta/roberta_classifier_test.py
+keras_nlp/src/models/roberta/roberta_masked_lm.py
+keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor.py
+keras_nlp/src/models/roberta/roberta_masked_lm_preprocessor_test.py
+keras_nlp/src/models/roberta/roberta_masked_lm_test.py
+keras_nlp/src/models/roberta/roberta_multi_segment_packer.py
+keras_nlp/src/models/roberta/roberta_preprocessor.py
+keras_nlp/src/models/roberta/roberta_preprocessor_test.py
+keras_nlp/src/models/roberta/roberta_presets.py
+keras_nlp/src/models/roberta/roberta_presets_test.py
+keras_nlp/src/models/roberta/roberta_tokenizer.py
+keras_nlp/src/models/roberta/roberta_tokenizer_test.py
+keras_nlp/src/models/t5/__init__.py
+keras_nlp/src/models/t5/t5_backbone.py
+keras_nlp/src/models/t5/t5_backbone_test.py
+keras_nlp/src/models/t5/t5_layer_norm.py
+keras_nlp/src/models/t5/t5_multi_head_attention.py
+keras_nlp/src/models/t5/t5_tokenizer.py
+keras_nlp/src/models/t5/t5_tokenizer_test.py
+keras_nlp/src/models/t5/t5_transformer_layer.py
+keras_nlp/src/models/whisper/__init__.py
+keras_nlp/src/models/whisper/whisper_backbone.py
+keras_nlp/src/models/whisper/whisper_backbone_test.py
+keras_nlp/src/models/whisper/whisper_decoder.py
+keras_nlp/src/models/whisper/whisper_encoder.py
+keras_nlp/src/models/xlm_roberta/__init__.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_backbone_test.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_classifier_test.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_masked_lm_test.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_preprocessor_test.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_presets.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_presets_test.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer.py
+keras_nlp/src/models/xlm_roberta/xlm_roberta_tokenizer_test.py
+keras_nlp/src/samplers/__init__.py
+keras_nlp/src/samplers/beam_sampler.py
+keras_nlp/src/samplers/beam_sampler_test.py
+keras_nlp/src/samplers/contrastive_sampler.py
+keras_nlp/src/samplers/contrastive_sampler_test.py
+keras_nlp/src/samplers/greedy_sampler.py
+keras_nlp/src/samplers/greedy_sampler_test.py
+keras_nlp/src/samplers/random_sampler.py
+keras_nlp/src/samplers/random_sampler_test.py
+keras_nlp/src/samplers/sampler.py
+keras_nlp/src/samplers/serialization.py
+keras_nlp/src/samplers/serialization_test.py
+keras_nlp/src/samplers/top_k_sampler.py
+keras_nlp/src/samplers/top_k_sampler_test.py
+keras_nlp/src/samplers/top_p_sampler.py
+keras_nlp/src/samplers/top_p_sampler_test.py
+keras_nlp/src/tests/__init__.py
+keras_nlp/src/tests/doc_tests/__init__.py
+keras_nlp/src/tests/doc_tests/docstring_lib.py
+keras_nlp/src/tests/doc_tests/docstring_test.py
+keras_nlp/src/tests/doc_tests/fenced_docstring_lib.py
+keras_nlp/src/tokenizers/__init__.py
+keras_nlp/src/tokenizers/byte_pair_tokenizer.py
+keras_nlp/src/tokenizers/byte_pair_tokenizer_test.py
+keras_nlp/src/tokenizers/byte_tokenizer.py
+keras_nlp/src/tokenizers/byte_tokenizer_test.py
+keras_nlp/src/tokenizers/sentence_piece_tokenizer.py
+keras_nlp/src/tokenizers/sentence_piece_tokenizer_test.py
+keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer.py
+keras_nlp/src/tokenizers/sentence_piece_tokenizer_trainer_test.py
+keras_nlp/src/tokenizers/tokenizer.py
+keras_nlp/src/tokenizers/tokenizer_test.py
+keras_nlp/src/tokenizers/unicode_codepoint_tokenizer.py
+keras_nlp/src/tokenizers/unicode_codepoint_tokenizer_test.py
+keras_nlp/src/tokenizers/word_piece_tokenizer.py
+keras_nlp/src/tokenizers/word_piece_tokenizer_test.py
+keras_nlp/src/tokenizers/word_piece_tokenizer_trainer.py
+keras_nlp/src/tokenizers/word_piece_tokenizer_trainer_test.py
+keras_nlp/src/utils/__init__.py
+keras_nlp/src/utils/keras_utils.py
+keras_nlp/src/utils/keras_utils_test.py
+keras_nlp/src/utils/pipeline_model.py
+keras_nlp/src/utils/pipeline_model_test.py
+keras_nlp/src/utils/python_utils.py
+keras_nlp/src/utils/python_utils_test.py
+keras_nlp/src/utils/tf_utils.py
+keras_nlp/src/utils/tf_utils_test.py
+keras_nlp/tokenizers/__init__.py
```

### Comparing `keras-nlp-0.5.0.dev0/setup.cfg` & `keras-nlp-0.5.0.dev4/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.5.0.dev0/setup.py` & `keras-nlp-0.5.0.dev4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,46 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Setup script."""
 
+import os
 import pathlib
 
 from setuptools import find_packages
 from setuptools import setup
 
+
+def read(rel_path):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with open(os.path.join(here, rel_path)) as fp:
+        return fp.read()
+
+
+def get_version(rel_path):
+    for line in read(rel_path).splitlines():
+        if line.startswith("__version__"):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    raise RuntimeError("Unable to find version string.")
+
+
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="keras-nlp",
     description=(
         "Industry-strength Natural Language Processing extensions for Keras."
     ),
     long_description=README,
     long_description_content_type="text/markdown",
-    version="0.5.0.dev0",
+    version=get_version("keras_nlp/__init__.py"),
     url="https://github.com/keras-team/keras-nlp",
     author="Keras team",
     author_email="keras-nlp@google.com",
     license="Apache License 2.0",
     install_requires=[
         "absl-py",
         "numpy",
```

