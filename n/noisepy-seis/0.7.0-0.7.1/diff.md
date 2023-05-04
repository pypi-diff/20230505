# Comparing `tmp/noisepy_seis-0.7.0.tar.gz` & `tmp/noisepy_seis-0.7.1.tar.gz`

## Comparing `noisepy_seis-0.7.0.tar` & `noisepy_seis-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    12728 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   112952 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35394 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/LICENSE
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/README.md
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 noisepy_seis-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    12728 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   112952 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35394 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/README.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     8722 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/PKG-INFO
```

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.7.1/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.7.1/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.7.1/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.7.1/src/noisepy/seis/S2_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/__init__.py` & `noisepy_seis-0.7.1/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.7.1/src/noisepy/seis/asdfstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.7.1/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.7.1/src/noisepy/seis/datatypes.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/main.py` & `noisepy_seis-0.7.1/src/noisepy/seis/main.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.7.1/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.7.1/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.7.1/src/noisepy/seis/scedc_s3store.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/stores.py` & `noisepy_seis-0.7.1/src/noisepy/seis/stores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.7.1/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.7.1/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.7.1/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.7.1/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/.gitignore` & `noisepy_seis-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/LICENSE` & `noisepy_seis-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/README.md` & `noisepy_seis-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.0/pyproject.toml` & `noisepy_seis-0.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "noisepy-seis"
 dynamic = ["version"]
 description = "A High-performance Computing Python Package for Ambient Noise Analysis"
 readme = "README.md"
 license = {file= "LICENSE"}
-requires-python = ">=3.8,<=3.10"
+requires-python = ">=3.8"
 authors = [
     { email = "mdenolle@uw.edu", name = "Marine Denolle" },
     { email = "chengxin_jiang@fas.harvard.edu", name = "Chengxin Jiang" },
 ]
 keywords = [
     "ambient",
     "change",
@@ -32,15 +32,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
 ]
 dependencies = [
     "DateTimeRange==2.0.0",
     "h5py>=3.8.0",
     "mpi4py>=3.1.4",
-    "numba>=0.56.4",
+    "numba>=0.57.0",
     "numpy>=1.22.0",
     "pandas>=1.5.3",
     "pyasdf>=0.7.5",
     "pycwt>=0.3.0a22",
     "diskcache>=5.5",
 ]
```

### Comparing `noisepy_seis-0.7.0/PKG-INFO` & `noisepy_seis-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.7.0
+Version: 0.7.1
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -28,20 +28,20 @@
 License-File: LICENSE
 Keywords: ambient,change,cross-correlation,dispersion,monitoring,noise,seismic,surface,velocity,wave
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: <=3.10,>=3.8
+Requires-Python: >=3.8
 Requires-Dist: datetimerange==2.0.0
 Requires-Dist: diskcache>=5.5
 Requires-Dist: h5py>=3.8.0
 Requires-Dist: mpi4py>=3.1.4
-Requires-Dist: numba>=0.56.4
+Requires-Dist: numba>=0.57.0
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: pyasdf>=0.7.5
 Requires-Dist: pycwt>=0.3.0a22
 Provides-Extra: dev
 Requires-Dist: memory-profiler>=0.61; extra == 'dev'
 Requires-Dist: pre-commit>=3.2; extra == 'dev'
```

