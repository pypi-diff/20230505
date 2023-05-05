# Comparing `tmp/bmtrain-0.2.1.tar.gz` & `tmp/bmtrain-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bmtrain-0.2.1.tar", last modified: Mon Jan 30 03:19:30 2023, max compression
+gzip compressed data, was "dist/bmtrain-0.2.2.tar", last modified: Fri May  5 02:09:17 2023, max compression
```

## Comparing `bmtrain-0.2.1.tar` & `bmtrain-0.2.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-30 03:19:00.000000 bmtrain-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-30 03:19:30.000000 bmtrain-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-01-30 03:19:00.000000 bmtrain-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/benchmark/all_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/benchmark/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/benchmark/send_recv.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/benchmark/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/benchmark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38391 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/block_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/distributed/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/global_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain/inspect/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/inspect/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/inspect/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/inspect/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain/loss/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/loss/cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/lr_scheduler/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/lr_scheduler/no_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/lr_scheduler/noam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/lr_scheduler/warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain/nccl/
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/nccl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/nccl/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/optim/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/optim/adam_offload.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/optim/optim_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/param_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27033 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/pipe_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/synchronize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-01-30 03:19:00.000000 bmtrain-0.2.1/bmtrain/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-30 03:19:30.000000 bmtrain-0.2.1/bmtrain.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/adam_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/adam_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/cross_entropy_loss.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/csrc/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/cuda/adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/cuda/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/cuda/has_inf_nan.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/cuda/reduce.cuh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:19:30.000000 bmtrain-0.2.1/csrc/include/
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/include/nccl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/include/nccl_net.h
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-01-30 03:19:00.000000 bmtrain-0.2.1/csrc/nccl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 03:19:30.000000 bmtrain-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-01-30 03:19:00.000000 bmtrain-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 02:08:46.000000 bmtrain-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 02:09:17.000000 bmtrain-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-05 02:08:46.000000 bmtrain-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/all_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/send_recv.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/benchmark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/block_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/distributed/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/global_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/inspect/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/inspect/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/inspect/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/inspect/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/loss/cross_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/no_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/noam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/lr_scheduler/warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/nccl/
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/nccl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/nccl/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/optim/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/optim/adam_offload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/optim/optim_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/param_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27322 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/pipe_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/synchronize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-05 02:08:46.000000 bmtrain-0.2.2/bmtrain/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 02:09:17.000000 bmtrain-0.2.2/bmtrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/adam_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/adam_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cross_entropy_loss.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/csrc/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cuda/adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cuda/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cuda/has_inf_nan.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/cuda/reduce.cuh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:09:17.000000 bmtrain-0.2.2/csrc/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/include/nccl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/include/nccl_net.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-05 02:08:46.000000 bmtrain-0.2.2/csrc/nccl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:09:17.000000 bmtrain-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-05 02:08:46.000000 bmtrain-0.2.2/setup.py
```

### Comparing `bmtrain-0.2.1/README.md` & `bmtrain-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/__init__.py` & `bmtrain-0.2.2/bmtrain/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/benchmark/all_gather.py` & `bmtrain-0.2.2/bmtrain/benchmark/all_gather.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/benchmark/reduce_scatter.py` & `bmtrain-0.2.2/bmtrain/benchmark/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/benchmark/send_recv.py` & `bmtrain-0.2.2/bmtrain/benchmark/send_recv.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/block_layer.py` & `bmtrain-0.2.2/bmtrain/block_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -525,14 +525,47 @@
                 d_device = self._storage_params[kw_name].device
                 torch.tensor([], dtype=d_dtype, device=d_device).set_(self._storage_params[kw_name].storage(), to_offset_st, (to_offset_end - to_offset_st,))[:] = \
                     torch.tensor([], dtype=d_dtype, device=d_device).set_(contiguous_param.storage(), offset_st, (offset_end - offset_st,))[:]
                 del contiguous_param
             elif strict:
                 missing_keys.append(key)
 
+        for name, param in self.named_parameters():
+            if isinstance(param, DistributedParameter) and not param._in_checkpoint_block:
+                key = prefix + name
+                all_keys.append(key)
+                if key in state_dict:
+                    input_param = state_dict[key]
+                    is_param_lazy = torch.nn.parameter.is_lazy(param)
+                    # Backward compatibility: loading 1-dim tensor from 0.3.* to version 0.4+
+                    if not is_param_lazy and len(param.shape) == 0 and len(input_param.shape) == 1:
+                        input_param = input_param[0]
+
+                    if not is_param_lazy and not isinstance(param, DistributedParameter) and input_param.shape != param.shape:
+                        # local shape should match the one in checkpoint
+                        error_msgs.append('size mismatch for {}: copying a param with shape {} from checkpoint, '
+                                        'the shape in current model is {}.'
+                                        .format(key, input_param.shape, param.shape))
+                        continue
+                    if not is_param_lazy and isinstance(param, DistributedParameter) and input_param.shape != param._original_shape:
+                        error_msgs.append('size mismatch for {}: copying a param with shape {} from checkpoint, '
+                                        'the shape in current model is {}.'
+                                        .format(key, input_param.shape, param.shape))
+                    try:
+                        with torch.no_grad():
+                            param._copy_data(input_param)
+                    except Exception as ex:
+                        error_msgs.append('While copying the parameter named "{}", '
+                                        'whose dimensions in the model are {} and '
+                                        'whose dimensions in the checkpoint are {}, '
+                                        'an exception occurred : {}.'
+                                        .format(key, param.size(), input_param.size(), ex.args))
+                elif strict:
+                    missing_keys.append(key)
+
         if strict:
             all_keys = set(all_keys)
             for key in state_dict.keys():
                 if key.startswith(prefix) and key not in all_keys:
                     unexpected_keys.append(key)
         
     def grouped_parameters(self):
@@ -643,70 +676,80 @@
         self._module.eval()
     
     def __repr__(self):
         return self._module.__repr__()
         
 class OpTransformerBlockList(torch.autograd.Function):
     @staticmethod
-    def forward(ctx, placeholder, self : 'TransformerBlockList', save_list, hidden_state, *args):
+    def forward(ctx, placeholder, self : 'TransformerBlockList', save_list, num_hidden, *args):
         tensors = []
         others = []
-        for arg in args:
+        for arg in args[num_hidden:]:
             if torch.is_tensor(arg):
                 tensors.append(arg)
                 others.append(None)
             else:
                 tensors.append(None)
                 others.append(arg)
+        hidden_states = args[:num_hidden]
     
         ctx.nontensor_inputs = others
         ctx.self = self
         ctx.save_list = copy.deepcopy(save_list)
         ctx.num_save_needed = save_list[-1][1]+1
-        ctx.layers_dict=[{} for _ in range(len(self))]
+        ctx.layers_dict = [{} for _ in range(len(self))]
         layer_inputs = []
         layer_inspector = []
         cuda_rng_state = []
         for i in range(len(self)):
             with torch.no_grad():
                 if save_list[i][0] == i:
-                    layer_inputs.append(hidden_state.detach())
+                    layer_inputs += [hidden_state.detach() for hidden_state in hidden_states]
                 cuda_rng_state.append( torch.cuda.get_rng_state() )
                 if config['zero_level']==2:
                     flag = 1
                 else:
                     flag = 0
                 block_ctx = CheckpointBlockContext(self._modules[str(i)], ctx.layers_dict[i], flag)
                 # gather parameter on load stream
                 block_ctx.enter()
                 # call inner module directly
                 with ScopedTensorInspectorContext() as inspector:
-                    hidden_state = self._modules[str(i)]._module._call_impl(hidden_state, *args)
+                    hidden_states = self._modules[str(i)]._module._call_impl(*hidden_states, *args[num_hidden:])
+                    if not isinstance(hidden_states, tuple):
+                        hidden_states = (hidden_states,)
                 block_ctx.exit()
             for it in inspector.hidden_states:
                 debug.append("_inspect_hidden_states", it)
             layer_inspector.append(inspector.hidden_states)
         
         ctx.layer_inspector = layer_inspector
         ctx.cuda_rng_state = cuda_rng_state
+        ctx.num_hidden = num_hidden
 
         ctx.save_for_backward(*layer_inputs, *tensors)
 
         if self.return_hidden_states:
             middle_hiddens = layer_inputs 
             for mid in middle_hiddens:
                 mid.requires_grad_()
-            middle_hiddens = torch.stack(middle_hiddens, dim=0)
+            middle_hiddens = [
+                torch.stack(middle_hiddens[i::num_hidden], dim=0)
+                for i in range(num_hidden)
+            ]
         else:
-            middle_hiddens = None
-        return tuple([hidden_state, middle_hiddens] + [it["tensor"] for inspector_hiddens in ctx.layer_inspector for it in inspector_hiddens])
+            middle_hiddens = [None] * num_hidden
+        return tuple(list(hidden_states) + middle_hiddens + [it["tensor"] for inspector_hiddens in ctx.layer_inspector for it in inspector_hiddens])
 
 
     @staticmethod
-    def backward(ctx, grad_hidden_state : torch.Tensor, grad_middle: List[torch.Tensor], *grad_inspectors):
+    def backward(ctx, *grads):
+        grad_hidden_states = grads[:ctx.num_hidden]
+        grad_middles = grads[ctx.num_hidden:2*ctx.num_hidden]
+        grad_inspectors = grads[2*ctx.num_hidden:]
         def exit_prev(prev_ctx, prev_grad):
             if prev_ctx is not None:
                 if prev_grad:
                     with torch.enable_grad():
                         prev_ctx.exit()
                         config["load_stream"].record_event(config["load_event"])
                 else:
@@ -718,16 +761,16 @@
             raise RuntimeError(
                 "Checkpointing is not compatible with .grad() or when an `inputs` parameter"
                 " is passed to .backward(). Please use .backward() and do not pass its `inputs`"
                 " argument.")
         all_inputs = []
         input_requires_grad = []
         
-        layer_inputs = ctx.saved_tensors[:ctx.num_save_needed]
-        save_args = ctx.saved_tensors[ctx.num_save_needed:]
+        layer_inputs = ctx.saved_tensors[:ctx.num_save_needed * ctx.num_hidden]
+        save_args = ctx.saved_tensors[ctx.num_save_needed * ctx.num_hidden:]
         for tensor, other in zip(save_args, ctx.nontensor_inputs):
             if tensor is None:
                 all_inputs.append(other)
                 input_requires_grad.append(False)
             else:
                 # detach for tensor inputs
                 input_requires_grad.append( tensor.requires_grad )
@@ -749,62 +792,81 @@
                                 if config['zero_level'] == 2:
                                     flag = 2
                                 else:
                                     flag = 0
                                 block_ctx = CheckpointBlockContext(ctx.self._modules[str(j)], ctx.layers_dict[j], flag)
                                 block_ctx.enter()
                                 exit_prev(prev_ctx, prev_grad)
-                                output = ctx.self._modules[str(j)]._module._call_impl(layer_inputs[ctx.save_list[j][1]], *all_inputs)
+                                outputs = ctx.self._modules[str(j)]._module._call_impl(
+                                    layer_inputs[ctx.save_list[j][1]*ctx.num_hidden: ctx.save_list[j][1]*ctx.num_hidden+ctx.num_hidden],
+                                    *all_inputs
+                                )
+                                if not isinstance(outputs, tuple):
+                                    outputs = (outputs,)
                                 prev_ctx = block_ctx
                                 prev_grad = False
-                                layer_inputs[ctx.save_list[j+1][1]].copy_(output)
+                                for k, output in enumerate(outputs):
+                                    layer_inputs[ctx.save_list[j+1][1]*ctx.num_hidden + k].copy_(output)
                                 ctx.save_list[j+1][0] = j+1
                 
                     torch.cuda.set_rng_state(ctx.cuda_rng_state[i])
-                    ipt = layer_inputs[ctx.save_list[i][1]].requires_grad_()
+                    ipts = [
+                        layer_inputs[ctx.save_list[i][1]*ctx.num_hidden + k].detach().requires_grad_()
+                        for k in range(ctx.num_hidden)
+                    ]
                     if config['zero_level'] == 2:
                         flag = 2
                     else:
                         flag = 0
                     block_ctx = CheckpointBlockContext(ctx.self._modules[str(i)], ctx.layers_dict[i], flag)
                     block_ctx.enter()
                     exit_prev(prev_ctx, prev_grad)
                     prev_ctx = block_ctx
                     prev_grad = True
 
                     with ScopedTensorInspectorContext() as inspector:
-                        output = ctx.self._modules[str(i)]._module._call_impl(ipt, *all_inputs)
+                        outputs = ctx.self._modules[str(i)]._module._call_impl(*ipts, *all_inputs)
+                        if not isinstance(outputs, tuple):
+                            outputs = (outputs,)
                     
                     assert len(ctx.layer_inspector[i]) == len(inspector.hidden_states), "Backward step changed"
                     for j, it in enumerate(inspector.hidden_states):
                         assert it["name"] == ctx.layer_inspector[i][j]["name"], "Backward step changed"
                         assert it["shape"] == ctx.layer_inspector[i][j]["shape"], "Backward step changed"
                         assert it["group"] == ctx.layer_inspector[i][j]["group"], "Backward step changed"
                         
                         # change the tensor in placeholder
                         ctx.layer_inspector[i][j]["tensor"] = it["tensor"]
                         ctx.layer_inspector[i][j]["requires_grad"] = it["requires_grad"]
-                    torch.autograd.backward(
-                        [output] + [hidden_state["tensor"] for hidden_state in inspector.hidden_states],
-                        (grad_hidden_state,) + grad_inspectors[-len(inspector.hidden_states):],
-                    )
-                    grad_inspectors = grad_inspectors[:-len(inspector.hidden_states)]
-                    grad_hidden_state = ipt.grad
-                    if grad_middle is not None:
-                        grad_hidden_state = grad_hidden_state + grad_middle[i]
+                    if len(inspector.hidden_states) > 0:
+                        torch.autograd.backward(
+                            list(outputs) + [hidden_state["tensor"] for hidden_state in inspector.hidden_states],
+                            grad_hidden_states + grad_inspectors[-len(inspector.hidden_states):],
+                        )
+                        grad_inspectors = grad_inspectors[:-len(inspector.hidden_states)]
+                    else:
+                        torch.autograd.backward(
+                            outputs,
+                            grad_hidden_states,
+                        )
+                    grad_hidden_states = [ipt.grad for ipt in ipts]
+                    for k in range(ctx.num_hidden):
+                        if grad_middles[k] is not None:
+                            grad_hidden_states[k] = grad_hidden_states[k] + grad_middles[k][i]
+                    grad_hidden_states = tuple(grad_hidden_states)
                 
                 exit_prev(prev_ctx, prev_grad)
 
         grads = []
         for inp, requires_grad in zip(all_inputs, input_requires_grad):
             if requires_grad:
                 grads.append(inp.grad)
             else:
                 grads.append(None)
-        return (None, None, None, grad_hidden_state) + tuple(grads)
+        return (None, None, None, None) + tuple(grad_hidden_states) + tuple(grads)
     
 class TransformerBlockList(torch.nn.Module):
     r"""
     TransformerBlockList is a list of CheckpointBlocks.
 
     This is designed to reduce the communication overhead by overlapping the computation and reduce_scatter operation during backward pass.
 
@@ -819,24 +881,26 @@
         >>>     hidden_state = layer.forward(hidden_state, ...)
         >>> # Calling transformer module list
         >>> hidden_state = transformer_module_list(hidden_state, ...)
 
     """
     _modules: Dict[str, CheckpointBlock]
 
-    def __init__(self, modules: Iterable[CheckpointBlock], sqrt=False) -> None:
+    def __init__(self, modules: Iterable[CheckpointBlock], num_hidden=1, sqrt=False) -> None:
         super().__init__()
         
         self._modules = {}
         for i, module in enumerate(modules):
             if not isinstance(module, CheckpointBlock):
                 module = CheckpointBlock(module)
             self._modules[str(i)] = module
             self.add_module(str(i), module)
 
+        self.num_hidden = num_hidden
+
         if sqrt:
             length = len(self)
             num_save_needed = 0
             num_freed = 0
             save_list = [None]*length
             for i in range(length-1, -1, -1):
                 if num_freed == 0 or i == 0:
@@ -858,16 +922,15 @@
     def __len__(self) -> int:
         return len(self._modules)
     def __iter__(self) -> Iterator[CheckpointBlock]:
         return iter(self._modules.values())
     def __getitem__(self, index: Union[int, str]) -> CheckpointBlock:
         return self._modules[str(index)]
 
-    def forward(self, hidden_state, *args, return_hidden_states = False):
+    def forward(self, *args, return_hidden_states = False):
         self.return_hidden_states = return_hidden_states
         placeholder = torch.tensor([], requires_grad=torch.is_grad_enabled())
-        outputs = OpTransformerBlockList.apply(placeholder, self, self.save_list, hidden_state, *args)
-        last_hidden, middle_hiddens = outputs[:2]
+        outputs = OpTransformerBlockList.apply(placeholder, self, self.save_list, self.num_hidden, *args)
         if return_hidden_states:
-            return last_hidden, middle_hiddens
+            return tuple(outputs[:2*self.num_hidden])
         else:
-            return last_hidden
+            return tuple(outputs[:self.num_hidden]) if self.num_hidden > 1 else outputs[0]
```

### Comparing `bmtrain-0.2.1/bmtrain/checkpointing.py` & `bmtrain-0.2.2/bmtrain/checkpointing.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/debug.py` & `bmtrain-0.2.2/bmtrain/debug.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/distributed/ops.py` & `bmtrain-0.2.2/bmtrain/distributed/ops.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/global_var.py` & `bmtrain-0.2.2/bmtrain/global_var.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/init.py` & `bmtrain-0.2.2/bmtrain/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,20 @@
     """
     torch.backends.cudnn.enabled = False
 
     local_rank = int(os.environ.get("LOCAL_RANK", "0"))
     rank = int(os.environ.get("RANK", "0"))
     world_size = int(os.environ.get("WORLD_SIZE", "1"))
     local_size = int(os.environ.get("LOCAL_WORLD_SIZE","1"))
-    addr = os.environ.get("MASTER_ADDR", "localhost")
-    port = os.environ.get("MASTER_PORT", "10010")
+    if "MASTER_ADDR" not in os.environ:
+        os.environ["MASTER_ADDR"]="localhost"
+    if "MASTER_PORT" not in os.environ:
+        os.environ["MASTER_PORT"]="10010"
+    addr = os.environ["MASTER_ADDR"]
+    port = os.environ["MASTER_PORT"]
     master = addr+":"+port
     timeout = datetime.timedelta(seconds=1800)
     rendezvous_iterator = dist.rendezvous(
         init_method, rank, world_size, timeout=timeout
     )
     store, rank, world_size = next(rendezvous_iterator)
     store.set_timeout(timeout)
```

### Comparing `bmtrain-0.2.1/bmtrain/inspect/format.py` & `bmtrain-0.2.2/bmtrain/inspect/format.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/inspect/model.py` & `bmtrain-0.2.2/bmtrain/inspect/model.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/inspect/tensor.py` & `bmtrain-0.2.2/bmtrain/inspect/tensor.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/layer.py` & `bmtrain-0.2.2/bmtrain/layer.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/loss/cross_entropy.py` & `bmtrain-0.2.2/bmtrain/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/lr_scheduler/cosine.py` & `bmtrain-0.2.2/bmtrain/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/lr_scheduler/exponential.py` & `bmtrain-0.2.2/bmtrain/lr_scheduler/exponential.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/lr_scheduler/linear.py` & `bmtrain-0.2.2/bmtrain/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/lr_scheduler/noam.py` & `bmtrain-0.2.2/bmtrain/lr_scheduler/noam.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/lr_scheduler/warmup.py` & `bmtrain-0.2.2/bmtrain/lr_scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/nccl/__init__.py` & `bmtrain-0.2.2/bmtrain/nccl/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/optim/adam.py` & `bmtrain-0.2.2/bmtrain/optim/adam.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,25 @@
             raise ValueError("Invalid beta parameter at index 1: {}".format(betas[1]))
         if not 0.0 <= weight_decay:
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
 
         defaults = dict(lr=lr, betas=betas, eps=eps, weight_decay=weight_decay)
         super().__init__(params, defaults)
 
-        self.load_stream = torch.cuda.Stream()
         self._hold_steps = hold_steps
 
     def _on_justify_scale(self, old_scale, new_scale):
         delta = new_scale / old_scale
         for group in self.param_groups:
             for p in group['params']:
-                state = self.state[p]
-                if len(state) > 0:
-                    state['exp_avg'] *= delta
-                    state['exp_avg_sq'] *= delta
+                if p in self.state:
+                    state = self.state[p]
+                    if len(state) > 0:
+                        state['exp_avg'] *= delta
+                        state['exp_avg_sq'] *= delta
 
     @torch.no_grad()
     def step(self, closure=None, scale=1):
         """Performs a single optimization step.
         Arguments:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
```

### Comparing `bmtrain-0.2.1/bmtrain/optim/adam_offload.py` & `bmtrain-0.2.2/bmtrain/optim/adam_offload.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/optim/optim_manager.py` & `bmtrain-0.2.2/bmtrain/optim/optim_manager.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/param_init.py` & `bmtrain-0.2.2/bmtrain/param_init.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
     modules = model.named_modules()
     for module_prefix, module in modules:
         if isinstance(module, CheckpointBlock):
             module.init_parameters()
         else:
             init_distributed_parameter( iterate_parameters(module) )
+    
+    current_stream = torch.cuda.current_stream()
+    config['load_stream'].wait_stream(current_stream)
 
 def grouped_parameters(model : torch.nn.Module) -> Generator[Tuple[str, List[torch.nn.Parameter]], None, None]:
     """
     Iterate over the parameters of the model grouped by the group name.
     This is similar to `torch.nn.Module.named_parameters()` .
     """
```

### Comparing `bmtrain-0.2.1/bmtrain/parameter.py` & `bmtrain-0.2.2/bmtrain/parameter.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/pipe_layer.py` & `bmtrain-0.2.2/bmtrain/pipe_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,19 +125,25 @@
                             assert it["name"] == ctx.layer_inspector[idx][j]["name"], "Backward step changed"
                             assert it["shape"] == ctx.layer_inspector[idx][j]["shape"], "Backward step changed"
                             assert it["group"] == ctx.layer_inspector[idx][j]["group"], "Backward step changed"
                             
                             # change the tensor in placeholder
                             ctx.layer_inspector[idx][j]["tensor"] = it["tensor"]
                             ctx.layer_inspector[idx][j]["requires_grad"] = it["requires_grad"]
-                        torch.autograd.backward(
-                            [output] + [hidden_state["tensor"] for hidden_state in inspector.hidden_states],
-                            [grad_hidden_state] + list(grad_inspector[-len(inspector.hidden_states):]),
-                        )
-                        grad_inspector = grad_inspector[:-len(inspector.hidden_states)]
+                        if len(inspector.hidden_states) > 0:
+                            torch.autograd.backward(
+                                [output] + [hidden_state["tensor"] for hidden_state in inspector.hidden_states],
+                                [grad_hidden_state] + list(grad_inspector[-len(inspector.hidden_states):]),
+                            )
+                            grad_inspector = grad_inspector[:-len(inspector.hidden_states)]
+                        else:
+                            torch.autograd.backward(
+                                [output],
+                                [grad_hidden_state],
+                            )
                         grad_hidden_state = ipt.grad
                         if grad_middle is not None:
                             grad_hidden_state = grad_hidden_state + grad_middle[idx]
                     if ctx.micro_idx == config["micros"]-1:
                         exit_prev(prev_ctx, prev_grad)
                 for inspector_hiddens in ctx.layer_inspector:
                     for it in inspector_hiddens:
```

### Comparing `bmtrain-0.2.1/bmtrain/store.py` & `bmtrain-0.2.2/bmtrain/store.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/synchronize.py` & `bmtrain-0.2.2/bmtrain/synchronize.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/utils.py` & `bmtrain-0.2.2/bmtrain/utils.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain/wrapper.py` & `bmtrain-0.2.2/bmtrain/wrapper.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/bmtrain.egg-info/SOURCES.txt` & `bmtrain-0.2.2/bmtrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/adam_cpu.cpp` & `bmtrain-0.2.2/csrc/adam_cpu.cpp`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/adam_cuda.cpp` & `bmtrain-0.2.2/csrc/adam_cuda.cpp`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/cross_entropy_loss.cpp` & `bmtrain-0.2.2/csrc/cross_entropy_loss.cpp`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/cuda/adam.cu` & `bmtrain-0.2.2/csrc/cuda/adam.cu`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/cuda/cross_entropy.cu` & `bmtrain-0.2.2/csrc/cuda/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/cuda/has_inf_nan.cu` & `bmtrain-0.2.2/csrc/cuda/has_inf_nan.cu`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/cuda/reduce.cuh` & `bmtrain-0.2.2/csrc/cuda/reduce.cuh`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/include/nccl.h` & `bmtrain-0.2.2/csrc/include/nccl.h`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/include/nccl_net.h` & `bmtrain-0.2.2/csrc/include/nccl_net.h`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/csrc/nccl.cpp` & `bmtrain-0.2.2/csrc/nccl.cpp`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.1/setup.py` & `bmtrain-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         ], extra_compile_args={}),
     ]
 else:
     ext_modules = []
 
 setup(
     name='bmtrain',
-    version='0.2.1',
+    version='0.2.2',
     author="Guoyang Zeng",
     author_email="qbjooo@qq.com",
     description="A toolkit for training big models",
     packages=find_packages(),
     install_requires=[
         "numpy",
     ],
```

