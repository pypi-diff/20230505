# Comparing `tmp/aeiou-0.0.7.tar.gz` & `tmp/aeiou-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeiou-0.0.7.tar", last modified: Sun Aug 21 19:08:41 2022, max compression
+gzip compressed data, was "aeiou-0.0.8.tar", last modified: Tue Aug 30 05:31:40 2022, max compression
```

## Comparing `aeiou-0.0.7.tar` & `aeiou-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2022-08-21 19:08:41.424470 aeiou-0.0.7/
--rw-r--r--   0 shawley    (501) staff       (20)    11357 2022-08-20 03:04:52.000000 aeiou-0.0.7/LICENSE
--rw-r--r--   0 shawley    (501) staff       (20)      111 2022-08-20 03:04:52.000000 aeiou-0.0.7/MANIFEST.in
--rw-r--r--   0 shawley    (501) staff       (20)     1369 2022-08-21 19:08:41.424287 aeiou-0.0.7/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      621 2022-08-21 05:34:40.000000 aeiou-0.0.7/README.md
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2022-08-21 19:08:41.422969 aeiou-0.0.7/aeiou/
--rw-r--r--   0 shawley    (501) staff       (20)       22 2022-08-21 19:07:14.000000 aeiou-0.0.7/aeiou/__init__.py
--rw-r--r--   0 shawley    (501) staff       (20)    15695 2022-08-21 19:07:14.000000 aeiou-0.0.7/aeiou/_modidx.py
--rw-r--r--   0 shawley    (501) staff       (20)     5132 2022-08-21 19:07:14.000000 aeiou-0.0.7/aeiou/chunkadelic.py
--rw-r--r--   0 shawley    (501) staff       (20)     2904 2022-08-21 19:07:14.000000 aeiou-0.0.7/aeiou/core.py
--rw-r--r--   0 shawley    (501) staff       (20)    10223 2022-08-21 19:07:14.000000 aeiou-0.0.7/aeiou/datasets.py
--rw-r--r--   0 shawley    (501) staff       (20)     3134 2022-08-21 19:07:14.000000 aeiou-0.0.7/aeiou/hpc.py
--rw-r--r--   0 shawley    (501) staff       (20)     3558 2022-08-21 19:07:14.000000 aeiou-0.0.7/aeiou/spectrofu.py
--rw-r--r--   0 shawley    (501) staff       (20)     7165 2022-08-21 19:07:14.000000 aeiou-0.0.7/aeiou/viz.py
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2022-08-21 19:08:41.424048 aeiou-0.0.7/aeiou.egg-info/
--rw-r--r--   0 shawley    (501) staff       (20)     1369 2022-08-21 19:08:41.000000 aeiou-0.0.7/aeiou.egg-info/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      388 2022-08-21 19:08:41.000000 aeiou-0.0.7/aeiou.egg-info/SOURCES.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2022-08-21 19:08:41.000000 aeiou-0.0.7/aeiou.egg-info/dependency_links.txt
--rw-r--r--   0 shawley    (501) staff       (20)      121 2022-08-21 19:08:41.000000 aeiou-0.0.7/aeiou.egg-info/entry_points.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2022-08-20 03:06:40.000000 aeiou-0.0.7/aeiou.egg-info/not-zip-safe
--rw-r--r--   0 shawley    (501) staff       (20)      120 2022-08-21 19:08:41.000000 aeiou-0.0.7/aeiou.egg-info/requires.txt
--rw-r--r--   0 shawley    (501) staff       (20)        6 2022-08-21 19:08:41.000000 aeiou-0.0.7/aeiou.egg-info/top_level.txt
--rw-r--r--   0 shawley    (501) staff       (20)     1135 2022-08-21 19:07:11.000000 aeiou-0.0.7/settings.ini
--rw-r--r--   0 shawley    (501) staff       (20)       38 2022-08-21 19:08:41.424524 aeiou-0.0.7/setup.cfg
--rw-r--r--   0 shawley    (501) staff       (20)     2541 2022-08-20 03:04:52.000000 aeiou-0.0.7/setup.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2022-08-30 05:31:40.911553 aeiou-0.0.8/
+-rw-r--r--   0 shawley    (501) staff       (20)    11357 2022-08-20 03:04:52.000000 aeiou-0.0.8/LICENSE
+-rw-r--r--   0 shawley    (501) staff       (20)      111 2022-08-20 03:04:52.000000 aeiou-0.0.8/MANIFEST.in
+-rw-r--r--   0 shawley    (501) staff       (20)     1594 2022-08-30 05:31:40.911419 aeiou-0.0.8/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      621 2022-08-21 05:34:40.000000 aeiou-0.0.8/README.md
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2022-08-30 05:31:40.910508 aeiou-0.0.8/aeiou/
+-rw-r--r--   0 shawley    (501) staff       (20)       22 2022-08-30 05:30:12.000000 aeiou-0.0.8/aeiou/__init__.py
+-rw-r--r--   0 shawley    (501) staff       (20)     6554 2022-08-30 05:30:12.000000 aeiou-0.0.8/aeiou/_modidx.py
+-rw-r--r--   0 shawley    (501) staff       (20)     5132 2022-08-30 05:30:12.000000 aeiou-0.0.8/aeiou/chunkadelic.py
+-rw-r--r--   0 shawley    (501) staff       (20)     2904 2022-08-30 05:30:12.000000 aeiou-0.0.8/aeiou/core.py
+-rw-r--r--   0 shawley    (501) staff       (20)    10223 2022-08-30 05:30:12.000000 aeiou-0.0.8/aeiou/datasets.py
+-rw-r--r--   0 shawley    (501) staff       (20)     3151 2022-08-30 05:30:12.000000 aeiou-0.0.8/aeiou/hpc.py
+-rw-r--r--   0 shawley    (501) staff       (20)     3558 2022-08-30 05:30:12.000000 aeiou-0.0.8/aeiou/spectrofu.py
+-rw-r--r--   0 shawley    (501) staff       (20)     7165 2022-08-30 05:30:12.000000 aeiou-0.0.8/aeiou/viz.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2022-08-30 05:31:40.911252 aeiou-0.0.8/aeiou.egg-info/
+-rw-r--r--   0 shawley    (501) staff       (20)     1594 2022-08-30 05:31:40.000000 aeiou-0.0.8/aeiou.egg-info/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      388 2022-08-30 05:31:40.000000 aeiou-0.0.8/aeiou.egg-info/SOURCES.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2022-08-30 05:31:40.000000 aeiou-0.0.8/aeiou.egg-info/dependency_links.txt
+-rw-r--r--   0 shawley    (501) staff       (20)      122 2022-08-30 05:31:40.000000 aeiou-0.0.8/aeiou.egg-info/entry_points.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2022-08-20 03:06:40.000000 aeiou-0.0.8/aeiou.egg-info/not-zip-safe
+-rw-r--r--   0 shawley    (501) staff       (20)      120 2022-08-30 05:31:40.000000 aeiou-0.0.8/aeiou.egg-info/requires.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        6 2022-08-30 05:31:40.000000 aeiou-0.0.8/aeiou.egg-info/top_level.txt
+-rw-r--r--   0 shawley    (501) staff       (20)     1135 2022-08-30 05:29:55.000000 aeiou-0.0.8/settings.ini
+-rw-r--r--   0 shawley    (501) staff       (20)       38 2022-08-30 05:31:40.911592 aeiou-0.0.8/setup.cfg
+-rw-r--r--   0 shawley    (501) staff       (20)     2541 2022-08-20 03:04:52.000000 aeiou-0.0.8/setup.py
```

### Comparing `aeiou-0.0.7/LICENSE` & `aeiou-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aeiou-0.0.7/PKG-INFO` & `aeiou-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: aeiou
-Version: 0.0.7
+Version: 0.0.8
 Summary: audio engineering i/o utils
 Home-page: https://github.com/drscotthawley/aeiou/
 Author: Scott Hawley
 Author-email: scott.hawley@belmont.edu
 License: Apache Software License 2.0
+Description: aeiou
+        ================
+        
+        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+        
+        Pronounced “[ayoo](https://youtu.be/Hv6RbEOlqRo?t=24)”
+        
+        ## Install
+        
+        We recommend you install the latest version from GitHub via
+        
+        ``` sh
+        pip install git+https://github.com/drscotthawley/aeiou.git
+        ```
+        
+        However binaries will be occasionally updated on PyPI, installed via
+        
+        ``` sh
+        pip install aeiou
+        ```
+        
+        ## How to use
+        
+        This is a series of utility routines developed in support of multiple
+        projects within [Harmonai](https://www.harmonai.org/). See individual
+        documentation pages for more specific instructions on how these can be
+        used.
+        
 Keywords: nbdev
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
-
-aeiou
-================
-
-<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-
-Pronounced “[ayoo](https://youtu.be/Hv6RbEOlqRo?t=24)”
-
-## Install
-
-We recommend you install the latest version from GitHub via
-
-``` sh
-pip install git+https://github.com/drscotthawley/aeiou.git
-```
-
-However binaries will be occasionally updated on PyPI, installed via
-
-``` sh
-pip install aeiou
-```
-
-## How to use
-
-This is a series of utility routines developed in support of multiple
-projects within [Harmonai](https://www.harmonai.org/). See individual
-documentation pages for more specific instructions on how these can be
-used.
```

### Comparing `aeiou-0.0.7/README.md` & `aeiou-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `aeiou-0.0.7/aeiou/chunkadelic.py` & `aeiou-0.0.8/aeiou/chunkadelic.py`

 * *Files identical despite different names*

### Comparing `aeiou-0.0.7/aeiou/core.py` & `aeiou-0.0.8/aeiou/core.py`

 * *Files identical despite different names*

### Comparing `aeiou-0.0.7/aeiou/datasets.py` & `aeiou-0.0.8/aeiou/datasets.py`

 * *Files identical despite different names*

### Comparing `aeiou-0.0.7/aeiou/hpc.py` & `aeiou-0.0.8/aeiou/hpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
     args,        # prefigure args dict, (we only use args.name)
     model,       # the model, pre-unwrapped
     opt=None,    # optimizer state
     epoch=None,  # training epoch number
     step=None    # training setp number
     ):
     "for checkpointing & model saves"
-    accelerator.wait_for_everyone()
+    #accelerator.wait_for_everyone() # hangs
     filename = f'{args.name}_{step:08}.pth' if (step is not None) else f'{args.name}.pth'
     if accelerator.is_main_process:
-        tqdm.write(f'Saving to {filename}...')
+        print(f'\nSaving checkpoint to {filename}...')
     obj = {'model': accelerator.unwrap_model(model).state_dict() }
     if opt is not None:   obj['opt'] = opt.state_dict()
     if epoch is not None: obj['epoch'] = epoch
     if step is not None:  obj['step'] = step
     accelerator.save(obj, filename)
 
 # %% ../05_hpc.ipynb 16
```

### Comparing `aeiou-0.0.7/aeiou/spectrofu.py` & `aeiou-0.0.8/aeiou/spectrofu.py`

 * *Files identical despite different names*

### Comparing `aeiou-0.0.7/aeiou/viz.py` & `aeiou-0.0.8/aeiou/viz.py`

 * *Files identical despite different names*

### Comparing `aeiou-0.0.7/aeiou.egg-info/PKG-INFO` & `aeiou-0.0.8/aeiou.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: aeiou
-Version: 0.0.7
+Version: 0.0.8
 Summary: audio engineering i/o utils
 Home-page: https://github.com/drscotthawley/aeiou/
 Author: Scott Hawley
 Author-email: scott.hawley@belmont.edu
 License: Apache Software License 2.0
+Description: aeiou
+        ================
+        
+        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+        
+        Pronounced “[ayoo](https://youtu.be/Hv6RbEOlqRo?t=24)”
+        
+        ## Install
+        
+        We recommend you install the latest version from GitHub via
+        
+        ``` sh
+        pip install git+https://github.com/drscotthawley/aeiou.git
+        ```
+        
+        However binaries will be occasionally updated on PyPI, installed via
+        
+        ``` sh
+        pip install aeiou
+        ```
+        
+        ## How to use
+        
+        This is a series of utility routines developed in support of multiple
+        projects within [Harmonai](https://www.harmonai.org/). See individual
+        documentation pages for more specific instructions on how these can be
+        used.
+        
 Keywords: nbdev
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
-
-aeiou
-================
-
-<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-
-Pronounced “[ayoo](https://youtu.be/Hv6RbEOlqRo?t=24)”
-
-## Install
-
-We recommend you install the latest version from GitHub via
-
-``` sh
-pip install git+https://github.com/drscotthawley/aeiou.git
-```
-
-However binaries will be occasionally updated on PyPI, installed via
-
-``` sh
-pip install aeiou
-```
-
-## How to use
-
-This is a series of utility routines developed in support of multiple
-projects within [Harmonai](https://www.harmonai.org/). See individual
-documentation pages for more specific instructions on how these can be
-used.
```

### Comparing `aeiou-0.0.7/settings.ini` & `aeiou-0.0.8/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified
 # see https://github.com/fastai/nbdev/blob/master/settings.ini for examples
 
 ### Python Library ###
 lib_name = aeiou
 min_python = 3.7
-version = 0.0.7
+version = 0.0.8
 
 ### OPTIONAL ###
 
 requirements = fastcore pandas numpy torch torchvision torchaudio wandb matplotlib pillow tqdm librosa>=0.8.1 einops accelerate
 # dev_requirements = 
 console_scripts = chunkadelic=aeiou.chunkadelic:main spectrofu=aeiou.spectrofu:main
```

### Comparing `aeiou-0.0.7/setup.py` & `aeiou-0.0.8/setup.py`

 * *Files identical despite different names*

