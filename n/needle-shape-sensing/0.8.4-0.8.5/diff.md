# Comparing `tmp/needle-shape-sensing-0.8.4.tar.gz` & `tmp/needle-shape-sensing-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\needle-shape-sensing-0.8.4.tar", last modified: Fri May  5 15:57:41 2023, max compression
+gzip compressed data, was "dist\needle-shape-sensing-0.8.5.tar", last modified: Fri May  5 16:00:36 2023, max compression
```

## Comparing `needle-shape-sensing-0.8.4.tar` & `needle-shape-sensing-0.8.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:57:41.000000 needle-shape-sensing-0.8.4/
--rw-rw-rw-   0        0        0     1072 2021-08-13 20:31:43.000000 needle-shape-sensing-0.8.4/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 15:57:41.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/
--rw-rw-rw-   0        0        0    12846 2023-03-31 17:18:02.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/cost_functions.py
--rw-rw-rw-   0        0        0     1452 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/fbg_signal_processing.py
--rw-rw-rw-   0        0        0     9347 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/geometry.py
--rw-rw-rw-   0        0        0    22289 2023-03-31 17:18:02.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/intrinsics.py
--rw-rw-rw-   0        0        0    24248 2023-04-11 02:33:25.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/numerical.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:57:41.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/
--rw-rw-rw-   0        0        0      588 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/config.py
--rw-rw-rw-   0        0        0     1278 2023-01-03 18:44:04.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/geometry.py
--rw-rw-rw-   0        0        0    13480 2023-01-03 18:44:04.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/intrinsics.py
--rw-rw-rw-   0        0        0     8017 2023-03-02 20:35:13.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/numerical.py
--rw-rw-rw-   0        0        0      106 2022-12-07 21:25:38.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/__init__.py
--rw-rw-rw-   0        0        0    41494 2023-05-05 15:46:00.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/sensorized_needles.py
--rw-rw-rw-   0        0        0    19678 2023-05-05 15:56:03.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/shape_sensing.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:57:41.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/tensorflow/
--rw-rw-rw-   0        0        0     1576 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/tensorflow/geometry.py
--rw-rw-rw-   0        0        0    12463 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/tensorflow/intrinsics.py
--rw-rw-rw-   0        0        0     8692 2023-03-02 20:35:13.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/tensorflow/numerical.py
--rw-rw-rw-   0        0        0       96 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/tensorflow/__init__.py
--rw-rw-rw-   0        0        0      214 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.4/needle_shape_sensing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:57:41.000000 needle-shape-sensing-0.8.4/needle_shape_sensing.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-05 15:57:39.000000 needle-shape-sensing-0.8.4/needle_shape_sensing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1678 2023-05-05 15:57:39.000000 needle-shape-sensing-0.8.4/needle_shape_sensing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-05 15:57:39.000000 needle-shape-sensing-0.8.4/needle_shape_sensing.egg-info/requires.txt
--rw-rw-rw-   0        0        0      935 2023-05-05 15:57:40.000000 needle-shape-sensing-0.8.4/needle_shape_sensing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       21 2023-05-05 15:57:39.000000 needle-shape-sensing-0.8.4/needle_shape_sensing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1678 2023-05-05 15:57:41.000000 needle-shape-sensing-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     1089 2021-08-13 16:01:29.000000 needle-shape-sensing-0.8.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 15:57:41.000000 needle-shape-sensing-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-05-05 15:56:48.000000 needle-shape-sensing-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:00:36.000000 needle-shape-sensing-0.8.5/
+-rw-rw-rw-   0        0        0     1072 2021-08-13 20:31:43.000000 needle-shape-sensing-0.8.5/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 16:00:36.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/
+-rw-rw-rw-   0        0        0    12846 2023-03-31 17:18:02.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/cost_functions.py
+-rw-rw-rw-   0        0        0     1452 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/fbg_signal_processing.py
+-rw-rw-rw-   0        0        0     9347 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/geometry.py
+-rw-rw-rw-   0        0        0    22289 2023-03-31 17:18:02.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/intrinsics.py
+-rw-rw-rw-   0        0        0    24248 2023-04-11 02:33:25.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/numerical.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:00:36.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/
+-rw-rw-rw-   0        0        0      588 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/config.py
+-rw-rw-rw-   0        0        0     1278 2023-01-03 18:44:04.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/geometry.py
+-rw-rw-rw-   0        0        0    13480 2023-01-03 18:44:04.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/intrinsics.py
+-rw-rw-rw-   0        0        0     8017 2023-03-02 20:35:13.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/numerical.py
+-rw-rw-rw-   0        0        0      106 2022-12-07 21:25:38.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/__init__.py
+-rw-rw-rw-   0        0        0    41392 2023-05-05 15:59:30.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/sensorized_needles.py
+-rw-rw-rw-   0        0        0    19678 2023-05-05 15:56:03.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/shape_sensing.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:00:36.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/tensorflow/
+-rw-rw-rw-   0        0        0     1576 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/tensorflow/geometry.py
+-rw-rw-rw-   0        0        0    12463 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/tensorflow/intrinsics.py
+-rw-rw-rw-   0        0        0     8692 2023-03-02 20:35:13.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/tensorflow/numerical.py
+-rw-rw-rw-   0        0        0       96 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0      214 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.5/needle_shape_sensing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:00:36.000000 needle-shape-sensing-0.8.5/needle_shape_sensing.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-05 16:00:35.000000 needle-shape-sensing-0.8.5/needle_shape_sensing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1678 2023-05-05 16:00:35.000000 needle-shape-sensing-0.8.5/needle_shape_sensing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-05 16:00:35.000000 needle-shape-sensing-0.8.5/needle_shape_sensing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      935 2023-05-05 16:00:35.000000 needle-shape-sensing-0.8.5/needle_shape_sensing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       21 2023-05-05 16:00:35.000000 needle-shape-sensing-0.8.5/needle_shape_sensing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1678 2023-05-05 16:00:36.000000 needle-shape-sensing-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1089 2021-08-13 16:01:29.000000 needle-shape-sensing-0.8.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 16:00:36.000000 needle-shape-sensing-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-05-05 15:59:08.000000 needle-shape-sensing-0.8.5/setup.py
```

### Comparing `needle-shape-sensing-0.8.4/LICENSE.txt` & `needle-shape-sensing-0.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/cost_functions.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/cost_functions.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/fbg_signal_processing.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/fbg_signal_processing.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/geometry.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/geometry.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/intrinsics.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/intrinsics.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/numerical.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/numerical.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/config.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/config.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/geometry.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/geometry.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/intrinsics.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/intrinsics.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/pytorch/numerical.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/pytorch/numerical.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/sensorized_needles.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/sensorized_needles.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,16 +645,14 @@
     def curvatures_processed( self, proc_signals: Union[ dict, np.ndarray ] ) -> Union[ dict, np.ndarray ]:
         """ Determine the curvatures from signals input
 
             Args:
                 proc_signals: {AA_index: processed signal} must be processed and temperature compensated
 
         """
-        print("FBGNeedle Curvatures processed")
-
         if isinstance( proc_signals, dict ):
             curvatures = { }
             for aa_i, proc_signal in proc_signals.items():
                 # get the appropriate calibration matrix
                 C_aa_i = self.aa_cal( f"AA{aa_i}" ) if isinstance( aa_i, int ) else self.aa_cal( aa_i )
 
                 curvatures[ aa_i ] = C_aa_i @ proc_signal  # 2 x num_AA @ num_AA x 1
@@ -1022,16 +1020,14 @@
     def curvatures_processed( self, proc_signals: Union[ dict, np.ndarray ] ) -> Union[ dict, np.ndarray ]:
         """ Determine the curvatures from signals input
 
             Args:
                 proc_signals: {AA_index: processed signal} must be processed and temperature compensated
 
         """
-        print("MCFNeedle curvatures processed")
-
         if isinstance( proc_signals, dict ):
             curvatures = { }
             for aa_i, proc_signal in proc_signals.items():
                 if 0 <= self.central_core_ch < proc_signal.shape[0]:
                     proc_signal = np.append(
                             proc_signal[:self.central_core_ch],
                             proc_signal[self.central_core_ch+1:-1]
```

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/shape_sensing.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/shape_sensing.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/tensorflow/geometry.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/tensorflow/geometry.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/tensorflow/intrinsics.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/tensorflow/intrinsics.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing/tensorflow/numerical.py` & `needle-shape-sensing-0.8.5/needle_shape_sensing/tensorflow/numerical.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing.egg-info/PKG-INFO` & `needle-shape-sensing-0.8.5/needle_shape_sensing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: needle-shape-sensing
-Version: 0.8.4
+Version: 0.8.5
 Summary: Needle Shape Sensing library
 Home-page: http://pypi.python.org/pypi/needle-shape-sensing/
 Author: Dimitri Lezcano
 Author-email: dlezcan1@jhu.edu
 License: LICENSE.txt
 Description: # python-needle-shape-sensing
         Author: Dimitri Lezcano
```

### Comparing `needle-shape-sensing-0.8.4/needle_shape_sensing.egg-info/SOURCES.txt` & `needle-shape-sensing-0.8.5/needle_shape_sensing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/PKG-INFO` & `needle-shape-sensing-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: needle-shape-sensing
-Version: 0.8.4
+Version: 0.8.5
 Summary: Needle Shape Sensing library
 Home-page: http://pypi.python.org/pypi/needle-shape-sensing/
 Author: Dimitri Lezcano
 Author-email: dlezcan1@jhu.edu
 License: LICENSE.txt
 Description: # python-needle-shape-sensing
         Author: Dimitri Lezcano
```

### Comparing `needle-shape-sensing-0.8.4/README.md` & `needle-shape-sensing-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.4/setup.py` & `needle-shape-sensing-0.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
         name='needle-shape-sensing',
-        version='0.8.4',
+        version='0.8.5',
         author='Dimitri Lezcano',
         author_email='dlezcan1@jhu.edu',
         packages=find_packages(),
         url='http://pypi.python.org/pypi/needle-shape-sensing/',
         license='LICENSE.txt',
         description='Needle Shape Sensing library',
         long_description=open( 'README.md' ).read(),
```

