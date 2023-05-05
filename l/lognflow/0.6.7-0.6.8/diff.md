# Comparing `tmp/lognflow-0.6.7.tar.gz` & `tmp/lognflow-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.6.7.tar", last modified: Thu Apr 27 10:51:46 2023, max compression
+gzip compressed data, was "lognflow-0.6.8.tar", last modified: Fri May  5 00:43:21 2023, max compression
```

## Comparing `lognflow-0.6.7.tar` & `lognflow-0.6.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.291388 lognflow-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-27 10:51:32.000000 lognflow-0.6.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-27 10:51:32.000000 lognflow-0.6.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-27 10:51:32.000000 lognflow-0.6.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 10:51:32.000000 lognflow-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 10:51:32.000000 lognflow-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-27 10:51:46.291388 lognflow-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-27 10:51:32.000000 lognflow-0.6.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.287388 lognflow-0.6.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 10:51:32.000000 lognflow-0.6.7/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.287388 lognflow-0.6.7/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 10:51:32.000000 lognflow-0.6.7/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69530 2023-04-27 10:51:32.000000 lognflow-0.6.7/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-27 10:51:32.000000 lognflow-0.6.7/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-27 10:51:32.000000 lognflow-0.6.7/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.287388 lognflow-0.6.7/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 10:51:46.000000 lognflow-0.6.7/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 10:51:46.291388 lognflow-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 10:51:32.000000 lognflow-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:51:46.287388 lognflow-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 10:51:32.000000 lognflow-0.6.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-27 10:51:32.000000 lognflow-0.6.7/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-27 10:51:32.000000 lognflow-0.6.7/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-27 10:51:32.000000 lognflow-0.6.7/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.962096 lognflow-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-05 00:42:57.000000 lognflow-0.6.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-05 00:42:57.000000 lognflow-0.6.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-05 00:42:57.000000 lognflow-0.6.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-05 00:42:57.000000 lognflow-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 00:42:57.000000 lognflow-0.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-05 00:43:21.962096 lognflow-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-05 00:42:57.000000 lognflow-0.6.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.958096 lognflow-0.6.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 00:42:57.000000 lognflow-0.6.8/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.962096 lognflow-0.6.8/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-05 00:42:57.000000 lognflow-0.6.8/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69466 2023-05-05 00:42:57.000000 lognflow-0.6.8/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-05 00:42:57.000000 lognflow-0.6.8/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-05 00:42:57.000000 lognflow-0.6.8/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.962096 lognflow-0.6.8/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 00:43:21.000000 lognflow-0.6.8/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-05 00:43:21.962096 lognflow-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-05 00:42:57.000000 lognflow-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:43:21.962096 lognflow-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-05 00:42:57.000000 lognflow-0.6.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-05 00:42:57.000000 lognflow-0.6.8/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-05 00:42:57.000000 lognflow-0.6.8/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-05 00:42:57.000000 lognflow-0.6.8/tests/test_printprogress.py
```

### Comparing `lognflow-0.6.7/CONTRIBUTING.rst` & `lognflow-0.6.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.7/HISTORY.rst` & `lognflow-0.6.8/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -68,8 +68,19 @@
 0.6.6 (2023-04-27)
 ------------------
 * Better documentation
 * added tifffile imread to logviewer and imwrite to lognflow
 
 0.6.7 (2023-04-27)
 ------------------
-* A bug in tifffile support was fixed
+* A bug in tifffile support was fixed
+
+0.6.8 (2023-05-04)
+------------------
+* Fixing readme for PyPI.
+* removed marker from log_plot. user marker and linestyle keyword arguments.
+* printprogress returns proper ETA every time if print_function is set to None::
+    pBar = printprogress(N, print_function = None)
+    for _ in range(N):
+        ETA = pBar()
+        print(f'ETA: {ETA}')
+
```

### Comparing `lognflow-0.6.7/LICENSE` & `lognflow-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.7/PKG-INFO` & `lognflow-0.6.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.7
+Version: 0.6.8
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -21,55 +21,37 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 lognflow
 ========
 
+Log and Flow tracking made easy with Python. You can install it by::
 
-.. image:: https://img.shields.io/pypi/v/lognflow.svg
-        :target: https://pypi.python.org/pypi/lognflow
-
-.. image:: https://img.shields.io/travis/arsadri/lognflow.svg
-        :target: https://travis-ci.com/arsadri/lognflow
-
-.. image:: https://readthedocs.org/projects/lognflow/badge/?version=latest
-        :target: https://lognflow.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-Log and Flow tracking made easy with Python. You can install it by:
-
-.. code-block:: python
 	pip install lognflow
 
+A simple program to use it would be similar to the following::
 
-A simple program to use it would be similar to the following:
-
-.. code-block:: python
 	from lognflow import lognflow
 	import numpy as np
 	vec = np.random.rand(100)
 	
 	logger = lognflow('c:\\test\\')
 	logger('This is a test for lognflow and log_var')
 	logger.log_single('vec', vec)
 
-The logviewer is also very useful.
+The logviewer is also very useful::
 
-.. code-block:: python
 	from lognflow import logviewer
-	
 	logged = logviewer('c:\\test\\some_log\')
 	vec = logged.get_single('vec')
 
-The printprogress makes a pretty nice progress bar.
+The printprogress makes a pretty nice progress bar::
 
-.. code-block:: python
 	from lognflow import printprogress
-	
 	N = 100
 	pbar = printprogress(N)
 	for _ in range(N):
 		# do_something()
 		pbar()
 
 In this package we use a folder on the HDD to generate files and folders in typical
@@ -179,7 +161,18 @@
 ------------------
 * Better documentation
 * added tifffile imread to logviewer and imwrite to lognflow
 
 0.6.7 (2023-04-27)
 ------------------
 * A bug in tifffile support was fixed
+
+0.6.8 (2023-05-04)
+------------------
+* Fixing readme for PyPI.
+* removed marker from log_plot. user marker and linestyle keyword arguments.
+* printprogress returns proper ETA every time if print_function is set to None::
+    pBar = printprogress(N, print_function = None)
+    for _ in range(N):
+        ETA = pBar()
+        print(f'ETA: {ETA}')
+
```

### Comparing `lognflow-0.6.7/README.rst` & `lognflow-0.6.8/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,33 @@
 lognflow
 ========
 
+Log and Flow tracking made easy with Python. You can install it by::
 
-.. image:: https://img.shields.io/pypi/v/lognflow.svg
-        :target: https://pypi.python.org/pypi/lognflow
-
-.. image:: https://img.shields.io/travis/arsadri/lognflow.svg
-        :target: https://travis-ci.com/arsadri/lognflow
-
-.. image:: https://readthedocs.org/projects/lognflow/badge/?version=latest
-        :target: https://lognflow.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-Log and Flow tracking made easy with Python. You can install it by:
-
-.. code-block:: python
 	pip install lognflow
 
+A simple program to use it would be similar to the following::
 
-A simple program to use it would be similar to the following:
-
-.. code-block:: python
 	from lognflow import lognflow
 	import numpy as np
 	vec = np.random.rand(100)
 	
 	logger = lognflow('c:\\test\\')
 	logger('This is a test for lognflow and log_var')
 	logger.log_single('vec', vec)
 
-The logviewer is also very useful.
+The logviewer is also very useful::
 
-.. code-block:: python
 	from lognflow import logviewer
-	
 	logged = logviewer('c:\\test\\some_log\')
 	vec = logged.get_single('vec')
 
-The printprogress makes a pretty nice progress bar.
+The printprogress makes a pretty nice progress bar::
 
-.. code-block:: python
 	from lognflow import printprogress
-	
 	N = 100
 	pbar = printprogress(N)
 	for _ in range(N):
 		# do_something()
 		pbar()
 
 In this package we use a folder on the HDD to generate files and folders in typical
```

### Comparing `lognflow-0.6.7/docs/Makefile` & `lognflow-0.6.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.7/docs/conf.py` & `lognflow-0.6.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.7/docs/installation.rst` & `lognflow-0.6.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.7/docs/make.bat` & `lognflow-0.6.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.7/lognflow/lognflow.py` & `lognflow-0.6.8/lognflow/lognflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,20 +721,20 @@
                         self.log_name,
                         f'x_values for {parameter_name} should have'\
                         + ' length of 1 or the same as parameters list.')
                     raise ValueError
             
             for list_cnt, parameter_value in enumerate(parameter_value_list):
                 if(x_values is None):
-                    plt.plot(parameter_value, '-*', **kwargs)
+                    plt.plot(parameter_value, **kwargs)
                 else:
                     if(len(x_values) == len(parameter_value)):
                         plt.plot(x_values[list_cnt], parameter_value, **kwargs)
                     else:
-                        plt.plot(x_values[0], parameter_value, '-*', **kwargs)
+                        plt.plot(x_values[0], parameter_value, **kwargs)
             
             fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
                         
             return fpath
@@ -898,15 +898,15 @@
             self.log_text(self.log_name,
                 f'Cannot make the hexbin for variable {parameter_name}.')
             return None
         
     def log_imshow(self, parameter_name: str, 
                    parameter_value,
                    image_format='jpeg', dpi=1200, cmap = 'jet',
-                   time_tag: bool = None, nan_borders = np.nan,
+                   time_tag: bool = None, borders = 0,
                    **kwargs):
         """log an image
             The image is logged using plt.imshow
             
             :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
@@ -944,15 +944,15 @@
                 use_multichannel_to_square = True
             elif(parameter_value_shape[0] == 1):
                 FLAG_img_ready = True
                 use_multichannel_to_square = True
         
         if(use_multichannel_to_square):
             parameter_value = self. multichannel_to_square(
-                parameter_value, nan_borders = nan_borders)
+                parameter_value, borders = borders)
         if(FLAG_img_ready):
             plt.figure()
             plt.imshow(parameter_value, cmap = cmap, **kwargs)
             plt.colorbar()
             fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
@@ -961,30 +961,30 @@
         else:
             self.log_text(
                 self.log_name,
                 f'Cannot plot variable {parameter_name} with shape' + \
                 f'{parameter_value.shape}')
             return
 
-    def multichannel_to_square(self, stack, nan_borders = np.nan):
+    def multichannel_to_square(self, stack, borders = 0):
         """ turn a stack of multi-channel images into stack of square images
             This is very useful when lots of images need to be tiled
             against each other.
         
             :param stack: np.ndarray
                     It must have the shape of either
                     n_r x n_c x n_ch
                     n_r x n_c x  3  x n_ch
                     n_f x n_r x n_c x n_ch
                     n_f x n_r x n_c x  3  x n_ch
                     
                 In both cases n_ch will be turned into a square tile
                 Remember if you have N images to put into a square, the input
                 shape should be 1 x n_r x n_c x N
-            :param nan_borders: literal or np.inf or np.nan
+            :param borders: literal or np.inf or np.nan
                 When plotting images with matplotlib.pyplot.imshow, there
                 needs to be a border between them. This is the value for the 
                 border elements.
                 
             output
             ---------
                 Since we have N channels to be laid into a square, the side
@@ -1012,47 +1012,47 @@
                 canv = np.zeros((n_imgs, new_n_R, new_n_C), 
                                 dtype = stack.dtype)
             if(len(stack.shape) == 5):
                 canv = np.zeros((n_imgs, new_n_R, new_n_C, 3),
                                  dtype = stack.dtype)
             used_ch_cnt = 0
 
-            stack[:,   :1      ] = nan_borders
-            stack[:,   : ,   :1] = nan_borders
-            stack[:, -1:       ] = nan_borders
-            stack[:,   : , -1: ] = nan_borders
+            stack[:,   :1      ] = borders
+            stack[:,   : ,   :1] = borders
+            stack[:, -1:       ] = borders
+            stack[:,   : , -1: ] = borders
             
             for rcnt in range(square_side):
                 for ccnt in range(square_side):
                     ch_cnt = rcnt + square_side*ccnt
                     if (ch_cnt<n_ch):
                         canv[:, rcnt*n_R: (rcnt + 1)*n_R,
                                 ccnt*n_C: (ccnt + 1)*n_C] = \
                             stack[..., used_ch_cnt]
                         used_ch_cnt += 1
         else:
             return None
         return canv
 
-    def _handle_images_stack(self, stack, nan_borders = np.nan):
+    def _handle_images_stack(self, stack, borders = 0):
         canv = None
         if(len(stack.shape) == 2):
             canv = np.expand_dims(stack, axis=0)
         if(len(stack.shape) == 3):
             if(stack.shape[2] == 3):
                 canv = np.expand_dims(stack, axis=0)
             else:
                 canv = stack
         if((len(stack.shape) == 4) | (len(stack.shape) == 5)):
-            canv = self.multichannel_to_square(stack, nan_borders = nan_borders)
+            canv = self.multichannel_to_square(stack, borders = borders)
         return canv
     
     def prepare_stack_of_images(self, 
                                 list_of_stacks, 
-                                nan_borders = np.nan):
+                                borders = 0):
         """Prepare the stack of images
             If you wish to use the log_canvas, chances are you have a list
             of stacks of images where one element, has many channels.
             In that case, the channels can be tiled beside each other
             to make one image for showing. This is very useful for ML apps.
     
             Each element of the list can appear as either:
@@ -1065,22 +1065,22 @@
                                          shown. 
                                          Channels will be tiled into square
             n_frm x n_row x n_clm x n_ch x 3 if channels are in RGB
     
             :param list_of_stacks
                     list_of_stacks would include arrays iteratable by their
                     first dimension.
-            :param nan_borders: float
+            :param borders: float
                     borders between tiles will be filled with this variable
                     default: np.nan
         """        
         if (not isinstance(list_of_stacks, list)):
             list_of_stacks = [list_of_stacks]
         for cnt, stack in enumerate(list_of_stacks):
-            stack = self._handle_images_stack(stack, nan_borders = nan_borders)
+            stack = self._handle_images_stack(stack, borders = borders)
             if(stack is None):
                 return
             list_of_stacks[cnt] = stack
         return(list_of_stacks)
 
     def log_canvas(self, 
                    parameter_name: str,
@@ -1200,14 +1200,15 @@
                              f'{data_canvas.min():.6f}', 
                              color = 'yellow',
                              fontsize = 2)
                 if(use_colorbar):
                     cbar = plt.colorbar(im, ax=ax1, fraction=0.046, pad=0.04)
                     cbar.ax.tick_params(labelsize=1)
                 ax1.set_aspect('equal')
+                ax1.axis('off')
         
         fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
         return fpath
```

### Comparing `lognflow-0.6.7/lognflow/logviewer.py` & `lognflow-0.6.8/lognflow/logviewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pathlib
 import numpy as np
-from scipy.io import loadmat
-from matplotlib.pyplot import imread
 
 class logviewer:
     """ log viewer
         Since lognflow makes lots of files and folders, maybe it is nice
         to have a logviewer that loads those information. In this module we
         provide a set of functions for a logged object that can load variables,
         texts, file lists and etc.. Use it simply by:
@@ -44,15 +42,15 @@
                 with open(flist[fcnt]) as f_txt:
                     txt.append(f_txt.readlines())
             if(n_files == 1):
                 txt = txt[0]
             return txt
 
     def get_single(self, var_name, single_shot_index = -1, 
-                     suffix = '.np*'):
+                     suffix = None):
         """ get a single variable
             return the value of a saved variable.
 
             Parameters
             ----------
             :param var_name:
                 variable name
@@ -66,26 +64,41 @@
                 
             .. note::
                 when reading a MATLAB file, the output is a dictionary.
         """
         var_name = var_name.replace('\t', '\\t').replace('\n', '\\n')\
             .replace('\r', '\\r').replace('\b', '\\b')
         
-        suffix = suffix.strip('.')
+        if suffix is None:
+            if len(var_name.split('.')) > 1:
+                suffix = var_name.split('.')[-1]
+                name_before_suffix = var_name.split('.')[:-1]
+                if((len(name_before_suffix) == 1) & 
+                   (name_before_suffix[0] == '')):
+                    var_name = '*'
+                else:
+                    var_name = ('.').join(var_name.split('.')[:-1])
+            else:
+                suffix = '.np*'
+
+        suffix = suffix.strip('.')        
         assert single_shot_index == int(single_shot_index), \
                     f'single_shot_index {single_shot_index} must be an integer'
         flist = []            
         if((self.log_dir / var_name).is_file()):
             flist = [self.log_dir / var_name]
         elif((self.log_dir / f'{var_name}.{suffix}').is_file()):
             flist = [self.log_dir / f'{var_name}.{suffix}']
         else:
             _var_name = (self.log_dir / var_name).name
             _var_dir = (self.log_dir / var_name).parent
-            flist = list(_var_dir.glob(f'{_var_name}*.{suffix}'))
+            search_patt = f'{_var_name}*.{suffix}'
+            while('**' in search_patt):
+                search_patt = search_patt.replace('**', '*')
+            flist = list(_var_dir.glob(search_patt))
             if(len(flist) == 0):
                 flist = list(_var_dir.glob(f'{_var_name}*.*'))
                 if(len(flist) > 0):
                     self.logger('Can not find the file with the given suffix, '\
                                 +'but found some with a different suffix, '\
                                 +f'one file is: {flist[single_shot_index]}')
                     
@@ -111,36 +124,39 @@
                 time_array = time_array[:n_logs]
                 data_array = buf['data_array']
                 data_array = data_array[:n_logs]
                 return((time_array, data_array))
             if(var_path.suffix == '.npy'):
                 return(np.load(var_path))
             if(var_path.suffix == '.mat'):
+                from scipy.io import loadmat
                 return(loadmat(var_path))
             if(var_path.suffix == '.txt'):
                 with open(var_path) as f_txt:
                     return(f_txt.read())
             if((var_path.suffix == '.tif') | (var_path.suffix == '.tiff')):
                 from tifffile import imread
                 return(imread(var_path))
             if(var_path.suffix == '.torch'):      
                 from torch import load as torch_load 
                 return(torch_load(var_path))
             try:
+                from matplotlib.pyplot import imread
                 img = imread(var_path)
                 return(img)
             except:
                 pass
         else:
             self.logger(f'{var_name} not found.')
             return
     
     def get_stack_of_files(self, 
-        var_name = None, flist = [], suffix = '*',
-        return_data = False, return_flist = True):
+        var_name = None, flist = [], suffix = None,
+        return_data = False, return_flist = True,
+        verbose = True):
         
         """ Get list or data of all files in a directory
         
             This function gives the list of paths of all files in a directory
             for a single variable. 
 
             Parameters
@@ -170,28 +186,41 @@
             
                 It returns a tuple, (dataset, flist),
                 dataset will be a numpy array in case all files produce same
                 shape numpy arrays.
                 flist is type pathlib.Path
             
         """
+        if suffix is None:
+            if len(var_name.split('.')) > 1:
+                suffix = var_name.split('.')[-1]
+                name_before_suffix = var_name.split('.')[:-1]
+                if((len(name_before_suffix) == 1) & 
+                   (name_before_suffix[0] == '')):
+                    var_name = '*'
+                else:
+                    var_name = ('.').join(var_name.split('.')[:-1])
+            else:
+                suffix = '*'
+
         suffix = suffix.strip('.')
         if not flist:
             assert var_name is not None, \
                 ' The file list is empty. Please provide the ' \
                 + 'variable name or a non-empty file list.'
             var_dir = self.log_dir / var_name
             if(var_dir.is_dir()):
                 var_fname = None
                 flist = list(var_dir.glob(f'*.{suffix}'))
             else:
                 var_fname = var_dir.name
                 var_dir = var_dir.parent
                 patt = f'{var_fname}*.{suffix}'
-                patt = patt.replace('**', '*')
+                while('**' in patt):
+                    patt = patt.replace('**', '*')
                 flist = list(var_dir.glob(patt))
         if flist:
             flist.sort()
             n_files = len(flist)
             if((not return_data) & return_flist):
                 return(flist)
             data_type = None
@@ -199,33 +228,37 @@
                 try:
                     fdata = np.load(flist[0])
                     data_type = 'numpy'
                 except:
                     pass
             if(data_type is None):
                 try:
+                    from matplotlib.pyplot import imread
                     fdata = imread(flist[0])
                     data_type = 'image'
                 except:
                     pass
             if(data_type is not None):
                 dataset = np.zeros((n_files, ) + fdata.shape, 
                                    dtype=fdata.dtype)
                 for fcnt, fpath in enumerate(flist):
                     if(data_type == 'numpy'):
                         dataset[fcnt] = np.load(fpath)
                     elif(data_type == 'image'):
                         dataset[fcnt] = imread(fpath)
-                self.logger(f'shape is: {dataset.shape}')
+                if(verbose):
+                    self.logger(f'logviewer: Reading dataset from {var_dir}'
+                                f', the shape would be: {dataset.shape}')
                 if(return_flist):
                     return(dataset, flist)
                 else:
                     return(dataset)
             else:
-                self.logger(f'File {flist[0].name} cannot be opened by '\
+                if(verbose):
+                    self.logger(f'File {flist[0].name} cannot be opened by '\
                           + r'np.load() or plt.imread()')
             
     def get_common_files(self, var_name_A, var_name_B):
         """ get common files in two directories
         
             It happens often in ML that there are two directories, A and B,
             and we are interested to get the flist in both that is common
```

### Comparing `lognflow-0.6.7/lognflow/printprogress.py` & `lognflow-0.6.8/lognflow/printprogress.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,28 +103,29 @@
                 self.FLAG_warning = True
                 self._print_func('-' * self.numTicks)
         else:
             self.ck += ck
             if(self.ck >= self.n_steps):
                 self.end()
             else:
+                remTimeS = self._calc_ETA() # useful when print_function is None
                 cProg = int(self.numTicks*self.ck/(self.n_steps-1)/3)    
                 #3: because 3 charachters are used
                 while((self.prog < cProg) & (not self.FLAG_ended)):
                     self.prog += 1
                     remTimeS = self._calc_ETA()
-                    if(remTimeS>=5940):
+                    if(remTimeS>5940): # less than 99h and more than 99m
                         progStr = "%02d" % int(ceil(remTimeS/3600))
                         self._print_func(progStr, end='')
                         self._print_func('h', end='')
-                    elif(remTimeS>=99):
+                    elif(remTimeS>99): # less than 99m and more than 99s
                         progStr = "%02d" % int(ceil(remTimeS/60))
                         self._print_func(progStr, end='')
                         self._print_func('m', end='')
-                    elif(remTimeS>0):
+                    elif(remTimeS>0): # less than 99s and more than 0
                         progStr = "%02d" % int(ceil(remTimeS))
                         self._print_func(progStr, end='')
                         self._print_func('s', end='')
                     else:
                         self.end()
         return remTimeS
     def end(self):
```

### Comparing `lognflow-0.6.7/lognflow.egg-info/PKG-INFO` & `lognflow-0.6.8/lognflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.7
+Version: 0.6.8
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -21,55 +21,37 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 lognflow
 ========
 
+Log and Flow tracking made easy with Python. You can install it by::
 
-.. image:: https://img.shields.io/pypi/v/lognflow.svg
-        :target: https://pypi.python.org/pypi/lognflow
-
-.. image:: https://img.shields.io/travis/arsadri/lognflow.svg
-        :target: https://travis-ci.com/arsadri/lognflow
-
-.. image:: https://readthedocs.org/projects/lognflow/badge/?version=latest
-        :target: https://lognflow.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-Log and Flow tracking made easy with Python. You can install it by:
-
-.. code-block:: python
 	pip install lognflow
 
+A simple program to use it would be similar to the following::
 
-A simple program to use it would be similar to the following:
-
-.. code-block:: python
 	from lognflow import lognflow
 	import numpy as np
 	vec = np.random.rand(100)
 	
 	logger = lognflow('c:\\test\\')
 	logger('This is a test for lognflow and log_var')
 	logger.log_single('vec', vec)
 
-The logviewer is also very useful.
+The logviewer is also very useful::
 
-.. code-block:: python
 	from lognflow import logviewer
-	
 	logged = logviewer('c:\\test\\some_log\')
 	vec = logged.get_single('vec')
 
-The printprogress makes a pretty nice progress bar.
+The printprogress makes a pretty nice progress bar::
 
-.. code-block:: python
 	from lognflow import printprogress
-	
 	N = 100
 	pbar = printprogress(N)
 	for _ in range(N):
 		# do_something()
 		pbar()
 
 In this package we use a folder on the HDD to generate files and folders in typical
@@ -179,7 +161,18 @@
 ------------------
 * Better documentation
 * added tifffile imread to logviewer and imwrite to lognflow
 
 0.6.7 (2023-04-27)
 ------------------
 * A bug in tifffile support was fixed
+
+0.6.8 (2023-05-04)
+------------------
+* Fixing readme for PyPI.
+* removed marker from log_plot. user marker and linestyle keyword arguments.
+* printprogress returns proper ETA every time if print_function is set to None::
+    pBar = printprogress(N, print_function = None)
+    for _ in range(N):
+        ETA = pBar()
+        print(f'ETA: {ETA}')
+
```

### Comparing `lognflow-0.6.7/lognflow.egg-info/SOURCES.txt` & `lognflow-0.6.8/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.7/setup.py` & `lognflow-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.6.7'
+__version__ = '0.6.8'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.6.7/tests/test_lognflow.py` & `lognflow-0.6.8/tests/test_lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.7/tests/test_logviewer.py` & `lognflow-0.6.8/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.7/tests/test_printprogress.py` & `lognflow-0.6.8/tests/test_printprogress.py`

 * *Files identical despite different names*

