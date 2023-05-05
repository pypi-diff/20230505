# Comparing `tmp/thermal_conductivity_step-2023.4.24.tar.gz` & `tmp/thermal_conductivity_step-2023.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermal_conductivity_step-2023.4.24.tar", last modified: Mon Apr 24 18:48:10 2023, max compression
+gzip compressed data, was "thermal_conductivity_step-2023.5.5.tar", last modified: Fri May  5 15:15:35 2023, max compression
```

## Comparing `thermal_conductivity_step-2023.4.24.tar` & `thermal_conductivity_step-2023.5.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.617558 thermal_conductivity_step-2023.4.24/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-24 18:48:10.617558 thermal_conductivity_step-2023.4.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.605558 thermal_conductivity_step-2023.4.24/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.609557 thermal_conductivity_step-2023.4.24/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/_static/SEAMM Inverted 288x181.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.609557 thermal_conductivity_step-2023.4.24/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9712 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.609557 thermal_conductivity_step-2023.4.24/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.609557 thermal_conductivity_step-2023.4.24/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.609557 thermal_conductivity_step-2023.4.24/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-24 18:48:10.617558 thermal_conductivity_step-2023.4.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.609557 thermal_conductivity_step-2023.4.24/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/tests/test_thermal_conductivity_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.617558 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 18:48:10.617558 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19122 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.613557 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    24984 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/thermal_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/thermal_conductivity_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/thermal_conductivity_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step/tk_thermal_conductivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:48:10.613557 thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-24 18:48:10.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-24 18:48:10.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:48:10.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 18:48:10.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 18:48:10.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-24 18:48:10.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:47:48.000000 thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-04-24 18:47:43.000000 thermal_conductivity_step-2023.4.24/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.993939 thermal_conductivity_step-2023.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-05 15:15:34.993939 thermal_conductivity_step-2023.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.985939 thermal_conductivity_step-2023.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/SEAMM Inverted 288x181.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9712 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 15:15:34.997939 thermal_conductivity_step-2023.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/tests/test_thermal_conductivity_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.997939 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 15:15:34.997939 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18589 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.993939 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27619 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/tk_thermal_conductivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.993939 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:15:05.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/versioneer.py
```

### Comparing `thermal_conductivity_step-2023.4.24/CONTRIBUTING.rst` & `thermal_conductivity_step-2023.5.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/LICENSE` & `thermal_conductivity_step-2023.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/PKG-INFO` & `thermal_conductivity_step-2023.5.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thermal_conductivity_step
-Version: 2023.4.24
+Version: 2023.5.5
 Summary: A SEAMM plug-in for Thermal Conductivity
 Home-page: https://github.com/molssi-seamm/thermal_conductivity_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -81,13 +81,20 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.5.5 -- Improved analysis
+    * Considerable improvements to the analysis, results now seem solid
+    * Fixed issues with fitting the linear portion of the Helfand moments
+    * Added plot of the slope from the Helfand moments, which is similar to the
+      Green-Kubo integral.
+    * Cleaned up both the output and graphs.
+      
 2023.4.24 -- Initial working version
     * Initial tests seem to work but needs more thorough testing.
     * Needs documentation!
       
 2023.4.18 (2023-04-18)
     * Plug-in created using the SEAMM plug-in cookiecutter.
```

### Comparing `thermal_conductivity_step-2023.4.24/README.rst` & `thermal_conductivity_step-2023.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/Makefile` & `thermal_conductivity_step-2023.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/_static/SEAMM Inverted 288x181.png` & `thermal_conductivity_step-2023.5.5/docs/_static/SEAMM Inverted 288x181.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/_static/SEAMM logo.png` & `thermal_conductivity_step-2023.5.5/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/_static/molssi_main_logo.png` & `thermal_conductivity_step-2023.5.5/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/_static/molssi_main_logo_inverted_white.png` & `thermal_conductivity_step-2023.5.5/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/_static/molssi_square.png` & `thermal_conductivity_step-2023.5.5/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/_static/nsf.png` & `thermal_conductivity_step-2023.5.5/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/conf.py` & `thermal_conductivity_step-2023.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/developer_guide/installation.rst` & `thermal_conductivity_step-2023.5.5/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/getting_started/index.rst` & `thermal_conductivity_step-2023.5.5/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/index.rst` & `thermal_conductivity_step-2023.5.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/docs/make.bat` & `thermal_conductivity_step-2023.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/setup.py` & `thermal_conductivity_step-2023.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step/__init__.py` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/__init__.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step/analysis.py` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 
 """Routines to help do Green-Kubo and Helfand moments analysis."""
 import warnings
 
 import numpy as np
 from scipy.integrate import cumulative_trapezoid
-from scipy.optimize import curve_fit
+from scipy.optimize import curve_fit, OptimizeWarning
 import statsmodels.tsa.stattools as stattools
 
 tensor_labels = [
     ("xx", "red", "rgba(255,0,0,0.1)"),
     ("yy", "green", "rgba(0,255,0,0.1)"),
     ("zz", "blue", "rgba(0,0,255,0.1)"),
     ("xy", "rgb(127,127,0)", "rgba(127,127,0,0.1)"),
     ("xz", "rgb(255,0,255)", "rgba(255,0,255,0.1)"),
     ("yz", "rgb(0,255,255)", "rgba(0,255,255,0.1)"),
 ]
+a1 = 0
+tau1 = 0
 
 
 def moving_average(a, n):
     ret = np.cumsum(a, dtype=float)
     ret[n:] = ret[n:] - ret[:-n]
     return ret[n - 1 :] / n
 
@@ -35,22 +37,31 @@
         print(f"{freqs[i]:.4f} {ps[i]:12.0f}")
 
 
 def exp_1(t, a, tau):
     return a * (1 - np.exp(-t / tau))
 
 
+def exp_1a(t, a2, tau2):
+    global a1, tau1
+    return a1 * (1 - np.exp(-t / tau1)) + a2 * (1 - np.exp(-t / tau2))
+
+
 def exp_2(t, a1, tau1, a2, tau2):
     return a1 * (1 - np.exp(-t / tau1)) + a2 * (1 - np.exp(-t / tau2))
 
 
 def axb(x, a, b):
     return a * x + b
 
 
+def fit_h(x, a, b, tau):
+    return a * (tau * np.exp(-x / tau) + x) + b
+
+
 def acf_err(acf):
     """The standard error of the autocorrelation function.
 
     Copied from statsmodels.tsa.stattools.acf
     """
     nobs = acf.shape[0]
     varacf = np.ones_like(acf) / nobs
@@ -71,39 +82,40 @@
     varccf[0] = 0
     varccf[1] = 1.0 / nobs
     varccf[2:] *= 1 + 2 * np.cumsum(acf1[1:-1] * acf2[1:-1])
     std = np.sqrt(varccf)
     return std
 
 
-def create_correlation_functions(J):
+def create_correlation_functions(J, m=None):
     """Create the correlation functions of the heat fluxes.
 
     Parameters
     ----------
     J : numpy.ndarray(3, n)
         The heat fluxes in x, y, and z
 
     Returns
     -------
     numpy.ndarray(6, n)
         The correlation functions
     """
 
-    n = J.shape[1]
+    if m is None:
+        m = J.shape[1]
 
-    ccf = np.zeros((6, n))
-    integral = np.zeros((6, n))
+    ccf = np.zeros((6, m))
+    integral = np.zeros((6, m))
 
-    ccf[0] = stattools.ccovf(J[0], J[0])
-    ccf[1] = stattools.ccovf(J[1], J[1])
-    ccf[2] = stattools.ccovf(J[2], J[2])
-    ccf[3] = stattools.ccovf(J[0], J[1])
-    ccf[4] = stattools.ccovf(J[0], J[2])
-    ccf[5] = stattools.ccovf(J[1], J[2])
+    ccf[0] = stattools.ccovf(J[0], J[0])[:m]
+    ccf[1] = stattools.ccovf(J[1], J[1])[:m]
+    ccf[2] = stattools.ccovf(J[2], J[2])[:m]
+    ccf[3] = stattools.ccovf(J[0], J[1])[:m]
+    ccf[4] = stattools.ccovf(J[0], J[2])[:m]
+    ccf[5] = stattools.ccovf(J[1], J[2])[:m]
 
     integral[0] = cumulative_trapezoid(ccf[0], initial=0.0)
     integral[1] = cumulative_trapezoid(ccf[1], initial=0.0)
     integral[2] = cumulative_trapezoid(ccf[2], initial=0.0)
     integral[3] = cumulative_trapezoid(ccf[3], initial=0.0)
     integral[4] = cumulative_trapezoid(ccf[4], initial=0.0)
     integral[5] = cumulative_trapezoid(ccf[5], initial=0.0)
@@ -173,109 +185,109 @@
         The standard error of the coefficients.
     tau_err : [float]
         The standard error of the time constants
     n : int
         The point in the x (time) vector that is 3*tau
     """
     # frequencies(y)
-    dt = xs[1] - xs[0]
-    width = int(0.4 / dt)
+    dx = xs[1] - xs[0]
+    width = int(0.4 / dx)
     ma = moving_average(y, width)
 
-    # for v in ma[:100]:
-    #     print(f"     {v:12.1f}")
-
     # Find the initial, steep rise. Ignore first couple points.
     for i in range(2, len(ma) // 2):
         if ma[i] > 0.9 * ma[i + width]:
             break
     npts = i + width
-    # print(f"{i=} + {width} = {npts}")
     tau_guess = xs[npts]
     a_guess = ma[i]
-    # print(f"{a_guess=} {tau_guess=}")
     npts *= 20
     if 2 * npts > y.size:
         npts = y.size // 2
 
     sigma0 = sigma + np.average(sigma[0 : y.size // 10])
 
+    # First fit with single exponential
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", RuntimeWarning)
+        warnings.simplefilter("ignore", OptimizeWarning)
+        popt1, pcov1, infodict1, msg1, ierr1 = curve_fit(
+            exp_1,
+            xs[1:npts],
+            y[1:npts],
+            full_output=True,
+            sigma=sigma0[1:npts],
+            absolute_sigma=True,
+            p0=[a_guess, tau_guess],
+        )
+
+    err = np.sqrt(np.diag(pcov1)).tolist()
+    a1 = popt1[0]
+    tau1 = popt1[1]
+
+    # find a range for the next fit to keep it a "good" part of the data
+    i_min = int(tau1 / dx / 2)  # tau / 2
+    i_max = int(tau1 / dx * 20)  # 20 * tau1
+
+    # And add a second exponential
     try:
-        if False:
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", RuntimeWarning)
+            warnings.simplefilter("ignore", OptimizeWarning)
             popt, pcov, infodict, msg, ierr = curve_fit(
                 exp_2,
-                xs[1:npts],
-                y[1:npts],
+                xs[i_min:i_max],
+                y[i_min:i_max],
                 full_output=True,
-                sigma=sigma[1:npts],
+                sigma=sigma[i_min:i_max],
                 absolute_sigma=True,
-                p0=[a_guess, tau_guess, 0.1 * a_guess, 5 * tau_guess],
+                p0=[a1, tau1, 0.1 * a1, 5 * tau1],
             )
-            err = np.sqrt(np.diag(pcov)).tolist()
-            a = [popt[0], popt[2]]
-            a_err = [err[0], err[2]]
-            tau = [popt[1], popt[3]]
-            tau_err = [err[1], err[3]]
-            kappa = a[0] + a[1]
-            kappa_err = a_err[0] + a_err[1]
-        else:
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore", RuntimeWarning)
-                popt, pcov, infodict, msg, ierr = curve_fit(
-                    exp_1,
-                    xs[1:npts],
-                    y[1:npts],
-                    full_output=True,
-                    sigma=sigma0[1:npts],
-                    absolute_sigma=True,
-                    p0=[a_guess, tau_guess],
-                )
-            err = np.sqrt(np.diag(pcov)).tolist()
-            a = [popt[0]]
+        err = np.sqrt(np.diag(pcov)).tolist()
+        a = [popt[0], popt[2]]
+        a_err = [err[0], err[2]]
+        tau = [popt[1], popt[3]]
+        tau_err = [err[1], err[3]]
+        kappa = a[0] + a[1]
+        kappa_err = a_err[0] + a_err[1]
+        if kappa > 2 * a1:  # Shouldn't change this much!
+            err = np.sqrt(np.diag(pcov1)).tolist()
+            a = [popt1[0]]
             a_err = [err[0]]
-            tau = [popt[1]]
+            tau = [popt1[1]]
             tau_err = [err[1]]
             kappa = a[0]
             kappa_err = a_err[0]
-    except Exception as e:
-        print(f"Exp-2 fit failed, {e}")
-        popt, pcov, infodict, msg, ierr = curve_fit(
-            exp_1,
-            xs[1:npts],
-            y[1:npts],
-            full_output=True,
-            sigma=sigma[1:npts],
-            absolute_sigma=True,
-            p0=[a_guess, tau_guess],
-        )
-        err = np.sqrt(np.diag(pcov)).tolist()
-        a = [popt[0]]
+    except Exception:
+        err = np.sqrt(np.diag(pcov1)).tolist()
+        a = [popt1[0]]
         a_err = [err[0]]
-        tau = [popt[1]]
+        tau = [popt1[1]]
         tau_err = [err[1]]
         kappa = a[0]
         kappa_err = a_err[0]
 
     # Find point for 3 * tau
-    for nf, val in enumerate(xs):
-        if val > 3 * tau[-1]:
-            break
+    tmp = max(tau)
+    nf = int(tmp / dx) * 20
+    if nf > len(xs):
+        nf = len(xs)
 
     fy = []
-    if len(popt) == 2:
+    if len(a) == 1:
         for t in xs[1:nf]:
-            fy.append(exp_1(t, *popt))
+            fy.append(exp_1(t, a[0], tau[0]))
     else:
         for t in xs[1:nf]:
-            fy.append(exp_2(t, *popt))
+            fy.append(exp_2(t, a[0], tau[0], a[1], tau[1]))
 
     return kappa, kappa_err, a, a_err, tau, tau_err, xs[1:nf], fy
 
 
-def fit_helfand_moment(y, xs, sigma=None):
+def fit_helfand_moment(y, xs, sigma=None, start=1):
     """Find the best linear fit to longest possible segment.
 
     Parameters
     ----------
     y : [float] or numpy.ndarray()
         The Helfand moment
 
@@ -292,172 +304,76 @@
     stderr : float
         The 95% standard error of the slope
     xs : [float]
         The x values (time) for the fit curve
     ys : [float]
         The y values for the fit curve.
     """
-    n = len(y)
+    dx = xs[1] - xs[0]
 
-    if sigma is not None:
-        ave = sigma[n // 20]
-        sigma_new = sigma + ave
-
-        # We know the curves curve near the origin, so ignore the first ps
-        for i, val in enumerate(xs):
-            if val > 1.0:
-                break
-
-        popt, pcov, infodict, msg, ierr = curve_fit(
-            axb,
-            xs[i:],
-            y[i:],
-            full_output=True,
-            sigma=sigma[i:],
-            absolute_sigma=True,
-        )
-        slope = float(popt[0])
-        b = float(popt[1])
-        err = float(np.sqrt(np.diag(pcov)[0]))
-
-        ys = []
-        for x in xs[i:]:
-            ys.append(axb(x, slope, b))
-
-        return slope, err, xs[i:], ys
-
-    # Try brute force to find the longest best fit.
-    nblocks = 20
-    blocksize = n // nblocks
-
-    i0 = None
-    j0 = None
-    slope0 = None
-    b0 = None
-    err0 = None
-    for j in range(nblocks, 1, -1):
-        # Ensure fairly long chunks
-        for i in range(j - 3, -1, -1):
-            first = i * blocksize
-            last = j * blocksize
-            if sigma is None:
-                popt, pcov, infodict, msg, ierr = curve_fit(
-                    axb,
-                    xs[first:last],
-                    y[first:last],
-                    full_output=True,
-                )
-            else:
-                popt, pcov, infodict, msg, ierr = curve_fit(
-                    axb,
-                    xs[first:last],
-                    y[first:last],
-                    full_output=True,
-                    sigma=sigma_new[first:last],
-                    absolute_sigma=True,
-                )
-            slope = float(popt[0])
-            b = float(popt[1])
-            err = float(np.sqrt(np.diag(pcov)[0]))
-            if i0 is None:
-                i0 = first
-                j0 = last
-                slope0 = slope
-                b0 = b
-                err0 = err
-            elif sigma is not None and err < err0:
-                i0 = first
-                j0 = last
-                slope0 = slope
-                b0 = b
-                err0 = err
-            elif err / np.sqrt(last - first) < err0 / np.sqrt(j0 - i0):
-                i0 = first
-                j0 = last
-                slope0 = slope
-                b0 = b
-                err0 = err
-    # print(f"1 -- {i0}:{j0} {slope0:.4f} {err0:.4f}")
-
-    # Try expanding the front of the range
-    last = j0
-    for first in range(i0 - 1, 0, -1):
-        if sigma is None:
-            popt, pcov, infodict, msg, ierr = curve_fit(
-                axb,
-                xs[first:last],
-                y[first:last],
-                full_output=True,
-            )
-        else:
-            popt, pcov, infodict, msg, ierr = curve_fit(
-                axb,
-                xs[first:last],
-                y[first:last],
-                full_output=True,
-                sigma=sigma_new[first:last],
-                absolute_sigma=True,
-            )
-        slope = float(popt[0])
-        b = float(popt[1])
-        err = float(np.sqrt(np.diag(pcov)[0]))
-        if sigma is not None and err < err0:
-            i0 = first
-            slope0 = slope
-            b0 = b
-            err0 = err
-        elif err / np.sqrt(last - first) < err0 / np.sqrt(last - i0):
-            i0 = first
-            slope0 = slope
-            b0 = b
-            err0 = err
-        else:
-            break
-    # print(f"2 -- {i0}:{j0} {slope0:.4f} {err0:.4f}")
+    # We know the curves curve near the origin, so ignore the first part
+    i = int(start / dx)
+    if i > len(y):
+        i = int(1 / dx)
+
+    popt, pcov, infodict, msg, ierr = curve_fit(
+        axb,
+        xs[i:],
+        y[i:],
+        full_output=True,
+        sigma=sigma[i:],
+        absolute_sigma=True,
+    )
+    slope = float(popt[0])
+    b = float(popt[1])
+    err = float(np.sqrt(np.diag(pcov)[0]))
 
-    # And end of the range
-    first = i0
-    for last in range(j0 + 1, n):
-        if sigma is None:
-            popt, pcov, infodict, msg, ierr = curve_fit(
-                axb,
-                xs[first:last],
-                y[first:last],
-                full_output=True,
-            )
-        else:
-            popt, pcov, infodict, msg, ierr = curve_fit(
-                axb,
-                xs[first:last],
-                y[first:last],
-                full_output=True,
-                sigma=sigma_new[first:last],
-                absolute_sigma=True,
-            )
-        slope = float(popt[0])
-        b = float(popt[1])
-        err = float(np.sqrt(np.diag(pcov)[0]))
-        if sigma is not None and err < err0:
-            j0 = last
-            slope0 = slope
-            b0 = b
-            err0 = err
-        elif err / np.sqrt(last - i0) < err0 / np.sqrt(j0 - i0):
-            j0 = last
-            slope0 = slope
-            b0 = b
-            err0 = err
-        else:
-            break
-    # print(f"3 -- {i0}:{j0} {slope0:.4f} ± {err0:.4f}, {b0:.4f}")
-    # print(f"{xs[0]=:.4f} --> {axb(xs[0], slope0, b0):.4f}")
     ys = []
-    for x in xs[i0:j0]:
-        ys.append(axb(x, slope0, b0))
-    return slope0, err0, xs[i0:j0], ys
+    for x in xs[i:]:
+        ys.append(axb(x, slope, b))
+
+    return slope, err, xs[i:], ys
+
+
+def get_helfand_slope(y, xs, sigma=None):
+    """Get the instantaneous slope of the Helfand moments
+
+    Parameters
+    ----------
+    y : [float] or numpy.ndarray()
+        The Helfand moment
+
+    xs : [float]
+        The time (x) coordinate
+
+    sigma : [float] or numpy.ndarray()
+        Optional standard error of y
+
+    Returns
+    -------
+    slope : float
+        The fit slope.
+    stderr : float
+        The 95% standard error of the slope
+    xs : [float]
+        The x values (time) for the fit curve
+    ys : [float]
+        The y values for the fit curve.
+    """
+    n = len(y)
+
+    dx = xs[1] - xs[0]
+    slope = np.zeros_like(y)
+    slope[2:] = (y[2:] - y[0 : n - 2]) / (2 * dx)
+    new_x = xs
+    new_sigma = np.zeros_like(y)
+    new_sigma[2:] = sigma[2:] + sigma[0 : n - 2]
+    new_sigma[0] = new_sigma[3]
+    new_sigma[1] = new_sigma[3]
+    return slope, new_x, new_sigma
 
 
 def plot_correlation_functions(
     figure, CCF, ts, err=None, fit=None, labels=tensor_labels
 ):
     """Create a plot for the heat flux cross-correlation functions.
 
@@ -583,14 +499,15 @@
                 y=fit[i]["ys"],
                 ylabel=f"fit{label}",
                 yunits="W/m/K",
                 color=color,
                 dash="dash",
                 width=3,
             )
+
         if err is not None:
             errs = np.concatenate((x[i] + err[i], x[i, ::-1] - err[i, ::-1]))
             plot.add_trace(
                 x_axis=x_axis,
                 y_axis=y_axis,
                 name=f"±{label}",
                 x=ts + ts[::-1],
@@ -682,7 +599,91 @@
             xunits="ps",
             y=M[i, :].tolist(),
             ylabel=f"M{label}",
             yunits="W/m/K*ps",
             color=color,
         )
     return plot
+
+
+def plot_helfand_slopes(
+    figure, x, ts, err=None, fit=None, labels=tensor_labels, _range=None
+):
+    """Create a plot of the slope of the Helfand moments
+
+    Parameters
+    ----------
+    figure : seamm_util.Figure
+        The figure that contains the plots.
+
+    x : numpy.mdarray(6, m)
+        The slope in W/m/K
+
+    ts : [float]
+        The times associated with the points, in ps
+
+    err : numpy.ndarray(6, m)
+        The standard errors of the points (optional)
+
+    fit :
+        The fit parameters for any fit of the slope (optional)
+
+    _range : [float]
+        The range of the x-axis in terms of units in x.
+    """
+    plot = figure.add_plot("Slope")
+
+    x_axis = plot.add_axis("x", label="t (ps)")
+    y_axis = plot.add_axis("y", label="Kappa (W/m/K)", anchor=x_axis)
+    x_axis.anchor = y_axis
+
+    if _range is not None:
+        x_axis["range"] = _range
+
+    for i, tmp in enumerate(labels):
+        label, color, colora = tmp
+        if fit is not None and i < len(fit):
+            hover = f"{label} = {fit[i]['kappa']:.3f} ± {fit[i]['stderr']:.3f} W/m/K"
+            plot.add_trace(
+                x_axis=x_axis,
+                y_axis=y_axis,
+                name=f"fit{label}",
+                hovertemplate=hover,
+                x=fit[i]["xs"],
+                xlabel="t",
+                xunits="ps",
+                y=fit[i]["ys"],
+                ylabel=f"fit{label}",
+                yunits="W/m/K",
+                color=color,
+                dash="dash",
+                width=3,
+            )
+        if err is not None:
+            errs = np.concatenate((x[i] + err[i], x[i][::-1] - err[i][::-1]))
+            plot.add_trace(
+                x_axis=x_axis,
+                y_axis=y_axis,
+                name=f"±{label}",
+                x=ts + ts[::-1],
+                xlabel="t",
+                xunits="ps",
+                y=errs.tolist(),
+                ylabel=f"±{label}",
+                yunits="W/m/K",
+                color=colora,
+                fill="toself",
+                visible="legendonly",
+            )
+        plot.add_trace(
+            x_axis=x_axis,
+            y_axis=y_axis,
+            name=f"K{label}",
+            x=ts,
+            xlabel="t",
+            xunits="ps",
+            y=x[i].tolist(),
+            ylabel=f"K{label}",
+            yunits="W/m/K",
+            color=color,
+        )
+    return plot
```

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step/data/references.bib` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step/metadata.py` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/metadata.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step/thermal_conductivity.py` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 from tabulate import tabulate
 
 from .analysis import (
     create_correlation_functions,
     create_helfand_moments,
     fit_green_kubo_integral,
     fit_helfand_moment,
+    get_helfand_slope,
     plot_correlation_functions,
     plot_GK_integrals,
     plot_helfand_moments,
+    plot_helfand_slopes,
 )
 from .thermal_conductivity_parameters import ThermalConductivityParameters
 import thermal_conductivity_step
 import molsystem
 import seamm
 import seamm_util
 from seamm_util import ureg, Q_  # noqa: F401
@@ -193,15 +195,15 @@
         # Now need to walk through the steps in the subflowchart...
         node = self.subflowchart.get_node("1").next()
         while node is not None:
             node = node.create_parser()
 
         return self.next()
 
-    def description_text(self, P=None):
+    def description_text(self, P=None, short=False):
         """Create the text description of what this step will do.
         The dictionary of control values is passed in as P so that
         the code can test values, etc.
 
         Parameters
         ----------
         P: dict
@@ -211,46 +213,51 @@
         -------
         str
             A description of the current step.
         """
         if P is None:
             P = self.parameters.values_to_dict()
 
-        # The subflowchart
-        self.subflowchart.root_directory = self.flowchart.root_directory
-
-        # Get the first real node
-        node = self.subflowchart.get_node("1").next()
-
         text = (
             f"Calculate the thermal conductivity at {P['T']} using "
             f"the {P['approach']} approach. {P['nruns']} runs will be averaged for "
             "the final results.\n\n"
         )
-        while node is not None:
-            try:
-                text += __(node.description_text()).__str__()
-            except Exception as e:
-                print(f"Error describing thermal_conductivity flowchart: {e} in {node}")
-                logger.critical(
-                    f"Error describing thermal_conductivity flowchart: {e} in {node}"
-                )
-                raise
-            except:  # noqa: E722
-                print(
-                    "Unexpected error describing thermal_conductivity flowchart: "
-                    f"{sys.exc_info()[0]} in {str(node)}"
-                )
-                logger.critical(
-                    "Unexpected error describing thermal_conductivity flowchart: "
-                    f"{sys.exc_info()[0]} in {str(node)}"
-                )
-                raise
-            text += "\n"
-            node = node.next()
+        if not short:
+            # The subflowchart
+            self.subflowchart.root_directory = self.flowchart.root_directory
+
+            # Get the first real node
+            node = self.subflowchart.get_node("1").next()
+
+            while node is not None:
+                try:
+                    text += __(node.description_text()).__str__()
+                except Exception as e:
+                    print(
+                        f"Error describing thermal_conductivity flowchart: {e} in "
+                        f"{node}"
+                    )
+                    logger.critical(
+                        f"Error describing thermal_conductivity flowchart: {e} in "
+                        f"{node}"
+                    )
+                    raise
+                except:  # noqa: E722
+                    print(
+                        "Unexpected error describing thermal_conductivity flowchart: "
+                        f"{sys.exc_info()[0]} in {str(node)}"
+                    )
+                    logger.critical(
+                        "Unexpected error describing thermal_conductivity flowchart: "
+                        f"{sys.exc_info()[0]} in {str(node)}"
+                    )
+                    raise
+                text += "\n"
+                node = node.next()
 
         return self.header + "\n" + __(text, **P, indent=4 * " ").__str__()
 
     def run(self):
         """Run a Thermal Conductivity step.
 
         Parameters
@@ -266,15 +273,15 @@
 
         # Get the values of the parameters, dereferencing any variables
         P = self.parameters.current_values_to_dict(
             context=seamm.flowchart_variables._data
         )
 
         # Print what we are doing
-        printer.important(__(self.description_text(P), indent=self.indent))
+        printer.important(__(self.description_text(P, short=True), indent=self.indent))
 
         # Find the handler for job.out and set the level up
         job_handler = None
         out_handler = None
         for handler in job.handlers:
             if (
                 isinstance(handler, logging.FileHandler)
@@ -372,15 +379,15 @@
 
         # Add other citations here or in the appropriate place in the code.
         # Add the bibtex to data/references.bib, and add a self.reference.cite
         # similar to the above to actually add the citation to the references.
 
         return next_node
 
-    def analyze(self, indent="", P=None, style="full", **kwargs):
+    def analyze(self, indent="", P=None, style="full", run=None, **kwargs):
         """Do any analysis of the output from this step.
 
         Also print important results to the local step.out file using
         "printer".
 
         Parameters
         ----------
@@ -413,18 +420,82 @@
                 "Units": [],
             }
 
         dt = Q_(self.timestep[0], "fs")
         ts = np.arange(self.M.shape[1]) * dt.m_as("ps")  # Scale to ps
         ts = ts.tolist()
 
+        # Get and plot the slopes of the Helfand moments
+        slopes = []
+        xs = []
+        errs = []
+        fit0 = []
+        for i in range(6):
+            slope, x, err = get_helfand_slope(self.M[i], ts, sigma=self.M_err[i])
+            slopes.append(slope)
+            xs.append(x)
+            errs.append(err)
+
+            if i < 3:
+                (
+                    kappa,
+                    kappa_err,
+                    a,
+                    a_err,
+                    tau,
+                    tau_err,
+                    tf,
+                    yf,
+                ) = fit_green_kubo_integral(slope, x, sigma=err)
+                # print(f"{kappa=} {tau=}")
+                fit0.append(
+                    {
+                        "kappa": kappa,
+                        "stderr": kappa_err,
+                        "xs": tf,
+                        "ys": yf,
+                        "a": a,
+                        "a_err": a_err,
+                        "tau": tau,
+                        "tau_err": tau_err,
+                    }
+                )
+
+        figure = self.create_figure(
+            module_path=("seamm",),
+            template="line.graph_template",
+            title="Helfand Slopes",
+        )
+
+        plot_helfand_slopes(
+            figure, slopes, xs[0], err=errs, fit=fit0, labels=self.tensor_labels
+        )
+
+        figure.grid_plots("Slope")
+
+        # Write to disk
+        filename = "Helfand_slopes.graph"
+        path = Path(self.directory) / filename
+        figure.dump(path)
+
+        if "html" in self.options and self.options["html"]:
+            path = path.with_suffix(".html")
+            figure.template = "line.html_template"
+            figure.dump(path)
+
         # Fit the slopes
         fit = []
         for i in range(6):
-            slope, err, xs, ys = fit_helfand_moment(self.M[i], ts, sigma=self.M_err[i])
+            if i < len(fit0):
+                start = max(fit0[i]["tau"]) * 3
+            else:
+                start = 1
+            slope, err, xs, ys = fit_helfand_moment(
+                self.M[i], ts, sigma=self.M_err[i], start=start
+            )
             fit.append(
                 {
                     "kappa": slope,
                     "stderr": err,
                     "xs": xs,
                     "ys": ys,
                 }
@@ -475,18 +546,14 @@
                     "tau": tau,
                     "tau_err": tau_err,
                 }
             )
             try:
                 v, e = fmt_err(kappa, 2 * kappa_err)
             except Exception:
-                print(f"{a=}")
-                print(f"{a_err=}")
-                print(f"{tau=}")
-                print(f"{tau_err=}")
                 v = f"{kappa:.2f}"
                 e = "--"
 
             if style == "1-line":
                 if i == 0:
                     table["Run"].append("")
                 alpha = self.tensor_labels[i][0]
@@ -520,19 +587,28 @@
                 disable_numparse=True,
             )
             if len(self.V) == 2:
                 length = len(tmp.splitlines()[0])
                 text += "\n"
                 text += "Thermal Conductivity".center(length)
                 text += "\n"
+                text += "--------------------".center(length)
+                text += "\n"
+                text += "First line is Helfand moments; second, Green-Kubo".center(
+                    length
+                )
+                text += "\n"
                 text += "\n".join(tmp.splitlines()[0:-1])
             else:
                 text = tmp.splitlines()[-3]
                 text += "\n"
                 text += tmp.splitlines()[-2]
+                if run is not None and run == P["nruns"]:
+                    text += "\n"
+                    text += tmp.splitlines()[-1]
 
             printer.normal(__(text, indent=8 * " ", wrap=False, dedent=False))
         else:
             text = ""
             tmp = tabulate(
                 table,
                 headers="keys",
@@ -584,15 +660,18 @@
 
         max_tau = 0
         for i in range(3):
             tau = fit[i]["tau"][-1]
             if tau > max_tau:
                 max_tau = tau
 
-        rng = [0, max_tau * 4]
+        if max_tau * 4 > ts[-1]:
+            rng = None
+        else:
+            rng = [0, max_tau * 4]
         plot_GK_integrals(
             figure, x, ts, err=err, fit=fit, labels=self.tensor_labels, _range=rng
         )
 
         figure.grid_plots("GKI")
 
         # Write to disk
@@ -711,22 +790,26 @@
         # We need properties like the temperature and volume.
         T = Q_(T, "K")
         V = Q_(V, "Å^3")
         dt = Q_(timestep, "fs")
         k_B = Q_("k_B")
         Jsq = Q_("W^2/m^4")
 
+        # Limit the lengths of the data
+        n = J.shape[1]
+        m = min(n // 20, 10000)
+
         # Create the Helfand moments
         constants = Jsq * V * dt**2 / (2 * k_B * T**2)
-        M = create_helfand_moments(J) * constants.m_as("W/m/K*ps")
+        M = create_helfand_moments(J, m=m) * constants.m_as("W/m/K*ps")
         self.Ms.append(M)
 
         # And correlation functions for Green-Kubo method
         constants = V / (k_B * T**2) * Jsq * dt
-        Jcf, integral = create_correlation_functions(J)
+        Jcf, integral = create_correlation_functions(J, m=m)
         self.Jcfs.append(Jcf)
         self.GK_integrals.append(integral * constants.m_as("W/m/K"))
         # Merge the results and get the averages and errors
         tmp = np.stack(self.Ms)
         self.M = np.average(tmp, axis=0)
         self.M_err = np.std(tmp, axis=0)
         tmp = np.stack(self.Jcfs)
```

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step/thermal_conductivity_parameters.py` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity_parameters.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step/thermal_conductivity_step.py` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity_step.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step/tk_thermal_conductivity.py` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/tk_thermal_conductivity.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/PKG-INFO` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thermal-conductivity-step
-Version: 2023.4.24
+Version: 2023.5.5
 Summary: A SEAMM plug-in for Thermal Conductivity
 Home-page: https://github.com/molssi-seamm/thermal_conductivity_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -81,13 +81,20 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.5.5 -- Improved analysis
+    * Considerable improvements to the analysis, results now seem solid
+    * Fixed issues with fitting the linear portion of the Helfand moments
+    * Added plot of the slope from the Helfand moments, which is similar to the
+      Green-Kubo integral.
+    * Cleaned up both the output and graphs.
+      
 2023.4.24 -- Initial working version
     * Initial tests seem to work but needs more thorough testing.
     * Needs documentation!
       
 2023.4.18 (2023-04-18)
     * Plug-in created using the SEAMM plug-in cookiecutter.
```

### Comparing `thermal_conductivity_step-2023.4.24/thermal_conductivity_step.egg-info/SOURCES.txt` & `thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.4.24/versioneer.py` & `thermal_conductivity_step-2023.5.5/versioneer.py`

 * *Files identical despite different names*

