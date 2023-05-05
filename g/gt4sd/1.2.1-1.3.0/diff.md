# Comparing `tmp/gt4sd-1.2.1.tar.gz` & `tmp/gt4sd-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gt4sd-1.2.1.tar", last modified: Fri Apr 21 07:21:27 2023, max compression
+gzip compressed data, was "gt4sd-1.3.0.tar", last modified: Fri May  5 07:22:36 2023, max compression
```

## Comparing `gt4sd-1.2.1.tar` & `gt4sd-1.3.0.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.063640 gt4sd-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-21 07:21:14.000000 gt4sd-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-04-21 07:21:27.063640 gt4sd-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-04-21 07:21:14.000000 gt4sd-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-21 07:21:15.000000 gt4sd-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-21 07:21:27.067640 gt4sd-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 07:21:15.000000 gt4sd-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.019639 gt4sd-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.031639 gt4sd-1.2.1/src/gt4sd/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.031639 gt4sd-1.2.1/src/gt4sd/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.031639 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.031639 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29460 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.031639 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/
--rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.031639 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/key_bert/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/key_bert/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.031639 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/molgx/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/molgx/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.031639 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    51522 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/template/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/template/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/template/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.035640 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    34978 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/hugging_face/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/hugging_face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/hugging_face/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/hugging_face/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/moler/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/moler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/moler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/moler/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/paccmann_vae/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/paccmann_vae/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/pgt/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/pgt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/pgt/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/pgt/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.039640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/polymer_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/polymer_blocks/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   128648 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/mol_dct.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_moler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_pgt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_torchdrug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/algorithms/generation/torchdrug/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/torchdrug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/torchdrug/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/generation/torchdrug/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/paccmann/
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/paccmann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/paccmann/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/paccmann/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/tests/test_paccmann.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/topics_zero_shot/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/algorithms/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/cli/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/cli/argument_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4380 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/cli/hf_to_st_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6910 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/cli/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/cli/load_arguments_from_dataclass.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7893 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/cli/saving.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/cli/trainer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8169 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/cli/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/domains/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/domains/materials/
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/domains/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/domains/materials/protein_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/domains/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/domains/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.043640 gt4sd-1.2.1/src/gt4sd/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/cgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/cgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15695 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/cgcnn/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/cgcnn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/crystals_rfc/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/crystals_rfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32266 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/crystals_rfc/feature_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/tests/test_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/arg_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/arg_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/arg_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/dataloader/data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/dataloader/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/dataloader/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/loss/td_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.047640 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34044 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/tests/qm9.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/tests/test_gfn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/train/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/train/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/arg_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/arg_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/arg_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/arg_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/dataloader/data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/dataloader/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/dataloader/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    35475 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.051640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/tests/test_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/frameworks/granular/train/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/granular/train/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/frameworks/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/frameworks/torch/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/properties/crystals/
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/crystals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/crystals/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/properties/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30897 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/molecules/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/molecules/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/properties/proteins/
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/proteins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/proteins/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/proteins/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/properties/scores/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/scores/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/properties/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/tests/test_properties_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/properties/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.055640 gt4sd-1.2.1/src/gt4sd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/cgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/cgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/cgcnn/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/crystals_crf/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/crystals_crf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/crystals_crf/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/diffusion/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/mock_training_pipeline.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/organ/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/organ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/organ/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/vae/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/vae/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/vae/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/vae/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.059640 gt4sd-1.2.1/src/gt4sd/training_pipelines/regression_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/regression_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/regression_transformer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/regression_transformer/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/regression_transformer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/terminator_training.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.063640 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/molecules.smi
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_cgnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_gflownet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.063640 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.063640 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/gcpn/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.063640 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/graphaf/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-21 07:21:15.000000 gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/unpatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:21:27.031639 gt4sd-1.2.1/src/gt4sd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-04-21 07:21:26.000000 gt4sd-1.2.1/src/gt4sd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-04-21 07:21:27.000000 gt4sd-1.2.1/src/gt4sd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 07:21:26.000000 gt4sd-1.2.1/src/gt4sd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-21 07:21:26.000000 gt4sd-1.2.1/src/gt4sd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-21 07:21:26.000000 gt4sd-1.2.1/src/gt4sd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 07:21:26.000000 gt4sd-1.2.1/src/gt4sd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.549211 gt4sd-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 07:22:24.000000 gt4sd-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-05-05 07:22:36.549211 gt4sd-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-05-05 07:22:24.000000 gt4sd-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-05 07:22:24.000000 gt4sd-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-05 07:22:36.553211 gt4sd-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 07:22:24.000000 gt4sd-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.485212 gt4sd-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.509212 gt4sd-1.3.0/src/gt4sd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.513212 gt4sd-1.3.0/src/gt4sd/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.513212 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.513212 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29460 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.517212 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.517212 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/key_bert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/key_bert/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.517212 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/molgx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/molgx/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.517212 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.517212 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53178 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/template/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/template/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34978 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.521211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.525211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.525211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.525211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/hugging_face/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/hugging_face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/hugging_face/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/hugging_face/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.525211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/moler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/moler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/moler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/moler/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.525211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/paccmann_vae/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/paccmann_vae/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.525211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/pgt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/pgt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/pgt/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/pgt/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.525211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/polymer_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/polymer_blocks/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128648 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/mol_dct.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_moler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_pgt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_torchdrug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/algorithms/generation/torchdrug/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/torchdrug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/torchdrug/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/generation/torchdrug/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/paccmann/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/paccmann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/paccmann/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/paccmann/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/tests/test_paccmann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/topics_zero_shot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/algorithms/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/cli/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/cli/argument_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4380 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/cli/hf_to_st_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6910 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/cli/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/cli/load_arguments_from_dataclass.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7893 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/cli/saving.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/cli/trainer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8169 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/cli/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/domains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/domains/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/domains/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/domains/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/domains/materials/protein_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/domains/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/domains/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.529211 gt4sd-1.3.0/src/gt4sd/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/cgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/cgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15695 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/cgcnn/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/cgcnn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/crystals_rfc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/crystals_rfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32266 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/crystals_rfc/feature_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/tests/test_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/arg_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/arg_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/arg_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/dataloader/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/dataloader/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/dataloader/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/loss/td_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.533211 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34044 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/tests/qm9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/tests/test_gfn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/train/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/arg_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/arg_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/arg_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/arg_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/dataloader/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/dataloader/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/dataloader/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35475 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.537211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/frameworks/granular/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/granular/train/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/frameworks/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/frameworks/torch/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/properties/crystals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/crystals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/crystals/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/properties/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30897 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/molecules/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/molecules/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/properties/proteins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/proteins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/proteins/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/proteins/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/properties/scores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/scores/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/properties/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/tests/test_properties_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/properties/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.541211 gt4sd-1.3.0/src/gt4sd/training_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/cgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/cgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/cgcnn/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/crystals_crf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/crystals_crf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/crystals_crf/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/diffusion/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/mock_training_pipeline.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/organ/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/organ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/organ/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/vae/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/vae/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.545211 gt4sd-1.3.0/src/gt4sd/training_pipelines/regression_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/regression_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/regression_transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/regression_transformer/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/regression_transformer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/terminator_training.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.549211 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/molecules.smi
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_cgnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_gflownet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.549211 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.549211 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/gcpn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.549211 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/graphaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-05 07:22:24.000000 gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/unpatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:36.513212 gt4sd-1.3.0/src/gt4sd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-05-05 07:22:36.000000 gt4sd-1.3.0/src/gt4sd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-05-05 07:22:36.000000 gt4sd-1.3.0/src/gt4sd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:22:36.000000 gt4sd-1.3.0/src/gt4sd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-05 07:22:36.000000 gt4sd-1.3.0/src/gt4sd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 07:22:36.000000 gt4sd-1.3.0/src/gt4sd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 07:22:36.000000 gt4sd-1.3.0/src/gt4sd.egg-info/top_level.txt
```

### Comparing `gt4sd-1.2.1/LICENSE` & `gt4sd-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/PKG-INFO` & `gt4sd-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt4sd
-Version: 1.2.1
+Version: 1.3.0
 Summary: Generative Toolkit for Scientific Discovery (GT4SD).
 Author: GT4SD team
 Keywords: GT4SD Generative Models Inference Training
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gt4sd-1.2.1/README.md` & `gt4sd-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/setup.cfg` & `gt4sd-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/__init__.py` & `gt4sd-1.3.0/src/gt4sd/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Module initialization."""
 
-__version__ = "1.2.1"
+__version__ = "1.3.0"
 __name__ = "gt4sd"
 
 # NOTE: configure SSL to allow unverified contexts by default
 from .configuration import GT4SDConfiguration
 
 gt4sd_configuration_instance = GT4SDConfiguration.get_instance()
```

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/key_bert/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/key_bert/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/molgx/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/molgx/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,22 @@
                 data.get("property_ranges", {}).get(p, [0, 1])[0]
                 for p in self.properties
             ]
             self._maxs = [
                 data.get("property_ranges", {}).get(p, [0, 1])[1]
                 for p in self.properties
             ]
+            # In case custom normalization/denormalization is required
+            self.normalization_fns = [
+                data.get("normalization_fns", {}).get(p, None) for p in self.properties
+            ]
+            self.denormalization_fns = [
+                data.get("denormalization_fns", {}).get(p, None)
+                for p in self.properties
+            ]
             self.metadata = data
 
             # If tolerance dict is given, ensure it is well-formed
             self.tolerance_dict = {}
             if isinstance(self.tolerance, Dict):
                 # Check that no extra properties are given
                 for key in self.tolerance.keys():
@@ -207,22 +215,33 @@
             x: normalized value (often in [0,1]).
             idx: index of the property.
             precision: optional rounding precision. Defaults to 4.
 
         Returns:
             float: Value in regular scale.
         """
-
         # If the property was not normalized, return the value
         if not self.do_normalize[idx]:
             return x
 
-        return round(
-            x * (self._maxs[idx] - self._mins[idx]) + self._mins[idx], precision
-        )
+        # The default normalization reverts a linear transformation to [0,1] scale
+        if self.denormalization_fns[idx] is None:
+            return round(
+                x * (self._maxs[idx] - self._mins[idx]) + self._mins[idx], precision
+            )
+
+        # This allows to revert arbitrarily complex preprocessing functions
+        fn = self.denormalization_fns[idx]
+        try:
+            denormed = eval(fn)(x)
+            return round(denormed, precision)
+        except SyntaxError:
+            raise SyntaxError(
+                f"Custom denormalization function {fn} seems improperly formatted"
+            )
 
     def normalize(self, x: str, idx: int, precision: int = 3) -> float:
         """
         Normalize from original scale to desired scale.
 
         Args:
             x: unnormalized input.
@@ -233,21 +252,40 @@
             float: Normalized value.
         """
         # Error handling
         if not isinstance(x, float) and not self.isfloat(x):
             raise TypeError(f"{x} is not a float and cant safely be casted.")
 
         x_float = float(x)
+        if x_float < self._mins[idx] or x_float > self._maxs[idx]:
+            raise ValueError(
+                f"Property value {x_float} for {self.properties[idx]} is outside of "
+                f"model's range [{self._mins[idx]}, {self._maxs[idx]}]."
+            )
         # If this property does not require normalization, return it
         if not self.do_normalize[idx]:
             return x_float
-        normed = round(
-            (x_float - self._mins[idx]) / (self._maxs[idx] - self._mins[idx]), precision
-        )
-        return normed
+
+        # This performs a standard linear normalization to [0,1]
+        if self.normalization_fns[idx] is None:
+            normed = round(
+                (x_float - self._mins[idx]) / (self._maxs[idx] - self._mins[idx]),
+                precision,
+            )
+            return normed
+
+        # Allows to apply arbitrary preprocessing functions
+        fn = self.normalization_fns[idx]
+        try:
+            normed = eval(fn)(x_float)
+            return round(normed, precision)
+        except SyntaxError:
+            raise SyntaxError(
+                f"Custom normalization function {fn} seems improperly formatted"
+            )
 
     def validate_input(self, x: str) -> None:
         """
         Sanity checking for formatting of the input string.
 
         Args:
             x: The string to be validated.
```

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/template/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/template/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/template/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/template/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/template/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/diffusion/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/diffusion/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/hugging_face/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/hugging_face/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/hugging_face/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/hugging_face/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/hugging_face/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/moler/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/moler/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/moler/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/moler/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/moler/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/moler/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/paccmann_vae/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/paccmann_vae/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/pgt/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/pgt/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/pgt/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/pgt/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/pgt/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/pgt/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/polymer_blocks/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/polymer_blocks/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/mol_dct.pkl` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/mol_dct.pkl`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_diffusion.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_hugging_face.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_hugging_face.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_moler.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_moler.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_pgt.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_pgt.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/tests/test_torchdrug.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/tests/test_torchdrug.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/torchdrug/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/torchdrug/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/torchdrug/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/torchdrug/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/generation/torchdrug/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/generation/torchdrug/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/paccmann/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/paccmann/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/paccmann/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/paccmann/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/paccmann/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/paccmann/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/tests/test_paccmann.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/tests/test_paccmann.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/registry.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/registry.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/tests/test_config.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/algorithms/tests/test_registry.py` & `gt4sd-1.3.0/src/gt4sd/algorithms/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/cli/__init__.py` & `gt4sd-1.3.0/src/gt4sd/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/cli/algorithms.py` & `gt4sd-1.3.0/src/gt4sd/cli/algorithms.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/cli/argument_parser.py` & `gt4sd-1.3.0/src/gt4sd/cli/argument_parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/cli/hf_to_st_converter.py` & `gt4sd-1.3.0/src/gt4sd/cli/hf_to_st_converter.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/cli/inference.py` & `gt4sd-1.3.0/src/gt4sd/cli/inference.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/cli/load_arguments_from_dataclass.py` & `gt4sd-1.3.0/src/gt4sd/cli/load_arguments_from_dataclass.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/cli/saving.py` & `gt4sd-1.3.0/src/gt4sd/cli/saving.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/cli/trainer.py` & `gt4sd-1.3.0/src/gt4sd/cli/trainer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/cli/upload.py` & `gt4sd-1.3.0/src/gt4sd/cli/upload.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/configuration.py` & `gt4sd-1.3.0/src/gt4sd/configuration.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/conftest.py` & `gt4sd-1.3.0/src/gt4sd/conftest.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/domains/__init__.py` & `gt4sd-1.3.0/src/gt4sd/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/domains/core.py` & `gt4sd-1.3.0/src/gt4sd/domains/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/domains/materials/__init__.py` & `gt4sd-1.3.0/src/gt4sd/domains/materials/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/domains/materials/protein_encoding.py` & `gt4sd-1.3.0/src/gt4sd/domains/materials/protein_encoding.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/domains/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/domains/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/exceptions.py` & `gt4sd-1.3.0/src/gt4sd/exceptions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/extras/__init__.py` & `gt4sd-1.3.0/src/gt4sd/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/cgcnn/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/cgcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/cgcnn/data.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/cgcnn/data.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/cgcnn/model.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/cgcnn/model.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/crystals_rfc/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/crystals_rfc/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv` & `gt4sd-1.3.0/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/crystals_rfc/feature_engine.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/crystals_rfc/feature_engine.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/optimization.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/optimization.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/processing.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/processing.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/enzeptional/tests/test_processing.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/enzeptional/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/arg_parser/parser.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/arg_parser/parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/arg_parser/utils.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/arg_parser/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/dataloader/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/dataloader/data_module.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/dataloader/data_module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/dataloader/dataset.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/dataloader/sampler.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/dataloader/sampler.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/envs/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/loss/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/loss/td_loss.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/loss/td_loss.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/models/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/ml/module.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/ml/module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/tests/qm9.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/tests/qm9.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/tests/test_gfn.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/tests/test_gfn.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/train/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/train/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/train/core.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/train/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/gflownet/util.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/gflownet/util.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/arg_parser/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/arg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/arg_parser/parser.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/arg_parser/parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/arg_parser/utils.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/arg_parser/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/dataloader/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/dataloader/data_module.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/dataloader/data_module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/dataloader/dataset.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/dataloader/sampler.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/dataloader/sampler.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/activation.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/activation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/base_model.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/base_model.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/loss.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/loss.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/model_builder.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/model_builder.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/module.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/utils.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/ml/module.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/ml/module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/tests/test_tokenizer.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/tokenizer/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/train/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/train/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/granular/train/core.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/granular/train/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/torch/__init__.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/frameworks/torch/vae.py` & `gt4sd-1.3.0/src/gt4sd/frameworks/torch/vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/__init__.py` & `gt4sd-1.3.0/src/gt4sd/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/core.py` & `gt4sd-1.3.0/src/gt4sd/properties/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/crystals/__init__.py` & `gt4sd-1.3.0/src/gt4sd/properties/crystals/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/crystals/core.py` & `gt4sd-1.3.0/src/gt4sd/properties/crystals/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/molecules/__init__.py` & `gt4sd-1.3.0/src/gt4sd/properties/molecules/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/molecules/core.py` & `gt4sd-1.3.0/src/gt4sd/properties/molecules/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/molecules/functions.py` & `gt4sd-1.3.0/src/gt4sd/properties/molecules/functions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/proteins/__init__.py` & `gt4sd-1.3.0/src/gt4sd/properties/proteins/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/proteins/core.py` & `gt4sd-1.3.0/src/gt4sd/properties/proteins/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/proteins/functions.py` & `gt4sd-1.3.0/src/gt4sd/properties/proteins/functions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/scorer.py` & `gt4sd-1.3.0/src/gt4sd/properties/scorer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/scores/__init__.py` & `gt4sd-1.3.0/src/gt4sd/properties/scores/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/scores/core.py` & `gt4sd-1.3.0/src/gt4sd/properties/scores/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/properties/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/tests/test_properties.py` & `gt4sd-1.3.0/src/gt4sd/properties/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/tests/test_properties_scorer.py` & `gt4sd-1.3.0/src/gt4sd/properties/tests/test_properties_scorer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/properties/utils.py` & `gt4sd-1.3.0/src/gt4sd/properties/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/s3.py` & `gt4sd-1.3.0/src/gt4sd/s3.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/tests/test_configuration.py` & `gt4sd-1.3.0/src/gt4sd/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/tests/test_exceptions.py` & `gt4sd-1.3.0/src/gt4sd/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/tests/test_s3.py` & `gt4sd-1.3.0/src/gt4sd/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/tests/utils.py` & `gt4sd-1.3.0/src/gt4sd/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/cgcnn/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/cgcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/cgcnn/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/cgcnn/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/crystals_crf/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/crystals_crf/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/crystals_crf/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/crystals_crf/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/diffusion/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/diffusion/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/diffusion/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/organ/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/organ/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/organ/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/organ/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/vae/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/vae/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/moses/vae/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/moses/vae/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/vae/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/vae/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/paccmann/vae/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/paccmann/vae/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/regression_transformer/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/regression_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/regression_transformer/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/regression_transformer/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/regression_transformer/implementation.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/regression_transformer/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/regression_transformer/utils.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/regression_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/terminator_training.json` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/terminator_training.json`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/molecules.smi` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/molecules.smi`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_argument_parser.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_argument_parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_cgnn.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_cgnn.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_diffusion.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_diffusion.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_gflownet.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_gflownet.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_pipelines.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_pipelines.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/dataset.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/dataset.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd/training_pipelines/torchdrug/unpatch.py` & `gt4sd-1.3.0/src/gt4sd/training_pipelines/torchdrug/unpatch.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.2.1/src/gt4sd.egg-info/PKG-INFO` & `gt4sd-1.3.0/src/gt4sd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt4sd
-Version: 1.2.1
+Version: 1.3.0
 Summary: Generative Toolkit for Scientific Discovery (GT4SD).
 Author: GT4SD team
 Keywords: GT4SD Generative Models Inference Training
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gt4sd-1.2.1/src/gt4sd.egg-info/SOURCES.txt` & `gt4sd-1.3.0/src/gt4sd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

