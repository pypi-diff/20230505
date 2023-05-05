# Comparing `tmp/ml-starter-0.0.27.tar.gz` & `tmp/ml-starter-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.27.tar", last modified: Wed May  3 08:16:16 2023, max compression
+gzip compressed data, was "ml-starter-0.0.28.tar", last modified: Fri May  5 13:05:23 2023, max compression
```

## Comparing `ml-starter-0.0.27.tar` & `ml-starter-0.0.28.tar`

### file list

```diff
@@ -1,154 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.813395 ml-starter-0.0.27/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 08:16:01.000000 ml-starter-0.0.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 08:16:01.000000 ml-starter-0.0.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 08:16:16.813395 ml-starter-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-03 08:16:01.000000 ml-starter-0.0.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.789395 ml-starter-0.0.27/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.793395 ml-starter-0.0.27/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    23447 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.793395 ml-starter-0.0.27/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/launchers/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/launchers/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.793395 ml-starter-0.0.27/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32994 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.793395 ml-starter-0.0.27/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.797395 ml-starter-0.0.27/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.797395 ml-starter-0.0.27/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.797395 ml-starter-0.0.27/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.801395 ml-starter-0.0.27/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.801395 ml-starter-0.0.27/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.801395 ml-starter-0.0.27/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.805395 ml-starter-0.0.27/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.805395 ml-starter-0.0.27/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.805395 ml-starter-0.0.27/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.805395 ml-starter-0.0.27/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.805395 ml-starter-0.0.27/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20360 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.809395 ml-starter-0.0.27/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.813395 ml-starter-0.0.27/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.813395 ml-starter-0.0.27/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-03 08:16:01.000000 ml-starter-0.0.27/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:16:16.813395 ml-starter-0.0.27/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 08:16:16.000000 ml-starter-0.0.27/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-03 08:16:16.000000 ml-starter-0.0.27/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:16:16.000000 ml-starter-0.0.27/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-03 08:16:16.000000 ml-starter-0.0.27/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-03 08:16:16.000000 ml-starter-0.0.27/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-03 08:16:01.000000 ml-starter-0.0.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 08:16:01.000000 ml-starter-0.0.27/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-03 08:16:01.000000 ml-starter-0.0.27/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-03 08:16:01.000000 ml-starter-0.0.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-03 08:16:16.817395 ml-starter-0.0.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-03 08:16:01.000000 ml-starter-0.0.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.746111 ml-starter-0.0.28/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 13:05:07.000000 ml-starter-0.0.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 13:05:07.000000 ml-starter-0.0.28/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-05 13:05:23.746111 ml-starter-0.0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-05 13:05:07.000000 ml-starter-0.0.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32994 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.730111 ml-starter-0.0.28/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.734111 ml-starter-0.0.28/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.738111 ml-starter-0.0.28/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.742111 ml-starter-0.0.28/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.742111 ml-starter-0.0.28/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-05 13:05:07.000000 ml-starter-0.0.28/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:05:23.746111 ml-starter-0.0.28/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 13:05:23.000000 ml-starter-0.0.28/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-05 13:05:07.000000 ml-starter-0.0.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 13:05:07.000000 ml-starter-0.0.28/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 13:05:07.000000 ml-starter-0.0.28/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-05 13:05:07.000000 ml-starter-0.0.28/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-05 13:05:23.746111 ml-starter-0.0.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-05 13:05:07.000000 ml-starter-0.0.28/setup.py
```

### Comparing `ml-starter-0.0.27/LICENSE` & `ml-starter-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/PKG-INFO` & `ml-starter-0.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.27
+Version: 0.0.28
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.27/README.md` & `ml-starter-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/api.py` & `ml-starter-0.0.28/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/core/config.py` & `ml-starter-0.0.28/ml/core/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Generic, TypeVar
+from typing import Any, Generic, TypeVar
 
-import torch
 from omegaconf import MISSING, DictConfig
 
-if TYPE_CHECKING:
-    from ml.core.registry import Objects
-
 FieldType = Any
 
 
 def conf_field(
     value: FieldType,
     *,
     help: str | None = None,  # pylint: disable=redefined-builtin
@@ -74,40 +70,19 @@
     """Defines the base class for all objects."""
 
     __constants__ = ["config"]
 
     def __init__(self, config: BaseConfigT) -> None:
         self.config: BaseConfigT = config
 
-
-class BaseObjectWithPointers(BaseObject[BaseConfigT], Generic[BaseConfigT]):
-    """Defines the base class for all objects with pointers to other objects."""
-
-    def __init__(self, config: BaseConfigT) -> None:
-        super().__init__(config)
-
         self._raw_config: DictConfig | None = None
-        self._objects: "Objects" | None = None
 
     @property
-    @torch.jit.unused
     def raw_config(self) -> DictConfig:
         if self._raw_config is None:
             raise RuntimeError("Cannot access raw config yet; it has yet to be assigned")
         return self._raw_config
 
     def set_raw_config(self, raw_config: DictConfig) -> None:
         if self._raw_config is not None:
             raise RuntimeError("The raw config object was already written")
         self._raw_config = raw_config
-
-    @property
-    @torch.jit.unused
-    def objects(self) -> "Objects":
-        if self._objects is None:
-            raise RuntimeError("Cannot access objects yet; it has yet to be assigned")
-        return self._objects
-
-    def set_objects(self, objects: "Objects") -> None:
-        if self._objects is not None:
-            raise RuntimeError("The objects field has already been written")
-        self._objects = objects
```

### Comparing `ml-starter-0.0.27/ml/core/env.py` & `ml-starter-0.0.28/ml/core/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,7 +144,11 @@
 # Disables using accelerator on Mac.
 DisableMetal = _BoolEnvVar("DISABLE_METAL", default=False)
 is_metal_disabled = DisableMetal.get
 
 # Disables using the GPU.
 DisableGPU = _BoolEnvVar("DISABLE_GPU", default=False)
 is_gpu_disabled = DisableGPU.get
+
+# Show full error message when trying to import a file.
+ShowFullImportError = _BoolEnvVar("SHOW_FULL_IMPORT_ERROR", default=False)
+should_show_full_import_error = ShowFullImportError.get
```

### Comparing `ml-starter-0.0.27/ml/core/registry.py` & `ml-starter-0.0.28/ml/core/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import functools
-import importlib.util
 import inspect
 import json
 import logging
-import sys
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Generic, Iterator, TypeVar, cast
 
 from omegaconf import DictConfig, ListConfig, OmegaConf
 from omegaconf.basecontainer import BaseContainer
 
-from ml.core.config import BaseConfig, BaseObject, BaseObjectWithPointers
+from ml.core.config import BaseConfig, BaseObject
+from ml.core.env import ShowFullImportError
 from ml.utils.colors import colorize
 from ml.utils.timer import Timer
 
 if TYPE_CHECKING:
     from ml.launchers.base import BaseLauncher, BaseLauncherConfig
     from ml.loggers.base import BaseLogger, BaseLoggerConfig
     from ml.lr_schedulers.base import BaseLRScheduler, BaseLRSchedulerConfig
@@ -83,14 +82,30 @@
         raise ValueError(f"Malformed {key} config; missing expected key {NAME_KEY}")
     name = config[NAME_KEY]
     if not isinstance(name, str):
         raise ValueError(f"Expected {key} name to be a string, got {name}")
     return name
 
 
+def get_names(key: str, config: BaseContainer) -> list[str]:
+    if not isinstance(config, ListConfig):
+        raise ValueError(f"Expected {key} config to be a list, got {type(config)}")
+    names = []
+    for i, subconfig in enumerate(config):
+        if not isinstance(subconfig, DictConfig):
+            raise ValueError(f"Expected {key} config item {i} to be a dictionary, got {type(subconfig)}")
+        if NAME_KEY not in subconfig:
+            raise ValueError(f"Malformed {key} config item {i}; missing expected key {NAME_KEY}")
+        name = subconfig[NAME_KEY]
+        if not isinstance(name, str):
+            raise ValueError(f"Expected {key} name to be a string, got {name}")
+        names.append(name)
+    return names
+
+
 class register_base(ABC, Generic[Entry, Config]):  # pylint: disable=invalid-name
     """Defines the base registry type."""
 
     REGISTRY: dict[str, tuple[type[Entry], type[Config]]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
 
     @classmethod
@@ -136,24 +151,25 @@
     @classmethod
     @functools.lru_cache(None)
     def manual_import(cls, path: Path) -> None:
         with Timer(f"importing '{path}'"):
             try:
                 rel_path = project_dirs.relative_path(path, parent=True)
                 module_name = ".".join(list(rel_path.parts[:-1]) + [rel_path.stem])
-                if module_name not in sys.modules:
-                    spec = importlib.util.spec_from_file_location(module_name, str(path))
-                    assert spec is not None
-                    module = importlib.util.module_from_spec(spec)
-                    sys.modules[module_name] = module
-                    loader = spec.loader
-                    assert loader is not None
-                    loader.exec_module(module)
+                __import__(module_name)
+
             except Exception:
-                logger.exception("Caught exception while importing %s", path)
+                if ShowFullImportError.get():
+                    logger.exception("Caught exception while importing %s", path)
+                else:
+                    logger.error(
+                        "Caught exception while importing %s (set %s to show the full exception)",
+                        path,
+                        ShowFullImportError.key,
+                    )
 
     @classmethod
     def populate_registry(cls, name: str) -> None:
         """Populates the registry until it has the requested name available.
 
         Args:
             name: The name of the registry item to get
@@ -249,52 +265,62 @@
             return cls.REGISTRY_LOCATIONS[name]
 
         options = "\n".join(f" - {k}" for k in sorted(cls.REGISTRY_LOCATIONS.keys()))
         logger.error("Couldn't locate %s '%s' in:\n%s", cls.config_key(), name, options)
         raise KeyError(f"Couldn't locate {cls.config_key()} '{name}' from {len(cls.REGISTRY_LOCATIONS)} options")
 
     @classmethod
+    def _build_entry_from_name(cls, reg_name: str, reg_cfg: DictConfig, raw_config: DictConfig) -> Entry:
+        with Timer(f"building {cls.config_key()}", spinner=True):
+            reg_cls, _ = cls.lookup(reg_name)
+
+        with Timer(f"building {reg_name}", spinner=True):
+            reg_obj = reg_cls(reg_cfg)
+            if isinstance(reg_obj, BaseObject):
+                reg_obj.set_raw_config(raw_config)
+
+        return reg_obj
+
+    @classmethod
     def build_entry(cls, raw_config: DictConfig) -> Entry | None:
         if cls.config_key() not in raw_config:
             return None
-        reg_cfg = raw_config[cls.config_key()]
-        reg_name = get_name(cls.config_key(), reg_cfg)
-        reg_cls, _ = cls.lookup(reg_name)
-        with Timer(f"building {reg_name}"):
-            reg_obj = reg_cls(reg_cfg)
-        if isinstance(reg_obj, BaseObjectWithPointers):
-            reg_obj.set_raw_config(raw_config)
-        return reg_obj
+        with Timer(f"getting {cls.config_key()} name", spinner=True):
+            reg_name = get_name(cls.config_key(), raw_config[cls.config_key()])
+        return cls._build_entry_from_name(reg_name, raw_config[cls.config_key()], raw_config)
 
     @classmethod
     def build_entry_non_null(cls, raw_config: DictConfig) -> Entry:
-        entry = cls.build_entry(raw_config)
-        if entry is None:
+        if (entry := cls.build_entry(raw_config)) is None:
             raise ValueError(f"Missing {cls.config_key()} in config")
         return entry
 
     @classmethod
     def update_config(cls, raw_config: DictConfig) -> None:
         if cls.config_key() not in raw_config:
             return
-        reg_cfg = raw_config[cls.config_key()]
-        reg_name = get_name(cls.config_key(), reg_cfg)
-        _, reg_cfg_cls = cls.lookup(reg_name)
-        reg_cfg = OmegaConf.merge(OmegaConf.structured(reg_cfg_cls), reg_cfg)
-        raw_config[cls.config_key()] = reg_cfg
+
+        with Timer(f"updating {cls.config_key()} config", spinner=True):
+            reg_cfg = raw_config[cls.config_key()]
+            reg_name = get_name(cls.config_key(), reg_cfg)
+            _, reg_cfg_cls = cls.lookup(reg_name)
+            reg_cfg = OmegaConf.merge(OmegaConf.structured(reg_cfg_cls), reg_cfg)
+            raw_config[cls.config_key()] = reg_cfg
 
     @classmethod
     def resolve_config(cls, raw_config: DictConfig) -> None:
         if cls.config_key() not in raw_config:
             return
-        reg_cfg = raw_config[cls.config_key()]
-        reg_name = get_name(cls.config_key(), reg_cfg)
-        _, reg_cfg_cls = cls.lookup(reg_name)
-        reg_cfg_cls.resolve(reg_cfg)
-        raw_config[cls.config_key()] = reg_cfg
+
+        with Timer(f"resolving {cls.config_key()} config", spinner=True):
+            reg_cfg = raw_config[cls.config_key()]
+            reg_name = get_name(cls.config_key(), reg_cfg)
+            _, reg_cfg_cls = cls.lookup(reg_name)
+            reg_cfg_cls.resolve(reg_cfg)
+            raw_config[cls.config_key()] = reg_cfg
 
     def __init__(self, name: str, config: type[Config]) -> None:
         self.name = name
         self.config = config
 
     def __call__(self, entry: SpecificEntry) -> SpecificEntry:
         if self.name in self.REGISTRY:
@@ -317,56 +343,96 @@
         return entry
 
 
 class multi_register_base(register_base[Entry, Config], Generic[Entry, Config]):  # pylint: disable=invalid-name
     """Defines a registry which produces multiple objects."""
 
     @classmethod
+    def build_entry(cls, raw_config: DictConfig) -> Entry | None:
+        raise NotImplementedError("`build_entry` not implemented; use `build_entries` instead")
+
+    @classmethod
+    def build_entry_non_null(cls, raw_config: DictConfig) -> Entry:
+        raise NotImplementedError("`build_entry_non_null` not implemented; use `build_entries_non_null` instead")
+
+    @classmethod
     def update_config(cls, raw_config: DictConfig) -> None:
-        if cls.config_key() not in raw_config:
-            return
-        reg_cfg = raw_config[cls.config_key()]
-        if isinstance(reg_cfg, DictConfig):
-            reg_cfgs = ListConfig([reg_cfg])
-        elif isinstance(reg_cfg, ListConfig):
-            reg_cfgs = reg_cfg
-        else:
-            raise NotImplementedError(f"Invalid logger config type: {type(reg_cfg)}")
-        for i, reg_cfg in enumerate(reg_cfgs):
-            reg_name = get_name(cls.config_key(), reg_cfg)
-            _, reg_cfg_cls = cls.lookup(reg_name)
-            reg_cfgs[i] = OmegaConf.merge(OmegaConf.structured(reg_cfg_cls), reg_cfg)
-        raw_config[cls.config_key()] = reg_cfgs
+        raise NotImplementedError("`update_config` not implemented; use `update_configs` instead")
 
     @classmethod
     def resolve_config(cls, raw_config: DictConfig) -> None:
+        raise NotImplementedError("`resolve_config` not implemented; use `resolve_configs` instead")
+
+    @classmethod
+    def build_entries(cls, raw_config: DictConfig) -> list[Entry] | None:
+        if cls.config_key() not in raw_config:
+            return None
+
+        # Attempts to build a single entry first.
+        try:
+            entry = super().build_entry(raw_config)
+            return [entry] if entry is not None else None
+        except ValueError:
+            pass
+
+        entries: list[Entry] = []
+        reg_names = get_names(cls.config_key(), raw_config[cls.config_key()])
+        for i, reg_name in enumerate(reg_names):
+            entries.append(cls._build_entry_from_name(reg_name, raw_config[cls.config_key()][i], raw_config))
+
+        return entries
+
+    @classmethod
+    def build_entries_non_null(cls, raw_config: DictConfig) -> list[Entry]:
+        entries = cls.build_entries(raw_config)
+        if entries is None:
+            raise ValueError(f"Missing {cls.config_key()} in config")
+        return entries
+
+    @classmethod
+    def update_configs(cls, raw_config: DictConfig) -> None:
         if cls.config_key() not in raw_config:
             return
-        reg_cfgs = cast(ListConfig, raw_config[cls.config_key()])
-        for i, reg_cfg in enumerate(reg_cfgs):
-            reg_name = get_name(cls.config_key(), reg_cfg)
-            _, reg_cfg_cls = cls.lookup(reg_name)
-            reg_cfg_cls.resolve(reg_cfg)
-            reg_cfgs[i] = reg_cfg
-        raw_config[cls.config_key()] = reg_cfgs
+
+        # Treat as a single entry first.
+        try:
+            super().update_config(raw_config)
+            return
+        except ValueError:
+            pass
+
+        with Timer(f"updating {cls.config_key()} config", spinner=True):
+            reg_cfgs = raw_config[cls.config_key()]
+            reg_names = get_names(cls.config_key(), reg_cfgs)
+            for i, (reg_name, reg_cfg) in enumerate(zip(reg_names, reg_cfgs)):
+                _, reg_cfg_cls = cls.lookup(reg_name)
+                reg_cfg = OmegaConf.merge(OmegaConf.structured(reg_cfg_cls), reg_cfg)
+                reg_cfgs[i] = reg_cfg
+            raw_config[cls.config_key()] = reg_cfgs
 
     @classmethod
-    def build_entry(cls, raw_config: DictConfig) -> list[Entry] | None:  # type: ignore
+    def resolve_configs(cls, raw_config: DictConfig) -> None:
         if cls.config_key() not in raw_config:
-            return None
-        reg_cfgs = cast(ListConfig, raw_config[cls.config_key()])
-        reg_objs = []
-        for reg_cfg in reg_cfgs:
-            reg_name = get_name(cls.config_key(), reg_cfg)
-            reg_cls, _ = cls.lookup(reg_name)
-            with Timer(f"building {reg_name}"):
-                reg_obj = reg_cls(reg_cfg)
-            reg_obj.set_raw_config(raw_config)
-            reg_objs.append(reg_obj)
-        return reg_objs
+            return
+
+        # Treat as a single entry first.
+        try:
+            super().resolve_config(raw_config)
+            return
+        except ValueError:
+            pass
+
+        with Timer(f"resolving {cls.config_key()} config", spinner=True):
+            reg_cfgs = raw_config[cls.config_key()]
+            reg_names = get_names(cls.config_key(), reg_cfgs)
+            for i, (reg_name, reg_cfg) in enumerate(zip(reg_names, reg_cfgs)):
+                _, reg_cfg_cls = cls.lookup(reg_name)
+                reg_cfg_cls.resolve(reg_cfg)
+                reg_cfgs[i] = reg_cfg
+            raw_config[cls.config_key()] = reg_cfgs
 
 
 class register_model(register_base["BaseModel", "BaseModelConfig"]):  # pylint: disable=invalid-name
     """Defines a registry for holding modules."""
 
     REGISTRY: dict[str, tuple[type["BaseModel"], type["BaseModelConfig"]]] = {}
     REGISTRY_LOCATIONS: dict[str, Path] = {}
@@ -476,31 +542,17 @@
     trainer: "BaseTrainer | None" = None
     optimizer: "BaseOptimizer | None" = None
     lr_scheduler: "BaseLRScheduler | None" = None
     logger: "list[BaseLogger] | None" = None
     launcher: "BaseLauncher | None" = None
 
     def __post_init__(self) -> None:
-        # After initializing the object container, we add a pointer to the
-        # current container to each of the constructed objects.
-        if self.task is not None:
-            self.task.set_objects(self)
         if self.trainer is not None:
-            self.trainer.set_objects(self)
             if self.logger is not None:
                 self.trainer.add_loggers(self.logger)
-        if self.optimizer is not None:
-            self.optimizer.set_objects(self)
-        if self.lr_scheduler is not None:
-            self.lr_scheduler.set_objects(self)
-        if self.logger is not None:
-            for sublogger in self.logger:
-                sublogger.set_objects(self)
-        if self.launcher is not None:
-            self.launcher.set_objects(self)
 
     def summarize(self) -> str:
         parts: dict[str, tuple[str, str]] = {}
         if self.model is not None:
             parts["Model"] = (
                 inspect.getfile(self.model.__class__),
                 f"{self.model.__class__.__module__}.{self.model.__class__.__name__}",
@@ -532,69 +584,68 @@
             )
         return "Components:" + "".join(
             f"\n ↪ {colorize(k, 'green')}: {colorize(v[1], 'cyan')} ({colorize(v[0], 'blue')})"
             for k, v in parts.items()
         )
 
     @classmethod
+    def update_config(cls, config: DictConfig) -> None:
+        """Updates the config in-place.
+
+        Args:
+            config: The config to update
+        """
+
+        # Pre-builds the config using the structured configs.
+        register_model.update_config(config)
+        register_task.update_config(config)
+        register_trainer.update_config(config)
+        register_optimizer.update_config(config)
+        register_lr_scheduler.update_config(config)
+        register_logger.update_configs(config)
+        register_launcher.update_config(config)
+
+    @classmethod
     def resolve_config(cls, config: DictConfig) -> None:
         """Resolves the config in-place.
 
         Args:
             config: The config to resolve
         """
 
-        with Timer("building config", spinner=True):
-            # Pre-builds the config using the structured configs.
-            register_model.update_config(config)
-            register_task.update_config(config)
-            register_trainer.update_config(config)
-            register_optimizer.update_config(config)
-            register_lr_scheduler.update_config(config)
-            register_logger.update_config(config)
-            register_launcher.update_config(config)
-
-        with Timer("resolving configs", spinner=True):
-            # Resolves the final config once all structured configs have been merged.
-            OmegaConf.resolve(config)
-
-            # Runs object-specific resolutions.
-            register_model.resolve_config(config)
-            register_task.resolve_config(config)
-            register_trainer.resolve_config(config)
-            register_optimizer.resolve_config(config)
-            register_lr_scheduler.resolve_config(config)
-            register_logger.resolve_config(config)
-            register_launcher.resolve_config(config)
+        # Resolves the final config once all structured configs have been merged.
+        OmegaConf.resolve(config)
+
+        # Runs object-specific resolutions.
+        register_model.resolve_config(config)
+        register_task.resolve_config(config)
+        register_trainer.resolve_config(config)
+        register_optimizer.resolve_config(config)
+        register_lr_scheduler.resolve_config(config)
+        register_logger.resolve_configs(config)
+        register_launcher.resolve_config(config)
 
     @classmethod
     def parse_raw_config(cls, config: DictConfig) -> "Objects":
         """Parses a raw config to the objects it contains.
 
         Args:
             config: The raw DictConfig to parse
 
         Returns:
             The parsed Objects dataclass
         """
 
-        with Timer("building model", spinner=True):
-            model = register_model.build_entry(config)
-        with Timer("building task", spinner=True):
-            task = register_task.build_entry(config)
-        with Timer("building trainer", spinner=True):
-            trainer = register_trainer.build_entry(config)
-        with Timer("building optimizer", spinner=True):
-            optimizer = register_optimizer.build_entry(config)
-        with Timer("building lr scheduler", spinner=True):
-            lr_scheduler = register_lr_scheduler.build_entry(config)
-        with Timer("building loggers", spinner=True):
-            loggers = register_logger.build_entry(config)
-        with Timer("building launcher", spinner=True):
-            launcher = register_launcher.build_entry(config)
+        model = register_model.build_entry(config)
+        task = register_task.build_entry(config)
+        trainer = register_trainer.build_entry(config)
+        optimizer = register_optimizer.build_entry(config)
+        lr_scheduler = register_lr_scheduler.build_entry(config)
+        loggers = register_logger.build_entries(config)
+        launcher = register_launcher.build_entry(config)
 
         objs = Objects(
             raw_config=config,
             model=model,
             task=task,
             trainer=trainer,
             optimizer=optimizer,
```

### Comparing `ml-starter-0.0.27/ml/core/state.py` & `ml-starter-0.0.28/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/launchers/ddp.py` & `ml-starter-0.0.28/ml/launchers/ddp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Defines a Distributed Data Parallel trainer.
+"""Defines a Distributed Data Parallel launcher.
 
 This is a light-weight wrapper around PyTorch's built-in Distributed Data
 Parallel class.
 
 For multiple devices, data is split along the batch dimension, passed to each
 device, which computes losses independently. The loss tensors are gathered to
 the master device to compute a single loss. In other words, each device
@@ -15,46 +15,55 @@
 import sys
 import traceback
 from dataclasses import dataclass
 from typing import Callable
 
 import torch
 import torch.multiprocessing as mp
-from omegaconf import DictConfig
+from omegaconf import MISSING, DictConfig, OmegaConf
 
+from ml.core.config import conf_field
 from ml.core.registry import Objects, register_launcher
 from ml.launchers.base import BaseLauncher, BaseLauncherConfig
-from ml.scripts.train import train_main
-from ml.trainers.base import BaseTrainer, MultiprocessConfig
+from ml.scripts.train import train_main_with_objects
 from ml.utils.distributed import (
     set_init_method,
     set_master_addr,
     set_master_port,
     set_rank,
     set_world_size,
 )
 from ml.utils.logging import configure_logging
 from ml.utils.networking import get_unused_port
 from ml.utils.torch_distributed import get_distributed_backend, init_process_group
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@dataclass
+class MultiprocessConfig:
+    rank: int = conf_field(-1, help="The rank of the process")
+    world_size: int = conf_field(MISSING, help="The total number of processes")
+    devices_per_rank: int = conf_field(1, help="The number of devices per rank")
+    master_addr: str = conf_field("localhost", help="The address of the master process")
+    master_port: int = conf_field(MISSING, help="The port of the master process")
+
+
 def process_main(cfg: MultiprocessConfig, raw_config: DictConfig) -> None:
     set_master_addr(cfg.master_addr)
     set_master_port(cfg.master_port)
     set_rank(cfg.rank)
     set_world_size(cfg.world_size)
     set_init_method("env://")
     configure_logging(rank=cfg.rank, world_size=cfg.world_size)
     logger.info("Initializing process group")
     init_process_group(backend=get_distributed_backend())
 
     objs = Objects.parse_raw_config(raw_config)
-    train_main(objs)
+    train_main_with_objects(objs)
 
 
 def func_wrapped(
     func: Callable[[MultiprocessConfig], None],
     cfg: MultiprocessConfig,
     error_queue: "mp.Queue[str]",
 ) -> None:
@@ -65,35 +74,44 @@
     except Exception:
         error_queue.put(traceback.format_exc())
         sys.exit(1)
 
 
 @dataclass
 class DDPLauncherConfig(BaseLauncherConfig):
-    pass
+    multiprocess: MultiprocessConfig = conf_field(MultiprocessConfig())
+
+    @classmethod
+    def resolve(cls: type["DDPLauncherConfig"], config: "DDPLauncherConfig") -> None:
+        super().resolve(config)
+
+        device_count = torch.cuda.device_count()
+        if config.multiprocess.devices_per_rank > device_count:
+            raise ValueError(
+                f"Requested {config.multiprocess.devices_per_rank} devices per rank, "
+                f"but only {device_count} are available"
+            )
+        if OmegaConf.is_missing(config.multiprocess, "world_size"):
+            config.multiprocess.world_size = device_count // config.multiprocess.devices_per_rank
+        if OmegaConf.is_missing(config.multiprocess, "master_port"):
+            config.multiprocess.master_port = get_unused_port()
 
 
 @register_launcher("ddp", DDPLauncherConfig)
 class DDPLauncher(BaseLauncher[DDPLauncherConfig]):
-    def launch(self, trainer: BaseTrainer) -> None:
+    def launch(self) -> None:
         if not torch.cuda.is_available():
             raise RuntimeError("DDPLauncher requires CUDA")
-        device_count = torch.cuda.device_count()
 
         func = functools.partial(process_main, raw_config=self.raw_config)
 
-        cfg = MultiprocessConfig(
-            rank=-1,
-            world_size=device_count,
-            devices_per_rank=1,
-            master_addr="localhost",
-            master_port=get_unused_port(),
-        )
+        # Config should have valid values at this point, post-resolution.
+        cfg = self.config.multiprocess
 
-        if device_count <= 1:
+        if cfg.world_size <= 1:
             logger.warning("Multi-process DDPTrainer expects more than one device")
             cfg.rank = 0
             func(cfg)
             return
 
         def set_env(rank: int) -> None:
             os.environ["CUDA_VISIBLE_DEVICES"] = str(rank)
```

### Comparing `ml-starter-0.0.27/ml/launchers/slurm.py` & `ml-starter-0.0.28/ml/launchers/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 from types import FrameType
 from typing import TypeVar
 
 from omegaconf import II, MISSING, OmegaConf
 
 from ml.core.config import conf_field
 from ml.core.env import get_stage_dir
-from ml.core.registry import Objects, project_dirs, register_launcher
+from ml.core.registry import Objects, project_dirs, register_launcher, register_trainer
 from ml.launchers.base import BaseLauncher, BaseLauncherConfig
-from ml.scripts.train import train_main
+from ml.scripts.train import train_main_with_objects
 from ml.trainers.base import BaseTrainer
 from ml.utils.distributed import (
     get_master_addr,
     get_master_port,
     get_random_port,
     is_master,
     set_init_method,
@@ -211,15 +211,17 @@
 
         with open(sbatch_path, "w", encoding="utf-8") as f:
             f.write(sbatch_file)
         logger.info("Wrote sbatch file to %s", sbatch_path)
 
         return sbatch_path
 
-    def launch(self, trainer: BaseTrainer) -> None:
+    def launch(self) -> None:
+        trainer = register_trainer.build_entry_non_null(self.raw_config)
+
         sbatch_path = self.write_sbatch_file(trainer)
 
         # Call `sbatch` on the given file.
         all_run_ids: list[str] = []
         for _ in range(self.config.num_jobs):
             command = ["sbatch", str(sbatch_path)]
             if all_run_ids:
@@ -269,12 +271,12 @@
     assert (trainer := objs.trainer) is not None
     trainer.add_lock_file("running", exists_ok=True)
     trainer.remove_lock_file("scheduled", missing_ok=True)
 
     signal.signal(signal.SIGTERM, ignore_signal)
     trainer.add_signal_handler(signal.SIGUSR1, requeue_job)
 
-    train_main(objs)
+    train_main_with_objects(objs)
 
 
 if __name__ == "__main__":
     slurm_main()
```

### Comparing `ml-starter-0.0.27/ml/loggers/base.py` & `ml-starter-0.0.28/ml/loggers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Callable, Generic, TypeVar, Union
 
 from omegaconf import DictConfig
 from torch import Tensor
 
-from ml.core.config import BaseConfig, BaseObjectWithPointers, conf_field
+from ml.core.config import BaseConfig, BaseObject, conf_field
 from ml.core.state import Phase, State
 
 Number = Union[int, float, Tensor]
 
 
 @dataclass
 class BaseLoggerConfig(BaseConfig):
@@ -20,15 +20,15 @@
     write_train_every_n_seconds: float | None = conf_field(None, help="Only write a train log line every N seconds")
     write_val_every_n_seconds: float | None = conf_field(None, help="Only write a val log line every N seconds")
 
 
 LoggerConfigT = TypeVar("LoggerConfigT", bound=BaseLoggerConfig)
 
 
-class BaseLogger(BaseObjectWithPointers[LoggerConfigT], Generic[LoggerConfigT], ABC):
+class BaseLogger(BaseObject[LoggerConfigT], Generic[LoggerConfigT], ABC):
     """Defines the base logger."""
 
     log_directory: Path
 
     def __init__(self, config: LoggerConfigT) -> None:
         super().__init__(config)
```

### Comparing `ml-starter-0.0.27/ml/loggers/meter.py` & `ml-starter-0.0.28/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/loggers/multi.py` & `ml-starter-0.0.28/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/loggers/stdout.py` & `ml-starter-0.0.28/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/loggers/tensorboard.py` & `ml-starter-0.0.28/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/lr_schedulers/base.py` & `ml-starter-0.0.28/ml/lr_schedulers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar
 
 from torch.optim.optimizer import Optimizer
 
-from ml.core.config import BaseConfig, BaseObjectWithPointers
+from ml.core.config import BaseConfig, BaseObject
 from ml.core.state import State
 
 
 class SchedulerAdapter:
     """Defines a general-purpose learning rate scheduler adapter."""
 
     last_state: State | None
@@ -40,15 +40,15 @@
 class BaseLRSchedulerConfig(BaseConfig):
     """Defines the base config for all learning rate schedulers."""
 
 
 LRSchedulerConfigT = TypeVar("LRSchedulerConfigT", bound=BaseLRSchedulerConfig)
 
 
-class BaseLRScheduler(BaseObjectWithPointers[LRSchedulerConfigT], Generic[LRSchedulerConfigT], ABC):
+class BaseLRScheduler(BaseObject[LRSchedulerConfigT], Generic[LRSchedulerConfigT], ABC):
     """Defines the base learning rate scheduler."""
 
     @abstractmethod
     def get_lr_scale(self, state: State) -> float:
         """Given a state, returns the current learning rate.
 
         Args:
```

### Comparing `ml-starter-0.0.27/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.28/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.28/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/lr_schedulers/linear.py` & `ml-starter-0.0.28/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.28/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.28/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/models/activations.py` & `ml-starter-0.0.28/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/models/base.py` & `ml-starter-0.0.28/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/models/embeddings.py` & `ml-starter-0.0.28/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/models/init.py` & `ml-starter-0.0.28/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/models/norms.py` & `ml-starter-0.0.28/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/optimizers/adam.py` & `ml-starter-0.0.28/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/optimizers/adamw.py` & `ml-starter-0.0.28/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/optimizers/adan.py` & `ml-starter-0.0.28/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/optimizers/base.py` & `ml-starter-0.0.28/ml/optimizers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar
 
 from torch import nn
 from torch.optim.optimizer import Optimizer
 
-from ml.core.config import BaseConfig, BaseObjectWithPointers
+from ml.core.config import BaseConfig, BaseObject
 
 
 @dataclass
 class BaseOptimizerConfig(BaseConfig):
     """Defines the base config for all optimizers."""
 
 
 OptimizerConfigT = TypeVar("OptimizerConfigT", bound=BaseOptimizerConfig)
 
 
-class BaseOptimizer(BaseObjectWithPointers[OptimizerConfigT], Generic[OptimizerConfigT], ABC):
+class BaseOptimizer(BaseObject[OptimizerConfigT], Generic[OptimizerConfigT], ABC):
     """Defines the base optimizer type."""
 
     @property
     def common_kwargs(self) -> dict[str, Any]:
         return {}
 
     @abstractmethod
```

### Comparing `ml-starter-0.0.27/ml/optimizers/sgd.py` & `ml-starter-0.0.28/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/optimizers/shampoo.py` & `ml-starter-0.0.28/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/scripts/cli.py` & `ml-starter-0.0.28/ml/scripts/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import shlex
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Callable
 
-from ml.scripts import launch
 from ml.utils.distributed import get_rank_optional, get_world_size_optional
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
 
 if TYPE_CHECKING:
     from omegaconf import DictConfig
 
@@ -19,70 +18,58 @@
     configure_logging(rank=get_rank_optional(), world_size=get_world_size_optional())
     logger.info("Command: %s", shlex.join(sys.argv))
 
     # Import here to avoid slow startup time.
     with Timer("importing", spinner=True):
         from ml.core.env import add_global_tag
         from ml.core.registry import Objects, add_project_dir
-        from ml.scripts import compiler, resolve, stage, train
+        from ml.scripts import launch, resolve, stage, train
         from ml.utils.cli import parse_cli
         from ml.utils.colors import colorize
-        from ml.utils.random import set_random_seed
 
-    if project_root is not None:
-        add_project_dir(Path(project_root).resolve())
+    with Timer("running pre-flight tasks", spinner=True):
+        if project_root is not None:
+            add_project_dir(Path(project_root).resolve())
+
+        scripts: dict[str, Callable[[DictConfig], None]] = {
+            "train": train.train_main,
+            "stage": stage.stage_main,
+            "resolve": resolve.resolve_main,
+            "launch": launch.launch_main,
+        }
+
+        def show_help() -> None:
+            script_names = (colorize(script_name, "cyan") for script_name in scripts)
+            print(f"Usage: ml < {' / '.join(script_names)} > ...\n", file=sys.stderr)
+            for key, func in sorted(scripts.items()):
+                if func.__doc__ is None:
+                    print(f" ↪ {colorize(key, 'green')}", file=sys.stderr)
+                else:
+                    docstring = func.__doc__.strip().split("\n")[0]
+                    print(f" ↪ {colorize(key, 'green')}: {docstring}", file=sys.stderr)
+            print()
+            sys.exit(1)
+
+        # Parses the raw command line options.
+        args = sys.argv[1:]
+        if len(args) == 0:
+            show_help()
+        option, args = args[0], args[1:]
 
-    set_random_seed()
+        # Adds a global tag with the currently-selected option.
+        add_global_tag(option)
 
-    without_objects_scripts: dict[str, Callable[[DictConfig], None]] = {
-        "compile": compiler.compile_main,
-        "stage": stage.stage_main,
-        "resolve": resolve.resolve_main,
-        "launch": launch.launch_main,
-    }
-
-    with_objects_scripts: dict[str, Callable[[Objects], None]] = {
-        "train": train.train_main,
-    }
-
-    scripts: dict[str, Callable[..., None]] = {**with_objects_scripts, **without_objects_scripts}
-
-    def show_help() -> None:
-        script_names = (colorize(script_name, "cyan") for script_name in scripts)
-        print(f"Usage: ml < {' / '.join(script_names)} > ...\n", file=sys.stderr)
-        for key, func in sorted(scripts.items()):
-            if func.__doc__ is None:
-                print(f" ↪ {colorize(key, 'green')}", file=sys.stderr)
-            else:
-                docstring = func.__doc__.strip().split("\n")[0]
-                print(f" ↪ {colorize(key, 'green')}: {docstring}", file=sys.stderr)
-        print()
-        sys.exit(1)
-
-    # Parses the raw command line options.
-    args = sys.argv[1:]
-    if len(args) == 0:
-        show_help()
-    option, args = args[0], args[1:]
-
-    # Adds a global tag with the currently-selected option.
-    add_global_tag(option)
-
-    if option in without_objects_scripts:
+    if option in scripts:
         # Special handling for multi-processing; don't initialize anything since
         # everything will be initialized inside the child processes.
-        config = parse_cli(args)
-        Objects.resolve_config(config)
-        without_objects_scripts[option](config)
-    elif option in with_objects_scripts:
-        # Converts the raw config to the objects they are pointing at.
-        config = parse_cli(args)
+        with Timer("parsing cli arguments"):
+            config = parse_cli(args)
+        Objects.update_config(config)
         Objects.resolve_config(config)
-        objs = Objects.parse_raw_config(config)
-        with_objects_scripts[option](objs)
+        scripts[option](config)
     else:
         print(f"Invalid option: {colorize(option, 'red')}\n", file=sys.stderr)
         show_help()
 
 
 if __name__ == "__main__":
     cli_main()
```

### Comparing `ml-starter-0.0.27/ml/scripts/stage.py` & `ml-starter-0.0.28/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/base.py` & `ml-starter-0.0.28/ml/tasks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from torch import Tensor, nn
 from torch.optim.optimizer import Optimizer
 from torch.utils.data.dataloader import DataLoader
 from torch.utils.data.dataset import Dataset
 from torch.utils.data.sampler import Sampler
 
 from ml.core.common_types import Batch, Loss, Output
-from ml.core.config import BaseConfig, BaseObjectWithPointers, conf_field
+from ml.core.config import BaseConfig, BaseObject, conf_field
 from ml.core.env import is_debugging
 from ml.core.state import Phase, State, cast_phase
 from ml.loggers.multi import MultiLogger
 from ml.lr_schedulers.base import SchedulerAdapter
 from ml.models.base import BaseModel
 from ml.tasks.datasets.collate import CollateMode, collate
 from ml.tasks.datasets.error_handling import (
@@ -192,23 +192,23 @@
 
 BaseTaskConfigT = TypeVar("BaseTaskConfigT", bound=BaseTaskConfig)
 ModelT = TypeVar("ModelT", bound=BaseModel)
 
 
 class BaseTask(
     nn.Module,
-    BaseObjectWithPointers[BaseTaskConfigT],
+    BaseObject[BaseTaskConfigT],
     Generic[BaseTaskConfigT, ModelT, Batch, Output, Loss],
     ABC,
 ):
     """Defines the base task type."""
 
     def __init__(self, config: BaseTaskConfigT) -> None:
         nn.Module.__init__(self)
-        BaseObjectWithPointers.__init__(self, config)
+        BaseObject.__init__(self, config)
 
         self.dataloader_configs: dict[Phase, DataLoaderConfig] = {
             cast_phase(k): v for k, v in config.dataloader.items()
         }
 
         # This flag can be toggled to end training from anywhere in the task.
         self.__training_over_flag = False
```

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.28/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.28/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/collate.py` & `ml-starter-0.0.28/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.28/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.28/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.28/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.28/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.28/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/utils.py` & `ml-starter-0.0.28/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.28/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/environments/base.py` & `ml-starter-0.0.28/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/environments/utils.py` & `ml-starter-0.0.28/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/environments/worker.py` & `ml-starter-0.0.28/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/losses/reduce.py` & `ml-starter-0.0.28/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/rl/base.py` & `ml-starter-0.0.28/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/rl/replay.py` & `ml-starter-0.0.28/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/tasks/sl/base.py` & `ml-starter-0.0.28/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/base.py` & `ml-starter-0.0.28/ml/trainers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Any, Callable, Generic, Literal, TypeVar, cast, get_args
 
 import torch
 from omegaconf import II, MISSING, DictConfig, ListConfig, OmegaConf
 from torch import Tensor
 from torch.optim.optimizer import Optimizer
 
-from ml.core.config import BaseConfig, BaseObjectWithPointers, conf_field
+from ml.core.config import BaseConfig, BaseObject, conf_field
 from ml.core.state import State
 from ml.loggers.base import BaseLogger
 from ml.loggers.multi import MultiLogger
 from ml.lr_schedulers.base import BaseLRScheduler, SchedulerAdapter
 from ml.models.base import BaseModel
 from ml.optimizers.base import BaseOptimizer
 from ml.tasks.base import BaseTask
@@ -26,23 +26,14 @@
 from ml.utils.device.base import BaseDevice, Prefetcher
 from ml.utils.distributed import is_master
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@dataclass
-class MultiprocessConfig:
-    rank: int
-    world_size: int
-    devices_per_rank: int
-    master_addr: str
-    master_port: int
-
-
 def resolve(path: str) -> str:
     return str(Path(path).resolve())
 
 
 def cpu_count(default: int) -> int:
     if (cpu_count := os.cpu_count()) is not None:
         return cpu_count
@@ -236,15 +227,15 @@
 
 
 TrainerConfigT = TypeVar("TrainerConfigT", bound=BaseTrainerConfig)
 ModelT = TypeVar("ModelT", bound=BaseModel)
 TaskT = TypeVar("TaskT", bound=BaseTask)
 
 
-class BaseTrainer(BaseObjectWithPointers[TrainerConfigT], Generic[TrainerConfigT, ModelT, TaskT]):
+class BaseTrainer(BaseObject[TrainerConfigT], Generic[TrainerConfigT, ModelT, TaskT]):
     """Defines the base trainer type."""
 
     logger: MultiLogger
     loggers: list[BaseLogger]
 
     def __init__(self, config: TrainerConfigT) -> None:
         super().__init__(config)
```

### Comparing `ml-starter-0.0.27/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.28/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.28/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.28/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.28/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.28/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.28/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.28/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.28/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/rl.py` & `ml-starter-0.0.28/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/sl.py` & `ml-starter-0.0.28/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/trainers/vanilla.py` & `ml-starter-0.0.28/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/argparse.py` & `ml-starter-0.0.28/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/atomic.py` & `ml-starter-0.0.28/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/augmentation.py` & `ml-starter-0.0.28/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/caching.py` & `ml-starter-0.0.28/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/call_train.py` & `ml-starter-0.0.28/ml/utils/call_train.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         show_help()
 
     # Adds a global tag with the currently-selected option.
     add_global_tag("train")
 
     # Resolves the config to the correct objects.
     config = parse_cli(args)
+    Objects.update_config(config)
     Objects.resolve_config(config)
-    objs = Objects.parse_raw_config(config)
 
     # Calls main training loop.
-    train_main(objs)
+    train_main(config)
 
 
 if __name__ == "__main__":
     call_train()
```

### Comparing `ml-starter-0.0.27/ml/utils/cli.py` & `ml-starter-0.0.28/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/colors.py` & `ml-starter-0.0.28/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/data.py` & `ml-starter-0.0.28/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/datetime.py` & `ml-starter-0.0.28/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/device/auto.py` & `ml-starter-0.0.28/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/device/base.py` & `ml-starter-0.0.28/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/device/cpu.py` & `ml-starter-0.0.28/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/device/gpu.py` & `ml-starter-0.0.28/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/device/metal.py` & `ml-starter-0.0.28/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/distributed.py` & `ml-starter-0.0.28/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/image.py` & `ml-starter-0.0.28/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/io.py` & `ml-starter-0.0.28/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/large_models.py` & `ml-starter-0.0.28/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/logging.py` & `ml-starter-0.0.28/ml/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import logging
 import math
 import sys
 
-import tqdm
-
 from ml.core.env import is_debugging
 from ml.utils.colors import Color, colorize, get_colorize_parts
 
 # Logging level to show on all ranks.
 INFOALL: int = logging.INFO + 1
 
 
@@ -83,14 +81,16 @@
             if self.use_color and levelname in self.COLORS:
                 record.levelname = colorize(levelname, self.COLORS[levelname], bold=True)
         return logging.Formatter.format(self, record)
 
 
 class TqdmHandler(logging.Handler):
     def emit(self, record: logging.LogRecord) -> None:
+        import tqdm
+
         try:
             msg = self.format(record)
             tqdm.tqdm.write(msg)
             self.flush()
         except Exception:
             self.handleError(record)
```

### Comparing `ml-starter-0.0.27/ml/utils/meter.py` & `ml-starter-0.0.28/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/staging.py` & `ml-starter-0.0.28/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/timer.py` & `ml-starter-0.0.28/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/torch_distributed.py` & `ml-starter-0.0.28/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml/utils/video.py` & `ml-starter-0.0.28/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.28/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.27
+Version: 0.0.28
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.27/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.28/ml_starter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ml/core/env.py
 ml/core/registry.py
 ml/core/state.py
 ml/launchers/__init__.py
 ml/launchers/base.py
 ml/launchers/ddp.py
 ml/launchers/slurm.py
+ml/launchers/torchrun.py
 ml/loggers/__init__.py
 ml/loggers/base.py
 ml/loggers/meter.py
 ml/loggers/multi.py
 ml/loggers/stdout.py
 ml/loggers/tensorboard.py
 ml/lr_schedulers/__init__.py
@@ -47,15 +48,14 @@
 ml/optimizers/adan.py
 ml/optimizers/base.py
 ml/optimizers/sgd.py
 ml/optimizers/shampoo.py
 ml/optimizers/types.py
 ml/scripts/__init__.py
 ml/scripts/cli.py
-ml/scripts/compiler.py
 ml/scripts/launch.py
 ml/scripts/resolve.py
 ml/scripts/stage.py
 ml/scripts/train.py
 ml/tasks/__init__.py
 ml/tasks/base.py
 ml/tasks/datasets/__init__.py
@@ -99,15 +99,14 @@
 ml/utils/atomic.py
 ml/utils/augmentation.py
 ml/utils/caching.py
 ml/utils/call_train.py
 ml/utils/checks.py
 ml/utils/cli.py
 ml/utils/colors.py
-ml/utils/compiler.py
 ml/utils/data.py
 ml/utils/datetime.py
 ml/utils/distributed.py
 ml/utils/image.py
 ml/utils/io.py
 ml/utils/large_models.py
 ml/utils/logging.py
```

### Comparing `ml-starter-0.0.27/pyproject.toml` & `ml-starter-0.0.28/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.27/setup.py` & `ml-starter-0.0.28/setup.py`

 * *Files identical despite different names*

