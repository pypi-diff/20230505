# Comparing `tmp/UtilsRL-0.5.8.tar.gz` & `tmp/UtilsRL-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UtilsRL-0.5.8.tar", last modified: Fri May  5 12:14:40 2023, max compression
+gzip compressed data, was "UtilsRL-0.5.9.tar", last modified: Fri May  5 13:05:27 2023, max compression
```

## Comparing `UtilsRL-0.5.8.tar` & `UtilsRL-0.5.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.082095 UtilsRL-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-05 12:14:40.082095 UtilsRL-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.078095 UtilsRL-0.5.8/UtilsRL/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.078095 UtilsRL-0.5.8/UtilsRL/data_structure/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/data_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/data_structure/data_structure.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.078095 UtilsRL-0.5.8/UtilsRL/env/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.078095 UtilsRL-0.5.8/UtilsRL/env/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/env/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/env/wrapper/atari_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/env/wrapper/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/env/wrapper/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/env/wrapper/dmc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/env/wrapper/mujoco_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.078095 UtilsRL-0.5.8/UtilsRL/exp/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/exp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/exp/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/exp/_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/exp/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/exp/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/exp/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.078095 UtilsRL-0.5.8/UtilsRL/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/logger/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/logger/composite_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/logger/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/logger/text_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/logger/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.078095 UtilsRL-0.5.8/UtilsRL/math/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/math/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.082095 UtilsRL-0.5.8/UtilsRL/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/misc/chore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/misc/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/misc/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.082095 UtilsRL-0.5.8/UtilsRL/net/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/net/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/net/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/net/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/net/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/net/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.082095 UtilsRL-0.5.8/UtilsRL/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/plot/tb_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.082095 UtilsRL-0.5.8/UtilsRL/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30972 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.082095 UtilsRL-0.5.8/UtilsRL/rl/buffer/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/buffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/buffer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/buffer/prioritized_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/buffer/transition_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/buffer/trjectory_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/critic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/rl/video_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.082095 UtilsRL-0.5.8/UtilsRL/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/UtilsRL/third_party/tqdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:14:40.078095 UtilsRL-0.5.8/UtilsRL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-05 12:14:40.000000 UtilsRL-0.5.8/UtilsRL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-05 12:14:40.000000 UtilsRL-0.5.8/UtilsRL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:14:40.000000 UtilsRL-0.5.8/UtilsRL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 12:14:40.000000 UtilsRL-0.5.8/UtilsRL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 12:14:40.000000 UtilsRL-0.5.8/UtilsRL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:14:40.082095 UtilsRL-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-05 12:14:28.000000 UtilsRL-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.012443 UtilsRL-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-05 13:05:27.012443 UtilsRL-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.004443 UtilsRL-0.5.9/UtilsRL/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.004443 UtilsRL-0.5.9/UtilsRL/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/data_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/data_structure/data_structure.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.004443 UtilsRL-0.5.9/UtilsRL/env/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.008443 UtilsRL-0.5.9/UtilsRL/env/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/env/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/env/wrapper/atari_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/env/wrapper/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/env/wrapper/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/env/wrapper/dmc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/env/wrapper/mujoco_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.008443 UtilsRL-0.5.9/UtilsRL/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/exp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/exp/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/exp/_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/exp/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/exp/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/exp/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.008443 UtilsRL-0.5.9/UtilsRL/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/logger/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/logger/composite_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/logger/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/logger/text_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/logger/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.008443 UtilsRL-0.5.9/UtilsRL/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/math/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.008443 UtilsRL-0.5.9/UtilsRL/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/misc/chore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/misc/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/misc/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.012443 UtilsRL-0.5.9/UtilsRL/net/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/net/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/net/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/net/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/net/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/net/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.012443 UtilsRL-0.5.9/UtilsRL/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/plot/tb_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.012443 UtilsRL-0.5.9/UtilsRL/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30972 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.012443 UtilsRL-0.5.9/UtilsRL/rl/buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/buffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/buffer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/buffer/prioritized_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/buffer/transition_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/buffer/trjectory_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/rl/video_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.012443 UtilsRL-0.5.9/UtilsRL/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/UtilsRL/third_party/tqdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:27.004443 UtilsRL-0.5.9/UtilsRL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-05 13:05:26.000000 UtilsRL-0.5.9/UtilsRL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-05 13:05:27.000000 UtilsRL-0.5.9/UtilsRL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:05:26.000000 UtilsRL-0.5.9/UtilsRL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 13:05:26.000000 UtilsRL-0.5.9/UtilsRL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 13:05:26.000000 UtilsRL-0.5.9/UtilsRL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:05:27.016443 UtilsRL-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-05 13:05:16.000000 UtilsRL-0.5.9/setup.py
```

### Comparing `UtilsRL-0.5.8/LICENSE` & `UtilsRL-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/PKG-INFO` & `UtilsRL-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UtilsRL
-Version: 0.5.8
+Version: 0.5.9
 Summary: A python module desgined for RL logging, monitoring and experiments managing. 
 Home-page: https://github.com/typoverflow/UtilsRL
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `UtilsRL-0.5.8/README.md` & `UtilsRL-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/data_structure/data_structure.cc` & `UtilsRL-0.5.9/UtilsRL/data_structure/data_structure.cc`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/env/__init__.py` & `UtilsRL-0.5.9/UtilsRL/env/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         camera_id=0,
         frame_skip=1,
         episode_length=1000,
         environment_kwargs=None,
         time_limit=None,
         channels_first=True
 ):
-    env_id = '%s-%s-v1' % (domain_name, task_name, seed)
+    env_id = '%s-%s-v1' % (domain_name, task_name)
 
     if from_pixels:
         assert not visualize_reward, 'cannot use visualize reward when learning from pixels'
 
     # shorten episode length
     max_episode_steps = (episode_length + frame_skip - 1) // frame_skip
```

### Comparing `UtilsRL-0.5.8/UtilsRL/env/wrapper/atari_wrapper.py` & `UtilsRL-0.5.9/UtilsRL/env/wrapper/atari_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/env/wrapper/base_wrapper.py` & `UtilsRL-0.5.9/UtilsRL/env/wrapper/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/env/wrapper/compat.py` & `UtilsRL-0.5.9/UtilsRL/env/wrapper/compat.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/env/wrapper/dmc_wrapper.py` & `UtilsRL-0.5.9/UtilsRL/env/wrapper/dmc_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/env/wrapper/mujoco_wrapper.py` & `UtilsRL-0.5.9/UtilsRL/env/wrapper/mujoco_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/exp/__init__.py` & `UtilsRL-0.5.9/UtilsRL/exp/__init__.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/exp/_device.py` & `UtilsRL-0.5.9/UtilsRL/exp/_device.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/exp/argparse.py` & `UtilsRL-0.5.9/UtilsRL/exp/argparse.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/exp/precision.py` & `UtilsRL-0.5.9/UtilsRL/exp/precision.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/exp/snapshot.py` & `UtilsRL-0.5.9/UtilsRL/exp/snapshot.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/logger/base_logger.py` & `UtilsRL-0.5.9/UtilsRL/logger/base_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/logger/composite_logger.py` & `UtilsRL-0.5.9/UtilsRL/logger/composite_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/logger/tensorboard_logger.py` & `UtilsRL-0.5.9/UtilsRL/logger/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/logger/text_logger.py` & `UtilsRL-0.5.9/UtilsRL/logger/text_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/logger/wandb_logger.py` & `UtilsRL-0.5.9/UtilsRL/logger/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/math/distributions.py` & `UtilsRL-0.5.9/UtilsRL/math/distributions.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/misc/chore.py` & `UtilsRL-0.5.9/UtilsRL/misc/chore.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/misc/decorator.py` & `UtilsRL-0.5.9/UtilsRL/misc/decorator.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/misc/namespace.py` & `UtilsRL-0.5.9/UtilsRL/misc/namespace.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/monitor.py` & `UtilsRL-0.5.9/UtilsRL/monitor.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/net/basic.py` & `UtilsRL-0.5.9/UtilsRL/net/basic.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/net/cnn.py` & `UtilsRL-0.5.9/UtilsRL/net/cnn.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/net/mlp.py` & `UtilsRL-0.5.9/UtilsRL/net/mlp.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/net/rnn.py` & `UtilsRL-0.5.9/UtilsRL/net/rnn.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/plot/tb_parser.py` & `UtilsRL-0.5.9/UtilsRL/plot/tb_parser.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/rl/actor.py` & `UtilsRL-0.5.9/UtilsRL/rl/actor.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/rl/buffer/__init__.py` & `UtilsRL-0.5.9/UtilsRL/rl/buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/rl/buffer/base.py` & `UtilsRL-0.5.9/UtilsRL/rl/buffer/base.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/rl/buffer/prioritized_replay.py` & `UtilsRL-0.5.9/UtilsRL/rl/buffer/prioritized_replay.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/rl/buffer/transition_replay.py` & `UtilsRL-0.5.9/UtilsRL/rl/buffer/transition_replay.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/rl/buffer/trjectory_replay.py` & `UtilsRL-0.5.9/UtilsRL/rl/buffer/trjectory_replay.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/rl/critic.py` & `UtilsRL-0.5.9/UtilsRL/rl/critic.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/rl/normalizer.py` & `UtilsRL-0.5.9/UtilsRL/rl/normalizer.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/rl/video_recorder.py` & `UtilsRL-0.5.9/UtilsRL/rl/video_recorder.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL/third_party/tqdm.py` & `UtilsRL-0.5.9/UtilsRL/third_party/tqdm.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/UtilsRL.egg-info/PKG-INFO` & `UtilsRL-0.5.9/UtilsRL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UtilsRL
-Version: 0.5.8
+Version: 0.5.9
 Summary: A python module desgined for RL logging, monitoring and experiments managing. 
 Home-page: https://github.com/typoverflow/UtilsRL
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `UtilsRL-0.5.8/UtilsRL.egg-info/SOURCES.txt` & `UtilsRL-0.5.9/UtilsRL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.8/setup.py` & `UtilsRL-0.5.9/setup.py`

 * *Files identical despite different names*

