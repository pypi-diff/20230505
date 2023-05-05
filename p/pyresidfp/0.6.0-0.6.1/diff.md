# Comparing `tmp/pyresidfp-0.6.0.tar.gz` & `tmp/pyresidfp-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresidfp-0.6.0.tar", last modified: Tue Dec 20 00:44:34 2022, max compression
+gzip compressed data, was "pyresidfp-0.6.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyresidfp-0.6.0.tar` & `pyresidfp-0.6.1.tar`

### file list

```diff
@@ -1,77 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:44:34.702050 pyresidfp-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:44:34.686050 pyresidfp-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:44:34.690050 pyresidfp-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/.github/workflows/build_wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2022-12-20 00:44:34.698050 pyresidfp-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 00:44:34.702050 pyresidfp-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:44:34.690050 pyresidfp-0.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/PythonSid.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/PythonSid.h
--rw-r--r--   0 runner    (1001) docker     (123)      435 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:44:34.690050 pyresidfp-0.6.0/src/pyresidfp/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/pyresidfp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/pyresidfp/musical_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/pyresidfp/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/pyresidfp/sound_interface_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/pyresidfp.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:44:34.690050 pyresidfp-0.6.0/src/pyresidfp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2022-12-20 00:44:34.000000 pyresidfp-0.6.0/src/pyresidfp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2022-12-20 00:44:34.000000 pyresidfp-0.6.0/src/pyresidfp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 00:44:34.000000 pyresidfp-0.6.0/src/pyresidfp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-20 00:44:34.000000 pyresidfp-0.6.0/src/pyresidfp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:44:34.698050 pyresidfp-0.6.0/src/residfp/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Dac.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Dac.h
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/EnvelopeGenerator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/EnvelopeGenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/ExternalFilter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/ExternalFilter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Filter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Filter6581.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Filter6581.h
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Filter8580.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Filter8580.h
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/FilterModelConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/FilterModelConfig.h
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/FilterModelConfig6581.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/FilterModelConfig6581.h
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/FilterModelConfig8580.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/FilterModelConfig8580.h
--rw-r--r--   0 runner    (1001) docker     (123)      965 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Integrator6581.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Integrator6581.h
--rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Integrator8580.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Integrator8580.h
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/OpAmp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/OpAmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Potentiometer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/README
--rw-r--r--   0 runner    (1001) docker     (123)    13758 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/SID.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/SID.h
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Spline.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Spline.h
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/Voice.h
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/WaveformCalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/WaveformCalculator.h
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/WaveformGenerator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/WaveformGenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/array.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:44:34.698050 pyresidfp-0.6.0/src/residfp/resample/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/resample/Resampler.h
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/resample/SincResampler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/resample/SincResampler.h
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/resample/TwoPassSincResampler.h
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/resample/ZeroOrderResampler.h
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/resample/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/siddefs-fp.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/residfp/version.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/sidcxx11.h
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2022-12-20 00:44:20.000000 pyresidfp-0.6.0/src/sidcxx14.h
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/.gitignore
+-rw-r--r--   0        0        0     3761 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/CMakeLists.txt
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/COPYING
+-rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/README.md
+-rw-r--r--   0        0        0     2293 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/PythonSid.cpp
+-rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/PythonSid.h
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/config.h.in
+-rw-r--r--   0        0        0     1110 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/pyresidfp/__init__.py
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/pyresidfp/_version.py
+-rw-r--r--   0        0        0     4147 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/pyresidfp/musical_scale.py
+-rw-r--r--   0        0        0     3141 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/pyresidfp/registers.py
+-rw-r--r--   0        0        0    10774 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/pyresidfp/sound_interface_device.py
+-rw-r--r--   0        0        0     8839 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/pyresidfp.cpp
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/AUTHORS
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/COPYING
+-rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Dac.cpp
+-rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Dac.h
+-rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/EnvelopeGenerator.cpp
+-rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/EnvelopeGenerator.h
+-rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/ExternalFilter.cpp
+-rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/ExternalFilter.h
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Filter.cpp
+-rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Filter.h
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Filter6581.cpp
+-rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Filter6581.h
+-rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Filter8580.cpp
+-rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Filter8580.h
+-rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/FilterModelConfig.cpp
+-rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/FilterModelConfig.h
+-rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/FilterModelConfig6581.cpp
+-rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/FilterModelConfig6581.h
+-rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/FilterModelConfig8580.cpp
+-rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/FilterModelConfig8580.h
+-rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Integrator6581.cpp
+-rw-r--r--   0        0        0     9208 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Integrator6581.h
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Integrator8580.cpp
+-rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Integrator8580.h
+-rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/OpAmp.cpp
+-rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/OpAmp.h
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Potentiometer.h
+-rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/README
+-rw-r--r--   0        0        0    13758 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/SID.cpp
+-rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/SID.h
+-rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Spline.cpp
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Spline.h
+-rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/Voice.h
+-rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/WaveformCalculator.cpp
+-rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/WaveformCalculator.h
+-rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/WaveformGenerator.cpp
+-rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/WaveformGenerator.h
+-rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/array.h
+-rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/resample/Resampler.h
+-rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/resample/SincResampler.cpp
+-rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/resample/SincResampler.h
+-rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/resample/TwoPassSincResampler.h
+-rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/resample/ZeroOrderResampler.h
+-rw-r--r--   0        0        0     2788 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/resample/test.cpp
+-rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/siddefs-fp.h.in
+-rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/residfp/version.cc
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/sidcxx11.h
+-rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/src/sidcxx14.h
+-rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.1/PKG-INFO
```

### Comparing `pyresidfp-0.6.0/CMakeLists.txt` & `pyresidfp-0.6.1/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-cmake_minimum_required(VERSION 3.25...3.25)
-project(${SKBUILD_PROJECT_NAME} VERSION ${SKBUILD_PROJECT_VERSION})
+cmake_minimum_required(VERSION 3.15...3.26)
 
+string(REGEX REPLACE "^([0-9]+\.[0-9]+(\.[0-9]+)?)(\.[^.]*)*$" "\\1" TRUNCATED_PROJECT_VERSION ${SKBUILD_PROJECT_VERSION})
+
+project(${SKBUILD_PROJECT_NAME} VERSION ${TRUNCATED_PROJECT_VERSION} LANGUAGES CXX)
+
+set(PYBIND11_NEWPYTHON ON)
 find_package(pybind11 CONFIG REQUIRED)
 
 include(CheckCXXSourceCompiles)
 include(CheckIncludeFileCXX)
+include(CheckIPOSupported)
 
 enable_testing()
 
 if(CMAKE_CXX_COMPILER_ID MATCHES "Clang")
   set(USE_CLANG TRUE)
 elseif(CMAKE_CXX_COMPILER_ID MATCHES "GNU")
   set(USE_GCC TRUE)
@@ -24,14 +29,16 @@
   set(HAVE_ARM_NEON_H FALSE)
 endif()
 
 check_cxx_source_compiles("
 int main(void) { if (__builtin_expect(0, 0)) return 1; return 0; }
 " HAVE_BUILTIN_EXPECT)
 
+check_ipo_supported(RESULT IPO_SUPPORTED OUTPUT IPO_ERROR)
+
 set(CMAKE_CXX_STANDARD 14)
 set(CMAKE_CXX_EXTENSIONS OFF)
 set(PACKAGE_VERSION ${PROJECT_VERSION})
 set(RESID_INLINE inline)
 set(RESID_INLINING 1)
 set(RESID_BRANCH_HINTS 1)
 set(HAVE_CXX11 1)
@@ -95,8 +102,15 @@
 target_include_directories(_pyresidfp
         PRIVATE ${CMAKE_CURRENT_BINARY_DIR} ${CMAKE_CURRENT_SOURCE_DIR}
         src/residfp src/residfp/resample)
 target_compile_definitions(_pyresidfp PRIVATE HAVE_CONFIG_H)
 target_compile_definitions(_pyresidfp PRIVATE PROJECT_VERSION)
 set_property(TARGET _pyresidfp PROPERTY CXX_STANDARD 14)
 
+if (IPO_SUPPORTED)
+  message(STATUS "IPO / LTO enabled")
+  set_property(TARGET _pyresidfp PROPERTY INTERPROCEDURAL_OPTIMIZATION TRUE)
+else()
+  message(STATUS "IPO / LTO not supported: <${IPO_ERROR}>")
+endif()
+
 install(TARGETS _pyresidfp DESTINATION .)
```

### Comparing `pyresidfp-0.6.0/COPYING` & `pyresidfp-0.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/PKG-INFO` & `pyresidfp-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pyresidfp
-Version: 0.6.0
+Version: 0.6.1
 Summary: Emulates the SID sound-chip
-Home-page: https://github.com/pyresidfp/pyresidfp
-Author: Sebastian Klemke
-Author-email: pypi@nerdheim.de
+Author-Email: Sebastian Klemke <pypi@nerdheim.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: Topic :: System :: Emulators
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.7.0,<4.0.0
+Project-URL: Homepage, https://github.com/pyresidfp/pyresidfp
+Project-URL: Bug tracker, https://github.com/pyresidfp/pyresidfp/issues
+Requires-Python: <4.0.0,>=3.7.0
 Description-Content-Type: text/markdown
-License-File: COPYING
 
 # pyresidfp
 
 Emulates the SID sound-chip in software. The C++ emulation code was copied over from
 [libsidplayfp](https://github.com/libsidplayfp/libsidplayfp).
 
 ## How to install
```

### Comparing `pyresidfp-0.6.0/README.md` & `pyresidfp-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/setup.py` & `pyresidfp-0.6.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  This file is part of pyresidfp, a SID emulation package for Python.
 #
-#  Copyright (c) 2018-2022.  Sebastian Klemke <packet@nerdheim.de>
+#  Copyright (c) 2018-2023.  Sebastian Klemke <pypi@nerdheim.de>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 2 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -12,47 +12,50 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
-import pybind11
-
-from skbuild import setup
-
-
-with open('README.md', 'r') as fh:
-    long_description = fh.read()
-
-pybind_dir = pybind11.get_cmake_dir()
-
-setup(
-    name='pyresidfp',
-    author='Sebastian Klemke',
-    author_email='pypi@nerdheim.de',
-    description='Emulates the SID sound-chip',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/pyresidfp/pyresidfp',
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: C++',
-        'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
-        'Operating System :: OS Independent',
-        'Topic :: Multimedia :: Sound/Audio :: Sound Synthesis',
-        'Topic :: System :: Emulators',
-        'Intended Audience :: Developers',
-        'Development Status :: 2 - Pre-Alpha'
-    ],
-    packages=["pyresidfp"],
-    package_dir={"": "src"},
-    cmake_install_dir="src/pyresidfp",
-    cmake_args=['-DCMAKE_PREFIX_PATH=' + pybind_dir] if pybind_dir else None,
-    python_requires='>=3.7.0,<4.0.0',
-)
+[build-system]
+requires = ["scikit-build-core", "pybind11"]
+build-backend = "scikit_build_core.build"
+
+[tool.scikit-build]
+metadata.version.provider = "scikit_build_core.metadata.setuptools_scm"
+sdist.include = ["src/pyresidfp/_version.py"]
+sdist.exclude = [".github", "scripts"]
+wheel.packages = ["src/pyresidfp"]
+minimum-version = "0.3"
+
+[tool.setuptools_scm]
+write_to = "src/pyresidfp/_version.py"
+
+[project]
+name = "pyresidfp"
+authors = [
+  { name="Sebastian Klemke", email="pypi@nerdheim.de" },
+]
+description = "Emulates the SID sound-chip"
+readme = "README.md"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: C++",
+    "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
+    "Operating System :: OS Independent",
+    "Topic :: Multimedia :: Sound/Audio :: Sound Synthesis",
+    "Topic :: System :: Emulators",
+    "Intended Audience :: Developers",
+    "Development Status :: 2 - Pre-Alpha",
+]
+requires-python = ">=3.7.0,<4.0.0"
+dynamic = ["version"]
+
+[project.urls]
+"Homepage" = "https://github.com/pyresidfp/pyresidfp"
+"Bug Tracker" = "https://github.com/pyresidfp/pyresidfp/issues"
```

### Comparing `pyresidfp-0.6.0/src/PythonSid.cpp` & `pyresidfp-0.6.1/src/PythonSid.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of pyresidfp, a SID emulation package for Python.
  *
- * Copyright (c) 2018-2022.  Sebastian Klemke <packet@nerdheim.de>
+ * Copyright (c) 2018-2023.  Sebastian Klemke <pypi@nerdheim.de>
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 2 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
```

### Comparing `pyresidfp-0.6.0/src/PythonSid.h` & `pyresidfp-0.6.1/src/PythonSid.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of pyresidfp, a SID emulation package for Python.
  *
- * Copyright (c) 2018-2022.  Sebastian Klemke <packet@nerdheim.de>
+ * Copyright (c) 2018-2023.  Sebastian Klemke <pypi@nerdheim.de>
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 2 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
```

### Comparing `pyresidfp-0.6.0/src/pyresidfp/__init__.py` & `pyresidfp-0.6.1/src/pyresidfp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  This file is part of pyresidfp, a SID emulation package for Python.
 #
-#  Copyright (c) 2018-2022.  Sebastian Klemke <packet@nerdheim.de>
+#  Copyright (c) 2018-2023.  Sebastian Klemke <pypi@nerdheim.de>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 2 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
```

### Comparing `pyresidfp-0.6.0/src/pyresidfp/musical_scale.py` & `pyresidfp-0.6.1/src/pyresidfp/musical_scale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  This file is part of pyresidfp, a SID emulation package for Python.
 #
-#  Copyright (c) 2018-2022.  Sebastian Klemke <packet@nerdheim.de>
+#  Copyright (c) 2018-2023.  Sebastian Klemke <pypi@nerdheim.de>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 2 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
```

### Comparing `pyresidfp-0.6.0/src/pyresidfp/registers.py` & `pyresidfp-0.6.1/src/pyresidfp/registers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  This file is part of pyresidfp, a SID emulation package for Python.
 #
-#  Copyright (c) 2018-2022.  Sebastian Klemke <packet@nerdheim.de>
+#  Copyright (c) 2018-2023.  Sebastian Klemke <pypi@nerdheim.de>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 2 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
```

### Comparing `pyresidfp-0.6.0/src/pyresidfp/sound_interface_device.py` & `pyresidfp-0.6.1/src/pyresidfp/sound_interface_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  This file is part of pyresidfp, a SID emulation package for Python.
 #
-#  Copyright (c) 2018-2022.  Sebastian Klemke <packet@nerdheim.de>
+#  Copyright (c) 2018-2023.  Sebastian Klemke <pypi@nerdheim.de>
 #
 #  This program is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 2 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -17,15 +17,15 @@
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 import datetime
 import logging
 from enum import Enum
 from typing import Any, Callable, Dict, Tuple
 
-from ._pyresidfp import ChipModel, SID, SamplingMethod
+from _pyresidfp import ChipModel, SID, SamplingMethod
 
 from .musical_scale import Tone
 from .registers import ReadableRegister, WritableRegister
 
 
 class Voice(Enum):
     """The three voices of an emulated MOS 6581 / MOS 8580"""
```

### Comparing `pyresidfp-0.6.0/src/pyresidfp.cpp` & `pyresidfp-0.6.1/src/pyresidfp.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of pyresidfp, a SID emulation package for Python.
  *
- * Copyright (c) 2018-2022.  Sebastian Klemke <packet@nerdheim.de>
+ * Copyright (c) 2018-2023.  Sebastian Klemke <pypi@nerdheim.de>
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 2 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
```

### Comparing `pyresidfp-0.6.0/src/residfp/COPYING` & `pyresidfp-0.6.1/src/residfp/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Dac.cpp` & `pyresidfp-0.6.1/src/residfp/Dac.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Dac.h` & `pyresidfp-0.6.1/src/residfp/Dac.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/EnvelopeGenerator.cpp` & `pyresidfp-0.6.1/src/residfp/EnvelopeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/EnvelopeGenerator.h` & `pyresidfp-0.6.1/src/residfp/EnvelopeGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/ExternalFilter.cpp` & `pyresidfp-0.6.1/src/residfp/ExternalFilter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/ExternalFilter.h` & `pyresidfp-0.6.1/src/residfp/ExternalFilter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Filter.cpp` & `pyresidfp-0.6.1/src/residfp/Filter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Filter.h` & `pyresidfp-0.6.1/src/residfp/Filter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Filter6581.cpp` & `pyresidfp-0.6.1/src/residfp/Filter6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Filter6581.h` & `pyresidfp-0.6.1/src/residfp/Filter6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Filter8580.cpp` & `pyresidfp-0.6.1/src/residfp/Filter8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Filter8580.h` & `pyresidfp-0.6.1/src/residfp/Filter8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/FilterModelConfig.cpp` & `pyresidfp-0.6.1/src/residfp/FilterModelConfig.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/FilterModelConfig.h` & `pyresidfp-0.6.1/src/residfp/FilterModelConfig.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/FilterModelConfig6581.cpp` & `pyresidfp-0.6.1/src/residfp/FilterModelConfig6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/FilterModelConfig6581.h` & `pyresidfp-0.6.1/src/residfp/FilterModelConfig6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/FilterModelConfig8580.cpp` & `pyresidfp-0.6.1/src/residfp/FilterModelConfig8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/FilterModelConfig8580.h` & `pyresidfp-0.6.1/src/residfp/FilterModelConfig8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Integrator6581.cpp` & `pyresidfp-0.6.1/src/residfp/Integrator6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Integrator6581.h` & `pyresidfp-0.6.1/src/residfp/Integrator6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Integrator8580.cpp` & `pyresidfp-0.6.1/src/residfp/Integrator8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Integrator8580.h` & `pyresidfp-0.6.1/src/residfp/Integrator8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/OpAmp.cpp` & `pyresidfp-0.6.1/src/residfp/OpAmp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/OpAmp.h` & `pyresidfp-0.6.1/src/residfp/OpAmp.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Potentiometer.h` & `pyresidfp-0.6.1/src/residfp/Potentiometer.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/README` & `pyresidfp-0.6.1/src/residfp/README`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/SID.cpp` & `pyresidfp-0.6.1/src/residfp/SID.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/SID.h` & `pyresidfp-0.6.1/src/residfp/SID.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Spline.cpp` & `pyresidfp-0.6.1/src/residfp/Spline.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Spline.h` & `pyresidfp-0.6.1/src/residfp/Spline.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/Voice.h` & `pyresidfp-0.6.1/src/residfp/Voice.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/WaveformCalculator.cpp` & `pyresidfp-0.6.1/src/residfp/WaveformCalculator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/WaveformCalculator.h` & `pyresidfp-0.6.1/src/residfp/WaveformCalculator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/WaveformGenerator.cpp` & `pyresidfp-0.6.1/src/residfp/WaveformGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/WaveformGenerator.h` & `pyresidfp-0.6.1/src/residfp/WaveformGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/array.h` & `pyresidfp-0.6.1/src/residfp/array.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/resample/Resampler.h` & `pyresidfp-0.6.1/src/residfp/resample/Resampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/resample/SincResampler.cpp` & `pyresidfp-0.6.1/src/residfp/resample/SincResampler.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/resample/SincResampler.h` & `pyresidfp-0.6.1/src/residfp/resample/SincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/resample/TwoPassSincResampler.h` & `pyresidfp-0.6.1/src/residfp/resample/TwoPassSincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/resample/ZeroOrderResampler.h` & `pyresidfp-0.6.1/src/residfp/resample/ZeroOrderResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/resample/test.cpp` & `pyresidfp-0.6.1/src/residfp/resample/test.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/siddefs-fp.h.in` & `pyresidfp-0.6.1/src/residfp/siddefs-fp.h.in`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/residfp/version.cc` & `pyresidfp-0.6.1/src/residfp/version.cc`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/sidcxx11.h` & `pyresidfp-0.6.1/src/sidcxx11.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.0/src/sidcxx14.h` & `pyresidfp-0.6.1/src/sidcxx14.h`

 * *Files identical despite different names*

