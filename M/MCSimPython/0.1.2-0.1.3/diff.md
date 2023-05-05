# Comparing `tmp/MCSimPython-0.1.2.tar.gz` & `tmp/MCSimPython-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCSimPython-0.1.2.tar", last modified: Mon May  1 10:53:07 2023, max compression
+gzip compressed data, was "MCSimPython-0.1.3.tar", last modified: Fri May  5 08:38:33 2023, max compression
```

## Comparing `MCSimPython-0.1.2.tar` & `MCSimPython-0.1.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-01 10:52:50.000000 MCSimPython-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-01 10:52:50.000000 MCSimPython-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-01 10:52:50.000000 MCSimPython-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/MCSimPython/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 10:53:00.000000 MCSimPython-0.1.2/src/MCSimPython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/MCSimPython/control/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/control/adaptiveFS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/control/backstepping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/control/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/MCSimPython/guidance/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/guidance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/guidance/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/guidance/path_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/observer/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/observer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/observer/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/observer/ltv_kf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/observer/nonlinobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/csad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/gunnerus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/thruster_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/vessel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/thruster.py
--rw-r--r--   0 runner    (1001) docker     (123)    27663 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/vessel_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/freqs.npy
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/headings.npy
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/thruster_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
--rw-r--r--   0 runner    (1001) docker     (123)  1961336 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/vessel_json.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.986147 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2939897 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  5568933 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/rvg_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  4723068 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/vessel.json
--rw-r--r--   0 runner    (1001) docker     (123)  4733857 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/src/MCSimPython/waves/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/waves/wave_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/waves/wave_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/waves/wave_spreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/MCSimPython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/tests/test_wave_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-05 08:37:48.000000 MCSimPython-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-05 08:37:48.000000 MCSimPython-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-05 08:37:48.000000 MCSimPython-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.092327 MCSimPython-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.092327 MCSimPython-0.1.3/src/MCSimPython/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 08:38:24.000000 MCSimPython-0.1.3/src/MCSimPython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/control/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/control/adaptiveFS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/control/backstepping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/control/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/guidance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/guidance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/guidance/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/guidance/path_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/observer/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/observer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/observer/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/observer/ltv_kf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/observer/nonlinobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/csad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/gunnerus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/thruster_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/vessel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/thruster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27663 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/vessel_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.100327 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/freqs.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/headings.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/thruster_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1961336 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/vessel_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.120327 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2939897 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  5568933 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/rvg_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4723068 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/vessel.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4733857 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/src/MCSimPython/waves/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/waves/wave_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/waves/wave_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/waves/wave_spreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.092327 MCSimPython-0.1.3/src/MCSimPython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/tests/test_wave_spectra.py
```

### Comparing `MCSimPython-0.1.2/LICENSE` & `MCSimPython-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/PKG-INFO` & `MCSimPython-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCSimPython
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python vessel simulation environment
 Author-email: Jan-Erik Hygen <janereh@stud.ntnu.no>
 Keywords: mcsim,MCSimPython,DP,dynamic positioning,Marine Cybernetics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `MCSimPython-0.1.2/README.md` & `MCSimPython-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/pyproject.toml` & `MCSimPython-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/control/adaptiveFS.py` & `MCSimPython-0.1.3/src/MCSimPython/control/adaptiveFS.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/control/backstepping.py` & `MCSimPython-0.1.3/src/MCSimPython/control/backstepping.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/control/basic.py` & `MCSimPython-0.1.3/src/MCSimPython/control/basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Tested:
 # 
 # Copyright (C) 2023: NTNU, Trondheim
 # Licensed under GPL-3.0-or-later
 # ---------------------------------------------------------------------------
 
 import numpy as np
-from MCSimPython.utils import Rz
+from MCSimPython.utils import Rz, pipi
 
 
 class PD:
     """Proportional-Derivative controller."""
     def __init__(self, kp: list, kd: list):
         self.Kp = np.diag(kp)
         self.Kd = np.diag(kd)
@@ -39,14 +39,15 @@
         Returns
         -------
         tau : array_like
             Controller load in surge, sway, and yaw (body-frame).
         """
         psi = eta[-1]
         z1 = Rz(psi).T@(eta-eta_d)
+        z1[2] = pipi(eta[2] - eta_d[2])
         z2 = nu - nu_d
         return -self.Kp@z1 - self.Kd@z2
     
     def set_kd(self, kd: list):
         """Set the derivative gain coefficients."""
         self.Kd = np.diag(kd)
     
@@ -81,17 +82,19 @@
         Returns
         -------
         tau : array_like
             Controller load in surge, sway, and yaw (body-frame).
         """
         psi = eta[-1]
         z1 = Rz(psi).T@(eta - eta_d)
+        z1[2] = pipi(eta[2] - eta_d[2])
         z2 = nu - nu_d
 
-        self.zi += self.dt*(eta - eta_d)
+        self.zi[:2] += self.dt*(eta[:2] - eta_d[:2])
+        self.zi[2] += self.dt*pipi(eta[2] - eta_d[2])
         return -self.Kp@z1 - self.Kd@z2 - Rz(psi).T@self.Ki@self.zi
 
 
 
 class DirectBiasCompensationController():
     '''
     Bias estimate provided from the observer as direct compensation in a nominal PD control law.
@@ -114,14 +117,15 @@
         nu_d : array_like
             Desired vessel velocity in surge, sway and yaw (body-frame).
         b : array_like
             Estimated bias in surge, sway and yaw (body-frame)
         '''
         psi = eta[-1]
         z1 = Rz(psi).T@(eta-eta_d)              # P
+        z1[2] = pipi(eta[2] - eta_d[2])
         z2 = nu - nu_d                          # D
         zb = Rz(psi).T@b                        # bias
         return -self.Kp@z1 - self.Kd@z2 - zb
     
     def set_kd(self, kd: list):
         self.Kd = np.diag(kd)
```

### Comparing `MCSimPython-0.1.2/src/MCSimPython/guidance/__init__.py` & `MCSimPython-0.1.3/src/MCSimPython/guidance/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/guidance/filter.py` & `MCSimPython-0.1.3/src/MCSimPython/guidance/filter.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/guidance/path_param.py` & `MCSimPython-0.1.3/src/MCSimPython/guidance/path_param.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/observer/__init__.py` & `MCSimPython-0.1.3/src/MCSimPython/observer/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/observer/ekf.py` & `MCSimPython-0.1.3/src/MCSimPython/observer/ekf.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/observer/ltv_kf.py` & `MCSimPython-0.1.3/src/MCSimPython/observer/ltv_kf.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/observer/nonlinobs.py` & `MCSimPython-0.1.3/src/MCSimPython/observer/nonlinobs.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/simulator/__init__.py` & `MCSimPython-0.1.3/src/MCSimPython/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/simulator/csad.py` & `MCSimPython-0.1.3/src/MCSimPython/simulator/csad.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/simulator/gunnerus.py` & `MCSimPython-0.1.3/src/MCSimPython/simulator/gunnerus.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/simulator/thruster_dynamics.py` & `MCSimPython-0.1.3/src/MCSimPython/simulator/thruster_dynamics.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/simulator/vessel.py` & `MCSimPython-0.1.3/src/MCSimPython/simulator/vessel.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/allocation.py` & `MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/allocation.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/constraints.py` & `MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/constraints.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/thruster.py` & `MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/thruster.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/utils.py` & `MCSimPython-0.1.3/src/MCSimPython/utils.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json` & `MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/vessel_json.json` & `MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/vessel_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json` & `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl` & `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl` & `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/rvg_config.json` & `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/rvg_config.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/vessel.json` & `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/vessel.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/vessel_2.json` & `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/vessel_2.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/waves/wave_loads.py` & `MCSimPython-0.1.3/src/MCSimPython/waves/wave_loads.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/waves/wave_spectra.py` & `MCSimPython-0.1.3/src/MCSimPython/waves/wave_spectra.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython/waves/wave_spreading.py` & `MCSimPython-0.1.3/src/MCSimPython/waves/wave_spreading.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/src/MCSimPython.egg-info/PKG-INFO` & `MCSimPython-0.1.3/src/MCSimPython.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCSimPython
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python vessel simulation environment
 Author-email: Jan-Erik Hygen <janereh@stud.ntnu.no>
 Keywords: mcsim,MCSimPython,DP,dynamic positioning,Marine Cybernetics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `MCSimPython-0.1.2/src/MCSimPython.egg-info/SOURCES.txt` & `MCSimPython-0.1.3/src/MCSimPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/tests/test_utils.py` & `MCSimPython-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.2/tests/test_wave_spectra.py` & `MCSimPython-0.1.3/tests/test_wave_spectra.py`

 * *Files identical despite different names*

