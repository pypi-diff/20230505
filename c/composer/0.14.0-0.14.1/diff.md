# Comparing `tmp/composer-0.14.0.tar.gz` & `tmp/composer-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composer-0.14.0.tar", last modified: Wed May  3 15:48:36 2023, max compression
+gzip compressed data, was "composer-0.14.1.tar", last modified: Fri May  5 05:53:21 2023, max compression
```

## Comparing `composer-0.14.0.tar` & `composer-0.14.1.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.853834 composer-0.14.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-03 15:48:18.000000 composer-0.14.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 15:48:18.000000 composer-0.14.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-05-03 15:48:36.853834 composer-0.14.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-05-03 15:48:18.000000 composer-0.14.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.745833 composer-0.14.0/composer/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-03 15:48:18.000000 composer-0.14.0/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 15:48:18.000000 composer-0.14.0/composer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 15:48:18.000000 composer-0.14.0/composer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.749833 composer-0.14.0/composer/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.749833 composer-0.14.0/composer/algorithms/alibi/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/alibi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.749833 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/alibi/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.753833 composer-0.14.0/composer/algorithms/augmix/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/augmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/augmix/augmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/augmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.753833 composer-0.14.0/composer/algorithms/blurpool/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/blurpool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/blurpool/blurpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/blurpool/blurpool_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/blurpool/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.753833 composer-0.14.0/composer/algorithms/channels_last/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/channels_last/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/channels_last/channels_last.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/channels_last/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.757833 composer-0.14.0/composer/algorithms/colout/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/colout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/colout/colout.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/colout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.757833 composer-0.14.0/composer/algorithms/cutmix/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutmix/cutmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.757833 composer-0.14.0/composer/algorithms/cutout/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutout/cutout.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/cutout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.757833 composer-0.14.0/composer/algorithms/ema/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ema/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ema/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.761833 composer-0.14.0/composer/algorithms/factorize/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/factorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/factorize_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/factorize_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/factorize/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.761833 composer-0.14.0/composer/algorithms/fused_layernorm/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/fused_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/fused_layernorm/fused_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/fused_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.765833 composer-0.14.0/composer/algorithms/gated_linear_units/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gated_linear_units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gated_linear_units/gated_linear_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gated_linear_units/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.765833 composer-0.14.0/composer/algorithms/ghost_batchnorm/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ghost_batchnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/ghost_batchnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.769833 composer-0.14.0/composer/algorithms/gradient_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gradient_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gradient_clipping/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gradient_clipping/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.769833 composer-0.14.0/composer/algorithms/gyro_dropout/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gyro_dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gyro_dropout/gyro_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/gyro_dropout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.769833 composer-0.14.0/composer/algorithms/label_smoothing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/label_smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/label_smoothing/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/label_smoothing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.769833 composer-0.14.0/composer/algorithms/layer_freezing/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/layer_freezing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/layer_freezing/layer_freezing.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/layer_freezing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.773833 composer-0.14.0/composer/algorithms/low_precision_groupnorm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_groupnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_groupnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.773833 composer-0.14.0/composer/algorithms/low_precision_layernorm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/low_precision_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.773833 composer-0.14.0/composer/algorithms/mixup/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/mixup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/mixup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/mixup/mixup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.777833 composer-0.14.0/composer/algorithms/no_op_model/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/no_op_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/no_op_model/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/no_op_model/no_op_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.777833 composer-0.14.0/composer/algorithms/progressive_resizing/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/progressive_resizing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/progressive_resizing/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/progressive_resizing/progressive_resizing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.777833 composer-0.14.0/composer/algorithms/randaugment/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/randaugment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/randaugment/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/randaugment/randaugment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.777833 composer-0.14.0/composer/algorithms/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/sam/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/sam/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.781833 composer-0.14.0/composer/algorithms/selective_backprop/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/selective_backprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/selective_backprop/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/selective_backprop/selective_backprop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.781833 composer-0.14.0/composer/algorithms/seq_length_warmup/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/seq_length_warmup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/seq_length_warmup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    18808 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/seq_length_warmup/seq_length_warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.781833 composer-0.14.0/composer/algorithms/squeeze_excite/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/squeeze_excite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/squeeze_excite/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/squeeze_excite/squeeze_excite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.785833 composer-0.14.0/composer/algorithms/stochastic_depth/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/stochastic_depth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/stochastic_depth/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/stochastic_depth/stochastic_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/stochastic_depth/stochastic_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.785833 composer-0.14.0/composer/algorithms/swa/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/swa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/swa/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/swa/swa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.785833 composer-0.14.0/composer/algorithms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/utils/augmentation_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/utils/augmentation_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.789833 composer-0.14.0/composer/algorithms/weight_standardization/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/weight_standardization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/weight_standardization/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-03 15:48:18.000000 composer-0.14.0/composer/algorithms/weight_standardization/weight_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.793833 composer-0.14.0/composer/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/activation_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/early_stopper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/export_for_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/image_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/mlperf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/optimizer_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/runtime_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/speed_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-03 15:48:18.000000 composer-0.14.0/composer/callbacks/threshold_stopper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.793833 composer-0.14.0/composer/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 15:48:18.000000 composer-0.14.0/composer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-03 15:48:18.000000 composer-0.14.0/composer/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21453 2023-05-03 15:48:18.000000 composer-0.14.0/composer/cli/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.801833 composer-0.14.0/composer/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/data_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)    67948 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-03 15:48:18.000000 composer-0.14.0/composer/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.805833 composer-0.14.0/composer/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/c4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/ffcv_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    51747 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/in_context_learning_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/lm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-03 15:48:18.000000 composer-0.14.0/composer/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.805833 composer-0.14.0/composer/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device_mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-03 15:48:18.000000 composer-0.14.0/composer/devices/device_tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.805833 composer-0.14.0/composer/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-03 15:48:18.000000 composer-0.14.0/composer/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.813834 composer-0.14.0/composer/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/cometml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/file_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/in_memory_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/logger_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/mosaicml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/progress_bar_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    28802 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/remote_uploader_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/slack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.813834 composer-0.14.0/composer/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loss/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-03 15:48:18.000000 composer-0.14.0/composer/loss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.817834 composer-0.14.0/composer/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-03 15:48:18.000000 composer-0.14.0/composer/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-05-03 15:48:18.000000 composer-0.14.0/composer/metrics/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-03 15:48:18.000000 composer-0.14.0/composer/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    25727 2023-05-03 15:48:18.000000 composer-0.14.0/composer/metrics/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.817834 composer-0.14.0/composer/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.817834 composer-0.14.0/composer/models/bert/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/bert/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.817834 composer-0.14.0/composer/models/classify_mnist/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/classify_mnist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/classify_mnist/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.821833 composer-0.14.0/composer/models/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/deeplabv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/deeplabv3/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.821833 composer-0.14.0/composer/models/efficientnetb0/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/efficientnetb0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/efficientnetb0/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/efficientnetb0/efficientnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/efficientnetb0/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.821833 composer-0.14.0/composer/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/gpt2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    34533 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/mmdetection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.821833 composer-0.14.0/composer/models/resnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.825834 composer-0.14.0/composer/models/resnet_cifar/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet_cifar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet_cifar/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/resnet_cifar/resnets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.825834 composer-0.14.0/composer/models/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/tasks/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.825834 composer-0.14.0/composer/models/timm/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/timm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.825834 composer-0.14.0/composer/models/unet/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/unet/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/unet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/unet/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.829834 composer-0.14.0/composer/models/vit_small_patch16/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/vit_small_patch16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-03 15:48:18.000000 composer-0.14.0/composer/models/vit_small_patch16/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.829834 composer-0.14.0/composer/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-03 15:48:18.000000 composer-0.14.0/composer/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20226 2023-05-03 15:48:18.000000 composer-0.14.0/composer/optim/decoupled_weight_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)    35768 2023-05-03 15:48:18.000000 composer-0.14.0/composer/optim/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.833834 composer-0.14.0/composer/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/json_trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/json_trace_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/profiler_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/profiler_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/system_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/torch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-03 15:48:18.000000 composer-0.14.0/composer/profiler/trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:18.000000 composer-0.14.0/composer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.837834 composer-0.14.0/composer/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/_scale_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    23655 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/dist_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/meta_safe_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/mosaic_fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)   153175 2023-05-03 15:48:18.000000 composer-0.14.0/composer/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.845834 composer-0.14.0/composer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/auto_log_hparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/batch_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30139 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/fx_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/import_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/iter_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/module_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.845834 composer-0.14.0/composer/utils/object_store/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/libcloud_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/oci_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/object_store/sftp_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/retrying.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-03 15:48:18.000000 composer-0.14.0/composer/utils/string_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.745833 composer-0.14.0/composer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 15:48:36.000000 composer-0.14.0/composer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34985 2023-05-03 15:48:18.000000 composer-0.14.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:48:36.853834 composer-0.14.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-03 15:48:18.000000 composer-0.14.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:48:36.853834 composer-0.14.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_full_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_simple_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_smoketest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_split_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-03 15:48:18.000000 composer-0.14.0/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.599103 composer-0.14.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-05 05:53:05.000000 composer-0.14.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 05:53:05.000000 composer-0.14.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20919 2023-05-05 05:53:21.599103 composer-0.14.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-05-05 05:53:05.000000 composer-0.14.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-05 05:53:05.000000 composer-0.14.1/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-05 05:53:05.000000 composer-0.14.1/composer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-05 05:53:05.000000 composer-0.14.1/composer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer/algorithms/alibi/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/alibi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.531102 composer-0.14.1/composer/algorithms/augmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/augmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/augmix/augmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/augmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.531102 composer-0.14.1/composer/algorithms/blurpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/blurpool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/blurpool/blurpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/blurpool/blurpool_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/blurpool/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.531102 composer-0.14.1/composer/algorithms/channels_last/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/channels_last/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/channels_last/channels_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/channels_last/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.535102 composer-0.14.1/composer/algorithms/colout/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/colout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/colout/colout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/colout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.535102 composer-0.14.1/composer/algorithms/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutmix/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.535102 composer-0.14.1/composer/algorithms/cutout/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutout/cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.535102 composer-0.14.1/composer/algorithms/ema/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ema/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ema/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/factorize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/factorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/factorize_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/factorize_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/fused_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/fused_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/fused_layernorm/fused_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/fused_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/gated_linear_units/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gated_linear_units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gated_linear_units/gated_linear_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gated_linear_units/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/ghost_batchnorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ghost_batchnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ghost_batchnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/gradient_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gradient_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gradient_clipping/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gradient_clipping/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/gyro_dropout/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gyro_dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gyro_dropout/gyro_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gyro_dropout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.543102 composer-0.14.1/composer/algorithms/label_smoothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/label_smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/label_smoothing/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/label_smoothing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.543102 composer-0.14.1/composer/algorithms/layer_freezing/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/layer_freezing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/layer_freezing/layer_freezing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/layer_freezing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.543102 composer-0.14.1/composer/algorithms/low_precision_groupnorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_groupnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_groupnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.543102 composer-0.14.1/composer/algorithms/low_precision_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/mixup/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/mixup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/mixup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/mixup/mixup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/no_op_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/no_op_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/no_op_model/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/no_op_model/no_op_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/progressive_resizing/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/progressive_resizing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/progressive_resizing/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/progressive_resizing/progressive_resizing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/randaugment/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/randaugment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/randaugment/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/randaugment/randaugment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/sam/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/sam/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.551102 composer-0.14.1/composer/algorithms/selective_backprop/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/selective_backprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/selective_backprop/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/selective_backprop/selective_backprop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.551102 composer-0.14.1/composer/algorithms/seq_length_warmup/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/seq_length_warmup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/seq_length_warmup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18808 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/seq_length_warmup/seq_length_warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.551102 composer-0.14.1/composer/algorithms/squeeze_excite/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/squeeze_excite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/squeeze_excite/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/squeeze_excite/squeeze_excite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.551102 composer-0.14.1/composer/algorithms/stochastic_depth/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/stochastic_depth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/stochastic_depth/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/stochastic_depth/stochastic_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/stochastic_depth/stochastic_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.555102 composer-0.14.1/composer/algorithms/swa/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/swa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/swa/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/swa/swa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.555102 composer-0.14.1/composer/algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/utils/augmentation_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/utils/augmentation_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.555102 composer-0.14.1/composer/algorithms/weight_standardization/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/weight_standardization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/weight_standardization/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/weight_standardization/weight_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.559102 composer-0.14.1/composer/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/activation_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/early_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/export_for_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/mlperf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/optimizer_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/runtime_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/speed_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/threshold_stopper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.559102 composer-0.14.1/composer/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 05:53:05.000000 composer-0.14.1/composer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 05:53:05.000000 composer-0.14.1/composer/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21453 2023-05-05 05:53:05.000000 composer-0.14.1/composer/cli/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.563102 composer-0.14.1/composer/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/passes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67948 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.567102 composer-0.14.1/composer/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/c4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/ffcv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51670 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/in_context_learning_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/lm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.567102 composer-0.14.1/composer/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device_mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device_tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.567102 composer-0.14.1/composer/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-05 05:53:05.000000 composer-0.14.1/composer/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.571102 composer-0.14.1/composer/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/cometml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/file_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/in_memory_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/logger_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/mosaicml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/progress_bar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28802 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/remote_uploader_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/slack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loss/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 05:53:05.000000 composer-0.14.1/composer/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-05-05 05:53:05.000000 composer-0.14.1/composer/metrics/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-05 05:53:05.000000 composer-0.14.1/composer/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25727 2023-05-05 05:53:05.000000 composer-0.14.1/composer/metrics/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/bert/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/models/classify_mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/classify_mnist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/classify_mnist/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/models/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/deeplabv3/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/efficientnetb0/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/efficientnetb0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/efficientnetb0/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/efficientnetb0/efficientnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/efficientnetb0/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/gpt2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34533 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/mmdetection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/resnet_cifar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet_cifar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet_cifar/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet_cifar/resnets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/tasks/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.583102 composer-0.14.1/composer/models/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/unet/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/unet/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.583102 composer-0.14.1/composer/models/vit_small_patch16/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/vit_small_patch16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/vit_small_patch16/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.583102 composer-0.14.1/composer/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-05 05:53:05.000000 composer-0.14.1/composer/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20226 2023-05-05 05:53:05.000000 composer-0.14.1/composer/optim/decoupled_weight_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35768 2023-05-05 05:53:05.000000 composer-0.14.1/composer/optim/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.587103 composer-0.14.1/composer/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/json_trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/json_trace_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/profiler_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/profiler_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/system_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/torch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:05.000000 composer-0.14.1/composer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.587103 composer-0.14.1/composer/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/_scale_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23655 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/dist_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/meta_safe_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/mosaic_fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153175 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.591102 composer-0.14.1/composer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/auto_log_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/batch_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30139 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/fx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/import_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/iter_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/module_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.595102 composer-0.14.1/composer/utils/object_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/libcloud_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/oci_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/sftp_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/retrying.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/string_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20919 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34985 2023-05-05 05:53:05.000000 composer-0.14.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:53:21.599103 composer-0.14.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-05 05:53:05.000000 composer-0.14.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.599103 composer-0.14.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_full_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_passes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_simple_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_smoketest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_split_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_time.py
```

### Comparing `composer-0.14.0/LICENSE` & `composer-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/PKG-INFO` & `composer-0.14.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.14.0
+Version: 0.14.1
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -218,17 +218,14 @@
 ## 🛠 Building Speedup Recipes
 
 Given two methods that speed up training by 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not necessarily.
 They may optimize the [same part of the training process](https://en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they may even interact in ways that prove detrimental.
 Determining which methods to compose together isn't as simple as assembling a set of methods that perform best individually.
 
 **We have come up with compositions of methods that work especially well together** through rigorous exploration of the design space of recipes and research on the science behind composition.
-The [MosaicML Explorer](https://app.mosaicml.com/) contains all of the data we have collected so far on composition, and it highlights the compositions of methods that are _pareto-optimal_ - that provide the **best possible tradeoffs between training time or cost and the quality of the trained model**.
-Whether you want to reach the same quality faster or get better quality within your current budget, Explorer can help you decide which speedup methods to use.
-We update this data regularly as we add new methods and develop better recipes.
 
 <p align="center">
 <img src="https://storage.googleapis.com/docs.mosaicml.com/images/methods/explorer.png"/>
 </p>
 
 As an example, here are two performant recipes, one for ResNet-101 on ImageNet, and the other for GPT-2 on OpenWebText, on 8xA100s:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: composer Version: 0.14.0 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.14.1 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
@@ -125,22 +125,15 @@
 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not
 necessarily. They may optimize the [same part of the training process](https://
 en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they
 may even interact in ways that prove detrimental. Determining which methods to
 compose together isn't as simple as assembling a set of methods that perform
 best individually. **We have come up with compositions of methods that work
 especially well together** through rigorous exploration of the design space of
-recipes and research on the science behind composition. The [MosaicML Explorer]
-(https://app.mosaicml.com/) contains all of the data we have collected so far
-on composition, and it highlights the compositions of methods that are _pareto-
-optimal_ - that provide the **best possible tradeoffs between training time or
-cost and the quality of the trained model**. Whether you want to reach the same
-quality faster or get better quality within your current budget, Explorer can
-help you decide which speedup methods to use. We update this data regularly as
-we add new methods and develop better recipes.
+recipes and research on the science behind composition.
 [https://storage.googleapis.com/docs.mosaicml.com/images/methods/explorer.png]
 As an example, here are two performant recipes, one for ResNet-101 on ImageNet,
 and the other for GPT-2 on OpenWebText, on 8xA100s: ### ResNet-101
 Name|Functional|tl;dr|Benchmark|Speed Up ----|----------|-----|---------|------
 -- [Blur Pool](https://github.com/mosaicml/composer/tree/dev/composer/
 algorithms/blurpool)|`cf.apply_blurpool`|[Applies an anti-aliasing filter
 before every downsampling operation.](https://arxiv.org/abs/1904.11486)|ResNet-
```

### Comparing `composer-0.14.0/README.md` & `composer-0.14.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -189,17 +189,14 @@
 ## 🛠 Building Speedup Recipes
 
 Given two methods that speed up training by 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not necessarily.
 They may optimize the [same part of the training process](https://en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they may even interact in ways that prove detrimental.
 Determining which methods to compose together isn't as simple as assembling a set of methods that perform best individually.
 
 **We have come up with compositions of methods that work especially well together** through rigorous exploration of the design space of recipes and research on the science behind composition.
-The [MosaicML Explorer](https://app.mosaicml.com/) contains all of the data we have collected so far on composition, and it highlights the compositions of methods that are _pareto-optimal_ - that provide the **best possible tradeoffs between training time or cost and the quality of the trained model**.
-Whether you want to reach the same quality faster or get better quality within your current budget, Explorer can help you decide which speedup methods to use.
-We update this data regularly as we add new methods and develop better recipes.
 
 <p align="center">
 <img src="https://storage.googleapis.com/docs.mosaicml.com/images/methods/explorer.png"/>
 </p>
 
 As an example, here are two performant recipes, one for ResNet-101 on ImageNet, and the other for GPT-2 on OpenWebText, on 8xA100s:
```

#### html2text {}

```diff
@@ -114,22 +114,15 @@
 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not
 necessarily. They may optimize the [same part of the training process](https://
 en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they
 may even interact in ways that prove detrimental. Determining which methods to
 compose together isn't as simple as assembling a set of methods that perform
 best individually. **We have come up with compositions of methods that work
 especially well together** through rigorous exploration of the design space of
-recipes and research on the science behind composition. The [MosaicML Explorer]
-(https://app.mosaicml.com/) contains all of the data we have collected so far
-on composition, and it highlights the compositions of methods that are _pareto-
-optimal_ - that provide the **best possible tradeoffs between training time or
-cost and the quality of the trained model**. Whether you want to reach the same
-quality faster or get better quality within your current budget, Explorer can
-help you decide which speedup methods to use. We update this data regularly as
-we add new methods and develop better recipes.
+recipes and research on the science behind composition.
 [https://storage.googleapis.com/docs.mosaicml.com/images/methods/explorer.png]
 As an example, here are two performant recipes, one for ResNet-101 on ImageNet,
 and the other for GPT-2 on OpenWebText, on 8xA100s: ### ResNet-101
 Name|Functional|tl;dr|Benchmark|Speed Up ----|----------|-----|---------|------
 -- [Blur Pool](https://github.com/mosaicml/composer/tree/dev/composer/
 algorithms/blurpool)|`cf.apply_blurpool`|[Applies an anti-aliasing filter
 before every downsampling operation.](https://arxiv.org/abs/1904.11486)|ResNet-
```

### Comparing `composer-0.14.0/composer/__init__.py` & `composer-0.14.1/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/__init__.py` & `composer-0.14.1/composer/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/alibi/__init__.py` & `composer-0.14.1/composer/algorithms/alibi/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/alibi/alibi.py` & `composer-0.14.1/composer/algorithms/alibi/alibi.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/__init__.py` & `composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/_bert.py` & `composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/_bert.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py` & `composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/alibi/attention_surgery_functions/utils.py` & `composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/augmix/__init__.py` & `composer-0.14.1/composer/algorithms/augmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/augmix/augmix.py` & `composer-0.14.1/composer/algorithms/augmix/augmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/blurpool/__init__.py` & `composer-0.14.1/composer/algorithms/blurpool/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/blurpool/blurpool.py` & `composer-0.14.1/composer/algorithms/blurpool/blurpool.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/blurpool/blurpool_layers.py` & `composer-0.14.1/composer/algorithms/blurpool/blurpool_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/channels_last/__init__.py` & `composer-0.14.1/composer/algorithms/channels_last/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/channels_last/channels_last.py` & `composer-0.14.1/composer/algorithms/channels_last/channels_last.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/channels_last/metadata.json` & `composer-0.14.1/composer/algorithms/channels_last/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/colout/__init__.py` & `composer-0.14.1/composer/algorithms/colout/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/colout/colout.py` & `composer-0.14.1/composer/algorithms/colout/colout.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/cutmix/__init__.py` & `composer-0.14.1/composer/algorithms/cutmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/cutmix/cutmix.py` & `composer-0.14.1/composer/algorithms/cutmix/cutmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/cutmix/metadata.json` & `composer-0.14.1/composer/algorithms/cutmix/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/cutout/cutout.py` & `composer-0.14.1/composer/algorithms/cutout/cutout.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/ema/ema.py` & `composer-0.14.1/composer/algorithms/ema/ema.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/factorize/__init__.py` & `composer-0.14.1/composer/algorithms/factorize/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/factorize/factorize.py` & `composer-0.14.1/composer/algorithms/factorize/factorize.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/factorize/factorize_core.py` & `composer-0.14.1/composer/algorithms/factorize/factorize_core.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/factorize/factorize_modules.py` & `composer-0.14.1/composer/algorithms/factorize/factorize_modules.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/fused_layernorm/__init__.py` & `composer-0.14.1/composer/algorithms/fused_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/fused_layernorm/fused_layernorm.py` & `composer-0.14.1/composer/algorithms/fused_layernorm/fused_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/fused_layernorm/metadata.json` & `composer-0.14.1/composer/algorithms/fused_layernorm/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/gated_linear_units/__init__.py` & `composer-0.14.1/composer/algorithms/gated_linear_units/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py` & `composer-0.14.1/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/gated_linear_units/gated_linear_units.py` & `composer-0.14.1/composer/algorithms/gated_linear_units/gated_linear_units.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/gated_linear_units/metadata.json` & `composer-0.14.1/composer/algorithms/gated_linear_units/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/ghost_batchnorm/__init__.py` & `composer-0.14.1/composer/algorithms/ghost_batchnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py` & `composer-0.14.1/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/ghost_batchnorm/metadata.json` & `composer-0.14.1/composer/algorithms/ghost_batchnorm/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/gradient_clipping/gradient_clipping.py` & `composer-0.14.1/composer/algorithms/gradient_clipping/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/gradient_clipping/metadata.json` & `composer-0.14.1/composer/algorithms/gradient_clipping/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/gyro_dropout/gyro_dropout.py` & `composer-0.14.1/composer/algorithms/gyro_dropout/gyro_dropout.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/label_smoothing/__init__.py` & `composer-0.14.1/composer/algorithms/label_smoothing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/label_smoothing/label_smoothing.py` & `composer-0.14.1/composer/algorithms/label_smoothing/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/label_smoothing/metadata.json` & `composer-0.14.1/composer/algorithms/label_smoothing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/layer_freezing/layer_freezing.py` & `composer-0.14.1/composer/algorithms/layer_freezing/layer_freezing.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/layer_freezing/metadata.json` & `composer-0.14.1/composer/algorithms/layer_freezing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/low_precision_groupnorm/__init__.py` & `composer-0.14.1/composer/algorithms/low_precision_groupnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py` & `composer-0.14.1/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/low_precision_layernorm/__init__.py` & `composer-0.14.1/composer/algorithms/low_precision_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py` & `composer-0.14.1/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/mixup/metadata.json` & `composer-0.14.1/composer/algorithms/mixup/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/mixup/mixup.py` & `composer-0.14.1/composer/algorithms/mixup/mixup.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/no_op_model/__init__.py` & `composer-0.14.1/composer/algorithms/no_op_model/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/no_op_model/no_op_model.py` & `composer-0.14.1/composer/algorithms/no_op_model/no_op_model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/progressive_resizing/__init__.py` & `composer-0.14.1/composer/algorithms/progressive_resizing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/progressive_resizing/metadata.json` & `composer-0.14.1/composer/algorithms/progressive_resizing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/progressive_resizing/progressive_resizing.py` & `composer-0.14.1/composer/algorithms/progressive_resizing/progressive_resizing.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/randaugment/metadata.json` & `composer-0.14.1/composer/algorithms/randaugment/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/randaugment/randaugment.py` & `composer-0.14.1/composer/algorithms/randaugment/randaugment.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/sam/__init__.py` & `composer-0.14.1/composer/algorithms/sam/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/sam/sam.py` & `composer-0.14.1/composer/algorithms/sam/sam.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/selective_backprop/__init__.py` & `composer-0.14.1/composer/algorithms/selective_backprop/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/selective_backprop/metadata.json` & `composer-0.14.1/composer/algorithms/selective_backprop/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/selective_backprop/selective_backprop.py` & `composer-0.14.1/composer/algorithms/selective_backprop/selective_backprop.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/seq_length_warmup/metadata.json` & `composer-0.14.1/composer/algorithms/seq_length_warmup/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/seq_length_warmup/seq_length_warmup.py` & `composer-0.14.1/composer/algorithms/seq_length_warmup/seq_length_warmup.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/squeeze_excite/__init__.py` & `composer-0.14.1/composer/algorithms/squeeze_excite/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/squeeze_excite/squeeze_excite.py` & `composer-0.14.1/composer/algorithms/squeeze_excite/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/stochastic_depth/__init__.py` & `composer-0.14.1/composer/algorithms/stochastic_depth/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/stochastic_depth/metadata.json` & `composer-0.14.1/composer/algorithms/stochastic_depth/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/stochastic_depth/stochastic_depth.py` & `composer-0.14.1/composer/algorithms/stochastic_depth/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/stochastic_depth/stochastic_layers.py` & `composer-0.14.1/composer/algorithms/stochastic_depth/stochastic_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/swa/swa.py` & `composer-0.14.1/composer/algorithms/swa/swa.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/utils/augmentation_common.py` & `composer-0.14.1/composer/algorithms/utils/augmentation_common.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/utils/augmentation_primitives.py` & `composer-0.14.1/composer/algorithms/utils/augmentation_primitives.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/warnings.py` & `composer-0.14.1/composer/algorithms/warnings.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/weight_standardization/metadata.json` & `composer-0.14.1/composer/algorithms/weight_standardization/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/algorithms/weight_standardization/weight_standardization.py` & `composer-0.14.1/composer/algorithms/weight_standardization/weight_standardization.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/__init__.py` & `composer-0.14.1/composer/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/activation_monitor.py` & `composer-0.14.1/composer/callbacks/activation_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/checkpoint_saver.py` & `composer-0.14.1/composer/callbacks/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/early_stopper.py` & `composer-0.14.1/composer/callbacks/early_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/export_for_inference.py` & `composer-0.14.1/composer/callbacks/export_for_inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/health_checker.py` & `composer-0.14.1/composer/callbacks/health_checker.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/image_visualizer.py` & `composer-0.14.1/composer/callbacks/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/lr_monitor.py` & `composer-0.14.1/composer/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/memory_monitor.py` & `composer-0.14.1/composer/callbacks/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/mlperf.py` & `composer-0.14.1/composer/callbacks/mlperf.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/optimizer_monitor.py` & `composer-0.14.1/composer/callbacks/optimizer_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/runtime_estimator.py` & `composer-0.14.1/composer/callbacks/runtime_estimator.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/speed_monitor.py` & `composer-0.14.1/composer/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/callbacks/threshold_stopper.py` & `composer-0.14.1/composer/callbacks/threshold_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/cli/launcher.py` & `composer-0.14.1/composer/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/__init__.py` & `composer-0.14.1/composer/core/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/algorithm.py` & `composer-0.14.1/composer/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/callback.py` & `composer-0.14.1/composer/core/callback.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/data_spec.py` & `composer-0.14.1/composer/core/data_spec.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/engine.py` & `composer-0.14.1/composer/core/engine.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/evaluator.py` & `composer-0.14.1/composer/core/evaluator.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/event.py` & `composer-0.14.1/composer/core/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                     loss = model.loss(outputs, batch)
                     # <AFTER_LOSS>
 
                     # <BEFORE_BACKWARD>
                     loss.backward()
                     # <AFTER_BACKWARD>
 
-                # Un-scale and clip gradients
+                # Un-scale gradients
 
                 # <AFTER_TRAIN_BATCH>
                 optimizer.step()
 
                 # <BATCH_END>
 
                 if should_eval(batch=True):
```

### Comparing `composer-0.14.0/composer/core/passes.py` & `composer-0.14.1/composer/core/passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/precision.py` & `composer-0.14.1/composer/core/precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/serializable.py` & `composer-0.14.1/composer/core/serializable.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/state.py` & `composer-0.14.1/composer/core/state.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/time.py` & `composer-0.14.1/composer/core/time.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/core/types.py` & `composer-0.14.1/composer/core/types.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/__init__.py` & `composer-0.14.1/composer/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/ade20k.py` & `composer-0.14.1/composer/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/brats.py` & `composer-0.14.1/composer/datasets/brats.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/c4.py` & `composer-0.14.1/composer/datasets/c4.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/cifar.py` & `composer-0.14.1/composer/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/ffcv_utils.py` & `composer-0.14.1/composer/datasets/ffcv_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/imagenet.py` & `composer-0.14.1/composer/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/in_context_learning_evaluation.py` & `composer-0.14.1/composer/datasets/in_context_learning_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -720,16 +720,15 @@
                 encoded_example['preamble']['input_ids'] = encoded_example['preamble']['input_ids'][:-1]
 
             encoded_example['gold_idx'] = gold_idx
             encoded_example['context_options'] = [self.tokenizer(c, add_special_tokens=False) for c in context_options]
 
             if self.prefix_space:
                 continuation = f' {continuation}' if not continuation.startswith(' ') else continuation
-            encoded_example['continuation'] = self.tokenizer(
-                f' {continuation}' if not continuation.startswith(' ') else continuation, add_special_tokens=False)
+            encoded_example['continuation'] = self.tokenizer(continuation, add_special_tokens=False)
             examples.append(encoded_example)
 
         return examples
 
     def collate_fn(self, data):
         inputs = []
         continuation_indices = []
```

### Comparing `composer-0.14.0/composer/datasets/lm_dataset.py` & `composer-0.14.1/composer/datasets/lm_dataset.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/mnist.py` & `composer-0.14.1/composer/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/synthetic.py` & `composer-0.14.1/composer/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/datasets/utils.py` & `composer-0.14.1/composer/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/devices/device.py` & `composer-0.14.1/composer/devices/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/devices/device_cpu.py` & `composer-0.14.1/composer/devices/device_cpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/devices/device_gpu.py` & `composer-0.14.1/composer/devices/device_gpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/devices/device_mps.py` & `composer-0.14.1/composer/devices/device_mps.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/devices/device_tpu.py` & `composer-0.14.1/composer/devices/device_tpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/functional/__init__.py` & `composer-0.14.1/composer/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/__init__.py` & `composer-0.14.1/composer/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/cometml_logger.py` & `composer-0.14.1/composer/loggers/cometml_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/console_logger.py` & `composer-0.14.1/composer/loggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/file_logger.py` & `composer-0.14.1/composer/loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/in_memory_logger.py` & `composer-0.14.1/composer/loggers/in_memory_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/logger.py` & `composer-0.14.1/composer/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/logger_destination.py` & `composer-0.14.1/composer/loggers/logger_destination.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/mlflow_logger.py` & `composer-0.14.1/composer/loggers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/mosaicml_logger.py` & `composer-0.14.1/composer/loggers/mosaicml_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/progress_bar_logger.py` & `composer-0.14.1/composer/loggers/progress_bar_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/remote_uploader_downloader.py` & `composer-0.14.1/composer/loggers/remote_uploader_downloader.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/slack_logger.py` & `composer-0.14.1/composer/loggers/slack_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/tensorboard_logger.py` & `composer-0.14.1/composer/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loggers/wandb_logger.py` & `composer-0.14.1/composer/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loss/loss.py` & `composer-0.14.1/composer/loss/loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/loss/utils.py` & `composer-0.14.1/composer/loss/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/metrics/__init__.py` & `composer-0.14.1/composer/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/metrics/map.py` & `composer-0.14.1/composer/metrics/map.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/metrics/metrics.py` & `composer-0.14.1/composer/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/metrics/nlp.py` & `composer-0.14.1/composer/metrics/nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/__init__.py` & `composer-0.14.1/composer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/base.py` & `composer-0.14.1/composer/models/base.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/bert/model.py` & `composer-0.14.1/composer/models/bert/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/classify_mnist/model.py` & `composer-0.14.1/composer/models/classify_mnist/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/deeplabv3/model.py` & `composer-0.14.1/composer/models/deeplabv3/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/efficientnetb0/__init__.py` & `composer-0.14.1/composer/models/efficientnetb0/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/efficientnetb0/_layers.py` & `composer-0.14.1/composer/models/efficientnetb0/_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/efficientnetb0/efficientnets.py` & `composer-0.14.1/composer/models/efficientnetb0/efficientnets.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/efficientnetb0/model.py` & `composer-0.14.1/composer/models/efficientnetb0/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/gpt2/__init__.py` & `composer-0.14.1/composer/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/gpt2/model.py` & `composer-0.14.1/composer/models/gpt2/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/huggingface.py` & `composer-0.14.1/composer/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/initializers.py` & `composer-0.14.1/composer/models/initializers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/mmdetection.py` & `composer-0.14.1/composer/models/mmdetection.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/resnet/__init__.py` & `composer-0.14.1/composer/models/resnet/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/resnet/model.py` & `composer-0.14.1/composer/models/resnet/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/resnet_cifar/__init__.py` & `composer-0.14.1/composer/models/resnet_cifar/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/resnet_cifar/model.py` & `composer-0.14.1/composer/models/resnet_cifar/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/resnet_cifar/resnets.py` & `composer-0.14.1/composer/models/resnet_cifar/resnets.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/tasks/classification.py` & `composer-0.14.1/composer/models/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/timm/model.py` & `composer-0.14.1/composer/models/timm/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/unet/_layers.py` & `composer-0.14.1/composer/models/unet/_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/unet/model.py` & `composer-0.14.1/composer/models/unet/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/unet/unet.py` & `composer-0.14.1/composer/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/models/vit_small_patch16/model.py` & `composer-0.14.1/composer/models/vit_small_patch16/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/optim/__init__.py` & `composer-0.14.1/composer/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/optim/decoupled_weight_decay.py` & `composer-0.14.1/composer/optim/decoupled_weight_decay.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/optim/scheduler.py` & `composer-0.14.1/composer/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/__init__.py` & `composer-0.14.1/composer/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/json_trace_handler.py` & `composer-0.14.1/composer/profiler/json_trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/json_trace_merger.py` & `composer-0.14.1/composer/profiler/json_trace_merger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/marker.py` & `composer-0.14.1/composer/profiler/marker.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/profiler.py` & `composer-0.14.1/composer/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/profiler_action.py` & `composer-0.14.1/composer/profiler/profiler_action.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/profiler_schedule.py` & `composer-0.14.1/composer/profiler/profiler_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/system_profiler.py` & `composer-0.14.1/composer/profiler/system_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/torch_profiler.py` & `composer-0.14.1/composer/profiler/torch_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/profiler/trace_handler.py` & `composer-0.14.1/composer/profiler/trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/trainer/_deepspeed.py` & `composer-0.14.1/composer/trainer/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/trainer/_scale_schedule.py` & `composer-0.14.1/composer/trainer/_scale_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/trainer/_scaler.py` & `composer-0.14.1/composer/trainer/_scaler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/trainer/dist_strategy.py` & `composer-0.14.1/composer/trainer/dist_strategy.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/trainer/meta_safe_apply.py` & `composer-0.14.1/composer/trainer/meta_safe_apply.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/trainer/mosaic_fsdp.py` & `composer-0.14.1/composer/trainer/mosaic_fsdp.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/trainer/trainer.py` & `composer-0.14.1/composer/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/__init__.py` & `composer-0.14.1/composer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/auto_log_hparams.py` & `composer-0.14.1/composer/utils/auto_log_hparams.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/batch_helpers.py` & `composer-0.14.1/composer/utils/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/checkpoint.py` & `composer-0.14.1/composer/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/collect_env.py` & `composer-0.14.1/composer/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/device.py` & `composer-0.14.1/composer/utils/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/dist.py` & `composer-0.14.1/composer/utils/dist.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/file_helpers.py` & `composer-0.14.1/composer/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/fx_utils.py` & `composer-0.14.1/composer/utils/fx_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/import_helpers.py` & `composer-0.14.1/composer/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/inference.py` & `composer-0.14.1/composer/utils/inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/iter_helpers.py` & `composer-0.14.1/composer/utils/iter_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/misc.py` & `composer-0.14.1/composer/utils/misc.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/module_surgery.py` & `composer-0.14.1/composer/utils/module_surgery.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/object_store/__init__.py` & `composer-0.14.1/composer/utils/object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/object_store/libcloud_object_store.py` & `composer-0.14.1/composer/utils/object_store/libcloud_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/object_store/object_store.py` & `composer-0.14.1/composer/utils/object_store/object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/object_store/oci_object_store.py` & `composer-0.14.1/composer/utils/object_store/oci_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/object_store/s3_object_store.py` & `composer-0.14.1/composer/utils/object_store/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/object_store/sftp_object_store.py` & `composer-0.14.1/composer/utils/object_store/sftp_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/reproducibility.py` & `composer-0.14.1/composer/utils/reproducibility.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/retrying.py` & `composer-0.14.1/composer/utils/retrying.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer/utils/string_enum.py` & `composer-0.14.1/composer/utils/string_enum.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer.egg-info/PKG-INFO` & `composer-0.14.1/composer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.14.0
+Version: 0.14.1
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -218,17 +218,14 @@
 ## 🛠 Building Speedup Recipes
 
 Given two methods that speed up training by 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not necessarily.
 They may optimize the [same part of the training process](https://en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they may even interact in ways that prove detrimental.
 Determining which methods to compose together isn't as simple as assembling a set of methods that perform best individually.
 
 **We have come up with compositions of methods that work especially well together** through rigorous exploration of the design space of recipes and research on the science behind composition.
-The [MosaicML Explorer](https://app.mosaicml.com/) contains all of the data we have collected so far on composition, and it highlights the compositions of methods that are _pareto-optimal_ - that provide the **best possible tradeoffs between training time or cost and the quality of the trained model**.
-Whether you want to reach the same quality faster or get better quality within your current budget, Explorer can help you decide which speedup methods to use.
-We update this data regularly as we add new methods and develop better recipes.
 
 <p align="center">
 <img src="https://storage.googleapis.com/docs.mosaicml.com/images/methods/explorer.png"/>
 </p>
 
 As an example, here are two performant recipes, one for ResNet-101 on ImageNet, and the other for GPT-2 on OpenWebText, on 8xA100s:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: composer Version: 0.14.0 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.14.1 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
@@ -125,22 +125,15 @@
 1.5x each, do they combine to provide a 2.25x (1.5x * 1.5x) speedup? Not
 necessarily. They may optimize the [same part of the training process](https://
 en.wikipedia.org/wiki/Amdahl's_law) and lead to diminishing returns, or they
 may even interact in ways that prove detrimental. Determining which methods to
 compose together isn't as simple as assembling a set of methods that perform
 best individually. **We have come up with compositions of methods that work
 especially well together** through rigorous exploration of the design space of
-recipes and research on the science behind composition. The [MosaicML Explorer]
-(https://app.mosaicml.com/) contains all of the data we have collected so far
-on composition, and it highlights the compositions of methods that are _pareto-
-optimal_ - that provide the **best possible tradeoffs between training time or
-cost and the quality of the trained model**. Whether you want to reach the same
-quality faster or get better quality within your current budget, Explorer can
-help you decide which speedup methods to use. We update this data regularly as
-we add new methods and develop better recipes.
+recipes and research on the science behind composition.
 [https://storage.googleapis.com/docs.mosaicml.com/images/methods/explorer.png]
 As an example, here are two performant recipes, one for ResNet-101 on ImageNet,
 and the other for GPT-2 on OpenWebText, on 8xA100s: ### ResNet-101
 Name|Functional|tl;dr|Benchmark|Speed Up ----|----------|-----|---------|------
 -- [Blur Pool](https://github.com/mosaicml/composer/tree/dev/composer/
 algorithms/blurpool)|`cf.apply_blurpool`|[Applies an anti-aliasing filter
 before every downsampling operation.](https://arxiv.org/abs/1904.11486)|ResNet-
```

### Comparing `composer-0.14.0/composer.egg-info/SOURCES.txt` & `composer-0.14.1/composer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/composer.egg-info/requires.txt` & `composer-0.14.1/composer.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,74 +10,75 @@
 coolname<3,>=1.1.0
 tabulate==0.9.0
 py-cpuinfo<10,>=8.0.0
 packaging<23,>=21.3.0
 importlib-metadata<7,>=5.0.0
 
 [all]
-fasteners==0.18
-jupyter==1.0.0
-myst-parser==0.16.1
-timm<0.6,>=0.5.4
-sphinxext.opengraph==0.8.2
-mosaicml-streaming<1.0
-pycocotools<3,>=2.0.4
-mlflow<3.0,>=2.0.1
-sphinx==4.4.0
-yamllint==1.31.0
-mock-ssh-server==0.9.1
-sphinx_markdown_tables==0.0.17
-deepspeed==0.8.3
-junitparser==3.0.0
-sphinx-argparse==0.4.0
+ipython==8.11.0
 paramiko<3,>=2.11.0
-recommonmark==0.7.1
-comet_ml<4.0.0,>=3.31.12
-monai<1.2,>=0.9.1
-slack_sdk<4,>=3.19.5
-toml==0.10.2
-vit_pytorch==0.35.8
-onnxruntime<2,>=1.12.1
-sphinx-copybutton==0.5.2
+timm<0.6,>=0.5.4
+sphinxcontrib-images==0.9.4
 sentencepiece==0.1.98
-oci<3.0.0,>=2.88.2
-traitlets==5.9.0
-pytest-httpserver<1.1,>=1.0.4
-datasets<3,>=2.4
-mosaicml-cli<0.4,>=0.3.6
-tensorboard<3.0.0,>=2.9.1
-pynvml<12,>=11.5.0
+recommonmark==0.7.1
+deepspeed==0.8.3
+testbook==0.4.2
+pycocotools<3,>=2.0.4
+boto3<2,>=1.21.45
 transformers<4.29,>=4.11
 pypandoc==1.11
-boto3<2,>=1.21.45
-ipykernel==6.22.0
-onnx<2,>=1.12.0
+junitparser==3.0.0
+docutils==0.17.1
+traitlets==5.9.0
 pre-commit<3,>=2.18.1
-sphinx_panels==0.6.0
-sphinxemoji==0.2.0
+mock-ssh-server==0.9.1
+mosaicml-cli<0.4,>=0.3.6
 furo==2022.9.29
-pytest==7.3.1
-apache-libcloud<4,>=3.3.1
-cryptography==38.0.4
-custom_inherit==2.4.1
+vit_pytorch==0.35.8
+sphinxext.opengraph==0.8.2
 setuptools<=59.5.0
-wandb<0.16,>=0.13.2
 sphinxcontrib.katex==0.9.4
-docutils==0.17.1
+sphinx-argparse==0.4.0
+onnxruntime<2,>=1.12.1
+nbsphinx==0.9.1
+cryptography==38.0.4
+datasets<3,>=2.4
 GitPython==3.1.31
-sphinxcontrib-images==0.9.4
+jupyter==1.0.0
+wandb<0.16,>=0.13.2
+custom_inherit==2.4.1
+mlflow<3.0,>=2.0.1
+sphinx_markdown_tables==0.0.17
+mosaicml-streaming<1.0
+oci<3.0.0,>=2.88.2
+slack_sdk<4,>=3.19.5
+myst-parser==0.16.1
+pandoc==2.3
+pytest==7.3.1
+pytest-httpserver<1.1,>=1.0.4
+sphinx==4.4.0
+monai<1.2,>=0.9.1
+moto[s3]<5,>=4.0.1
+protobuf<3.21
+py-cpuinfo<10,>=8.0.0
 coverage[toml]==7.2.5
-testbook==0.4.2
+onnx<2,>=1.12.0
 pytest_codeblocks==0.16.1
-nbsphinx==0.9.1
-pandoc==2.3
+pynvml<12,>=11.5.0
+comet_ml<4.0.0,>=3.31.12
+ipykernel==6.22.0
+sphinx_panels==0.6.0
 scikit-learn<2,>=1.0.1
-py-cpuinfo<10,>=8.0.0
-moto[s3]<5,>=4.0.1
-ipython==8.11.0
+apache-libcloud<4,>=3.3.1
+yamllint==1.31.0
+tensorboard<3.0.0,>=2.9.1
+sphinx-copybutton==0.5.2
+fasteners==0.18
+toml==0.10.2
+sphinxemoji==0.2.0
 
 [base]
 
 [coco]
 pycocotools<3,>=2.0.4
 
 [comet_ml]
@@ -147,14 +148,15 @@
 oci<3.0.0,>=2.88.2
 
 [onnx]
 onnx<2,>=1.12.0
 onnxruntime<2,>=1.12.1
 
 [sentencepiece]
+protobuf<3.21
 sentencepiece==0.1.98
 
 [slack]
 slack_sdk<4,>=3.19.5
 
 [streaming]
 mosaicml-streaming<1.0
```

### Comparing `composer-0.14.0/pyproject.toml` & `composer-0.14.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/setup.py` & `composer-0.14.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,18 @@
 ]
 
 extra_deps['nlp'] = [
     'transformers>=4.11,<4.29',
     'datasets>=2.4,<3',
 ]
 
-extra_deps['sentencepiece'] = ['sentencepiece==0.1.98']
+extra_deps['sentencepiece'] = [
+    'protobuf<3.21',
+    'sentencepiece==0.1.98',
+]
 
 extra_deps['mlperf'] = [
     # TODO: use pip when available: https://github.com/mlcommons/logging/issues/218
     # "mlperf_logging @ git+https://github.com/mlperf/logging.git",
     'py-cpuinfo>=8.0.0,<10',
 ]
```

### Comparing `composer-0.14.0/tests/test_device.py` & `composer-0.14.1/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_docker.py` & `composer-0.14.1/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_docs.py` & `composer-0.14.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_engine.py` & `composer-0.14.1/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_events.py` & `composer-0.14.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_full_nlp.py` & `composer-0.14.1/tests/test_full_nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_loss.py` & `composer-0.14.1/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_notebooks.py` & `composer-0.14.1/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_passes.py` & `composer-0.14.1/tests/test_passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_precision.py` & `composer-0.14.1/tests/test_precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_simple_nlp.py` & `composer-0.14.1/tests/test_simple_nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_smoketest.py` & `composer-0.14.1/tests/test_smoketest.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_split_batch.py` & `composer-0.14.1/tests/test_split_batch.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_state.py` & `composer-0.14.1/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.0/tests/test_time.py` & `composer-0.14.1/tests/test_time.py`

 * *Files identical despite different names*

