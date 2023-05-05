# Comparing `tmp/diffq-0.2.3.tar.gz` & `tmp/diffq-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffq-0.2.3.tar", last modified: Wed Aug 24 15:32:56 2022, max compression
+gzip compressed data, was "diffq-0.2.4.tar", last modified: Fri May  5 12:28:06 2023, max compression
```

## Comparing `diffq-0.2.3.tar` & `diffq-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-08-24 15:32:56.700776 diffq-0.2.3/
--rw-r--r--   0 defossez   (501) staff       (20)      351 2022-08-24 14:50:55.000000 diffq-0.2.3/CHANGELOG.md
--rw-r--r--   0 defossez   (501) staff       (20)     3355 2021-02-18 17:37:21.000000 diffq-0.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 defossez   (501) staff       (20)      826 2021-02-23 17:23:17.000000 diffq-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 defossez   (501) staff       (20)    19332 2021-02-18 17:37:21.000000 diffq-0.2.3/LICENSE
--rw-r--r--   0 defossez   (501) staff       (20)      176 2021-12-10 13:37:50.000000 diffq-0.2.3/MANIFEST.in
--rw-r--r--   0 defossez   (501) staff       (20)      697 2021-10-28 12:15:41.000000 diffq-0.2.3/Makefile
--rw-r--r--   0 defossez   (501) staff       (20)     9943 2022-08-24 15:32:56.701178 diffq-0.2.3/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)     7819 2022-08-24 14:51:26.000000 diffq-0.2.3/README.md
--rw-r--r--   0 defossez   (501) staff       (20)     2987 2021-11-22 10:59:58.000000 diffq-0.2.3/bitpack.pyx
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-08-24 15:32:56.674935 diffq-0.2.3/diffq/
--rw-r--r--   0 defossez   (501) staff       (20)     1050 2022-08-24 14:50:30.000000 diffq-0.2.3/diffq/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)    12075 2021-11-22 10:59:58.000000 diffq-0.2.3/diffq/base.py
--rw-r--r--   0 defossez   (501) staff       (20)    13499 2022-08-24 13:58:27.000000 diffq-0.2.3/diffq/diffq.py
--rw-r--r--   0 defossez   (501) staff       (20)     6818 2021-11-22 10:59:58.000000 diffq-0.2.3/diffq/lsq.py
--rw-r--r--   0 defossez   (501) staff       (20)     3003 2021-11-22 10:59:58.000000 diffq-0.2.3/diffq/torch_pack.py
--rw-r--r--   0 defossez   (501) staff       (20)     7679 2022-03-03 15:23:09.000000 diffq-0.2.3/diffq/ts_export.py
--rw-r--r--   0 defossez   (501) staff       (20)     4745 2021-11-22 10:59:58.000000 diffq-0.2.3/diffq/uniform.py
--rw-r--r--   0 defossez   (501) staff       (20)     1736 2021-10-20 16:09:37.000000 diffq-0.2.3/diffq/utils.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-08-24 15:32:56.677835 diffq-0.2.3/diffq.egg-info/
--rw-r--r--   0 defossez   (501) staff       (20)     9943 2022-08-24 15:32:56.000000 diffq-0.2.3/diffq.egg-info/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)      854 2022-08-24 15:32:56.000000 diffq-0.2.3/diffq.egg-info/SOURCES.txt
--rw-r--r--   0 defossez   (501) staff       (20)        1 2022-08-24 15:32:56.000000 diffq-0.2.3/diffq.egg-info/dependency_links.txt
--rw-r--r--   0 defossez   (501) staff       (20)       60 2022-08-24 15:32:56.000000 diffq-0.2.3/diffq.egg-info/requires.txt
--rw-r--r--   0 defossez   (501) staff       (20)        6 2022-08-24 15:32:56.000000 diffq-0.2.3/diffq.egg-info/top_level.txt
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-08-24 15:32:56.660688 diffq-0.2.3/examples/
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-08-24 15:32:56.678415 diffq-0.2.3/examples/cifar/
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-08-24 15:32:56.679036 diffq-0.2.3/examples/cifar/conf/
--rw-r--r--   0 defossez   (501) staff       (20)     3279 2021-11-08 13:49:10.000000 diffq-0.2.3/examples/cifar/conf/config.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-08-24 15:32:56.681136 diffq-0.2.3/examples/cifar/conf/preset/
--rw-r--r--   0 defossez   (501) staff       (20)       32 2021-11-08 13:49:10.000000 diffq-0.2.3/examples/cifar/conf/preset/default.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      237 2021-11-08 13:49:10.000000 diffq-0.2.3/examples/cifar/conf/preset/res20.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-08-24 15:32:56.699678 diffq-0.2.3/examples/cifar/src/
--rw-r--r--   0 defossez   (501) staff       (20)      196 2021-11-08 13:49:10.000000 diffq-0.2.3/examples/cifar/src/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     2328 2022-03-03 15:23:09.000000 diffq-0.2.3/examples/cifar/src/data.py
--rw-r--r--   0 defossez   (501) staff       (20)     2774 2021-11-05 09:43:23.000000 diffq-0.2.3/examples/cifar/src/distrib.py
--rw-r--r--   0 defossez   (501) staff       (20)     2886 2021-11-05 09:43:26.000000 diffq-0.2.3/examples/cifar/src/executor.py
--rw-r--r--   0 defossez   (501) staff       (20)     3391 2021-11-05 09:43:34.000000 diffq-0.2.3/examples/cifar/src/mobilenet.py
--rw-r--r--   0 defossez   (501) staff       (20)     5686 2021-11-05 09:43:39.000000 diffq-0.2.3/examples/cifar/src/resnet.py
--rw-r--r--   0 defossez   (501) staff       (20)     6891 2021-11-08 13:49:10.000000 diffq-0.2.3/examples/cifar/src/resnet20.py
--rw-r--r--   0 defossez   (501) staff       (20)    11302 2021-11-08 13:49:10.000000 diffq-0.2.3/examples/cifar/src/solver.py
--rw-r--r--   0 defossez   (501) staff       (20)     2630 2021-11-05 09:43:51.000000 diffq-0.2.3/examples/cifar/src/utils.py
--rw-r--r--   0 defossez   (501) staff       (20)     5773 2022-03-03 15:24:33.000000 diffq-0.2.3/examples/cifar/src/vit.py
--rw-r--r--   0 defossez   (501) staff       (20)     4311 2021-11-05 09:43:54.000000 diffq-0.2.3/examples/cifar/src/wide_resnet.py
--rwxr-xr-x   0 defossez   (501) staff       (20)     5837 2022-03-03 15:25:13.000000 diffq-0.2.3/examples/cifar/train.py
--rw-r--r--   0 defossez   (501) staff       (20)      127 2022-08-24 15:32:56.702704 diffq-0.2.3/setup.cfg
--rw-r--r--   0 defossez   (501) staff       (20)     1777 2021-11-22 10:59:58.000000 diffq-0.2.3/setup.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-05 12:28:06.423456 diffq-0.2.4/
+-rw-r--r--   0 defossez   (501) staff       (20)      414 2023-05-05 10:46:10.000000 diffq-0.2.4/CHANGELOG.md
+-rw-r--r--   0 defossez   (501) staff       (20)     3355 2021-02-18 17:37:21.000000 diffq-0.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 defossez   (501) staff       (20)      826 2021-02-23 17:23:17.000000 diffq-0.2.4/CONTRIBUTING.md
+-rw-r--r--   0 defossez   (501) staff       (20)    19332 2021-02-18 17:37:21.000000 diffq-0.2.4/LICENSE
+-rw-r--r--   0 defossez   (501) staff       (20)      176 2021-12-10 13:37:50.000000 diffq-0.2.4/MANIFEST.in
+-rw-r--r--   0 defossez   (501) staff       (20)      697 2021-10-28 12:15:41.000000 diffq-0.2.4/Makefile
+-rw-r--r--   0 defossez   (501) staff       (20)     9916 2023-05-05 12:28:06.423672 diffq-0.2.4/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)     7792 2023-05-05 10:45:19.000000 diffq-0.2.4/README.md
+-rw-r--r--   0 defossez   (501) staff       (20)   876872 2023-05-05 12:28:06.000000 diffq-0.2.4/bitpack.c
+-rw-r--r--   0 defossez   (501) staff       (20)     2987 2021-11-22 10:59:58.000000 diffq-0.2.4/bitpack.pyx
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-05 12:28:06.396627 diffq-0.2.4/diffq/
+-rw-r--r--   0 defossez   (501) staff       (20)     1050 2023-05-05 10:45:25.000000 diffq-0.2.4/diffq/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)    12075 2021-11-22 10:59:58.000000 diffq-0.2.4/diffq/base.py
+-rw-r--r--   0 defossez   (501) staff       (20)    13499 2022-08-24 13:58:27.000000 diffq-0.2.4/diffq/diffq.py
+-rw-r--r--   0 defossez   (501) staff       (20)     6818 2021-11-22 10:59:58.000000 diffq-0.2.4/diffq/lsq.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3003 2021-11-22 10:59:58.000000 diffq-0.2.4/diffq/torch_pack.py
+-rw-r--r--   0 defossez   (501) staff       (20)     7679 2022-03-03 15:23:09.000000 diffq-0.2.4/diffq/ts_export.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4745 2021-11-22 10:59:58.000000 diffq-0.2.4/diffq/uniform.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1736 2021-10-20 16:09:37.000000 diffq-0.2.4/diffq/utils.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-05 12:28:06.402389 diffq-0.2.4/diffq.egg-info/
+-rw-r--r--   0 defossez   (501) staff       (20)     9916 2023-05-05 12:28:06.000000 diffq-0.2.4/diffq.egg-info/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)      879 2023-05-05 12:28:06.000000 diffq-0.2.4/diffq.egg-info/SOURCES.txt
+-rw-r--r--   0 defossez   (501) staff       (20)        1 2023-05-05 12:28:06.000000 diffq-0.2.4/diffq.egg-info/dependency_links.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       60 2023-05-05 12:28:06.000000 diffq-0.2.4/diffq.egg-info/requires.txt
+-rw-r--r--   0 defossez   (501) staff       (20)        6 2023-05-05 12:28:06.000000 diffq-0.2.4/diffq.egg-info/top_level.txt
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-05 12:28:06.376969 diffq-0.2.4/examples/
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-05 12:28:06.403282 diffq-0.2.4/examples/cifar/
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-05 12:28:06.404782 diffq-0.2.4/examples/cifar/conf/
+-rw-r--r--   0 defossez   (501) staff       (20)     3279 2021-11-08 13:49:10.000000 diffq-0.2.4/examples/cifar/conf/config.yaml
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-05 12:28:06.410925 diffq-0.2.4/examples/cifar/conf/preset/
+-rw-r--r--   0 defossez   (501) staff       (20)       32 2021-11-08 13:49:10.000000 diffq-0.2.4/examples/cifar/conf/preset/default.yaml
+-rw-r--r--   0 defossez   (501) staff       (20)      237 2021-11-08 13:49:10.000000 diffq-0.2.4/examples/cifar/conf/preset/res20.yaml
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-05 12:28:06.422677 diffq-0.2.4/examples/cifar/src/
+-rw-r--r--   0 defossez   (501) staff       (20)      196 2021-11-08 13:49:10.000000 diffq-0.2.4/examples/cifar/src/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2328 2022-03-03 15:23:09.000000 diffq-0.2.4/examples/cifar/src/data.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2774 2021-11-05 09:43:23.000000 diffq-0.2.4/examples/cifar/src/distrib.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2886 2021-11-05 09:43:26.000000 diffq-0.2.4/examples/cifar/src/executor.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3391 2021-11-05 09:43:34.000000 diffq-0.2.4/examples/cifar/src/mobilenet.py
+-rw-r--r--   0 defossez   (501) staff       (20)     5686 2021-11-05 09:43:39.000000 diffq-0.2.4/examples/cifar/src/resnet.py
+-rw-r--r--   0 defossez   (501) staff       (20)     6891 2021-11-08 13:49:10.000000 diffq-0.2.4/examples/cifar/src/resnet20.py
+-rw-r--r--   0 defossez   (501) staff       (20)    11302 2021-11-08 13:49:10.000000 diffq-0.2.4/examples/cifar/src/solver.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2630 2021-11-05 09:43:51.000000 diffq-0.2.4/examples/cifar/src/utils.py
+-rw-r--r--   0 defossez   (501) staff       (20)     5773 2022-03-03 15:24:33.000000 diffq-0.2.4/examples/cifar/src/vit.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4311 2021-11-05 09:43:54.000000 diffq-0.2.4/examples/cifar/src/wide_resnet.py
+-rwxr-xr-x   0 defossez   (501) staff       (20)     5837 2022-03-03 15:25:13.000000 diffq-0.2.4/examples/cifar/train.py
+-rw-r--r--   0 defossez   (501) staff       (20)       60 2023-05-05 10:45:19.000000 diffq-0.2.4/pyproject.toml
+-rw-r--r--   0 defossez   (501) staff       (20)      127 2023-05-05 12:28:06.424397 diffq-0.2.4/setup.cfg
+-rw-r--r--   0 defossez   (501) staff       (20)     1823 2023-05-05 10:45:19.000000 diffq-0.2.4/setup.py
```

### Comparing `diffq-0.2.3/CODE_OF_CONDUCT.md` & `diffq-0.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/CONTRIBUTING.md` & `diffq-0.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/LICENSE` & `diffq-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/Makefile` & `diffq-0.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/PKG-INFO` & `diffq-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffq
-Version: 0.2.3
+Version: 0.2.4
 Summary: Differentiable quantization framework for PyTorch.
 Home-page: https://github.com/facebookresearch/diffq
 Author: Alexandre Défossez, Yossi Adi, Gabriel Synnaeve
 Author-email: defossez@fb.com
 License: Creative Commons Attribution-NonCommercial 4.0 International
 Description: 
         # Differentiable Model Compression via Pseudo Quantization Noise
@@ -188,16 +188,16 @@
         
         If you use this code or results in your paper, please cite our work as:
         
         ```
         @article{defossez2021differentiable,
           title={Differentiable Model Compression via Pseudo Quantization Noise},
           author={D{\'e}fossez, Alexandre and Adi, Yossi and Synnaeve, Gabriel},
-          journal={arXiv preprint arXiv:2104.09987},
-          year={2021}
+          journal={TMLR},
+          year={2022}
         }
         ```
         
         ## License
         
         This repository is released under the CC-BY-NC 4.0. license as found in the
         [LICENSE](LICENSE) file, except for the following parts that is under the MIT license.
```

### Comparing `diffq-0.2.3/README.md` & `diffq-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,16 @@
 
 If you use this code or results in your paper, please cite our work as:
 
 ```
 @article{defossez2021differentiable,
   title={Differentiable Model Compression via Pseudo Quantization Noise},
   author={D{\'e}fossez, Alexandre and Adi, Yossi and Synnaeve, Gabriel},
-  journal={arXiv preprint arXiv:2104.09987},
-  year={2021}
+  journal={TMLR},
+  year={2022}
 }
 ```
 
 ## License
 
 This repository is released under the CC-BY-NC 4.0. license as found in the
 [LICENSE](LICENSE) file, except for the following parts that is under the MIT license.
```

### Comparing `diffq-0.2.3/bitpack.pyx` & `diffq-0.2.4/bitpack.pyx`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/diffq/__init__.py` & `diffq-0.2.4/diffq/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 from .uniform import UniformQuantizer
 from .diffq import DiffQuantizer
 from .lsq import LSQ
 from .base import restore_quantized_state
 from . import ts_export
 
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
```

### Comparing `diffq-0.2.3/diffq/base.py` & `diffq-0.2.4/diffq/base.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/diffq/diffq.py` & `diffq-0.2.4/diffq/diffq.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/diffq/lsq.py` & `diffq-0.2.4/diffq/lsq.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/diffq/torch_pack.py` & `diffq-0.2.4/diffq/torch_pack.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/diffq/ts_export.py` & `diffq-0.2.4/diffq/ts_export.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/diffq/uniform.py` & `diffq-0.2.4/diffq/uniform.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/diffq/utils.py` & `diffq-0.2.4/diffq/utils.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/diffq.egg-info/PKG-INFO` & `diffq-0.2.4/diffq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffq
-Version: 0.2.3
+Version: 0.2.4
 Summary: Differentiable quantization framework for PyTorch.
 Home-page: https://github.com/facebookresearch/diffq
 Author: Alexandre Défossez, Yossi Adi, Gabriel Synnaeve
 Author-email: defossez@fb.com
 License: Creative Commons Attribution-NonCommercial 4.0 International
 Description: 
         # Differentiable Model Compression via Pseudo Quantization Noise
@@ -188,16 +188,16 @@
         
         If you use this code or results in your paper, please cite our work as:
         
         ```
         @article{defossez2021differentiable,
           title={Differentiable Model Compression via Pseudo Quantization Noise},
           author={D{\'e}fossez, Alexandre and Adi, Yossi and Synnaeve, Gabriel},
-          journal={arXiv preprint arXiv:2104.09987},
-          year={2021}
+          journal={TMLR},
+          year={2022}
         }
         ```
         
         ## License
         
         This repository is released under the CC-BY-NC 4.0. license as found in the
         [LICENSE](LICENSE) file, except for the following parts that is under the MIT license.
```

### Comparing `diffq-0.2.3/diffq.egg-info/SOURCES.txt` & `diffq-0.2.4/diffq.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
+bitpack.c
 bitpack.pyx
+pyproject.toml
 setup.cfg
 setup.py
 diffq/__init__.py
 diffq/base.py
 diffq/diffq.py
 diffq/lsq.py
 diffq/torch_pack.py
```

### Comparing `diffq-0.2.3/examples/cifar/conf/config.yaml` & `diffq-0.2.4/examples/cifar/conf/config.yaml`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/data.py` & `diffq-0.2.4/examples/cifar/src/data.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/distrib.py` & `diffq-0.2.4/examples/cifar/src/distrib.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/executor.py` & `diffq-0.2.4/examples/cifar/src/executor.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/mobilenet.py` & `diffq-0.2.4/examples/cifar/src/mobilenet.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/resnet.py` & `diffq-0.2.4/examples/cifar/src/resnet.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/resnet20.py` & `diffq-0.2.4/examples/cifar/src/resnet20.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/solver.py` & `diffq-0.2.4/examples/cifar/src/solver.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/utils.py` & `diffq-0.2.4/examples/cifar/src/utils.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/vit.py` & `diffq-0.2.4/examples/cifar/src/vit.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/src/wide_resnet.py` & `diffq-0.2.4/examples/cifar/src/wide_resnet.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/examples/cifar/train.py` & `diffq-0.2.4/examples/cifar/train.py`

 * *Files identical despite different names*

### Comparing `diffq-0.2.3/setup.py` & `diffq-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 # Inspired from https://github.com/kennethreitz/setup.py
 
 from pathlib import Path
 from setuptools import setup, Extension
+from Cython.Build import cythonize
 
 NAME = 'diffq'
 DESCRIPTION = ('Differentiable quantization framework for PyTorch.')
 URL = 'https://github.com/facebookresearch/diffq'
 EMAIL = 'defossez@fb.com'
 AUTHOR = 'Alexandre Défossez, Yossi Adi, Gabriel Synnaeve'
 REQUIRES_PYTHON = '>=3.7.0'
@@ -39,17 +40,17 @@
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=['diffq'],
     install_requires=['Cython', 'numpy', 'torch'],
-    ext_modules=[Extension(
+    ext_modules=cythonize([Extension(
         "diffq.bitpack",
-        sources=["bitpack.pyx"])],
+        sources=["bitpack.pyx"])]),
     extras_require={'dev': ['coverage', 'flake8', 'pdoc3', 'torchvision']},
     include_package_data=True,
     license='Creative Commons Attribution-NonCommercial 4.0 International',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

