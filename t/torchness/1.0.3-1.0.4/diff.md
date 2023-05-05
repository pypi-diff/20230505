# Comparing `tmp/torchness-1.0.3.tar.gz` & `tmp/torchness-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchness-1.0.3.tar", last modified: Sat Apr  1 19:39:13 2023, max compression
+gzip compressed data, was "dist/torchness-1.0.4.tar", last modified: Fri May  5 19:15:46 2023, max compression
```

## Comparing `torchness-1.0.3.tar` & `torchness-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-01 19:39:13.000000 torchness-1.0.3/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      202 2023-04-01 19:39:13.000000 torchness-1.0.3/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2023-04-01 19:39:13.000000 torchness-1.0.3/setup.cfg
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      624 2023-04-01 19:38:48.000000 torchness-1.0.3/setup.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-01 19:39:13.000000 torchness-1.0.3/torchness/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2022-11-21 13:13:23.000000 torchness-1.0.3/torchness/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3224 2023-03-18 18:49:36.000000 torchness-1.0.3/torchness/base_elements.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-01 19:39:13.000000 torchness-1.0.3/torchness/comoneural/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2022-04-29 09:41:51.000000 torchness-1.0.3/torchness/comoneural/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      501 2023-03-11 13:46:24.000000 torchness-1.0.3/torchness/comoneural/avg_probs.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     6530 2023-03-30 15:17:56.000000 torchness-1.0.3/torchness/comoneural/batcher.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1791 2023-01-31 22:05:03.000000 torchness-1.0.3/torchness/comoneural/zeroes_processor.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    27507 2023-03-10 11:57:11.000000 torchness-1.0.3/torchness/encoders.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     4546 2023-03-07 20:19:33.000000 torchness-1.0.3/torchness/grad_clipping.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     7598 2023-03-10 11:50:02.000000 torchness-1.0.3/torchness/layers.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-01 19:39:13.000000 torchness-1.0.3/torchness/models/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-01-15 19:48:10.000000 torchness-1.0.3/torchness/models/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2917 2023-03-30 15:39:16.000000 torchness-1.0.3/torchness/models/simple_feats_classifier.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     4663 2023-02-28 20:01:47.000000 torchness-1.0.3/torchness/models/simple_text_classifier.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     4571 2023-03-10 13:56:54.000000 torchness-1.0.3/torchness/models/text_embbeder.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    37377 2023-03-30 15:40:54.000000 torchness-1.0.3/torchness/motorch.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2209 2023-02-28 20:01:47.000000 torchness-1.0.3/torchness/scaled_LR.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1480 2023-03-01 22:37:33.000000 torchness-1.0.3/torchness/tbwr.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      303 2022-12-28 08:56:57.000000 torchness-1.0.3/torchness/types.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-01 19:39:13.000000 torchness-1.0.3/torchness.egg-info/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      202 2023-04-01 19:39:13.000000 torchness-1.0.3/torchness.egg-info/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      661 2023-04-01 19:39:13.000000 torchness-1.0.3/torchness.egg-info/SOURCES.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2023-04-01 19:39:13.000000 torchness-1.0.3/torchness.egg-info/dependency_links.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       70 2023-04-01 19:39:13.000000 torchness-1.0.3/torchness.egg-info/requires.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       10 2023-04-01 19:39:13.000000 torchness-1.0.3/torchness.egg-info/top_level.txt
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:15:46.000000 torchness-1.0.4/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      202 2023-05-05 19:15:46.000000 torchness-1.0.4/PKG-INFO
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2023-05-05 19:15:46.000000 torchness-1.0.4/setup.cfg
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      624 2023-05-05 19:14:23.000000 torchness-1.0.4/setup.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:15:46.000000 torchness-1.0.4/torchness/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2022-11-21 13:13:23.000000 torchness-1.0.4/torchness/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3224 2023-03-18 18:49:36.000000 torchness-1.0.4/torchness/base_elements.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:15:46.000000 torchness-1.0.4/torchness/comoneural/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2022-04-29 09:41:51.000000 torchness-1.0.4/torchness/comoneural/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      501 2023-03-11 13:46:24.000000 torchness-1.0.4/torchness/comoneural/avg_probs.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     6530 2023-03-30 15:17:56.000000 torchness-1.0.4/torchness/comoneural/batcher.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1791 2023-01-31 22:05:03.000000 torchness-1.0.4/torchness/comoneural/zeroes_processor.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    27507 2023-03-10 11:57:11.000000 torchness-1.0.4/torchness/encoders.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     4546 2023-03-07 20:19:33.000000 torchness-1.0.4/torchness/grad_clipping.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     7598 2023-03-10 11:50:02.000000 torchness-1.0.4/torchness/layers.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:15:46.000000 torchness-1.0.4/torchness/models/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-01-15 19:48:10.000000 torchness-1.0.4/torchness/models/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2917 2023-03-30 15:39:16.000000 torchness-1.0.4/torchness/models/simple_feats_classifier.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     4663 2023-02-28 20:01:47.000000 torchness-1.0.4/torchness/models/simple_text_classifier.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     4571 2023-03-10 13:56:54.000000 torchness-1.0.4/torchness/models/text_embbeder.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    37751 2023-04-24 12:38:13.000000 torchness-1.0.4/torchness/motorch.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2209 2023-02-28 20:01:47.000000 torchness-1.0.4/torchness/scaled_LR.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1480 2023-03-01 22:37:33.000000 torchness-1.0.4/torchness/tbwr.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      303 2022-12-28 08:56:57.000000 torchness-1.0.4/torchness/types.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:15:46.000000 torchness-1.0.4/torchness.egg-info/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      202 2023-05-05 19:15:46.000000 torchness-1.0.4/torchness.egg-info/PKG-INFO
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      661 2023-05-05 19:15:46.000000 torchness-1.0.4/torchness.egg-info/SOURCES.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2023-05-05 19:15:46.000000 torchness-1.0.4/torchness.egg-info/dependency_links.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       70 2023-05-05 19:15:46.000000 torchness-1.0.4/torchness.egg-info/requires.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       10 2023-05-05 19:15:46.000000 torchness-1.0.4/torchness.egg-info/top_level.txt
```

### Comparing `torchness-1.0.3/setup.py` & `torchness-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('requirements.txt') as file:
         lines = [l[:-1] if l[-1]=='\n' else l for l in file.readlines()]
         return lines
 
 
 setup(
     name=               'torchness',
-    version=            'v1.0.3',
+    version=            'v1.0.4',
     url=                'https://github.com/piteren/torchness.git',
     author=             'Piotr Niewinski',
     author_email=       'pioniewinski@gmail.com',
     description=        'PyTorch tools',
     packages=           find_packages(),
     install_requires=   get_requirements(),
     license=            'MIT')
```

### Comparing `torchness-1.0.3/torchness/base_elements.py` & `torchness-1.0.4/torchness/base_elements.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/comoneural/batcher.py` & `torchness-1.0.4/torchness/comoneural/batcher.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/comoneural/zeroes_processor.py` & `torchness-1.0.4/torchness/comoneural/zeroes_processor.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/encoders.py` & `torchness-1.0.4/torchness/encoders.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/grad_clipping.py` & `torchness-1.0.4/torchness/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/layers.py` & `torchness-1.0.4/torchness/layers.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/models/simple_feats_classifier.py` & `torchness-1.0.4/torchness/models/simple_feats_classifier.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/models/simple_text_classifier.py` & `torchness-1.0.4/torchness/models/simple_text_classifier.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/models/text_embbeder.py` & `torchness-1.0.4/torchness/models/text_embbeder.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/motorch.py` & `torchness-1.0.4/torchness/motorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from pypaq.lipytools.printout import stamp
 from pypaq.lipytools.files import prep_folder
 from pypaq.lipytools.pylogger import get_pylogger, get_child
 from pypaq.lipytools.moving_average import MovAvg
 from pypaq.pms.base import get_params, point_trim
 from pypaq.pms.parasave import ParaSave
 from pypaq.mpython.devices import get_devices
+from pypaq.mpython.mpdecor import proc_wait
 from torchness.comoneural.batcher import Batcher
 from torchness.types import TNS, DTNS
 from torchness.base_elements import mrg_ckpts
 from torchness.scaled_LR import ScaledLR
 from torchness.grad_clipping import GradClipperMAVG
 from torchness.tbwr import TBwr
 
@@ -628,20 +629,27 @@
                 name_child=         name_child,
                 save_topdir_A=      save_topdir_parent_main,
                 save_topdir_B=      save_topdir_parent_scnd,
                 save_topdir_child=  save_topdir_child,
                 ratio=              ratio,
                 noise=              noise)
         else:
-            cls.copy_checkpoint(
-                name_src=           name_parent_main,
-                name_trg=           name_child,
-                save_topdir_src=    save_topdir_parent_main,
-                save_topdir_trg=    save_topdir_child)
 
+            # wrapped into subprocess for better separation of torch objects (similar to mrg_ckpts() in base_elements)
+            @proc_wait
+            def build_with_subprocess():
+                mod = cls(
+                    name=               name_child,
+                    save_topdir=        save_topdir_child or save_topdir_parent_main,
+                    save_fn_pfx=        save_fn_pfx,
+                    logger=             logger,
+                    loglevel=           loglevel)
+                mod.save() # save checkpoint
+
+            build_with_subprocess()
 
     # ***************************************************************************************************** train / test
 
     # converts and loads data to Batcher
     def load_data(
             self,
             data_TR: Dict[str,np.ndarray],
```

### Comparing `torchness-1.0.3/torchness/scaled_LR.py` & `torchness-1.0.4/torchness/scaled_LR.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness/tbwr.py` & `torchness-1.0.4/torchness/tbwr.py`

 * *Files identical despite different names*

### Comparing `torchness-1.0.3/torchness.egg-info/SOURCES.txt` & `torchness-1.0.4/torchness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

