# Comparing `tmp/repvgg-pytorch-1.0.0.tar.gz` & `tmp/repvgg-pytorch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repvgg-pytorch-1.0.0.tar", last modified: Thu May  4 22:07:46 2023, max compression
+gzip compressed data, was "repvgg-pytorch-1.0.1.tar", last modified: Fri May  5 08:55:24 2023, max compression
```

## Comparing `repvgg-pytorch-1.0.0.tar` & `repvgg-pytorch-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-04 22:07:46.631906 repvgg-pytorch-1.0.0/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1062 2023-05-04 16:27:06.000000 repvgg-pytorch-1.0.0/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      604 2023-05-04 22:07:46.631906 repvgg-pytorch-1.0.0/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2639 2023-05-04 21:59:24.000000 repvgg-pytorch-1.0.0/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-04 22:07:46.631906 repvgg-pytorch-1.0.0/repvgg_pytorch/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      178 2023-05-04 21:41:51.000000 repvgg-pytorch-1.0.0/repvgg_pytorch/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16875 2023-05-04 19:31:13.000000 repvgg-pytorch-1.0.0/repvgg_pytorch/repvgg.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    17679 2023-05-04 19:37:53.000000 repvgg-pytorch-1.0.0/repvgg_pytorch/repvggplus.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      867 2023-05-04 16:28:02.000000 repvgg-pytorch-1.0.0/repvgg_pytorch/se_block.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-04 22:07:46.631906 repvgg-pytorch-1.0.0/repvgg_pytorch.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      604 2023-05-04 22:07:45.000000 repvgg-pytorch-1.0.0/repvgg_pytorch.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      323 2023-05-04 22:07:45.000000 repvgg-pytorch-1.0.0/repvgg_pytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-04 22:07:45.000000 repvgg-pytorch-1.0.0/repvgg_pytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-04 22:07:45.000000 repvgg-pytorch-1.0.0/repvgg_pytorch.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       15 2023-05-04 22:07:45.000000 repvgg-pytorch-1.0.0/repvgg_pytorch.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-04 22:07:46.631906 repvgg-pytorch-1.0.0/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      952 2023-05-04 20:40:57.000000 repvgg-pytorch-1.0.0/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 08:55:24.507593 repvgg-pytorch-1.0.1/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1062 2023-05-04 16:27:06.000000 repvgg-pytorch-1.0.1/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3240 2023-05-05 08:55:24.507593 repvgg-pytorch-1.0.1/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2634 2023-05-04 22:16:11.000000 repvgg-pytorch-1.0.1/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 08:55:24.507593 repvgg-pytorch-1.0.1/repvgg_pytorch/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      178 2023-05-04 21:41:51.000000 repvgg-pytorch-1.0.1/repvgg_pytorch/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16875 2023-05-04 19:31:13.000000 repvgg-pytorch-1.0.1/repvgg_pytorch/repvgg.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    17679 2023-05-04 19:37:53.000000 repvgg-pytorch-1.0.1/repvgg_pytorch/repvggplus.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      867 2023-05-04 16:28:02.000000 repvgg-pytorch-1.0.1/repvgg_pytorch/se_block.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 08:55:24.507593 repvgg-pytorch-1.0.1/repvgg_pytorch.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3240 2023-05-05 08:55:24.000000 repvgg-pytorch-1.0.1/repvgg_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      323 2023-05-05 08:55:24.000000 repvgg-pytorch-1.0.1/repvgg_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-05 08:55:24.000000 repvgg-pytorch-1.0.1/repvgg_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-05 08:55:24.000000 repvgg-pytorch-1.0.1/repvgg_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       15 2023-05-05 08:55:24.000000 repvgg-pytorch-1.0.1/repvgg_pytorch.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-05 08:55:24.507593 repvgg-pytorch-1.0.1/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1150 2023-05-05 08:43:08.000000 repvgg-pytorch-1.0.1/setup.py
```

### Comparing `repvgg-pytorch-1.0.0/LICENSE` & `repvgg-pytorch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repvgg-pytorch-1.0.0/README.md` & `repvgg-pytorch-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 🎁 Repvgg-packaged 🎁
+# Repvgg-packaged 🎁
 
 A Python-packaged version of RepVGG: Making VGG-style ConvNets Great Again 🚀. The main contribution of this repo is to provide an easy-to-use backbone for RepVGG, which can be effortlessly used for downstream computer vision tasks
 
 This project is based on the excellent original RepVGG implementation by authors Ding, Xiaohan et al. 🌟:
 - [GitHub repository (code)](https://github.com/DingXiaoH/RepVGG)
 - [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Ding_RepVGG_Making_VGG-Style_ConvNets_Great_Again_CVPR_2021_paper.pdf)
```

### Comparing `repvgg-pytorch-1.0.0/repvgg_pytorch/repvgg.py` & `repvgg-pytorch-1.0.1/repvgg_pytorch/repvgg.py`

 * *Files identical despite different names*

### Comparing `repvgg-pytorch-1.0.0/repvgg_pytorch/repvggplus.py` & `repvgg-pytorch-1.0.1/repvgg_pytorch/repvggplus.py`

 * *Files identical despite different names*

### Comparing `repvgg-pytorch-1.0.0/repvgg_pytorch/se_block.py` & `repvgg-pytorch-1.0.1/repvgg_pytorch/se_block.py`

 * *Files identical despite different names*

