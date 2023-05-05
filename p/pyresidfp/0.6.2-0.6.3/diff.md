# Comparing `tmp/pyresidfp-0.6.2.tar.gz` & `tmp/pyresidfp-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresidfp-0.6.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyresidfp-0.6.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyresidfp-0.6.2.tar` & `pyresidfp-0.6.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/.gitignore
--rw-r--r--   0        0        0     3761 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/CMakeLists.txt
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/COPYING
--rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/README.md
--rw-r--r--   0        0        0     2293 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/PythonSid.cpp
--rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/PythonSid.h
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/config.h.in
--rw-r--r--   0        0        0     1110 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/pyresidfp/__init__.py
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/pyresidfp/_version.py
--rw-r--r--   0        0        0     4147 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/pyresidfp/musical_scale.py
--rw-r--r--   0        0        0     3141 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/pyresidfp/registers.py
--rw-r--r--   0        0        0    10774 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/pyresidfp/sound_interface_device.py
--rw-r--r--   0        0        0     8839 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/pyresidfp.cpp
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/AUTHORS
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/COPYING
--rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Dac.cpp
--rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Dac.h
--rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/EnvelopeGenerator.cpp
--rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/EnvelopeGenerator.h
--rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/ExternalFilter.cpp
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/ExternalFilter.h
--rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Filter.cpp
--rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Filter.h
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Filter6581.cpp
--rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Filter6581.h
--rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Filter8580.cpp
--rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Filter8580.h
--rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/FilterModelConfig.cpp
--rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/FilterModelConfig.h
--rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/FilterModelConfig6581.cpp
--rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/FilterModelConfig6581.h
--rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/FilterModelConfig8580.cpp
--rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/FilterModelConfig8580.h
--rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Integrator6581.cpp
--rw-r--r--   0        0        0     9208 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Integrator6581.h
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Integrator8580.cpp
--rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Integrator8580.h
--rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/OpAmp.cpp
--rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/OpAmp.h
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Potentiometer.h
--rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/README
--rw-r--r--   0        0        0    13758 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/SID.cpp
--rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/SID.h
--rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Spline.cpp
--rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Spline.h
--rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/Voice.h
--rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/WaveformCalculator.cpp
--rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/WaveformCalculator.h
--rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/WaveformGenerator.cpp
--rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/WaveformGenerator.h
--rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/array.h
--rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/resample/Resampler.h
--rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/resample/SincResampler.cpp
--rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/resample/SincResampler.h
--rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/resample/TwoPassSincResampler.h
--rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/resample/ZeroOrderResampler.h
--rw-r--r--   0        0        0     2788 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/resample/test.cpp
--rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/siddefs-fp.h.in
--rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/residfp/version.cc
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/sidcxx11.h
--rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/src/sidcxx14.h
--rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/.gitignore
+-rw-r--r--   0        0        0     3761 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/CMakeLists.txt
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/COPYING
+-rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/README.md
+-rw-r--r--   0        0        0     2293 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/PythonSid.cpp
+-rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/PythonSid.h
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/config.h.in
+-rw-r--r--   0        0        0     1110 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/pyresidfp/__init__.py
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/pyresidfp/_version.py
+-rw-r--r--   0        0        0     4147 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/pyresidfp/musical_scale.py
+-rw-r--r--   0        0        0     3141 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/pyresidfp/registers.py
+-rw-r--r--   0        0        0    10774 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/pyresidfp/sound_interface_device.py
+-rw-r--r--   0        0        0     8839 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/pyresidfp.cpp
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/AUTHORS
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/COPYING
+-rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Dac.cpp
+-rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Dac.h
+-rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/EnvelopeGenerator.cpp
+-rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/EnvelopeGenerator.h
+-rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/ExternalFilter.cpp
+-rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/ExternalFilter.h
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Filter.cpp
+-rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Filter.h
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Filter6581.cpp
+-rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Filter6581.h
+-rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Filter8580.cpp
+-rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Filter8580.h
+-rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/FilterModelConfig.cpp
+-rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/FilterModelConfig.h
+-rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/FilterModelConfig6581.cpp
+-rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/FilterModelConfig6581.h
+-rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/FilterModelConfig8580.cpp
+-rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/FilterModelConfig8580.h
+-rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Integrator6581.cpp
+-rw-r--r--   0        0        0     9208 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Integrator6581.h
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Integrator8580.cpp
+-rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Integrator8580.h
+-rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/OpAmp.cpp
+-rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/OpAmp.h
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Potentiometer.h
+-rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/README
+-rw-r--r--   0        0        0    13758 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/SID.cpp
+-rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/SID.h
+-rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Spline.cpp
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Spline.h
+-rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/Voice.h
+-rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/WaveformCalculator.cpp
+-rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/WaveformCalculator.h
+-rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/WaveformGenerator.cpp
+-rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/WaveformGenerator.h
+-rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/array.h
+-rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/resample/Resampler.h
+-rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/resample/SincResampler.cpp
+-rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/resample/SincResampler.h
+-rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/resample/TwoPassSincResampler.h
+-rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/resample/ZeroOrderResampler.h
+-rw-r--r--   0        0        0     2788 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/resample/test.cpp
+-rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/siddefs-fp.h.in
+-rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/residfp/version.cc
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/sidcxx11.h
+-rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/src/sidcxx14.h
+-rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.3/PKG-INFO
```

### Comparing `pyresidfp-0.6.2/CMakeLists.txt` & `pyresidfp-0.6.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/COPYING` & `pyresidfp-0.6.3/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/README.md` & `pyresidfp-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/pyproject.toml` & `pyresidfp-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/PythonSid.cpp` & `pyresidfp-0.6.3/src/PythonSid.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/PythonSid.h` & `pyresidfp-0.6.3/src/PythonSid.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/pyresidfp/__init__.py` & `pyresidfp-0.6.3/src/pyresidfp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/pyresidfp/musical_scale.py` & `pyresidfp-0.6.3/src/pyresidfp/musical_scale.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/pyresidfp/registers.py` & `pyresidfp-0.6.3/src/pyresidfp/registers.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/pyresidfp/sound_interface_device.py` & `pyresidfp-0.6.3/src/pyresidfp/sound_interface_device.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/pyresidfp.cpp` & `pyresidfp-0.6.3/src/pyresidfp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/COPYING` & `pyresidfp-0.6.3/src/residfp/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Dac.cpp` & `pyresidfp-0.6.3/src/residfp/Dac.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Dac.h` & `pyresidfp-0.6.3/src/residfp/Dac.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/EnvelopeGenerator.cpp` & `pyresidfp-0.6.3/src/residfp/EnvelopeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/EnvelopeGenerator.h` & `pyresidfp-0.6.3/src/residfp/EnvelopeGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/ExternalFilter.cpp` & `pyresidfp-0.6.3/src/residfp/ExternalFilter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/ExternalFilter.h` & `pyresidfp-0.6.3/src/residfp/ExternalFilter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Filter.cpp` & `pyresidfp-0.6.3/src/residfp/Filter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Filter.h` & `pyresidfp-0.6.3/src/residfp/Filter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Filter6581.cpp` & `pyresidfp-0.6.3/src/residfp/Filter6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Filter6581.h` & `pyresidfp-0.6.3/src/residfp/Filter6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Filter8580.cpp` & `pyresidfp-0.6.3/src/residfp/Filter8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Filter8580.h` & `pyresidfp-0.6.3/src/residfp/Filter8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/FilterModelConfig.cpp` & `pyresidfp-0.6.3/src/residfp/FilterModelConfig.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/FilterModelConfig.h` & `pyresidfp-0.6.3/src/residfp/FilterModelConfig.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/FilterModelConfig6581.cpp` & `pyresidfp-0.6.3/src/residfp/FilterModelConfig6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/FilterModelConfig6581.h` & `pyresidfp-0.6.3/src/residfp/FilterModelConfig6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/FilterModelConfig8580.cpp` & `pyresidfp-0.6.3/src/residfp/FilterModelConfig8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/FilterModelConfig8580.h` & `pyresidfp-0.6.3/src/residfp/FilterModelConfig8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Integrator6581.cpp` & `pyresidfp-0.6.3/src/residfp/Integrator6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Integrator6581.h` & `pyresidfp-0.6.3/src/residfp/Integrator6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Integrator8580.cpp` & `pyresidfp-0.6.3/src/residfp/Integrator8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Integrator8580.h` & `pyresidfp-0.6.3/src/residfp/Integrator8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/OpAmp.cpp` & `pyresidfp-0.6.3/src/residfp/OpAmp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/OpAmp.h` & `pyresidfp-0.6.3/src/residfp/OpAmp.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Potentiometer.h` & `pyresidfp-0.6.3/src/residfp/Potentiometer.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/README` & `pyresidfp-0.6.3/src/residfp/README`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/SID.cpp` & `pyresidfp-0.6.3/src/residfp/SID.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/SID.h` & `pyresidfp-0.6.3/src/residfp/SID.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Spline.cpp` & `pyresidfp-0.6.3/src/residfp/Spline.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Spline.h` & `pyresidfp-0.6.3/src/residfp/Spline.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/Voice.h` & `pyresidfp-0.6.3/src/residfp/Voice.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/WaveformCalculator.cpp` & `pyresidfp-0.6.3/src/residfp/WaveformCalculator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/WaveformCalculator.h` & `pyresidfp-0.6.3/src/residfp/WaveformCalculator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/WaveformGenerator.cpp` & `pyresidfp-0.6.3/src/residfp/WaveformGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/WaveformGenerator.h` & `pyresidfp-0.6.3/src/residfp/WaveformGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/array.h` & `pyresidfp-0.6.3/src/residfp/array.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/resample/Resampler.h` & `pyresidfp-0.6.3/src/residfp/resample/Resampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/resample/SincResampler.cpp` & `pyresidfp-0.6.3/src/residfp/resample/SincResampler.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/resample/SincResampler.h` & `pyresidfp-0.6.3/src/residfp/resample/SincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/resample/TwoPassSincResampler.h` & `pyresidfp-0.6.3/src/residfp/resample/TwoPassSincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/resample/ZeroOrderResampler.h` & `pyresidfp-0.6.3/src/residfp/resample/ZeroOrderResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/resample/test.cpp` & `pyresidfp-0.6.3/src/residfp/resample/test.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/siddefs-fp.h.in` & `pyresidfp-0.6.3/src/residfp/siddefs-fp.h.in`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/residfp/version.cc` & `pyresidfp-0.6.3/src/residfp/version.cc`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/sidcxx11.h` & `pyresidfp-0.6.3/src/sidcxx11.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/src/sidcxx14.h` & `pyresidfp-0.6.3/src/sidcxx14.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.2/PKG-INFO` & `pyresidfp-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresidfp
-Version: 0.6.2
+Version: 0.6.3
 Summary: Emulates the SID sound-chip
 Author-Email: Sebastian Klemke <pypi@nerdheim.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

