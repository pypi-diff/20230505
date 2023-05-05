# Comparing `tmp/zospy-0.6.2.tar.gz` & `tmp/zospy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zospy-0.6.2.tar", last modified: Wed Mar 22 10:04:33 2023, max compression
+gzip compressed data, was "zospy-1.0.0.tar", last modified: Fri May  5 14:30:15 2023, max compression
```

## Comparing `zospy-0.6.2.tar` & `zospy-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:04:33.192307 zospy-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-22 10:04:17.000000 zospy-0.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 10:04:17.000000 zospy-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-03-22 10:04:33.192307 zospy-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-03-22 10:04:17.000000 zospy-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-22 10:04:18.000000 zospy-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-22 10:04:33.192307 zospy-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-22 10:04:18.000000 zospy-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:04:33.188307 zospy-0.6.2/zospy/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:04:33.192307 zospy-0.6.2/zospy/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/analyses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/analyses/mtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/analyses/psf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13860 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/analyses/raysandspots.py
--rw-r--r--   0 runner    (1001) docker     (123)    35777 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/analyses/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/analyses/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/analyses/wavefront.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:04:33.192307 zospy-0.6.2/zospy/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/api/apisupport.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/api/zptypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:04:33.192307 zospy-0.6.2/zospy/functions/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/functions/lde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/functions/nce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:04:33.192307 zospy-0.6.2/zospy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/utils/clrutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/utils/pyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/utils/zputils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-03-22 10:04:18.000000 zospy-0.6.2/zospy/zpcore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:04:33.188307 zospy-0.6.2/zospy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-03-22 10:04:33.000000 zospy-0.6.2/zospy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-22 10:04:33.000000 zospy-0.6.2/zospy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 10:04:33.000000 zospy-0.6.2/zospy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-22 10:04:33.000000 zospy-0.6.2/zospy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 10:04:33.000000 zospy-0.6.2/zospy.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2023-05-05 14:30:02.620558 zospy-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     6956 2023-05-05 14:30:02.620558 zospy-1.0.0/README.md
+-rw-r--r--   0        0        0     1940 2023-05-05 14:30:02.856561 zospy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      430 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/__init__.py
+-rw-r--r--   0        0        0    19416 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/base.py
+-rw-r--r--   0        0        0     7810 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/mtf.py
+-rw-r--r--   0        0        0     5771 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/psf.py
+-rwxr-xr-x   0        0        0    12892 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/raysandspots.py
+-rw-r--r--   0        0        0    34758 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/reports.py
+-rw-r--r--   0        0        0     7204 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/surface.py
+-rw-r--r--   0        0        0     8770 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/analyses/wavefront.py
+-rw-r--r--   0        0        0       88 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI.py
+-rw-r--r--   0        0        0    17150 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Data/__init__.pyi
+-rw-r--r--   0        0        0     7459 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/PhysicalOptics/__init__.pyi
+-rw-r--r--   0        0        0     1500 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/RayTracing/__init__.pyi
+-rw-r--r--   0        0        0    13181 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Aberrations/__init__.pyi
+-rw-r--r--   0        0        0     7370 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/DiffractionEfficiency/__init__.pyi
+-rw-r--r--   0        0        0     6951 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/EncircledEnergy/__init__.pyi
+-rw-r--r--   0        0        0     8224 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/ExtendedScene/__init__.pyi
+-rw-r--r--   0        0        0     1710 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Fans/__init__.pyi
+-rw-r--r--   0        0        0     3185 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Materials/__init__.pyi
+-rw-r--r--   0        0        0    20338 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Mtf/__init__.pyi
+-rw-r--r--   0        0        0     3248 2023-05-05 14:30:02.868561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/NSCSurface/__init__.pyi
+-rw-r--r--   0        0        0     6857 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Psf/__init__.pyi
+-rw-r--r--   0        0        0      289 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/RMSField/__init__.pyi
+-rw-r--r--   0        0        0      309 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/RMSFieldMap/__init__.pyi
+-rw-r--r--   0        0        0     9314 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RMS/__init__.pyi
+-rw-r--r--   0        0        0     6028 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/RayTracing/__init__.pyi
+-rw-r--r--   0        0        0     2847 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Spot/__init__.pyi
+-rw-r--r--   0        0        0    10174 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Surface/__init__.pyi
+-rw-r--r--   0        0        0     2748 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/Wavefront/__init__.pyi
+-rw-r--r--   0        0        0    12350 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Settings/__init__.pyi
+-rw-r--r--   0        0        0     1276 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/QuickYield/__init__.pyi
+-rw-r--r--   0        0        0     3789 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/Tolerancing/__init__.pyi
+-rw-r--r--   0        0        0    29718 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Analysis/__init__.pyi
+-rw-r--r--   0        0        0     7010 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Common/__init__.pyi
+-rw-r--r--   0        0        0   221316 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/LDE/__init__.pyi
+-rw-r--r--   0        0        0     4886 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/MCE/__init__.pyi
+-rw-r--r--   0        0        0    10272 2023-05-05 14:30:02.872561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/MFE/__init__.pyi
+-rw-r--r--   0        0        0   321725 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/NCE/__init__.pyi
+-rw-r--r--   0        0        0     5024 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/TDE/__init__.pyi
+-rw-r--r--   0        0        0    15871 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Editors/__init__.pyi
+-rw-r--r--   0        0        0     4438 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Preferences/__init__.pyi
+-rw-r--r--   0        0        0    21244 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/SystemData/__init__.pyi
+-rw-r--r--   0        0        0    19510 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/General/__init__.pyi
+-rw-r--r--   0        0        0    22251 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/LMx/__init__.pyi
+-rw-r--r--   0        0        0     5075 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/Optimization/__init__.pyi
+-rw-r--r--   0        0        0    16386 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/RayTrace/__init__.pyi
+-rw-r--r--   0        0        0    18928 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/Tolerancing/__init__.pyi
+-rw-r--r--   0        0        0    16271 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Tools/__init__.pyi
+-rw-r--r--   0        0        0    26695 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/Wizards/__init__.pyi
+-rw-r--r--   0        0        0    12760 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI/py.typed
+-rw-r--r--   0        0        0       93 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants.py
+-rw-r--r--   0        0        0     1477 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/PhysicalOptics/__init__.pyi
+-rw-r--r--   0        0        0      358 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/RayTracing/__init__.pyi
+-rw-r--r--   0        0        0     1325 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Aberrations/__init__.pyi
+-rw-r--r--   0        0        0      655 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/EncircledEnergy/__init__.pyi
+-rw-r--r--   0        0        0      613 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/ExtendedScene/__init__.pyi
+-rw-r--r--   0        0        0      395 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Fans/__init__.pyi
+-rw-r--r--   0        0        0      768 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Mtf/__init__.pyi
+-rw-r--r--   0        0        0      517 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/NSCSurface/__init__.pyi
+-rw-r--r--   0        0        0      626 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Psf/__init__.pyi
+-rw-r--r--   0        0        0      282 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/RMSField/__init__.pyi
+-rw-r--r--   0        0        0      302 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/RMSFieldMap/__init__.pyi
+-rw-r--r--   0        0        0     2589 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/RMS/__init__.pyi
+-rw-r--r--   0        0        0      548 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Spot/__init__.pyi
+-rw-r--r--   0        0        0      744 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/Wavefront/__init__.pyi
+-rw-r--r--   0        0        0     1982 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Settings/__init__.pyi
+-rw-r--r--   0        0        0      637 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/QuickYield/__init__.pyi
+-rw-r--r--   0        0        0      560 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/Tolerancing/__init__.pyi
+-rw-r--r--   0        0        0    11188 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Analysis/__init__.pyi
+-rw-r--r--   0        0        0      937 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Common/__init__.pyi
+-rw-r--r--   0        0        0     9011 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/LDE/__init__.pyi
+-rw-r--r--   0        0        0     1792 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/MCE/__init__.pyi
+-rw-r--r--   0        0        0     6853 2023-05-05 14:30:02.876561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/MFE/__init__.pyi
+-rw-r--r--   0        0        0    11143 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/NCE/__init__.pyi
+-rw-r--r--   0        0        0     1158 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/TDE/__init__.pyi
+-rw-r--r--   0        0        0     1854 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Editors/__init__.pyi
+-rw-r--r--   0        0        0      522 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Preferences/__init__.pyi
+-rw-r--r--   0        0        0     3392 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/SystemData/__init__.pyi
+-rw-r--r--   0        0        0     2561 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/General/__init__.pyi
+-rw-r--r--   0        0        0      254 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/LMx/__init__.pyi
+-rw-r--r--   0        0        0      680 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/Optimization/__init__.pyi
+-rw-r--r--   0        0        0     1330 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/RayTrace/__init__.pyi
+-rw-r--r--   0        0        0     3821 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/Tolerancing/__init__.pyi
+-rw-r--r--   0        0        0     1742 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Tools/__init__.pyi
+-rw-r--r--   0        0        0     1224 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/Wizards/__init__.pyi
+-rw-r--r--   0        0        0     1461 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/_ZOSAPI_constants/py.typed
+-rw-r--r--   0        0        0        0 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/__init__.py
+-rw-r--r--   0        0        0     5642 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/apisupport.py
+-rw-r--r--   0        0        0      254 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/config.py
+-rw-r--r--   0        0        0     3996 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/api/constants.py
+-rw-r--r--   0        0        0       49 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/functions/__init__.py
+-rw-r--r--   0        0        0     1997 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/functions/lde.py
+-rw-r--r--   0        0        0     1169 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/functions/nce.py
+-rw-r--r--   0        0        0     6119 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/solvers/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/utils/__init__.py
+-rw-r--r--   0        0        0     3689 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/utils/clrutils.py
+-rw-r--r--   0        0        0     1338 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/utils/pyutils.py
+-rw-r--r--   0        0        0     4471 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/utils/zputils.py
+-rw-r--r--   0        0        0    14957 2023-05-05 14:30:02.880561 zospy-1.0.0/zospy/zpcore.py
+-rw-r--r--   0        0        0     7998 1970-01-01 00:00:00.000000 zospy-1.0.0/PKG-INFO
```

### Comparing `zospy-0.6.2/LICENSE.txt` & `zospy-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zospy-0.6.2/zospy/analyses/mtf.py` & `zospy-1.0.0/zospy/analyses/mtf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,196 +1,201 @@
+"""Zemax OpticStudio analyses from the MTF category."""
+
+from __future__ import annotations
+
 import pandas as pd
 
 from zospy import utils
-from zospy.analyses.base import AnalysisResult
+from zospy.analyses.base import AnalysisResult, OnComplete, new_analysis
 from zospy.api import constants
+from zospy.zpcore import OpticStudioSystem
 
 
-def fft_through_focus_mtf(oss, sampling='64x64', deltafocus=0.1, frequency=0,
-                          numberofsteps=5, wavelength='All', field='All', mtftype='Modulation',
-                          use_polarization=False, use_dashes=False, oncomplete='Close'):
+def fft_through_focus_mtf(
+    oss: OpticStudioSystem,
+    sampling: str | int = "64x64",
+    deltafocus: float = 0.1,
+    frequency: float = 0,
+    numberofsteps: int = 5,
+    wavelength: str | int = "All",
+    field: str | int = "All",
+    mtftype: constants.Analysis.Settings.Mtf.MtfTypes | str = "Modulation",
+    use_polarization: bool = False,
+    use_dashes: bool = False,
+    oncomplete: OnComplete | str = OnComplete.Close,
+) -> AnalysisResult:
     """Wrapper around the OpticStudio FFT Through Focus MTF.
 
     For an in depth explanation of the parameters, see the Zemax OpticStudio user manual
 
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
-    sampling: str or int
+    sampling: str | int
         The sampling, either string (e.g. '64x64') or int. The integer will be treated as a ZOSAPI Constants integer.
     deltafocus: float
         The delta focus, defaults to 0.1
     frequency: float
         The frequency. Defaults to 0.
     numberofsteps: int
         The number of steps. Defaults to 5.
-    wavelength: str or int
+    wavelength: str | int
         The wavelength to use in the MTF. Either 'All' or an integer specifying the wavelength number.
-    field: str or int
+    field: str | int
         The field to use in the MTF. Either 'All' or an integer specifying the field number.
-    mtftype: str or int
-        The MTF type (e.g. 'Modulation') that is calculated.
+    mtftype: zospy.constants.Analysis.Settings.Mtf.MtfTypes.Modulation
+        The MTF type (e.g. `Modulation`) that is calculated.
     use_polarization: bool
         Use polarization. Defaults to False.
     use_dashes: bool
         Use dashes. Defaults to False.
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
 
     Returns
     -------
     AnalysisResult
         A FftThroughFocusMtf analysis result
     """
-    analysistype = 'FftThroughFocusMtf'
+    analysis_type = constants.Analysis.AnalysisIDM.FftThroughFocusMtf
 
     # Create analysis
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysis_type)
 
     # Apply settings
-    analysis.Settings.SampleSize = utils.zputils.proc_constant(constants.Analysis.SampleSizes,
-                                                               utils.zputils.standardize_sampling(sampling))
+    analysis.Settings.SampleSize = getattr(constants.Analysis.SampleSizes, utils.zputils.standardize_sampling(sampling))
     analysis.Settings.DeltaFocus = deltafocus
     analysis.Settings.Frequency = frequency
     analysis.Settings.NumberOfSteps = numberofsteps
-    utils.zputils.analysis_set_wavelength(analysis, wavelength)
-    utils.zputils.analysis_set_field(analysis, field)
-    analysis.Settings.Type = utils.zputils.proc_constant(constants.Analysis.Settings.Mtf.MtfTypes, mtftype)
+    analysis.set_wavelength(wavelength)
+    analysis.set_field(field)
+    analysis.Settings.Type = constants.process_constant(constants.Analysis.Settings.Mtf.MtfTypes, mtftype)
     analysis.Settings.UsePolarization = use_polarization
     analysis.Settings.UseDashes = use_dashes
 
     # Calculate
     analysis.ApplyAndWaitForCompletion()
-    
+
     # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Get settings
-    settings = pd.Series(name='Settings')
+    settings = pd.Series(name="Settings", dtype=object)
+
+    settings.loc["SampleSize"] = str(analysis.Settings.SampleSize)
+    settings.loc["DeltaFocus"] = analysis.Settings.DeltaFocus
+    settings.loc["Frequency"] = analysis.Settings.Frequency
+    settings.loc["Wavelength"] = analysis.get_wavelength()
+    settings.loc["Field"] = analysis.get_field()
+    settings.loc["Type"] = str(analysis.Settings.Type)
+    settings.loc["UsePolarization"] = analysis.Settings.UsePolarization
+    settings.loc["UseDashes"] = analysis.Settings.UseDashes
 
-    settings.loc['SampleSize'] = utils.zputils.series_index_by_value(constants.Analysis.SampleSizes,
-                                                                     analysis.Settings.SampleSize)
-    settings.loc['DeltaFocus'] = analysis.Settings.DeltaFocus
-    settings.loc['Frequency'] = analysis.Settings.Frequency
-    settings.loc['Wavelength'] = utils.zputils.analysis_get_wavelength(analysis)
-    settings.loc['Field'] = utils.zputils.analysis_get_field(analysis)
-    settings.loc['Type'] = utils.zputils.series_index_by_value(constants.Analysis.Settings.Mtf.MtfTypes,
-                                                               analysis.Settings.Type)
-    settings.loc['UsePolarization'] = analysis.Settings.UsePolarization
-    settings.loc['UseDashes'] = analysis.Settings.UseDashes
-    
     # Get data and unpack
     data = []
     for ii in range(analysis.Results.NumberOfDataSeries):
         data.append(utils.zputils.unpack_dataseries(analysis.Results.DataSeries[ii]))
 
     if not len(data):
         data = pd.DataFrame()
     elif len(data) == 1:
         data = data[0]
     else:
         data = pd.concat(data, axis=1)
-    
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages)
-
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
 
-    return ret
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+    )
+
+    return analysis.complete(oncomplete, result)
 
 
-def fft_through_focus_mtf_fromcfg(oss, cfgfile, oncomplete='Close'):
+def fft_through_focus_mtf_fromcfg(
+    oss: OpticStudioSystem, cfgfile: str, oncomplete: OnComplete | str = OnComplete.Close
+):
     """Wrapper around the OpticStudio FFT Through Focus MTF using a configuration file.
 
     For an in depth explanation of the parameters, see the Zemax OpticStudio user manual
 
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
     cfgfile: str
         Full filepath (including extension) to a configuration file.
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
 
     Returns
     -------
     AnalysisResult
         An FftThroughFocusMtf analysis result. Next to the standard data, the cfgfile will be added under 'UsedCfgFile'
     """
-    analysistype = 'FftThroughFocusMtf'
+    analysis_type = constants.Analysis.AnalysisIDM.FftThroughFocusMtf
 
     # Create analysis
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysis_type)
 
     # Apply settings
     analysis.Settings.LoadFrom(cfgfile)
 
     # Calculate
     analysis.ApplyAndWaitForCompletion()
 
     # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Get settings
-    settings = pd.Series()
+    settings = pd.Series(name="Settings", dtype=object)
     settings.drop(settings.index, inplace=True)
 
-    settings.loc['SampleSize'] = constants.get_constantname_by_value(
-        constants.Analysis.SampleSizes, analysis.Settings.SampleSize)
-    settings.loc['DeltaFocus'] = analysis.Settings.DeltaFocus
-    settings.loc['Frequency'] = analysis.Settings.Frequency
-    settings.loc['NumberOfSteps'] = analysis.Settings.NumberOfSteps
-    settings.loc['Wavelength'] = analysis.Settings.Wavelength.GetWavelengthNumber()  # Todo Evaluate
-    settings.loc['Field'] = analysis.Settings.Field.GetFieldNumber()  # Todo Evaluate
-    settings.loc['Type'] = constants.get_constantname_by_value(
-        constants.Analysis.Settings.Mtf.MtfTypes, analysis.Settings.Type)
-    settings.loc['UsePolarization'] = analysis.Settings.UsePolarization
-    settings.loc['UseDashes'] = analysis.Settings.UseDashes
+    settings.loc["SampleSize"] = str(analysis.Settings.SampleSize)
+    settings.loc["DeltaFocus"] = analysis.Settings.DeltaFocus
+    settings.loc["Frequency"] = analysis.Settings.Frequency
+    settings.loc["NumberOfSteps"] = analysis.Settings.NumberOfSteps
+    settings.loc["Wavelength"] = analysis.Settings.Wavelength.GetWavelengthNumber()  # Todo Evaluate
+    settings.loc["Field"] = analysis.Settings.Field.GetFieldNumber()  # Todo Evaluate
+    settings.loc["Type"] = str(analysis.Settings.Type)
+    settings.loc["UsePolarization"] = analysis.Settings.UsePolarization
+    settings.loc["UseDashes"] = analysis.Settings.UseDashes
 
     # Get data and unpack
     data = []
     for ii in range(analysis.Results.NumberOfDataSeries):
         data.append(utils.zputils.unpack_dataseries(analysis.Results.DataSeries[ii]))
 
     if not len(data):
         data = pd.DataFrame()
     elif len(data) == 1:
         data = data[0]
     else:
         data = pd.concat(data, axis=1)
 
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages,
-                         UsedCfgFile=cfgfile)
-
-    # Process oncomplete
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+        UsedCfgFile=cfgfile,
+    )
 
-    return ret
+    return analysis.complete(oncomplete, result)
```

### Comparing `zospy-0.6.2/zospy/analyses/psf.py` & `zospy-1.0.0/zospy/analyses/psf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,136 @@
+"""Zemax OpticStudio analyses from the PSF category."""
+
+from __future__ import annotations
+
 import pandas as pd
 
 from zospy import utils
-from zospy.analyses.base import AnalysisResult, AttrDict
+from zospy.analyses.base import AnalysisResult, AttrDict, OnComplete, new_analysis
 from zospy.api import constants
 
 
-def huygens_psf(oss, pupil_sampling='32x32', image_sampling='32x32', image_delta=0, rotation=0, wavelength='All',
-                field=1, psftype='Linear', show_as='Surface', use_polarization=False, use_centroid=False,
-                normalize=False, oncomplete='Close'):
-    """Wrapper around the OpticStudio Huygens PSF
-    
+def huygens_psf(
+    oss,
+    pupil_sampling: str | int = "32x32",
+    image_sampling: str | int = "32x32",
+    image_delta: float = 0,
+    rotation: float = 0,
+    wavelength: str | int = "All",
+    field: str | int = 1,
+    psftype: constants.Analysis.Settings.HuygensPsfTypes | str = "Linear",
+    show_as: constants.Analysis.HuygensShowAsTypes | str = "Surface",
+    use_polarization: bool = False,
+    use_centroid: bool = False,
+    normalize: bool = False,
+    oncomplete: OnComplete | str = OnComplete.Close,
+) -> AnalysisResult:
+    """Wrapper around the OpticStudio Huygens PSF.
+
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
-    pupil_sampling: str or int
-        The pupil sampling, either string (e.g. '64x64') or int. The integer will be treated as a ZOSAPI Constants 
+    pupil_sampling: str | int
+        The pupil sampling, either string (e.g. '64x64') or int. The integer will be treated as a ZOSAPI Constants
         integer.
-    image_sampling: str or int
-        The image sampling, either string (e.g. '64x64') or int. The integer will be treated as a ZOSAPI Constants 
+    image_sampling: str | int
+        The image sampling, either string (e.g. '64x64') or int. The integer will be treated as a ZOSAPI Constants
         integer.
-    image_delta: float or int
+    image_delta: float | int
         The image delta
     rotation: int
-        The rotation, should be one off [0, 90, 180, 270].
-    wavelength: str or int
-        The wavelength number that is to be used. Either 'All' or an integer specifying the wavelength number. 
+        The rotation, should be one of [0, 90, 180, 270].
+    wavelength: str | int
+        The wavelength number that is to be used. Either 'All' or an integer specifying the wavelength number.
         Defaults to 'All'.
-    field: str or int
-        The field number that is to be used. Either 'All' or an integer specifying the field number. Defaults to 1. 
-    psftype: str or int
+    field: str | int
+        The field number that is to be used. Either 'All' or an integer specifying the field number. Defaults to 1.
+    psftype: str | int
         The PSF type (e.g. 'Linear') that is calculated. Defaults to 'Linear'.
-    show_as: str or int
+    show_as: str | int
         Defines how the data is showed within OpticStudio. Defaults to 'Surface'
     use_polarization: bool
         Defines if polarization is used. Defaults to False.
     use_centroid: bool
         Defines if centroid is used. Defaults to False.
     normalize: bool
         Defines if normalization is used. Defaults to False.
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
 
     Returns
     -------
     AnalysisResult
         A HuygensPsf analysis result
     """  # ToDo check if default for filed is correct
-
-    analysistype = 'HuygensPsf'
+    analysistype = constants.Analysis.AnalysisIDM.HuygensPsf
 
     # Create analysis
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysistype)
 
     # Apply settings
-    analysis.Settings.PupilSampleSize = utils.zputils.proc_constant(constants.Analysis.SampleSizes,
-                                                                    utils.zputils.standardize_sampling(pupil_sampling))
-    analysis.Settings.ImageSampleSize = utils.zputils.proc_constant(constants.Analysis.SampleSizes,
-                                                                    utils.zputils.standardize_sampling(image_sampling))
+    analysis.Settings.PupilSampleSize = getattr(
+        constants.Analysis.SampleSizes, utils.zputils.standardize_sampling(pupil_sampling)
+    )
+    analysis.Settings.ImageSampleSize = getattr(
+        constants.Analysis.SampleSizes, utils.zputils.standardize_sampling(image_sampling)
+    )
     analysis.Settings.ImageDelta = image_delta
-    analysis.Settings.Rotation = constants.Analysis.Settings.Rotations.loc[f'Rotate_{rotation}']
-    utils.zputils.analysis_set_wavelength(analysis, wavelength)
-    utils.zputils.analysis_set_field(analysis, field)
-    analysis.Settings.Type = constants.Analysis.Settings.HuygensPsfTypes.loc[psftype]
-    analysis.Settings.ShowAsType = constants.Analysis.HuygensShowAsTypes.loc[show_as]
+    analysis.Settings.Rotation = getattr(constants.Analysis.Settings.Rotations, f"Rotate_{rotation}")
+    analysis.set_wavelength(wavelength)
+    analysis.set_field(field)
+    analysis.Settings.Type = constants.process_constant(constants.Analysis.Settings.HuygensPsfTypes, psftype)
+    analysis.Settings.ShowAsType = constants.process_constant(constants.Analysis.HuygensShowAsTypes, show_as)
     analysis.Settings.UsePolarization = use_polarization
     analysis.Settings.UseCentroid = use_centroid
     analysis.Settings.Normalize = normalize
 
     # Calculate
     analysis.ApplyAndWaitForCompletion()
 
     # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Get settings
-    settings = pd.Series(name='Settings')
+    settings = pd.Series(name="Settings", dtype=object)
 
-    settings.loc['PupilSampleSize'] = constants.get_constantname_by_value(constants.Analysis.SampleSizes,
-                                                                          analysis.Settings.PupilSampleSize)
-    settings.loc['ImageSampleSize'] = constants.get_constantname_by_value(constants.Analysis.SampleSizes,
-                                                                          analysis.Settings.ImageSampleSize)
-    settings.loc['ImageDelta'] = analysis.Settings.ImageDelta
-    settings.loc['Rotation'] = int(constants.get_constantname_by_value(constants.Analysis.Settings.Rotations,
-                                                                       analysis.Settings.Rotation).split('_')[1])
-    settings.loc['Wavelength'] = utils.zputils.analysis_get_wavelength(analysis)
-    settings.loc['Field'] = utils.zputils.analysis_get_field(analysis)
-    settings.loc['Type'] = constants.get_constantname_by_value(constants.Analysis.Settings.HuygensPsfTypes,
-                                                               analysis.Settings.Type)
-    settings.loc['ShowAsType'] = constants.get_constantname_by_value(constants.Analysis.HuygensShowAsTypes,
-                                                                     analysis.Settings.Type)
-    settings.loc['UsePolarization'] = analysis.Settings.UsePolarization
-    settings.loc['UseCentroid'] = analysis.Settings.UseCentroid
-    settings.loc['Normalize'] = analysis.Settings.Normalize
+    settings.loc["PupilSampleSize"] = str(analysis.Settings.PupilSampleSize)
+    settings.loc["ImageSampleSize"] = str(analysis.Settings.ImageSampleSize)
+    settings.loc["ImageDelta"] = analysis.Settings.ImageDelta
+    settings.loc["Rotation"] = int(str(analysis.Settings.Rotation).split("_")[1])
+    settings.loc["Wavelength"] = analysis.get_wavelength()
+    settings.loc["Field"] = analysis.get_field()
+    settings.loc["Type"] = str(analysis.Settings.Type)
+    settings.loc["ShowAsType"] = str(analysis.Settings.ShowAsType)
+    settings.loc["UsePolarization"] = analysis.Settings.UsePolarization
+    settings.loc["UseCentroid"] = analysis.Settings.UseCentroid
+    settings.loc["Normalize"] = analysis.Settings.Normalize
 
     # Get data
     if analysis.Results.NumberOfDataGrids <= 0:
         data = None
     elif analysis.Results.NumberOfDataGrids == 1:
         data = utils.zputils.unpack_datagrid(analysis.Results.DataGrids[0])
     else:
         data = AttrDict()
         for ii in range(analysis.Results.NumberOfDataGrids):
             desc = analysis.Results.DataGrids[ii].Description
-            key = desc if desc != '' else str(ii)
+            key = desc if desc != "" else str(ii)
             data[key] = utils.zputils.unpack_datagrid(analysis.Results.DataGrids[ii])
 
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages)
-
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
+    result = AnalysisResult(
+        analysistype=str(analysistype),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+    )
 
-    return ret
+    return analysis.complete(oncomplete, result)
```

### Comparing `zospy-0.6.2/zospy/analyses/raysandspots.py` & `zospy-1.0.0/zospy/analyses/raysandspots.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,315 +1,337 @@
-import os
-import re
-
-from tempfile import mkstemp
-from io import StringIO
-
-import numpy as np
-import pandas as pd
-
-from zospy import utils
-from zospy.analyses.base import AnalysisResult, AttrDict
-from zospy.api import constants
-import zospy.api.config as _config
-
-def _structure_ray_trace_data_result(line_list):
-    """Structures the result of a ray trace data report.
-
-    Parameters
-    ----------
-    line_list: list of str
-        The line list obtained by reading in the results
-
-    Returns
-    -------
-    dict
-        The results structured in a dictionary
-    """
-    # Create output dict
-    res = AttrDict()
-
-    # Add header
-    hdr = line_list[0].strip().replace('\ufeff', '')
-    res['Header'] = hdr
-
-    # Register landmarks
-    landmarks = ['Real Ray Trace Data',
-                 'Paraxial Ray Trace Data',
-                 'Trace of Paraxial Y marginal, U marginal, Y chief, U chief only']
-    comp = re.compile(rf'^({"|".join(landmarks)})', re.IGNORECASE)
-    inds = {comp.match(line).group().lower(): {'rnum': rnum, 'name': comp.match(line).group()}
-            for rnum, line in enumerate(line_list) if comp.match(line)}
-
-    order_of_appearance = [item[0] for item in sorted(inds.items(), key=lambda x: x[1]['rnum'])]
-
-    # Add general lens data
-    for target in inds.keys():
-        section_start = inds[target]['rnum'] + 1  # + 1 to ignore section title
-
-        # Get endpoint
-        if order_of_appearance.index(target) == len(inds) - 1:
-            section_end = len(line_list)
-        else:
-            target2 = order_of_appearance[order_of_appearance.index(target) + 1]
-            section_end = inds[target2]['rnum']
-
-        # Read as dataframe
-        df = pd.read_csv(StringIO(''.join(line_list[section_start:section_end]).replace(' ','')),
-                          delimiter='\t', decimal=_config.DECIMAL)
-
-        # Recover case of target
-        keyname = inds[target]['name'].replace(' ','')
-
-        # Add to result dictionary
-        res[keyname] = df
-
-    return res
-
-
-def single_ray_trace(oss, hx=0, hy=0, px=0, py=1, wavelength=1, field=0, rttype='DirectionCosines',
-                     global_coordinates=False, oncomplete='Close', txtoutfile=None):
-    """Wrapper around the OpticStudio Single Ray Trace Analysis.
-
-    Due to limitations in the ZOS-API, the output is obtained by writing the OpticStudio results to a file and
-    subsequently reading in this file
-
-    Parameters
-    ----------
-    oss: zospy.core.OpticStudioSystem
-        A ZOSPy OpticStudioSystem instance. Should be sequential.
-    hx: float
-        Normalized X Field Coord. Defaults to 0.
-    hy: float
-        Normalized Y Field Coord. Defaults to 0.
-    px: float
-        Normalized X Pupil Coord. Defaults to 0.
-    py: float
-        Normalized Y Pupil Coord. Defaults to 1.
-    rttype: str or int
-        The Ray Trace type (e.g. 'DirectionCosines') that is calculated. Defaults to 'DirectionCosines'.
-    wavelength: int
-        The wavelength number that is to be used. Must be an integer specifying the wavelength number. 
-        Defaults to 1.
-    field: int
-        The field number that is to be used. Must be an integer specifying the field number. "Arbitrary" is 0. Defaults 
-        to 0.
-    global_coordinates: bool
-        Defines if global coordinates are used. Defaults to False.
-    oncomplete: str
-        Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
-        the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
-        the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
-        with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
-        instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
-    txtoutfile: str or None
-        The textfile to which the OpticStudio output is saved. If None, a temporary file will be created and deleted. If
-        string, it should be a full system path with '.txt' as extension, after which the file will be saved in that
-        location. Defaults to None.
-
-    Returns
-    -------
-    AnalysisResult
-        A Single Ray Trace result. Next to the standard data, the raw text return obtained from the analysis
-        will be present under 'RawTextData', and the txtoutfile under 'TxtOutFile'.
-    """
-
-    analysistype = 'RayTrace'
-
-    # Temp file
-    if txtoutfile is None:
-        fd, txtoutfile = mkstemp(suffix='.txt', prefix='zospy_')
-        os.close(fd)
-        cleantxt = True
-    else:
-        if not txtoutfile.endswith('.txt'):
-            raise ValueError('txtfile should end with ".txt"')
-        cleantxt = False
-
-
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
-
-    # Settings for ray trace
-    analysis.Settings.Hx = hx
-    analysis.Settings.Hy = hy
-    analysis.Settings.Px = px
-    analysis.Settings.Py = py
-    utils.zputils.analysis_set_wavelength(analysis, wavelength)
-    utils.zputils.analysis_set_field(analysis, field)
-    analysis.Settings.Type = utils.zputils.proc_constant(constants.Analysis.Settings.Aberrations.RayTraceType, rttype)
-    analysis.Settings.UseGlobal = global_coordinates
-    
-    # Run analysis
-    analysis.ApplyAndWaitForCompletion()
-
-    # Get results
-    analysis.Results.GetTextFile(txtoutfile)
-    line_list = [line for line in open(txtoutfile, 'r', encoding='utf-16-le')]
-    data = _structure_ray_trace_data_result(line_list)
-
-    # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
-
-    # Get settings
-    settings = pd.Series(name='Settings')
-
-    settings.loc['Hx'] = analysis.Settings.Hx
-    settings.loc['Hy'] = analysis.Settings.Hy
-    settings.loc['Px'] = analysis.Settings.Px
-    settings.loc['Py'] = analysis.Settings.Py
-    settings.loc['Wavelength'] = utils.zputils.analysis_get_wavelength(analysis)
-    settings.loc['Field'] = utils.zputils.analysis_get_field(analysis)
-    settings.loc['Type'] = utils.zputils.series_index_by_value(constants.Analysis.Settings.Aberrations.RayTraceType,
-                                                               analysis.Settings.Type)
-    settings.loc['GlobalCoordinates'] = analysis.Settings.UseGlobal
-
-    # Create output
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages,
-                         RawTextData=line_list, TxtOutFile=txtoutfile)  # Set additional params
-
-    # cleanup if needed
-    if cleantxt:
-        os.remove(txtoutfile)
-
-    # Process oncomplete
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
-
-    return ret
-
-
-
-def ray_fan(oss, plot_scale=0, number_of_rays=20, field='All', wavelength='All', tangential='Aberration_Y',
-            sagittal='Aberration_X', surface='Image', use_dashes=False, vignetted_pupil=True, check_apertures=True,
-            oncomplete='Close'):
-    """Wrapper around the OpticStudio Ray Fan Analysis.
-
-    Parameters
-    ----------
-    oss: zospy.core.OpticStudioSystem
-        A ZOSPy OpticStudioSystem instance. Should be sequential.
-    plot_scale: int or float
-        Sets the maximum vertical scale for the plots. When 0, automatic scaling is used. Defaults to 0.
-    number_of_rays: int
-        This is the number of rays traced on each side of the origin of the plot.
-    field: str or int
-        The field number that is to be used. Either 'All' or an integer specifying the field number. Defaults to 'All'.
-    wavelength: str or int
-        The wavelength number that is to be used. Either 'All' or an integer specifying the wavelength number. 
-        Defaults to 'All'.
-    tangential: str or int
-        The aberration component that is plotted for the tangential fan. Accepts sting ('Aberration_Y' or
-        'Aberration_X') or int (respectively 0 and 1). Defaults to 'Aberration_Y'.
-    sagittal: str or int
-        The aberration component that is plotted for the sagittal fan. Accepts sting ('Aberration_X' or
-        'Aberration_Y') or int (respectively 0 and 1). Defaults to 'Aberration_X'.
-    surface: str or int
-        The surface that is to be analyzed. Either 'Image', 'Object' or an integer. Defaults to 'Image'.
-    use_dashes: bool
-        Defines whether solid lines or dashes are used to differentiate curves. Defaults to False.
-    vignetted_pupil: bool
-        Defines whether the pupil axis is scaled to the unvignetted pupil or not. Defaults to True.
-    check_apertures: bool
-        Defines whether only rays that pass all surface apertures are drawn or not. Defaults to True.
-    oncomplete: str
-        Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
-        the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
-        the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
-        with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
-        instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
-
-    Returns
-    -------
-    AnalysisResult
-        A Ray Fan result.
-    """
-
-    # Set up analysis type
-    analysistype = 'RayFan'
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
-
-    # Settings for ray fan
-    utils.zputils.analysis_set_field(analysis, field)
-    utils.zputils.analysis_set_surface(analysis, surface)
-    utils.zputils.analysis_set_wavelength(analysis, wavelength)
-    analysis.Settings.NumberOfRays = number_of_rays
-    analysis.Settings.PlotScale = plot_scale
-    analysis.Settings.CheckApertures = check_apertures
-    analysis.Settings.VignettedPupil = vignetted_pupil
-    analysis.Settings.UseDashes = use_dashes
-    analysis.Settings.Sagittal = \
-        utils.zputils.proc_constant(constants.Analysis.Settings.Fans.SagittalAberrationComponent, sagittal)
-    analysis.Settings.Tangential = \
-        utils.zputils.proc_constant(constants.Analysis.Settings.Fans.TangentialAberrationComponent, tangential)
-
-    # Run analysis
-    analysis.ApplyAndWaitForCompletion()
-
-    # Parse results
-    results = analysis.GetResults()
-    data = AttrDict()
-    data['Header'] = 'Ray Fan Data'
-    for ii in range(results.DataSeries.Length):
-        # get raw .NET data into numpy array
-        ds = results.GetDataSeries(ii)
-        xRaw = np.asarray(tuple(ds.XData.Data))
-        yRaw = np.asarray(tuple(ds.YData.Data))
-
-        # Reshape data
-        x = xRaw
-        y = yRaw.reshape(ds.YData.Data.GetLength(0), ds.YData.Data.GetLength(1))
-
-        # Make data frame
-        df = {ds.XLabel:x}
-        for jj, label in enumerate(ds.SeriesLabels):
-            df[label] = y[:,jj]
-        df = pd.DataFrame(data=df)
-        
-        # Add data to dictionary
-        data[ds.Description] = df
-
-    # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
-
-    # Get settings
-    settings = pd.Series(name='Settings')
-    settings.loc['Field'] = utils.zputils.analysis_get_field(analysis)
-    settings.loc['Surface'] = analysis.Settings.Surface.GetSurfaceNumber()
-    settings.loc['Wavelength'] = utils.zputils.analysis_get_wavelength(analysis)
-    settings.loc['NumberOfRays'] = analysis.Settings.NumberOfRays
-    settings.loc['PlotScale'] = analysis.Settings.PlotScale
-    settings.loc['CheckApertures'] = analysis.Settings.CheckApertures
-    settings.loc['VignettedPupil'] = analysis.Settings.VignettedPupil
-    settings.loc['UseDashes'] = analysis.Settings.UseDashes
-    settings.loc['Sagittal'] = \
-        utils.zputils.series_index_by_value(constants.Analysis.Settings.Fans.SagittalAberrationComponent,
-                                            analysis.Settings.Sagittal)
-    settings.loc['Tangential'] = \
-        utils.zputils.series_index_by_value(constants.Analysis.Settings.Fans.TangentialAberrationComponent,
-                                            analysis.Settings.Tangential)
-
-    # Create output
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages)  # Set additional params
-
-    # Process oncomplete
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
-
-    return ret
+"""Zemax OpticStudio analyses from the Rays and Spots category."""
+
+from __future__ import annotations
+
+import os
+import re
+from io import StringIO
+from tempfile import mkstemp
+from typing import Any
+
+import numpy as np
+import pandas as pd
+
+import zospy.api.config as _config
+from zospy.analyses.base import AnalysisResult, AttrDict, OnComplete, new_analysis
+from zospy.api import constants
+from zospy.zpcore import OpticStudioSystem
+
+
+def _structure_ray_trace_data_result(line_list: list[str]) -> dict[str, Any]:
+    """Structures the result of a ray trace data report.
+
+    Parameters
+    ----------
+    line_list: list[str]
+        The line list obtained by reading in the results
+
+    Returns
+    -------
+    dict
+        The results structured in a dictionary
+    """
+    # Create output dict
+    res = AttrDict()
+
+    # Add header
+    hdr = line_list[0].strip().replace("\ufeff", "")
+    res["Header"] = hdr
+
+    # Register landmarks
+    landmarks = [
+        "Real Ray Trace Data",
+        "Paraxial Ray Trace Data",
+        "Trace of Paraxial Y marginal, U marginal, Y chief, U chief only",
+    ]
+    comp = re.compile(rf'^({"|".join(landmarks)})', re.IGNORECASE)
+    inds = {
+        comp.match(line).group().lower(): {"rnum": rnum, "name": comp.match(line).group()}
+        for rnum, line in enumerate(line_list)
+        if comp.match(line)
+    }
+
+    order_of_appearance = [item[0] for item in sorted(inds.items(), key=lambda x: x[1]["rnum"])]
+
+    # Add general lens data
+    for target in inds.keys():
+        section_start = inds[target]["rnum"] + 1  # + 1 to ignore section title
+
+        # Get endpoint
+        if order_of_appearance.index(target) == len(inds) - 1:
+            section_end = len(line_list)
+        else:
+            target2 = order_of_appearance[order_of_appearance.index(target) + 1]
+            section_end = inds[target2]["rnum"]
+
+        # Read as dataframe
+        df = pd.read_csv(
+            StringIO("".join(line_list[section_start:section_end]).replace(" ", "")),
+            delimiter="\t",
+            decimal=_config.DECIMAL,
+        )
+
+        # Recover case of target
+        keyname = inds[target]["name"].replace(" ", "")
+
+        # Add to result dictionary
+        res[keyname] = df
+
+    return res
+
+
+def single_ray_trace(
+    oss: OpticStudioSystem,
+    hx: float = 0,
+    hy: float = 0,
+    px: float = 0,
+    py: float = 1,
+    wavelength: str | int = 1,
+    field: str | int = 0,
+    raytrace_type: constants.Analysis.Settings.Aberrations.RayTraceType | str = "DirectionCosines",
+    global_coordinates: bool = False,
+    oncomplete: OnComplete | str = OnComplete.Close,
+    txtoutfile: str | None = None,
+) -> AnalysisResult:
+    """Wrapper around the OpticStudio Single Ray Trace Analysis.
+
+    Due to limitations in the ZOS-API, the output is obtained by writing the OpticStudio results to a file and
+    subsequently reading in this file
+
+    Parameters
+    ----------
+    oss: zospy.core.OpticStudioSystem
+        A ZOSPy OpticStudioSystem instance. Should be sequential.
+    hx: float
+        Normalized X Field Coord. Defaults to 0.
+    hy: float
+        Normalized Y Field Coord. Defaults to 0.
+    px: float
+        Normalized X Pupil Coord. Defaults to 0.
+    py: float
+        Normalized Y Pupil Coord. Defaults to 1.
+    raytrace_type: zospy.api.constants.Analysis.Settings.Aberrations.RayTraceType
+        The Ray Trace type (e.g. 'DirectionCosines') that is calculated. Defaults to 'DirectionCosines'.
+    wavelength: int
+        The wavelength number that is to be used. Must be an integer specifying the wavelength number.
+        Defaults to 1.
+    field: int
+        The field number that is to be used. Must be an integer specifying the field number. "Arbitrary" is 0. Defaults
+        to 0.
+    global_coordinates: bool
+        Defines if global coordinates are used. Defaults to False.
+    oncomplete: OnComplete | str
+        Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
+        the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
+        the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
+        with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
+        instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
+    txtoutfile: str | None
+        The textfile to which the OpticStudio output is saved. If None, a temporary file will be created and deleted. If
+        string, it should be a full system path with '.txt' as extension, after which the file will be saved in that
+        location. Defaults to None.
+
+    Returns
+    -------
+    AnalysisResult
+        A Single Ray Trace result. Next to the standard data, the raw text return obtained from the analysis
+        will be present under 'RawTextData', and the txtoutfile under 'TxtOutFile'.
+    """
+    analysis_type = constants.Analysis.AnalysisIDM.RayTrace
+
+    # Temp file
+    if txtoutfile is None:
+        fd, txtoutfile = mkstemp(suffix=".txt", prefix="zospy_")
+        os.close(fd)
+        cleantxt = True
+    else:
+        if not txtoutfile.endswith(".txt"):
+            raise ValueError('txtfile should end with ".txt"')
+        cleantxt = False
+
+    analysis = new_analysis(oss, analysis_type)
+
+    analysis.Settings.Hx = hx
+    analysis.Settings.Hy = hy
+    analysis.Settings.Px = px
+    analysis.Settings.Py = py
+    analysis.set_wavelength(wavelength)
+    analysis.set_field(field)
+    analysis.Settings.Type = constants.process_constant(
+        constants.Analysis.Settings.Aberrations.RayTraceType, raytrace_type
+    )
+    analysis.Settings.UseGlobal = global_coordinates
+
+    # Run analysis
+    analysis.ApplyAndWaitForCompletion()
+
+    # Get results
+    analysis.Results.GetTextFile(txtoutfile)
+    line_list = [line for line in open(txtoutfile, "r", encoding="utf-16-le")]
+    data = _structure_ray_trace_data_result(line_list)
+
+    # Get headerdata, metadata and messages
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
+
+    # Get settings
+    settings = pd.Series(name="Settings", dtype=object)
+
+    settings.loc["Hx"] = analysis.Settings.Hx
+    settings.loc["Hy"] = analysis.Settings.Hy
+    settings.loc["Px"] = analysis.Settings.Px
+    settings.loc["Py"] = analysis.Settings.Py
+    settings.loc["Wavelength"] = analysis.get_wavelength()
+    settings.loc["Field"] = analysis.get_field()
+    settings.loc["Type"] = str(analysis.Settings.Type)
+    settings.loc["GlobalCoordinates"] = analysis.Settings.UseGlobal
+
+    # Create output
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+        RawTextData=line_list,
+        TxtOutFile=txtoutfile,
+    )  # Set additional params
+
+    # cleanup if needed
+    if cleantxt:
+        os.remove(txtoutfile)
+
+    return analysis.complete(oncomplete, result)
+
+
+def ray_fan(
+    oss: OpticStudioSystem,
+    plot_scale: float = 0,
+    number_of_rays: int = 20,
+    field: str | int = "All",
+    wavelength: str | int = "All",
+    tangential: constants.Analysis.Settings.Fans.TangentialAberrationComponent | str = "Aberration_Y",
+    sagittal: constants.Analysis.Settings.Fans.SagittalAberrationComponent | str = "Aberration_X",
+    surface: str | int = "Image",
+    use_dashes: bool = False,
+    vignetted_pupil: bool = True,
+    check_apertures: bool = True,
+    oncomplete: OnComplete | str = OnComplete.Close,
+) -> AnalysisResult:
+    """Wrapper around the OpticStudio Ray Fan Analysis.
+
+    Parameters
+    ----------
+    oss: zospy.core.OpticStudioSystem
+        A ZOSPy OpticStudioSystem instance. Should be sequential.
+    plot_scale: int | float
+        Sets the maximum vertical scale for the plots. When 0, automatic scaling is used. Defaults to 0.
+    number_of_rays: int
+        This is the number of rays traced on each side of the origin of the plot.
+    field: str or int
+        The field number that is to be used. Either 'All' or an integer specifying the field number. Defaults to 'All'.
+    wavelength: str | int
+        The wavelength number that is to be used. Either 'All' or an integer specifying the wavelength number.
+        Defaults to 'All'.
+    tangential: str | int
+        The aberration component that is plotted for the tangential fan. Accepts sting ('Aberration_Y' or
+        'Aberration_X') or int (respectively 0 and 1). Defaults to 'Aberration_Y'.
+    sagittal: str | int
+        The aberration component that is plotted for the sagittal fan. Accepts sting ('Aberration_X' or
+        'Aberration_Y') or int (respectively 0 and 1). Defaults to 'Aberration_X'.
+    surface: str | int
+        The surface that is to be analyzed. Either 'Image', 'Object' or an integer. Defaults to 'Image'.
+    use_dashes: bool
+        Defines whether solid lines or dashes are used to differentiate curves. Defaults to False.
+    vignetted_pupil: bool
+        Defines whether the pupil axis is scaled to the unvignetted pupil or not. Defaults to True.
+    check_apertures: bool
+        Defines whether only rays that pass all surface apertures are drawn or not. Defaults to True.
+    oncomplete: OnComplete | str
+        Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
+        the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
+        the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
+        with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
+        instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
+
+    Returns
+    -------
+    AnalysisResult
+        A Ray Fan result.
+    """
+    # Set up analysis type
+    analysis_type = constants.Analysis.AnalysisIDM.RayFan
+    analysis = new_analysis(oss, analysis_type)
+
+    # Settings for ray fan
+    analysis.set_field(field)
+    analysis.set_surface(surface)
+    analysis.set_wavelength(wavelength)
+    analysis.Settings.NumberOfRays = number_of_rays
+    analysis.Settings.PlotScale = plot_scale
+    analysis.Settings.CheckApertures = check_apertures
+    analysis.Settings.VignettedPupil = vignetted_pupil
+    analysis.Settings.UseDashes = use_dashes
+    analysis.Settings.Sagittal = constants.process_constant(
+        constants.Analysis.Settings.Fans.SagittalAberrationComponent, sagittal
+    )
+    analysis.Settings.Tangential = constants.process_constant(
+        constants.Analysis.Settings.Fans.TangentialAberrationComponent, tangential
+    )
+
+    # Run analysis
+    analysis.ApplyAndWaitForCompletion()
+
+    # Parse results
+    results = analysis.GetResults()
+    data = AttrDict()
+    data["Header"] = "Ray Fan Data"
+    for ii in range(results.DataSeries.Length):
+        # get raw .NET data into numpy array
+        ds = results.GetDataSeries(ii)
+        xRaw = np.asarray(tuple(ds.XData.Data))
+        yRaw = np.asarray(tuple(ds.YData.Data))
+
+        # Reshape data
+        x = xRaw
+        y = yRaw.reshape(ds.YData.Data.GetLength(0), ds.YData.Data.GetLength(1))
+
+        # Make data frame
+        df = {ds.XLabel: x}
+        for jj, label in enumerate(ds.SeriesLabels):
+            df[label] = y[:, jj]
+        df = pd.DataFrame(data=df)
+
+        # Add data to dictionary
+        data[ds.Description] = df
+
+    # Get headerdata, metadata and messages
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
+
+    # Get settings
+    settings = pd.Series(name="Settings", dtype=object)
+    settings.loc["Field"] = analysis.get_field()
+    settings.loc["Surface"] = analysis.Settings.Surface.GetSurfaceNumber()
+    settings.loc["Wavelength"] = analysis.get_wavelength()
+    settings.loc["NumberOfRays"] = analysis.Settings.NumberOfRays
+    settings.loc["PlotScale"] = analysis.Settings.PlotScale
+    settings.loc["CheckApertures"] = analysis.Settings.CheckApertures
+    settings.loc["VignettedPupil"] = analysis.Settings.VignettedPupil
+    settings.loc["UseDashes"] = analysis.Settings.UseDashes
+    settings.loc["Sagittal"] = str(analysis.Settings.Sagittal)
+    settings.loc["Tangential"] = str(analysis.Settings.Tangential)
+
+    # Create output
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+    )  # Set additional params
+
+    return analysis.complete(oncomplete, result)
```

### Comparing `zospy-0.6.2/zospy/analyses/reports.py` & `zospy-1.0.0/zospy/analyses/reports.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,561 +1,582 @@
+"""Zemax OpticStudio analyses from the Reports category."""
+
+from __future__ import annotations
+
 import os
 import re
 from tempfile import mkstemp
+from typing import Any
 
 import numpy as np
 import pandas as pd
 
-from zospy import utils
-from zospy.analyses.base import AnalysisResult, AttrDict
+from zospy.analyses.base import AnalysisResult, AttrDict, OnComplete, new_analysis
 from zospy.api import constants
+from zospy.zpcore import OpticStudioSystem
 
-REFLOAT = re.compile(r'^[-+]?(?:(?:\d*\.\d+)|(?:\d+\.?))(?:[Ee][+-]?\d+)?$')
-RECOMMASEP = re.compile(r'(?<=\d),(?=\d)')
+# TODO use value from zospy.api._config
+REFLOAT = re.compile(r"^[-+]?(?:(?:\d*\.\d+)|(?:\d+\.?))(?:[Ee][+-]?\d+)?$")
+RECOMMASEP = re.compile(r"(?<=\d),(?=\d)")
 
 
-def _structure_surface_data_result(line_list):
+def _structure_surface_data_result(line_list: list[str]) -> pd.Series:
     """Structures the result of a surface data analysis.
 
     Parameters
     ----------
     line_list: list of str
         The line list obtained by reading in the results
 
     Returns
     -------
     pd.Series
         The results structured in a Series
     """
     res = pd.Series(index=pd.MultiIndex([[]] * 2, [[]] * 2), dtype=object)
 
-    lm = pd.Series(index=['Thickness', 'Index of Refraction',
-                          'Best Fit Glass',
-                          'Surface Powers (as situated)',
-                          'Surface Powers (in air)',
-                          'Shape Factor'], dtype=int)
+    lm = pd.Series(
+        index=[
+            "Thickness",
+            "Index of Refraction",
+            "Best Fit Glass",
+            "Surface Powers (as situated)",
+            "Surface Powers (in air)",
+            "Shape Factor",
+        ],
+        data=[0] * 6,
+        dtype=int,
+    )
 
     for item in lm.index:
         for num, line in enumerate(line_list):
             if line.lstrip().startswith(item):
                 lm.loc[item] = num
                 break
 
-    general_lm = ['File', 'Title', 'Date', 'Comment', 'Lens units']
-    surface_lm = ['Thickness', 'Diameter', 'Y Edge Thick', 'X Edge Thick']
-    ri_lm = ['nd', 'Abbe', 'dPgF', 'Best Fit Glass']
+    general_lm = ["File", "Title", "Date", "Comment", "Lens units"]
+    surface_lm = ["Thickness", "Diameter", "Y Edge Thick", "X Edge Thick"]
+    ri_lm = ["nd", "Abbe", "dPgF", "Best Fit Glass"]
 
-    for line in line_list[:lm['Thickness']]:
+    for line in line_list[: lm["Thickness"]]:
         for item in general_lm:
             if line.lstrip().startswith(item):
-                val = line.split(':')[-1].strip()
+                val = line.split(":")[-1].strip()
 
-                fval = val.replace(',', '.')  # to enable conversion to float
+                fval = val.replace(",", ".")  # to enable conversion to float
                 if REFLOAT.match(fval):
                     val = float(fval)
 
-                res.loc['General', item] = val
+                res.loc["General", item] = val
 
-    for line in line_list[lm['Thickness']:lm['Index of Refraction']]:
+    for line in line_list[lm["Thickness"] : lm["Index of Refraction"]]:
         for item in surface_lm:
             if line.lstrip().startswith(item):
+                val = line.split(":")[-1].strip()
 
-                val = line.split(':')[-1].strip()
-
-                fval = val.replace(',', '.')  # to enable conversion to float
+                fval = val.replace(",", ".")  # to enable conversion to float
                 if REFLOAT.match(fval):
                     val = float(fval)
 
-                res.loc['Surface', item] = val
+                res.loc["Surface", item] = val
 
-    for line in line_list[lm['Index of Refraction']:lm['Best Fit Glass'] + 1]:  # + 1 as bfg should be included
+    for line in line_list[lm["Index of Refraction"] : lm["Best Fit Glass"] + 1]:  # + 1 as bfg should be included
         for item in ri_lm:
             if line.lstrip().startswith(item):
+                val = line.split(":")[-1].strip()
 
-                val = line.split(':')[-1].strip()
-
-                fval = val.replace(',', '.')  # to enable conversion to float
+                fval = val.replace(",", ".")  # to enable conversion to float
                 if REFLOAT.match(fval):
                     val = float(fval)
 
-                res.loc['IndexOfRefraction', item] = val
+                res.loc["IndexOfRefraction", item] = val
 
-    for line in line_list[lm['Best Fit Glass'] + 1:lm['Surface Powers (as situated)']]:  # + 1 as bfg should be excluded
-        if len(line.split('\t')) == 3:
-            _, wl, ri = line.split('\t')
-            fwl = wl.strip().replace(',', '.')
+    for line in line_list[
+        lm["Best Fit Glass"] + 1 : lm["Surface Powers (as situated)"]
+    ]:  # + 1 as bfg should be excluded
+        if len(line.split("\t")) == 3:
+            _, wl, ri = line.split("\t")
+            fwl = wl.strip().replace(",", ".")
             if REFLOAT.match(fwl):
                 wl = float(fwl)
             else:
                 continue  # is not an actual wavelength
 
-            ri = ri.strip().replace(',', '.')
+            ri = ri.strip().replace(",", ".")
             if REFLOAT.match(ri):
                 ri = float(ri)
 
-            res.loc['IndexOfRefractionPerWavelength', wl] = ri
+            res.loc["IndexOfRefractionPerWavelength", wl] = ri
 
-    for line in line_list[lm['Surface Powers (as situated)'] + 1:lm['Surface Powers (in air)']]:
-        if len(line.split(':')) == 2:
-            param, val = line.split(':')
-            param = re.sub(r' +', ' ', param).strip()
+    for line in line_list[lm["Surface Powers (as situated)"] + 1 : lm["Surface Powers (in air)"]]:
+        if len(line.split(":")) == 2:
+            param, val = line.split(":")
+            param = re.sub(r" +", " ", param).strip()
 
-            fval = val.strip().replace(',', '.')
+            fval = val.strip().replace(",", ".")
             if REFLOAT.match(fval):
                 val = float(fval)
 
-            res.loc['SurfacePowerAsSituated', param] = val
+            res.loc["SurfacePowerAsSituated", param] = val
 
-    for line in line_list[lm['Surface Powers (in air)'] + 1:lm['Shape Factor']]:
-        if len(line.split(':')) == 2:
-            param, val = line.split(':')
-            param = re.sub(r' +', ' ', param).strip()
+    for line in line_list[lm["Surface Powers (in air)"] + 1 : lm["Shape Factor"]]:
+        if len(line.split(":")) == 2:
+            param, val = line.split(":")
+            param = re.sub(r" +", " ", param).strip()
 
-            fval = val.strip().replace(',', '.')
+            fval = val.strip().replace(",", ".")
             if REFLOAT.match(fval):
                 val = float(fval)
 
-            res.loc['SurfacePowerInAir', param] = val
+            res.loc["SurfacePowerInAir", param] = val
 
-    for line in line_list[lm['Shape Factor']:]:
-        if len(line.split(':')) == 2:
-            param, val = line.split(':')
-            param = re.sub(r' +', ' ', param).strip()
+    for line in line_list[lm["Shape Factor"] :]:
+        if len(line.split(":")) == 2:
+            param, val = line.split(":")
+            param = re.sub(r" +", " ", param).strip()
 
             val = val.strip()
-            fval = val.replace(',', '.')
+            fval = val.replace(",", ".")
             if REFLOAT.match(fval):
                 val = float(fval)
 
-            res.loc['Other', param] = val
+            res.loc["Other", param] = val
 
     return res
 
 
-def surface_data(oss, surf, oncomplete='Close', cfgoutfile=None, txtoutfile=None):
+def surface_data(
+    oss: OpticStudioSystem,
+    surface: int,
+    oncomplete: OnComplete | str = OnComplete.Close,
+    cfgoutfile: str | None = None,
+    txtoutfile: str | None = None,
+) -> AnalysisResult:
     """Wrapper around the OpticStudio Surface Data Analysis.
 
     Due to limitations in the ZOS-API, the output is obtained by writing the OpticStudio results to a file and
     subsequently reading in this file
 
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
-    surf: int
+    surface: int
         The surface number that is to be analyzed
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
-    cfgoutfile: str or None
+    cfgoutfile: str | None
         The configuration file to which the current configuration is saved. If None, a temporary file will be created
         and deleted. If string, it should be a full system path with '.CFG' as extension, after which the file will be
         saved in that location. (Allowing usage of this configuration file using surface_data_fromcfg()). Defaults to
         None.
-    txtoutfile: str or None
+    txtoutfile: str | None
         The textfile to which the OpticStudio output is saved. If None, a temporary file will be created and deleted. If
         string, it should be a full system path with '.txt' as extension, after which the file will be saved in that
         location. Defaults to None.
 
     Returns
     -------
     AnalysisResult
         A SurfaceDataSettings analysis result. Next to the standard data, the raw text return obtained from the analysis
         will be present under 'RawTextData', the cfgoutfile under 'CfgOutFile', and the txtoutfile under 'TxtOutFile'.
     """
-
-    analysistype = 'SurfaceDataSettings'
+    analysis_type = constants.Analysis.AnalysisIDM.SurfaceDataSettings
 
     if cfgoutfile is None:
-        fd, cfgoutfile = mkstemp(suffix='.CFG', prefix='zospy_')
+        fd, cfgoutfile = mkstemp(suffix=".CFG", prefix="zospy_")
         os.close(fd)
         cleancfg = True
     else:
-        if not cfgoutfile.endswith('.CFG'):
+        if not cfgoutfile.endswith(".CFG"):
             raise ValueError('cfgfile should end with ".CFG"')
         cleancfg = False
 
     if txtoutfile is None:
-        fd, txtoutfile = mkstemp(suffix='.txt', prefix='zospy_')
+        fd, txtoutfile = mkstemp(suffix=".txt", prefix="zospy_")
         os.close(fd)
         cleantxt = True
     else:
-        if not txtoutfile.endswith('.txt'):
+        if not txtoutfile.endswith(".txt"):
             raise ValueError('txtfile should end with ".txt"')
         cleantxt = False
 
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysis_type)
 
     # Modify surface in the settings file
     an_sett = analysis.GetSettings()
     an_sett.SaveTo(cfgoutfile)
 
-    settingsbstr = b''.join(open(cfgoutfile, 'rb').readlines())
+    settingsbstr = b"".join(open(cfgoutfile, "rb").readlines())
     settingsbarr = bytearray(settingsbstr)
-    settingsbarr[20] = surf  # 20 maps to the selected surface
+    settingsbarr[20] = surface  # 20 maps to the selected surface
 
-    with open(cfgoutfile, 'wb') as bfile:
+    with open(cfgoutfile, "wb") as bfile:
         bfile.write(settingsbarr)
 
     an_sett.LoadFrom(cfgoutfile)
 
     # Run analysis
     analysis.ApplyAndWaitForCompletion()
 
     # Get results
     analysis.Results.GetTextFile(txtoutfile)
-    line_list = [line for line in open(txtoutfile, 'r', encoding='utf-16-le')]
+    line_list = [line for line in open(txtoutfile, "r", encoding="utf-16-le")]
     data = _structure_surface_data_result(line_list)
 
     # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Manually create settings as they cannot be accessed
-    settings = pd.Series(name='Settings')
-    settings.loc['Surface'] = surf
+    settings = pd.Series(name="Settings", dtype=object)
+    settings.loc["Surface"] = surface
 
     # Create output
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages,
-                         RawTextData=line_list, CgfOutFile=cfgoutfile, TxtOutFile=txtoutfile)  # Set additional params
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+        RawTextData=line_list,
+        CgfOutFile=cfgoutfile,
+        TxtOutFile=txtoutfile,
+    )  # Set additional params
 
     # cleanup if needed
     if cleancfg:
         os.remove(cfgoutfile)
     if cleantxt:
         os.remove(txtoutfile)
 
-    # Process oncomplete
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
-
-    return ret
+    return analysis.complete(oncomplete, result)
 
 
-def surface_data_fromcfg(oss, cfgfile, oncomplete='Close', txtoutfile=None):
+def surface_data_fromcfg(
+    oss: OpticStudioSystem, cfgfile: str, oncomplete: OnComplete | str = OnComplete.Close, txtoutfile: str | None = None
+) -> AnalysisResult:
     """Wrapper around the OpticStudio Surface Data Analysis that uses a predefined configuration file.
 
     Due to limitations in the ZOS-API, the output is obtained by writing the OpticStudio results to a file and
     subsequently reading in this file
 
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
     cfgfile: str
         The configuration file that is to be used. Should be a full system path with '.CFG' as extension.
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
-    txtoutfile: str or None
+    txtoutfile: str | None
         The textfile to which the Zemax output is saved. If None, a temporary file will be created and deleted. If
         string, it should be a full system path with '.txt' as extension, after which the file will be saved in that
         location. Defaults to None.
 
     Returns
     -------
     AnalysisResult
         A SurfaceDataSettings analysis result. Next to the standard data, the used cfgfile will be present under
         'UsedCfgFile', raw text return under 'RawTextData' and the txtoutfile under 'TxtOutFile'.
     """
+    analysis_type = constants.Analysis.AnalysisIDM.SurfaceDataSettings
 
-    analysistype = 'SurfaceDataSettings'
-
-    if not cfgfile.endswith('.CFG'):
+    if not cfgfile.endswith(".CFG"):
         raise ValueError('cfgfile should end with ".CFG"')
 
     if txtoutfile is None:
-        fd, txtoutfile = mkstemp(suffix='.txt', prefix='zospy_')
+        fd, txtoutfile = mkstemp(suffix=".txt", prefix="zospy_")
         os.close(fd)
         cleantxt = True
     else:
-        if not txtoutfile.endswith('.txt'):
+        if not txtoutfile.endswith(".txt"):
             raise ValueError('txtfile should end with ".txt"')
         cleantxt = False
 
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysis_type)
 
     # Load settings
     analysis.Settings.LoadFrom(cfgfile)
 
     # Run analysis
     analysis.ApplyAndWaitForCompletion()
 
     # Get results
     analysis.Results.GetTextFile(txtoutfile)
-    line_list = [line for line in open(txtoutfile, 'r', encoding='utf-16-le')]
+    line_list = [line for line in open(txtoutfile, "r", encoding="utf-16-le")]
     data = _structure_surface_data_result(line_list)
 
     # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Manually create settings as they cannot be accessed
-    settings = pd.Series(name='Settings')
+    # TODO replace by None
+    settings = pd.Series(name="Settings", dtype=object)
 
     # Create output
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages,
-                         UsedCfgFile=cfgfile, RawTextData=line_list, TxtOutFile=txtoutfile)  # Set additional params
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+        UsedCfgFile=cfgfile,
+        RawTextData=line_list,
+        TxtOutFile=txtoutfile,
+    )  # Set additional params
 
     # cleanup
     if cleantxt:
         os.remove(txtoutfile)
 
-    # Process oncomplete
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
+    return analysis.complete(oncomplete, result)
 
-    return ret
 
-
-def _structure_system_data_result(line_list):
+def _structure_system_data_result(line_list: list[str]) -> dict[str, Any]:
     """Structures the result of a system data report.
 
     Parameters
     ----------
-    line_list: list of str
+    line_list: list[str]
         The line list obtained by reading in the results
 
     Returns
     -------
     dict
         The results structured in a dictionary
     """
     # Create output dict
     res = AttrDict()
 
     # Add header
-    hdr = line_list[0].strip().replace('\ufeff', '')
-    res['Header'] = hdr
+    hdr = line_list[0].strip().replace("\ufeff", "")
+    res["Header"] = hdr
 
     # Register landmarks
-    landmarks = ['GENERAL LENS DATA', 'Fields', 'Vignetting Factors', 'Wavelengths', 'Predicted coordinate ABCD matrix']
+    landmarks = ["GENERAL LENS DATA", "Fields", "Vignetting Factors", "Wavelengths", "Predicted coordinate ABCD matrix"]
     comp = re.compile(rf'^({"|".join(landmarks)})', re.IGNORECASE)
-    inds = {comp.match(line).group().lower(): {'rnum': rnum, 'name': comp.match(line).group()}
-            for rnum, line in enumerate(line_list) if comp.match(line)}
+    inds = {
+        comp.match(line).group().lower(): {"rnum": rnum, "name": comp.match(line).group()}
+        for rnum, line in enumerate(line_list)
+        if comp.match(line)
+    }
 
-    order_of_appearance = [item[0] for item in sorted(inds.items(), key=lambda x: x[1]['rnum'])]
+    order_of_appearance = [item[0] for item in sorted(inds.items(), key=lambda x: x[1]["rnum"])]
 
     # Add general lens data
-    target = 'general lens data'
+    target = "general lens data"
     gld = pd.Series(dtype=object)
     if target in inds:
-        section_start = inds[target]['rnum'] + 1  # + 1 to ignore section title
+        section_start = inds[target]["rnum"] + 1  # + 1 to ignore section title
 
         # Get endpoint
         if order_of_appearance.index(target) == len(inds) - 1:
             section_end = len(line_list)
         else:
             target2 = order_of_appearance[order_of_appearance.index(target) + 1]
-            section_end = inds[target2]['rnum']
+            section_end = inds[target2]["rnum"]
 
         for line in line_list[section_start:section_end]:
-            if line.strip() == '':
+            if line.strip() == "":
                 continue
 
             # Get param and value, strip whitespaces
-            param, val = line.split(':')
-            param = re.sub(r'\s+', ' ', param).strip()
+            param, val = line.split(":")
+            param = re.sub(r"\s+", " ", param).strip()
 
             # convert value to float if needed
-            val = re.sub(r'\s+', ' ', val).strip()
-            val = RECOMMASEP.sub('.', val)
+            val = re.sub(r"\s+", " ", val).strip()
+            val = RECOMMASEP.sub(".", val)
             if REFLOAT.match(val):
-                if '.' in val:
+                if "." in val or "e" in val:
                     val = float(val)
                 else:
                     val = int(val)
 
             # add
             ii = 0
             while param in gld.index:
                 ii += 1
-                param = f'{param} {ii}'
+                param = f"{param} {ii}"
             gld.loc[param] = val
-    res['GeneralLensData'] = gld
+    res["GeneralLensData"] = gld
 
     # Fields, Wavelengths
-    for target in ['fields', 'wavelengths']:
+    for target in ["fields", "wavelengths"]:
         info = pd.Series(dtype=object)
         data = pd.DataFrame()
         if target in inds:
-            section_start = inds[target]['rnum']
+            section_start = inds[target]["rnum"]
 
             # Get endpoint
             if order_of_appearance.index(target) == len(inds) - 1:
                 section_end = len(line_list)
             else:
                 target2 = order_of_appearance[order_of_appearance.index(target) + 1]
-                section_end = inds[target2]['rnum']
+                section_end = inds[target2]["rnum"]
 
             for ii, line in enumerate(line_list[section_start:section_end]):
-                if line.strip().startswith('#'):
+                if line.strip().startswith("#"):
                     ht_loc = section_start + ii
                     break
             else:
                 ht_loc = None
 
             param_end = ht_loc if ht_loc is not None else section_end
             for line in line_list[section_start:param_end]:
-                if line.strip() == '':
+                if line.strip() == "":
                     continue
 
                 # Get param and value, strip whitespaces
-                param, val = line.split(':')
-                param = re.sub(r'\s+', ' ', param).strip()
+                param, val = line.split(":")
+                param = re.sub(r"\s+", " ", param).strip()
 
                 # convert value to float if needed
-                val = re.sub(r'\s+', ' ', val).strip()
-                val = RECOMMASEP.sub('.', val)
+                val = re.sub(r"\s+", " ", val).strip()
+                val = RECOMMASEP.sub(".", val)
                 if REFLOAT.match(val):
-                    if '.' in val:
+                    if "." in val:
                         val = float(val)
                     else:
                         val = int(val)
 
                 # add
                 ii = 0
                 while param in gld.index:
                     ii += 1
-                    param = f'{param} {ii}'
+                    param = f"{param} {ii}"
                 info.loc[param] = val
 
             if ht_loc is not None:
-                columns = re.sub(r'\s+', ' ', line_list[ht_loc]).strip().split(' ')
+                columns = re.sub(r"\s+", " ", line_list[ht_loc]).strip().split(" ")
                 data = []
-                for ii in range(ht_loc+1, section_end):
-                    if line_list[ii].strip() == '':
+                for ii in range(ht_loc + 1, section_end):
+                    if line_list[ii].strip() == "":
                         continue
-                    items = re.sub(r'\s+', ' ', line_list[ii]).strip().split(' ')
+                    items = re.sub(r"\s+", " ", line_list[ii]).strip().split(" ")
                     values = []
                     for item in items:
-                        val = RECOMMASEP.sub('.', item)
+                        val = RECOMMASEP.sub(".", item)
                         if REFLOAT.match(val):
-                            if '.' in val:
+                            if "." in val:
                                 val = float(val)
                             else:
                                 val = int(val)
                         values.append(val)
                     data.append(values)
                 data = pd.DataFrame(columns=columns, data=data)
-            res[inds[target]['name']] = AttrDict(Info=info, Data=data)
+            res[inds[target]["name"]] = AttrDict(Info=info, Data=data)
 
     # Vignetting factors
-    target = 'vignetting factors'
+    target = "vignetting factors"
     if target in inds:
-        section_start = inds[target]['rnum'] + 1  # + 1 to ignore section title
+        section_start = inds[target]["rnum"] + 1  # + 1 to ignore section title
 
         # Get endpoint
         if order_of_appearance.index(target) == len(inds) - 1:
             section_end = len(line_list)
         else:
             target2 = order_of_appearance[order_of_appearance.index(target) + 1]
-            section_end = inds[target2]['rnum']
+            section_end = inds[target2]["rnum"]
 
         for ii, line in enumerate(line_list[section_start:section_end]):
-            if line.strip().startswith('#'):
+            if line.strip().startswith("#"):
                 ht_loc = section_start + ii
                 break
         else:
             ht_loc = None
 
         if ht_loc is not None:
-            columns = re.sub(r'\s+', ' ', line_list[ht_loc]).strip().split(' ')
+            columns = re.sub(r"\s+", " ", line_list[ht_loc]).strip().split(" ")
             data = []
-            for ii in range(ht_loc+1, section_end):
-                if line_list[ii].strip() == '':
+            for ii in range(ht_loc + 1, section_end):
+                if line_list[ii].strip() == "":
                     continue
-                items = re.sub(r'\s+', ' ', line_list[ii]).strip().split(' ')
+                items = re.sub(r"\s+", " ", line_list[ii]).strip().split(" ")
                 values = []
                 for item in items:
-                    val = RECOMMASEP.sub('.', item)
+                    val = RECOMMASEP.sub(".", item)
                     if REFLOAT.match(val):
-                        if '.' in val:
+                        if "." in val:
                             val = float(val)
                         else:
                             val = int(val)
                     values.append(val)
                 data.append(values)
             data = pd.DataFrame(columns=columns, data=data)
-        res['VignettingFactors'] = data
+        res["VignettingFactors"] = data
 
     # Predicted ABCD matrix
-    target = 'predicted coordinate abcd matrix'
+    target = "predicted coordinate abcd matrix"
     abcd = pd.Series(dtype=object)
     if target in inds:
-        section_start = inds[target]['rnum'] + 1  # + 1 to ignore section title
+        section_start = inds[target]["rnum"] + 1  # + 1 to ignore section title
 
         # Get endpoint
         if order_of_appearance.index(target) == len(inds) - 1:
             section_end = len(line_list)
         else:
             target2 = order_of_appearance[order_of_appearance.index(target) + 1]
-            section_end = inds[target2]['rnum']
+            section_end = inds[target2]["rnum"]
 
         for line in line_list[section_start:section_end]:
-            if line.strip() == '':
+            if line.strip() == "":
                 continue
 
             # Get param and value, strip whitespaces
-            param, val = line.split('=')
-            param = re.sub(r'\s+', ' ', param).strip()
+            param, val = line.split("=")
+            param = re.sub(r"\s+", " ", param).strip()
 
             # convert value to float if needed
-            val = re.sub(r'\s+', ' ', val).strip()
-            val = RECOMMASEP.sub('.', val)
+            val = re.sub(r"\s+", " ", val).strip()
+            val = RECOMMASEP.sub(".", val)
             if REFLOAT.match(val):
-                if '.' in val:
+                if "." in val:
                     val = float(val)
                 else:
                     val = int(val)
 
             # add
             ii = 0
             while param in gld.index:
                 ii += 1
-                param = f'{param} {ii}'
+                param = f"{param} {ii}"
             abcd.loc[param] = val
-        res['PredictedCoordinateABCDMatrix'] = abcd
+        res["PredictedCoordinateABCDMatrix"] = abcd
 
         return res
 
 
-def system_data(oss, oncomplete='Close', txtoutfile=None):
+def system_data(
+    oss: OpticStudioSystem, oncomplete: OnComplete | str = OnComplete.Close, txtoutfile: str | None = None
+) -> AnalysisResult:
     """Wrapper around the OpticStudio System Data Analysis.
 
     Due to limitations in the ZOS-API, the output is obtained by writing the OpticStudio results to a file and
     subsequently reading in this file
 
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
     txtoutfile: str or None
         The textfile to which the OpticStudio output is saved. If None, a temporary file will be created and deleted. If
@@ -564,354 +585,366 @@
 
     Returns
     -------
     AnalysisResult
         A SystemData analysis result. Next to the standard data, the raw text return obtained from the analysis
         will be present under 'RawTextData', the cfgoutfile under 'CfgOutFile', and the txtoutfile under 'TxtOutFile'.
     """
-
-    analysistype = 'SystemData'
+    analysis_type = constants.Analysis.AnalysisIDM.SystemData
 
     if txtoutfile is None:
-        fd, txtoutfile = mkstemp(suffix='.txt', prefix='zospy_')
+        fd, txtoutfile = mkstemp(suffix=".txt", prefix="zospy_")
         os.close(fd)
         cleantxt = True
     else:
-        if not txtoutfile.endswith('.txt'):
+        if not txtoutfile.endswith(".txt"):
             raise ValueError('txtfile should end with ".txt"')
         cleantxt = False
 
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysis_type)
 
     # Run analysis
     analysis.ApplyAndWaitForCompletion()
 
     # Get results
     analysis.Results.GetTextFile(txtoutfile)
-    line_list = [line for line in open(txtoutfile, 'r', encoding='utf-16-le')]
+    line_list = [line for line in open(txtoutfile, "r", encoding="utf-16-le")]
     data = _structure_system_data_result(line_list)
 
     # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Create output
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=None, metadata=metadata,
-                         headerdata=headerdata, messages=messages,
-                         RawTextData=line_list, TxtOutFile=txtoutfile)  # Set additional params
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=None,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+        RawTextData=line_list,
+        TxtOutFile=txtoutfile,
+    )  # Set additional params
 
     # cleanup if needed
     if cleantxt:
         os.remove(txtoutfile)
 
-    # Process oncomplete
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
-
-    return ret
+    return analysis.complete(oncomplete, result)
 
 
-def _structure_cardinal_point_result(line_list):
+def _structure_cardinal_point_result(line_list: list[str]) -> pd.Series:
     """Structures the result of a cardinal point analysis.
 
     Parameters
     ----------
-    line_list: list of str
+    line_list: list[str]
         The line list obtained by reading in the results
 
     Returns
     -------
     pd.Series
         The results structured in a Series
     """
     res = pd.Series(index=pd.MultiIndex([[]] * 2, [[]] * 2), dtype=object)
 
     # Determine landmarks
-    idx = ['Starting surface',
-           'Ending surface',
-           'Object space positions',
-           'Focal Length',
-           'Anti-Nodal Planes',
-           'Error computing cardinal points']
-    lm = pd.Series(index=idx, data=[pd.NA]*len(idx), dtype=object)
+    idx = [
+        "Starting surface",
+        "Ending surface",
+        "Object space positions",
+        "Focal Length",
+        "Anti-Nodal Planes",
+        "Error computing cardinal points",
+    ]
+    lm = pd.Series(index=idx, data=[pd.NA] * len(idx), dtype=object)
 
     for item in lm.index:
         for num, line in enumerate(line_list):
             if line.lstrip().startswith(item):
                 lm.loc[item] = num
                 break
 
-    general_lm = ['File', 'Title', 'Date', 'Wavelength', 'Orientation', 'Lens units']
-    surface_lm = ['Starting surface', 'Ending surface']
-    carpoints_lm = ['Focal Length', 'Focal Planes', 'Principal Planes', 'Anti-Principal Planes',
-                    'Nodal Planes', 'Anti-Nodal Planes']
+    general_lm = ["File", "Title", "Date", "Wavelength", "Orientation", "Lens units"]
+    surface_lm = ["Starting surface", "Ending surface"]
+    carpoints_lm = [
+        "Focal Length",
+        "Focal Planes",
+        "Principal Planes",
+        "Anti-Principal Planes",
+        "Nodal Planes",
+        "Anti-Nodal Planes",
+    ]
 
     # Get general info
-    for line in line_list[:lm['Object space positions']]:
+    for line in line_list[: lm["Object space positions"]]:
         for item in general_lm:
             if line.lstrip().startswith(item):
-                val = line.split(':')[-1].strip()
+                val = line.split(":")[-1].strip()
 
-                fval = val.replace(',', '.')  # to enable conversion to float
+                fval = val.replace(",", ".")  # to enable conversion to float
                 if REFLOAT.match(fval):
                     val = float(fval)
 
-                res.loc['General', item] = val
+                res.loc["General", item] = val
 
-    space1 = space2 = 'Space'
-    for option in ['Focal Length', 'Error computing cardinal points']:
+    space1 = space2 = "Space"
+    for option in ["Focal Length", "Error computing cardinal points"]:
         try:
-            res.loc['General', 'Info'] = '\n'.join([item.strip() for item in
-                                                    line_list[lm['Object space positions']:lm[option]-1]
-                                                    if item.strip() != ''])
-            _, space1, space2 = line_list[lm[option] - 1].split('\t')
+            res.loc["General", "Info"] = "\n".join(
+                [
+                    item.strip()
+                    for item in line_list[lm["Object space positions"] : lm[option] - 1]
+                    if item.strip() != ""
+                ]
+            )
+            _, space1, space2 = line_list[lm[option] - 1].split("\t")
             space1 = space1.strip()
             space2 = space2.strip()
 
             break
         except TypeError:
             continue
     else:
-        res.loc['General', 'Info'] = 'ZOSPy: Cannot determine spaces'
+        res.loc["General", "Info"] = "ZOSPy: Cannot determine spaces"
 
-    for line in line_list[lm['Starting surface']:lm['Ending surface'] + 1]:
+    for line in line_list[lm["Starting surface"] : lm["Ending surface"] + 1]:
         for item in surface_lm:
             if line.lstrip().startswith(item):
-                val = line.split(':')[-1].strip()
+                val = line.split(":")[-1].strip()
 
-                fval = val.replace(',', '.')  # to enable conversion to float
+                fval = val.replace(",", ".")  # to enable conversion to float
                 if REFLOAT.match(fval):
                     val = float(fval)
 
-                res.loc['Surface', item] = val
+                res.loc["Surface", item] = val
 
     try:
-        for line in line_list[lm['Focal Length']:lm['Anti-Nodal Planes'] + 1]:
+        for line in line_list[lm["Focal Length"] : lm["Anti-Nodal Planes"] + 1]:
             for item in carpoints_lm:
                 if line.lstrip().startswith(item):
-                    val1, val2 = line.split(':')[-1].strip().split('\t')
+                    val1, val2 = line.split(":")[-1].strip().split("\t")
                     val1 = val1.strip()
                     val2 = val2.strip()
 
-                    fval1 = val1.replace(',', '.')  # to enable conversion to float
+                    fval1 = val1.replace(",", ".")  # to enable conversion to float
                     if REFLOAT.match(fval1):
                         val1 = float(fval1)
 
-                    fval2 = val2.replace(',', '.')  # to enable conversion to float
+                    fval2 = val2.replace(",", ".")  # to enable conversion to float
                     if REFLOAT.match(fval2):
                         val2 = float(fval2)
 
                     res.loc[space1, item] = val1
                     res.loc[space2, item] = val2
     except TypeError:
         for item in carpoints_lm:
             res.loc[space1, item] = np.nan
             res.loc[space2, item] = np.nan
     res = res.loc[res.index.get_level_values(0).unique()]
 
     return res
 
 
-def cardinal_points(oss, surf1, surf2, oncomplete='Close', cfgoutfile=None, txtoutfile=None):
+def cardinal_points(
+    oss: OpticStudioSystem,
+    surface_1: int,
+    surface_2: int,
+    oncomplete: OnComplete | str = OnComplete.Close,
+    cfgoutfile: str | None = None,
+    txtoutfile: str | None = None,
+) -> AnalysisResult:
     """Wrapper around the OpticStudio Cardinal Point Analysis.
 
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
-    surf1: int
+    surface_1: int
         The surface number corresponding to the first surface of the analyzed system
-    surf2: int
+    surface_2: int
         The surface number corresponding to the last surface of the analyzed system
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
-    cfgoutfile: str or None
+    cfgoutfile: str | None
         The configuration file to which the current configuration is saved. If None, a temporary file will be created
         and deleted. If string, it should be a full system path with '.CFG' as extension, after which the file will be
         saved in that location. (Allowing usage of this configuration file using surface_data_fromcfg()). Defaults to
         None.
-    txtoutfile: str or None
+    txtoutfile: str | None
         The textfile to which the OpticStudio output is saved. If None, a temporary file will be created and deleted. If
         string, it should be a full system path with '.txt' as extension, after which the file will be saved in that
         location. Defaults to None.
 
     Returns
     -------
     AnalysisResult
         A SurfaceDataSettings analysis result. Next to the standard data, the raw text return obtained from the analysis
         will be present under 'RawTextData', the cfgoutfile under 'CfgOutFile', and the txtoutfile under 'TxtOutFile'.
     """
+    analysis_type = constants.Analysis.AnalysisIDM.CardinalPoints
 
-    analysistype = 'CardinalPoints'
-
-    if surf1 > surf2:
-        raise ValueError('Surface 1 cannot be higher than Surface 2')
+    if surface_1 > surface_2:
+        raise ValueError("Surface 1 cannot be higher than Surface 2")
 
     if cfgoutfile is None:
-        fd, cfgoutfile = mkstemp(suffix='.CFG', prefix='zospy_')
+        fd, cfgoutfile = mkstemp(suffix=".CFG", prefix="zospy_")
         os.close(fd)
         cleancfg = True
     else:
-        if not cfgoutfile.endswith('.CFG'):
+        if not cfgoutfile.endswith(".CFG"):
             raise ValueError('cfgoutfile should end with ".CFG"')
         cleancfg = False
 
     if txtoutfile is None:
-        fd, txtoutfile = mkstemp(suffix='.txt', prefix='zospy_')
+        fd, txtoutfile = mkstemp(suffix=".txt", prefix="zospy_")
         os.close(fd)
         cleantxt = True
     else:
-        if not txtoutfile.endswith('.txt'):
+        if not txtoutfile.endswith(".txt"):
             raise ValueError('txtoutfile should end with ".txt"')
         cleantxt = False
 
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysis_type)
 
     # Modify surface in the settings file
-    an_sett = analysis.GetSettings()
-    an_sett.SaveTo(cfgoutfile)
+    analysis_settings = analysis.Settings
+    analysis_settings.SaveTo(cfgoutfile)
 
-    settingsbstr = b''.join(open(cfgoutfile, 'rb').readlines())
+    settingsbstr = b"".join(open(cfgoutfile, "rb").readlines())
     settingsbarr = bytearray(settingsbstr)
-    settingsbarr[20] = surf1  # byte 20 maps to the first surface
-    settingsbarr[24] = surf2  # byte 24 maps to the first surface
+    settingsbarr[20] = surface_1  # byte 20 maps to the first surface
+    settingsbarr[24] = surface_2  # byte 24 maps to the first surface
 
-    with open(cfgoutfile, 'wb') as bfile:
+    with open(cfgoutfile, "wb") as bfile:
         bfile.write(settingsbarr)
 
-    an_sett.LoadFrom(cfgoutfile)
+    analysis_settings.LoadFrom(cfgoutfile)
 
     # Run analysis
     analysis.ApplyAndWaitForCompletion()
 
     # Get results
     analysis.Results.GetTextFile(txtoutfile)
-    line_list = [line for line in open(txtoutfile, 'r', encoding='utf-16-le')]
+    line_list = [line for line in open(txtoutfile, "r", encoding="utf-16-le")]
     data = _structure_cardinal_point_result(line_list)
 
     # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Manually create settings as they cannot be accessed
-    settings = pd.Series(name='Settings')
-    settings.loc['Surface1'] = surf1
-    settings.loc['Surface2'] = surf2
+    settings = pd.Series(name="Settings", dtype=object)
+    settings.loc["Surface1"] = surface_1
+    settings.loc["Surface2"] = surface_2
 
     # Create output
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages,
-                         RawTextData=line_list, CgfOutFile=cfgoutfile, TxtOutFile=txtoutfile)  # Set additional params
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+        RawTextData=line_list,
+        CgfOutFile=cfgoutfile,
+        TxtOutFile=txtoutfile,
+    )  # Set additional params
 
     # cleanup if needed
     if cleancfg:
         os.remove(cfgoutfile)
     if cleantxt:
         os.remove(txtoutfile)
 
-    # Process oncomplete
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
-
-    return ret
+    return analysis.complete(oncomplete, result)
 
 
-def cardinal_points_fromcfg(oss, cfgfile, oncomplete='Close', txtoutfile=None):
+def cardinal_points_fromcfg(
+    oss: OpticStudioSystem, cfgfile: str, oncomplete: OnComplete | str = OnComplete.Close, txtoutfile: str | None = None
+) -> AnalysisResult:
     """Wrapper around the OpticStudio Cardinal Point Analysis that uses a predefined configuration file.
 
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
     cfgfile: str
         The configuration file that is to be used. Should be a full system path with '.CFG' as extension.
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
-    txtoutfile: str or None
+    txtoutfile: str | None
         The textfile to which the OpticStudio output is saved. If None, a temporary file will be created and deleted. If
         string, it should be a full system path with '.txt' as extension, after which the file will be saved in that
         location. Defaults to None.
 
     Returns
     -------
     AnalysisResult
         A SurfaceDataSettings analysis result. Next to the standard data, the used cfgfile will be present under
         'UsedCfgFile', raw text return under 'RawTextData' and the txtoutfile under 'TxtOutFile'.
     """
+    analysis_type = constants.Analysis.AnalysisIDM.CardinalPoints
 
-    analysistype = 'CardinalPoints'
-
-    if not cfgfile.endswith('.CFG'):
+    if not cfgfile.endswith(".CFG"):
         raise ValueError('cfgfile should end with ".CFG"')
 
     if txtoutfile is None:
-        fd, txtoutfile = mkstemp(suffix='.txt', prefix='zospy_')
+        fd, txtoutfile = mkstemp(suffix=".txt", prefix="zospy_")
         os.close(fd)
         cleantxt = True
     else:
-        if not txtoutfile.endswith('.txt'):
+        if not txtoutfile.endswith(".txt"):
             raise ValueError('txtfile should end with ".txt"')
         cleantxt = False
 
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysis_type)
 
     # Load the settings file
     analysis.Settings.LoadFrom(cfgfile)
 
     # Run analysis
     analysis.ApplyAndWaitForCompletion()
 
     # Get results
     analysis.Results.GetTextFile(txtoutfile)
-    line_list = [line for line in open(txtoutfile, 'r', encoding='utf-16-le')]
+    line_list = [line for line in open(txtoutfile, "r", encoding="utf-16-le")]
     data = _structure_cardinal_point_result(line_list)
 
     # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Manually create settings as they cannot be accessed
-    settings = pd.Series(name='Settings')
+    # TODO replace by None
+    settings = pd.Series(name="Settings", dtype=object)
 
     # Create output
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages,
-                         UsedCfgFile=cfgfile, RawTextData=line_list, TxtOutFile=txtoutfile)  # Set additional params
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+        UsedCfgFile=cfgfile,
+        RawTextData=line_list,
+        TxtOutFile=txtoutfile,
+    )  # Set additional params
 
     # cleanup if needed
     if cleantxt:
         os.remove(txtoutfile)
 
-    # Process oncomplete
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
-
-    return ret
+    return analysis.complete(oncomplete, result)
```

### Comparing `zospy-0.6.2/zospy/analyses/surface.py` & `zospy-1.0.0/zospy/analyses/surface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,142 +1,147 @@
+"""Zemax OpticStudio analyses from the Surface category."""
+
+from __future__ import annotations
+
 import pandas as pd
 
-from zospy.analyses.base import AnalysisResult, AttrDict
+from zospy.analyses.base import AnalysisResult, AttrDict, OnComplete, new_analysis
 from zospy.api import constants
 from zospy.utils import zputils
+from zospy.zpcore import OpticStudioSystem
 
 
-def curvature(oss, sampling='65x65', data='TangentialCurvature', remove='None', surface=1, showas='Contour',
-              offaxiscoordinates=False, contourformat='', bfs_criterion='MinimumVolume', bfs_reversedirection=False,
-              oncomplete='Close'):
-    """
-    
+def curvature(
+    oss: OpticStudioSystem,
+    sampling: str = "65x65",
+    data: constants.Analysis.SurfaceCurvatureData | str = "TangentialCurvature",
+    remove: constants.Analysis.RemoveOptions | str | None = "None_",
+    surface: int = 1,
+    showas: constants.Analysis.ShowAs | str = "Contour",
+    offaxiscoordinates: bool = False,
+    contourformat: str = "",
+    bfs_criterion: constants.Analysis.BestFitSphereOptions | str = "MinimumVolume",
+    bfs_reversedirection: bool = False,
+    oncomplete: OnComplete | str = OnComplete.Close,
+) -> AnalysisResult:
+    """Wrapper around the OpticStudio Curvature analysis.
+
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
-    sampling: str or int
+    sampling: str | int
         The size of the used grid, either string (e.g. '65x65') or int. The integer will be treated as if obtained from
         zospy.constants.Analysis.SampleSizes_Pow2Plus1_X. Defaults to '65x65'.
-    data: str or int
-        The used data type. Should be one of ['TangentialCurvature', 'SagitalCurvature', 'X_Curvature', 'Y_Curvature'] 
-        or int. The integer will be treated as if obtained from zospy.constants.Analysis.SurfaceCurvatureData. Defaults 
+    data: str
+        The used data type. Should be one of ['TangentialCurvature', 'SagittalCurvature', 'X_Curvature', 'Y_Curvature']
+        or int. The integer will be treated as if obtained from zospy.constants.Analysis.SurfaceCurvatureData. Defaults
         to 'TangentialCurvature'.
-    remove: str or int
-        Defines whether a reference volume is removed or not. Should be one of ['None', 'BaseROC', 'BestFitSphere'] or 
-        int. The integer will be treated as if obtained from zospy.constants.Analysis.RemoveOptions. Defaults 
+    remove: str | int
+        Defines whether a reference volume is removed or not. Should be one of ['None', 'BaseROC', 'BestFitSphere'] or
+        int. The integer will be treated as if obtained from zospy.constants.Analysis.RemoveOptions. Defaults
         to 'None'.
     surface: int
         The surface that is te be analyzed. defaults to 1.
-    showas: str or int
-        Defines how the data is displayed in OpticStudio. Should be one of ['Surface', 'Contour', 'GreyScale', 
-        'InverseGreyScale', 'FalseColor', 'InverseFalseColor'] or int. The integer will be treated as if obtained from 
+    showas: str | int
+        Defines how the data is displayed in OpticStudio. Should be one of ['Surface', 'Contour', 'GreyScale',
+        'InverseGreyScale', 'FalseColor', 'InverseFalseColor'] or int. The integer will be treated as if obtained from
         zospyconstants.Analysis.ShowAs. Defaults to 'Contour'.
     offaxiscoordinates: bool
-        Defines whether apertures defined in the Surface Properties of the surface are considered or not. Defaults to 
+        Defines whether apertures defined in the Surface Properties of the surface are considered or not. Defaults to
         False.
-
     contourformat: str
         The contour format. Only usable when showas == 'Contour'. Defaults to ''.
-    
-    bfs_criterion: str or int
+    bfs_criterion: str | int
         The criterion for BFS removal. Only usable when remove == 'BestFitSphere'. Should be one of ['MinimumVolume',
         'MinimumRMS', 'MinimumRMSWithOffset'] or int. The integer will be treated as if obtained from
         constants.Analysis.BestFitSphereOptions. Defaults to 'MinimumVolume'.
     bfs_reversedirection: bool
         Defines if the sign of the BFS radius should be reversed or not. Only usable when remove == 'BestFitSphere'
         and bfs_criterion == 'MinimumVolume'. Defaults to False.
-
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
 
     Returns
     -------
     AnalysisResult
         A SurfaceCurvature analysis result
     """
-    analysistype = 'SurfaceCurvature'
+    analysis_type = constants.Analysis.AnalysisIDM.SurfaceCurvature
 
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysis_type)
 
     # Apply settings
-    analysis.Settings.Sampling = zputils.proc_constant(constants.Analysis.SampleSizes_Pow2Plus1_X,
-                                                       zputils.standardize_sampling(sampling))
-    analysis.Settings.Data = zputils.proc_constant(constants.Analysis.SurfaceCurvatureData, data)
-    analysis.Settings.RemoveOption = zputils.proc_constant(constants.Analysis.RemoveOptions, remove)
-    zputils.analysis_set_surface(analysis, surface)
-    analysis.Settings.ShowAs = zputils.proc_constant(constants.Analysis.ShowAs, showas)
+    analysis.Settings.Sampling = getattr(
+        constants.Analysis.SampleSizes_Pow2Plus1_X, zputils.standardize_sampling(sampling)
+    )
+    analysis.Settings.Data = constants.process_constant(constants.Analysis.SurfaceCurvatureData, data)
+    analysis.Settings.RemoveOption = constants.process_constant(constants.Analysis.RemoveOptions, remove)
+    analysis.set_surface(surface)
+    analysis.Settings.ShowAs = constants.process_constant(constants.Analysis.ShowAs, showas)
 
     analysis.Settings.ConsiderOffAxisAperture = offaxiscoordinates
     if analysis.Settings.ShowAs == constants.Analysis.ShowAs.Contour:  # ContourFormat becomes available
         analysis.Settings.ContourFormat = contourformat
 
     if analysis.Settings.RemoveOption == constants.Analysis.RemoveOptions.BestFitSphere:  # Add Best fit sphere options
-        analysis.Settings.BestFitSphereOptions = zputils.proc_constant(constants.Analysis.BestFitSphereOptions,
-                                                                       bfs_criterion)
+        analysis.Settings.BestFitSphereOption = constants.process_constant(
+            constants.Analysis.BestFitSphereOptions, bfs_criterion
+        )
 
-        if analysis.Settings.BestFitSphereOptions == constants.Analysis.BestFitSphereOptions.MinimumVolume:
+        if analysis.Settings.BestFitSphereOption == constants.Analysis.BestFitSphereOptions.MinimumVolume:
             # Reversed direction becomes available
             analysis.Settings.ReverseDirection = bfs_reversedirection
 
     # Calculate
     analysis.ApplyAndWaitForCompletion()
 
     # Get headerdata, metadata and messages
-    headerdata = zputils.analysis_get_headerdata(analysis)
-    metadata = zputils.analysis_get_metadata(analysis)
-    messages = zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Get settings
-    settings = pd.Series(name='Settings')
+    settings = pd.Series(name="Settings", dtype=object)
 
-    settings.loc['Sampling'] = constants.get_constantname_by_value(constants.Analysis.SampleSizes_Pow2Plus1_X,
-                                                                   analysis.Settings.Sampling)
-    settings.loc['Data'] = constants.get_constantname_by_value(constants.Analysis.SurfaceCurvatureData,
-                                                               analysis.Settings.Data)
-    settings.loc['RemoveOption'] = constants.get_constantname_by_value(constants.Analysis.RemoveOptions,
-                                                                       analysis.Settings.RemoveOption)
-    settings.loc['Surface'] = analysis.Settings.Surface.GetSurfaceNumber()
-    settings.loc['ShowAs'] = constants.get_constantname_by_value(constants.Analysis.ShowAs,
-                                                                 analysis.Settings.ShowAs)
-    settings.loc['ConsiderOffAxisAperture'] = analysis.Settings.ConsiderOffAxisAperture
+    settings.loc["Sampling"] = str(analysis.Settings.Sampling)
+    settings.loc["Data"] = str(analysis.Settings.Data)
+    settings.loc["RemoveOption"] = str(analysis.Settings.RemoveOption)
+    settings.loc["Surface"] = analysis.Settings.Surface.GetSurfaceNumber()
+    settings.loc["ShowAs"] = str(analysis.Settings.ShowAs)
+    settings.loc["ConsiderOffAxisAperture"] = analysis.Settings.ConsiderOffAxisAperture
 
     if analysis.Settings.ShowAs == constants.Analysis.ShowAs.Contour:  # ContourFormat is available
-        settings.loc['Contourformat'] = analysis.Settings.ContourFormat
+        settings.loc["Contourformat"] = str(analysis.Settings.ContourFormat)
 
     if analysis.Settings.RemoveOption == constants.Analysis.RemoveOptions.BestFitSphere:  # Add Best fit sphere options
-        settings.loc['BestFitSphereOptions'] = \
-            constants.get_constantname_by_value(constants.Analysis.BestFitSphereOptions,
-                                                analysis.Settings.BestFitSphereOptions)
-        if analysis.Settings.BestFitSphereOptions == constants.Analysis.BestFitSphereOptions.MinimumVolume:
+        settings.loc["BestFitSphereOptions"] = str(analysis.Settings.BestFitSphereOption)
+        if analysis.Settings.BestFitSphereOption == constants.Analysis.BestFitSphereOptions.MinimumVolume:
             # Reversed direction is available
-            settings.loc['ReverseDirection'] = analysis.Settings.ReverseDirection
+            settings.loc["ReverseDirection"] = analysis.Settings.ReverseDirection
 
     # Get data
     if analysis.Results.NumberOfDataGrids <= 0:
         data = None
     elif analysis.Results.NumberOfDataGrids == 1:
         data = zputils.unpack_datagrid(analysis.Results.DataGrids[0])
     else:
         data = AttrDict()
         for ii in range(analysis.Results.NumberOfDataGrids):
             desc = analysis.Results.DataGrids[ii].Description
-            key = desc if desc != '' else str(ii)
+            key = desc if desc != "" else str(ii)
             data[key] = zputils.unpack_datagrid(analysis.Results.DataGrids[ii])
 
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages)
-
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+    )
 
-    return ret
+    return analysis.complete(oncomplete, result)
```

### Comparing `zospy-0.6.2/zospy/analyses/wavefront.py` & `zospy-1.0.0/zospy/analyses/wavefront.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,202 +1,212 @@
+"""Zemax OpticStudio analyses from the Wavefront category."""
+
+from __future__ import annotations
+
 import os
 import re
 from tempfile import mkstemp
 
 import numpy as np
 import pandas as pd
 
 from zospy import utils
-from zospy.analyses.base import AnalysisResult, AttrDict
+from zospy.analyses.base import AnalysisResult, AttrDict, OnComplete, new_analysis
 from zospy.api import constants
+from zospy.zpcore import OpticStudioSystem
 
 
-def _structure_zernike_standard_coefficients_result(line_list):
+def _structure_zernike_standard_coefficients_result(line_list: list[str]) -> tuple[pd.DataFrame, pd.DataFrame]:
     """Structures the result of a zernike standard coefficients analysis.
 
     Parameters
     ----------
     line_list: list of str
         The line list obtained by reading in the results
 
     Returns
     -------
     (pd.DataFrame, pd.DataFrame)
         Two dataframes, respectively the general results and the coefficients
     """
-    zlinepat = re.compile(r'^Z\s+\d+')
-    valuepat_start = re.compile(r'^((-)?\d+\.\d+)')
-    valuepat_any = re.compile(r'((-)?\d+(\.\d+)?)')
+    zlinepat = re.compile(r"^Z\s+\d+")
+    valuepat_start = re.compile(r"^((-)?\d+\.\d+)")
+    valuepat_any = re.compile(r"((-)?\d+(\.\d+)?)")
 
     zernike_lines = [line for line in line_list if (zlinepat.search(line) is not None)]
 
     general_lines = [line for line in line_list if line not in zernike_lines]
-    general_arr = [' '.join(line.split()) for line in general_lines if ':' in line]
-    zernike_arr = np.array([line.replace(' ', '').split() for line in zernike_lines])
-    general_data = pd.DataFrame(columns=['Value', 'Unit'])
+    general_arr = [" ".join(line.split()) for line in general_lines if ":" in line]
+    zernike_arr = np.array([line.replace(" ", "").split() for line in zernike_lines])
+    general_data = pd.DataFrame(columns=["Value", "Unit"])
     for line in general_arr:
-        spl = line.split(':', 1)
+        spl = line.split(":", 1)
         if len(spl) == 1:
-            ind = ''.join([item.title() for item in spl[0].split()])
-            general_data.loc[ind] = ['', '']
+            ind = "".join([item.title() for item in spl[0].split()])
+            general_data.loc[ind] = ["", ""]
         else:
-            ind = ''.join([item.title() for item in spl[0].split()])
-            nvals = len(valuepat_any.findall(spl[1].replace(',', '.')))
+            ind = "".join([item.title() for item in spl[0].split()])
+            nvals = len(valuepat_any.findall(spl[1].replace(",", ".")))
             dat = spl[1].strip().split(maxsplit=nvals)
             if len(dat) == 0:
-                val = ''
-                unit = ''
+                val = ""
+                unit = ""
                 general_data.loc[ind] = [val, unit]
             elif len(dat) == 1:
-                if valuepat_start.search(dat[0].replace(',', '.')):  # value is number
-                    val = float(dat[0].replace(',', '.'))
+                if valuepat_start.search(dat[0].replace(",", ".")):  # value is number
+                    val = float(dat[0].replace(",", "."))
                 else:
                     val = dat[0]
-                unit = ''
+                unit = ""
                 general_data.loc[ind] = [val, unit]
             elif len(dat) == 2:
-                if valuepat_start.search(dat[0].replace(',', '.')):  # value is number
-                    val = float(dat[0].replace(',', '.'))
+                if valuepat_start.search(dat[0].replace(",", ".")):  # value is number
+                    val = float(dat[0].replace(",", "."))
                 else:
                     val = dat[0]
                 unit = dat[1]
                 general_data.loc[ind] = [val, unit]
             else:
                 for ii in range(len(dat) - 1):
-                    if valuepat_start.search(dat[ii].replace(',', '.')):  # value is number
-                        val = float(valuepat_start.search(dat[ii].replace(',', '.')).group())
+                    if valuepat_start.search(dat[ii].replace(",", ".")):  # value is number
+                        val = float(valuepat_start.search(dat[ii].replace(",", ".")).group())
                     else:
                         val = dat[ii]
                     unit = dat[-1]
-                    general_data.loc['{}_{}'.format(ind, ii)] = [val, unit]
-    zernike_data = pd.DataFrame(index=zernike_arr[:, 0].copy(),
-                                columns=['Value', 'Unit', 'Function'])
-    zernike_data.loc[zernike_arr[:, 0], 'Value'] = list(map(lambda s: float(s.replace(',', '.')),
-                                                            zernike_arr[:, 1].copy()))
-    zernike_data.loc[zernike_arr[:, 0], 'Unit'] = 'waves'
-    zernike_data.loc[zernike_arr[:, 0], 'Function'] = zernike_arr[:, 3].copy()
+                    general_data.loc["{}_{}".format(ind, ii)] = [val, unit]
+    zernike_data = pd.DataFrame(index=zernike_arr[:, 0].copy(), columns=["Value", "Unit", "Function"])
+    zernike_data.loc[zernike_arr[:, 0], "Value"] = list(
+        map(lambda s: float(s.replace(",", ".")), zernike_arr[:, 1].copy())
+    )
+    zernike_data.loc[zernike_arr[:, 0], "Unit"] = "waves"
+    zernike_data.loc[zernike_arr[:, 0], "Function"] = zernike_arr[:, 3].copy()
 
     return general_data, zernike_data
 
 
-def zernike_standard_coefficients(oss, sampling='64x64', maximum_term=37, wavelength=1, field=1,
-                                  reference_opd_to_vertex=False, surface='Image', sx=0.0, sy=0.0, sr=0.0,
-                                  oncomplete='Close', txtoutfile=None):
+def zernike_standard_coefficients(
+    oss: OpticStudioSystem,
+    sampling: str = "64x64",
+    maximum_term: int = 37,
+    wavelength: str | int = 1,
+    field: str | int = 1,
+    reference_opd_to_vertex: bool = False,
+    surface: str | int = "Image",
+    sx: float = 0.0,
+    sy: float = 0.0,
+    sr: float = 0.0,
+    oncomplete: OnComplete | str = OnComplete.Close,
+    txtoutfile: str = None,
+) -> AnalysisResult:
     """Wrapper around the OpticStudio Zernike Standard Coefficient Analysis.
 
     Parameters
     ----------
     oss: zospy.core.OpticStudioSystem
         A ZOSPy OpticStudioSystem instance. Should be sequential.
-    sampling: str or int
+    sampling: str | int
         The sampling, either string (e.g. '64x64') or int. The integer will be treated as a ZOSAPI Constants integer.
     maximum_term: int
         The maximum Zernike term, defaults to 37.
     wavelength: int
         The wavelength number that is to be used. Defaults to 1 (the first wavelength).
     field:
         The field that is to be analyzed. Defaults to 1.
     reference_opd_to_vertex: bool
         If the OPD should be referenced to vertex. Defaults to False.
-    surface: str or int
+    surface: str | int
         The surface that is to be analyzed. Either 'Image', 'Object' or an integer. Defaults to 'Image'.
     sx: float
         The sx.
     sy: float
         The sy.
     sr: float
         The sr.
-    oncomplete: str
+    oncomplete: OnComplete | str
         Defines behaviour upon completion of the analysis. Should be one of ['Close', 'Release', 'Sustain']. If 'Close',
         the analysis will be closed after completion. If 'Release', the analysis will remain open in OpticStudio, but
         the link with python will be destroyed. If 'Sustain' the analysis will be kept open in OpticStudio and the link
         with python will be sustained. To enable interaction when oncomplete == 'Sustain', the OpticStudio Analysis
         instance will be available in the returned AnalysisResult through AnalysisResult.Analysis. Defaults to 'Close'.
-    txtoutfile: str or None
+    txtoutfile: str | None
         The textfile to which the OpticStudio output is saved. If None, a temporary file will be created and deleted. If
         string, it should be a full system path with '.txt' as extension, after which the file will be saved in that
         location. Defaults to None.
 
     Returns
     -------
     AnalysisResult
         A ZernikeStandardCoefficients analysis result. Next to the standard data, the raw text return obtained from the
         analysis will be present under 'RawTextData' and the txtoutfile under 'TxtOutFile'.
     """
-
-    analysistype = 'ZernikeStandardCoefficients'
+    analysis_type = constants.Analysis.AnalysisIDM.ZernikeStandardCoefficients
 
     if txtoutfile is None:
-        fd, txtoutfile = mkstemp(suffix='.txt', prefix='zospy_')
+        fd, txtoutfile = mkstemp(suffix=".txt", prefix="zospy_")
         os.close(fd)
         cleantxt = True
     else:
-        if not txtoutfile.endswith('.txt'):
+        if not txtoutfile.endswith(".txt"):
             raise ValueError('txtfile should end with ".txt"')
         cleantxt = False
 
     # Create analysis
-    analysis = oss.Analyses.New_Analysis_SettingsFirst(constants.Analysis.AnalysisIDM.loc[analysistype])
+    analysis = new_analysis(oss, analysis_type)
 
     # Apply settings
-    analysis.Settings.SampleSize = utils.zputils.proc_constant(constants.Analysis.SampleSizes,
-                                                               utils.zputils.standardize_sampling(sampling))
+    analysis.Settings.SampleSize = getattr(constants.Analysis.SampleSizes, utils.zputils.standardize_sampling(sampling))
     analysis.Settings.MaximumNumberOfTerms = maximum_term
-    utils.zputils.analysis_set_wavelength(analysis, wavelength)
-    utils.zputils.analysis_set_field(analysis, field)
+    analysis.set_wavelength(wavelength)
+    analysis.set_field(field)
     analysis.Settings.ReferenceOBDToVertex = reference_opd_to_vertex  # ToDo: Monitor name with zemax updates
-    utils.zputils.analysis_set_surface(analysis, surface)
+    analysis.set_surface(surface)
     analysis.Settings.Sx = sx
     analysis.Settings.Sy = sy
     analysis.Settings.Sr = sr
 
     # Calculate
     analysis.ApplyAndWaitForCompletion()
 
     # Get results
     analysis.Results.GetTextFile(txtoutfile)
-    line_list = [line for line in open(txtoutfile, 'r', encoding='utf-16-le')]
+    line_list = [line for line in open(txtoutfile, "r", encoding="utf-16-le")]
 
     general_data, zernike_data = _structure_zernike_standard_coefficients_result(line_list)
     data = AttrDict(GeneralData=general_data, Coefficients=zernike_data)
 
     # Get headerdata, metadata and messages
-    headerdata = utils.zputils.analysis_get_headerdata(analysis)
-    metadata = utils.zputils.analysis_get_metadata(analysis)
-    messages = utils.zputils.analysis_get_messages(analysis)
+    headerdata = analysis.get_header_data()
+    metadata = analysis.get_metadata()
+    messages = analysis.get_messages()
 
     # Manually create settings as they cannot be accessed
-    settings = pd.Series(name='Settings')
+    settings = pd.Series(name="Settings", dtype=object)
 
-    settings.loc['SampleSize'] = constants.get_constantname_by_value(constants.Analysis.SampleSizes,
-                                                                     analysis.Settings.SampleSize)
-    settings.loc['MaximumNumberOfTerms'] = analysis.Settings.MaximumNumberOfTerms
-    settings.loc['Wavelength'] = analysis.Settings.Wavelength.GetWavelengthNumber()  # Todo Evaluate with 'all'
-    settings.loc['Field'] = analysis.Settings.Field.GetFieldNumber()  # Todo Evaluate with 'all'
-    settings.loc['ReferenceOBDToVertex'] = analysis.Settings.ReferenceOBDToVertex
-    settings.loc['Wavelength'] = analysis.Settings.Wavelength.GetWavelengthNumber()  # Todo Evaluate with 'all'
-    settings.loc['Field'] = analysis.Settings.Field.GetFieldNumber()  # Todo Evaluate with 'all'
-    settings.loc['ReferenceOBDToVertex'] = analysis.Settings.Surface.GetSurfaceNumber()  # Todo Evaluate with 'all'
-    settings.loc['Sx'] = sx
-    settings.loc['Sy'] = sy
-    settings.loc['Sr'] = sr
+    settings.loc["SampleSize"] = str(analysis.Settings.SampleSize)
+    settings.loc["MaximumNumberOfTerms"] = analysis.Settings.MaximumNumberOfTerms
+    settings.loc["Wavelength"] = analysis.Settings.Wavelength.GetWavelengthNumber()  # Todo Evaluate with 'all'
+    settings.loc["Field"] = analysis.Settings.Field.GetFieldNumber()  # Todo Evaluate with 'all'
+    settings.loc["ReferenceOBDToVertex"] = analysis.Settings.ReferenceOBDToVertex
+    settings.loc["Wavelength"] = analysis.Settings.Wavelength.GetWavelengthNumber()  # Todo Evaluate with 'all'
+    settings.loc["Field"] = analysis.Settings.Field.GetFieldNumber()  # Todo Evaluate with 'all'
+    settings.loc["ReferenceOBDToVertex"] = analysis.Settings.Surface.GetSurfaceNumber()  # Todo Evaluate with 'all'
+    settings.loc["Sx"] = sx
+    settings.loc["Sy"] = sy
+    settings.loc["Sr"] = sr
 
     # Create output
-    ret = AnalysisResult(analysistype=analysistype, data=data, settings=settings, metadata=metadata,
-                         headerdata=headerdata, messages=messages,
-                         RawTextData=line_list, TxtOutFile=txtoutfile)  # Set additional params
+    result = AnalysisResult(
+        analysistype=str(analysis_type),
+        data=data,
+        settings=settings,
+        metadata=metadata,
+        headerdata=headerdata,
+        messages=messages,
+        RawTextData=line_list,
+        TxtOutFile=txtoutfile,
+    )  # Set additional params
 
     # cleanup
     if cleantxt:
         os.remove(txtoutfile)
 
-    # Process oncomplete
-    if oncomplete == 'Close':  # Close if needed
-        analysis.Close()
-    elif oncomplete == 'Release':  # Keep the analysis open within OpticStudio but release it
-        analysis.Release()
-    elif oncomplete == 'Sustain':  # Add the analysis to the return
-        ret.Analysis = analysis
-    else:
-        raise ValueError('oncomplete should be one of "Close", "Release", "Sustain"')
-
-    return ret
+    return analysis.complete(oncomplete, result)
```

### Comparing `zospy-0.6.2/zospy/api/apisupport.py` & `zospy-1.0.0/zospy/api/apisupport.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,36 +21,36 @@
 
     Raises
     ------
     FileNotFoundError
         If either Zemax OpticStudio cannot be found in the Windows Registry or the Zemax OpticStudio root folder could
         not be obtained from the registry.
     """
-    logger.info('Obtaining Zemax Location from Windows Registry')
+    logger.info("Obtaining Zemax Location from Windows Registry")
 
     # Search for Zemax OpticStudio in the Windows Registry
     try:
-        regkey = winreg.OpenKey(winreg.HKEY_CURRENT_USER, 'Software\Zemax')
+        regkey = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Zemax")
     except FileNotFoundError as e:
-        logger.exception('Zemax cannot be found in the registry, '
-                         'the following error is raised:\n{}'.format(e))
+        logger.exception("Zemax cannot be found in the registry, " "the following error is raised:\n{}".format(e))
         raise e
 
     # Obtain the Zemax OpticStudio root path from the registry
     try:
-        zemaxfolder, _ = winreg.QueryValueEx(regkey, 'ZemaxRoot')
-        logger.info('Found ZemaxFolder at {}'.format(zemaxfolder))
+        zemaxfolder, _ = winreg.QueryValueEx(regkey, "ZemaxRoot")
+        logger.info("Found ZemaxFolder at {}".format(zemaxfolder))
     except FileNotFoundError as e:
-        logger.exception('The Zemax Root folder cannot be found in the registry key, '
-                         'the following error is raised:\n{}'.format(e))
+        logger.exception(
+            "The Zemax Root folder cannot be found in the registry key, " "the following error is raised:\n{}".format(e)
+        )
         raise e
     finally:  # Clean up
-        logger.debug('Closing registry key')
+        logger.debug("Closing registry key")
         winreg.CloseKey(regkey)
-        logger.debug('Registry key closed')
+        logger.debug("Registry key closed")
 
     return zemaxfolder
 
 
 def load_zosapi_nethelper(filepath=None, preload=False):
     """Loads the ZOSAPI_NetHelper.
 
@@ -62,34 +62,33 @@
         Specifies if CLR should import with preload on (True) or off (False). Defaults to False).
 
     Returns
     -------
     ZOSAPI_NetHelper: netModuleObject
         The ZOSAPI_NetHelper as module object
     """
-
     if not filepath:  # get the path through the windows registry
         zos_root = get_zos_root()
-        znh_filepath = os.path.join(zos_root, r'ZOS-API\Libraries\ZOSAPI_NetHelper.dll')
+        znh_filepath = os.path.join(zos_root, r"ZOS-API\Libraries\ZOSAPI_NetHelper.dll")
     else:
         znh_filepath = filepath
 
-    logger.debug('Adding reference {} to clr'.format(znh_filepath))
+    logger.debug("Adding reference {} to clr".format(znh_filepath))
     sys.path.append(os.path.basename(znh_filepath))
     clr.AddReference(znh_filepath)
 
-    logger.debug('Importing ZOSAPI_NetHelper')
-    znh = __import__('ZOSAPI_NetHelper', globals(), locals(), [], 0)
-    logger.info('ZOSAPI_NetHelper imported successfully')
+    logger.debug("Importing ZOSAPI_NetHelper")
+    znh = __import__("ZOSAPI_NetHelper", globals(), locals(), [], 0)
+    logger.info("ZOSAPI_NetHelper imported successfully")
 
     return znh
 
 
 def load_zosapi(zosapi_nethelper=None, zemaxdirectory=None, preload=False):
-    """
+    """Load the ZOS-API using the ZOSAPI NetHelper DLL.
 
     Parameters
     ----------
     zosapi_nethelper: netModuleObject, optional
         The loaded ZOSAPI_NetHelper DLL. If None, the zemaxdirectory parameter will be used. Note that either the
         zosapi_nethelper or the zemaxdirectory has to be specified, not both.
     zemaxdirectory: str, optional
@@ -106,53 +105,52 @@
     Raises
     ------
     ValueError:
         If either both or None of zosapi_nethelper and zemaxdirectory are specified.
     FileNotFoundError:
         If one of ZOSAPI_Interfaces.dll or ZOSAPI.dll cannot be found.
     """
-
     if not any((zosapi_nethelper, zemaxdirectory)):
-        raise ValueError('Either the zosapi_nethelper or the zemaxdirectory should be specified.')
+        raise ValueError("Either the zosapi_nethelper or the zemaxdirectory should be specified.")
     elif all((zosapi_nethelper, zemaxdirectory)):
-        raise ValueError('Only one of zosapi_nethelper and zemaxdirectory should be specified.')
+        raise ValueError("Only one of zosapi_nethelper and zemaxdirectory should be specified.")
     else:
         pass
 
     # Get the Zemax OpticStudio directory and add it to the path
     if zosapi_nethelper:
-        logger.info('Obtaining Zemax Directory from ZOSAPI_NetHelper')
+        logger.info("Obtaining Zemax Directory from ZOSAPI_NetHelper")
         zosapi_nethelper.ZOSAPI_Initializer.Initialize()
         zos_dir = zosapi_nethelper.ZOSAPI_Initializer.GetZemaxDirectory()
-        logger.info('Zemax OpticStudio found at {}'.format(zos_dir))
+        logger.info("Zemax OpticStudio found at {}".format(zos_dir))
     else:
-        logger.info('Zemax Directory specified by user ({})'.format(zemaxdirectory))
+        logger.info("Zemax Directory specified by user ({})".format(zemaxdirectory))
         zos_dir = zemaxdirectory
     sys.path.append(zos_dir)
 
-    logger.info('Searching and registering ZOSAPI DLLs')
-    for dll in ['ZOSAPI_Interfaces', 'ZOSAPI']:
+    logger.info("Searching and registering ZOSAPI DLLs")
+    for dll in ["ZOSAPI_Interfaces", "ZOSAPI"]:
         if clr.FindAssembly(dll):
-            logger.debug('{}.dll found'.format(dll))
+            logger.debug("{}.dll found".format(dll))
             clr.AddReference(dll)
-            logger.info('{} imported to clr'.format(dll))
+            logger.info("{} imported to clr".format(dll))
         else:
-            logger.critical('Cannot locate {}.dll'.format(dll))
-            raise FileNotFoundError('Cannot locate {}.dll in {}'.format(dll, zos_dir))
+            logger.critical("Cannot locate {}.dll".format(dll))
+            raise FileNotFoundError("Cannot locate {}.dll in {}".format(dll, zos_dir))
 
-    logger.debug('Checking content of ZOSAPI_Interfaces.dll')
-    content = clrutils.reflect_dll_content(os.path.join(zos_dir, 'ZOSAPI_Interfaces.dll'))
+    logger.debug("Checking content of ZOSAPI_Interfaces.dll")
+    content = clrutils.reflect_dll_content(os.path.join(zos_dir, "ZOSAPI_Interfaces.dll"))
 
-    logger.debug('Loading ZOSAPI')
-    zosapi = __import__('ZOSAPI', globals(), locals(), [], 0)
-    logger.debug('ZOSAPI loaded')
-
-    logger.debug('Loading nested namespaces')
-    for nsp in content['namespaces']:
-        if nsp == 'ZOSAPI':
+    logger.debug("Loading ZOSAPI")
+    zosapi = __import__("ZOSAPI", globals(), locals(), [], 0)
+    logger.debug("ZOSAPI loaded")
+
+    logger.debug("Loading nested namespaces")
+    for nsp in content["namespaces"]:
+        if nsp == "ZOSAPI":
             continue
         __import__(nsp, globals(), locals(), [], 0)
-        logger.debug('Nested namespace {} preloaded'.format(nsp))
+        logger.debug("Nested namespace {} preloaded".format(nsp))
 
-    zospy.api.constants._construct_from_zosapi_and_enumkeys(zosapi, content['enums'])  # noqa
+    zospy.api.constants._construct_from_zosapi_and_enumkeys(zosapi, content["enums"])  # noqa
 
     return zosapi
```

### Comparing `zospy-0.6.2/zospy/api/constants.py` & `zospy-1.0.0/zospy/api/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-"""
+"""Constants for the ZOS-API.
+
 Submodule used for package wide access to all ZOS api constants. Note that the constant-naming within this module breaks
 pep, but is kept as such to be in-sync with the api documentation. Constants should in general be accessed through
 'zospy.constants' (or 'zp.constants'). All constants are obtained dynamically from the api. Therefore, they are only
 available after running the code stated under examples.
 
 Examples
 --------
 import zospy as zp
 zos = zp.ZOS()
 zos.wakeup()
 zp.constants
 """
+from __future__ import annotations
 
 import itertools as _itertools
 import logging as _logging
 from types import SimpleNamespace as _SimpleNamespace
+from typing import Iterable, TypeVar
 
-from pandas import Index as _Index
-
+from zospy.api._ZOSAPI_constants import *  # noqa
 from zospy.utils import clrutils as _clrutils
 from zospy.utils import pyutils as _pyutils
 
 _logger = _logging.getLogger(__name__)
 
+
 # Note: the above imports (and all but one function) are named private, to incease clarity on which Module components
 # are constants and which are not.
 
 
 def _itertools_joinfunc(*args):
-    return '.'.join(args)
+    return ".".join(args)
 
 
 def _construct_from_zosapi_and_enumkeys(zosapi, zosapi_enumkeys):
     """Constructs the constants from the zosapi and zosapi_enumkeys.
 
     The acquired constants are added to the zp.constants namespace
 
@@ -43,63 +46,76 @@
     zosapi_enumkeys: list[str]
         The enumeration keys obtained from can be obtained through zp.utils.clrutils.reflect_dll_content()
 
     Returns
     -------
     None
     """
-
     zosapi_enumkeys = sorted(zosapi_enumkeys)
     added_namespaces = set()
     for enumkey in zosapi_enumkeys:
-
-        subkeys = enumkey.split('.')
+        subkeys = enumkey.split(".")
 
         assert len(subkeys) > 1  # should at least be 2
 
         if len(subkeys) == 2:  # No nesting
             clrattr = getattr(zosapi, subkeys[-1], None)
 
             # Set constant
-            globals()[subkeys[-1]] = _clrutils.series_from_system_enum(clrattr)
+            globals()[subkeys[-1]] = _clrutils.system_enum_to_namedtuple(clrattr)
 
         else:  # with nesting
             base = subkeys[1]
             nsp_parts = list(_itertools.accumulate(subkeys[2:-1], func=_itertools_joinfunc))
 
             if base not in added_namespaces:
                 globals()[base] = _SimpleNamespace()  # Create the base as simplenamespace
                 added_namespaces.add(base)
             for nsp in nsp_parts:
-                if '.'.join((base, nsp)) in added_namespaces:  # check if already added
+                if ".".join((base, nsp)) in added_namespaces:  # check if already added
                     continue
                 else:
                     _pyutils.rsetattr(globals()[base], nsp, _SimpleNamespace())  # add nested objects
-                    added_namespaces.add('.'.join((base, nsp)))
+                    added_namespaces.add(".".join((base, nsp)))
 
-            clrattr = _pyutils.rgetattr(zosapi, '.'.join(subkeys[1:]), None)
+            clrattr = _pyutils.rgetattr(zosapi, ".".join(subkeys[1:]), None)
 
             # set constants
-            _pyutils.rsetattr(globals()[base], '.'.join(subkeys[2:]),
-                              _clrutils.series_from_system_enum(clrattr))
+            _pyutils.rsetattr(globals()[base], ".".join(subkeys[2:]), _clrutils.system_enum_to_namedtuple(clrattr))
+
 
+Constant = TypeVar("Constant")
 
-def get_constantname_by_value(constant_series, value):
-    """Obtain a constant name from a value
+
+def process_constant(constant: Iterable[Constant], value: Constant | str | None) -> Constant:
+    if (value is None or value == "None") and hasattr(constant, "None_"):
+        return getattr(constant, "None_")
+    elif isinstance(value, str) and hasattr(constant, value):
+        return getattr(constant, value)
+    elif value in constant:
+        return value
+
+    raise ValueError(f"Constant {type(constant).__name__} does not contain value {str(value)}")
+
+
+def get_constantname_by_value(constant_tuple, value):
+    """Obtain a constant name from a value.
 
     Parameters
     ----------
-    constant_series: pd.Series
+    constant_tuple: tuple
         The set of constants used to look up the value
     value: int
         The value for which the constant name is to be found
 
     Returns
     -------
     str
         The constant name
     """
-
     try:
-        return constant_series.index[_Index(constant_series).get_loc(value)]
+        if isinstance(value, int):
+            return constant_tuple._fields[value]  # noqa
+
+        return constant_tuple._fields[constant_tuple.index(value)]  # noqa
     except KeyError:
-        raise ValueError('None of the constants has value {} assigned'.format(value))
+        raise ValueError(f"None of the constants has value {value} assigned")
```

### Comparing `zospy-0.6.2/zospy/functions/nce.py` & `zospy-1.0.0/zospy/functions/nce.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from zospy.api import constants
-from zospy.utils.zputils import proc_constant
+from __future__ import annotations
 
+from zospy.api import _ZOSAPI, constants
 
-def object_change_type(obj, newtype):
-    """Simple function to change the type of an object in the NCE
+
+def object_change_type(obj: _ZOSAPI.Editors.NCE.INCERow, new_type: constants.Editors.NCE.ObjectType | str):
+    """Simple function to change the object type in the NCE.
 
     Parameters
     ----------
-    obj: INCERow
+    obj: ZOSAPI.Editors.NCE.INCERow
         The Row/Object for which the change is to be made.
-    newtype: str or int
+    new_type: zospy.constants.Editors.NCE.ObjectType | str
         The new object type, either string (e.g. 'StandardLens') or int. The integer will be treated as if obtained from
         zp.constants.Editors.NCE.ObjectType.
 
     Returns
     -------
     None
 
@@ -21,16 +22,14 @@
     --------
     >>> import zospy as zp
     >>> zos = zp.ZOS()
     >>> zos.connect_as_extension()
     >>> oss = zos.get_primary_system()
     >>> oss.make_nonsequential()
     >>> newobj = oss.NCE.InsertNewObjectAt(0)
-    >>> object_change_type(newobj, 'StandardLens')
+    >>> object_change_type(newobj, zp.constants.Editors.NCE.ObjectType.StandardLens)
     """
-    # Obtain the integer representing the new type if needed
-    newtype = proc_constant(constants.Editors.NCE.ObjectType, newtype)
+    new_type = constants.process_constant(constants.Editors.NCE.ObjectType, new_type)
 
     # Apply
-    newsurftypesettings = obj.GetObjectTypeSettings(newtype)
-    obj.ChangeType(newsurftypesettings)
-
+    new_surface_type_settings = obj.GetObjectTypeSettings(new_type)
+    obj.ChangeType(new_surface_type_settings)
```

### Comparing `zospy-0.6.2/zospy/utils/clrutils.py` & `zospy-1.0.0/zospy/utils/clrutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
+from collections import namedtuple
 from datetime import datetime as dt
 
-import clr  # noqa
-from System import Enum, Double, Reflection  # noqa
-from pandas import Series
+import clr
+from System import Double, Enum, Reflection  # noqa
 
-DUMMY_DOUBLE = Double(0.)
+DUMMY_DOUBLE = Double(0.0)
 DUMMY_ENUM = 0
 
 
 def clr_get_available_assemblies(with_meta=True):
     """Gets all the avaialble assemblies from the Common Language Runtime.
 
     Parameters
@@ -35,23 +35,23 @@
 
     Returns
     -------
     dict
         A dictionary containing the namespaces ('namespaces') and the enumerations ('enums').
     """
     if not os.path.isabs(dllfilepath):
-        raise ValueError('dllfilepath should be an absolute path')
-    if not dllfilepath.lower().endswith('.dll'):
-        raise ValueError('dllfilepath should end with .dll (case is ignored)')
+        raise ValueError("dllfilepath should be an absolute path")
+    if not dllfilepath.lower().endswith(".dll"):
+        raise ValueError("dllfilepath should end with .dll (case is ignored)")
 
     content = list(Reflection.Assembly.LoadFile(dllfilepath).GetTypes())
 
     namespaces = sorted(list(set([item.Namespace for item in content])))
     enums = sorted([item.FullName for item in content if item.IsEnum])
-    ret = {'namespaces': namespaces, 'enums': enums}
+    ret = {"namespaces": namespaces, "enums": enums}
     return ret
 
 
 def system_get_enum_key_from_value(enum, value):
     """Gets the key corresponding to a certain value from a System.Enum instance.
 
     Parameters
@@ -71,15 +71,15 @@
 
 def system_get_enum_names(enum):
     """Gets all names from a System.Enum instance.
 
     Parameters
     ----------
     enum: System.Enum
-        A Enum instance.
+        An Enum instance.
 
     Returns
     -------
     list
         A list containing the names of the Enum instance
     """
     return list(Enum.GetNames(enum))
@@ -87,43 +87,49 @@
 
 def system_get_enum_values(enum):
     """Gets all values from a System.Enum instance.
 
     Parameters
     ----------
     enum: System.Enum
-        A Enum instance.
+        An Enum instance.
 
     Returns
     -------
     list
         A list containing the values of the Enum instance
     """
     return list(Enum.GetValues(enum))
 
 
-def series_from_system_enum(enum):
-    """Converts a System.Enum into a pandas series
+def system_enum_to_namedtuple(enum):
+    """Converts a System.Enum into a namedtuple.
+
+    If the Enum contains a member with name `None`, its name is changed to `None_`.
 
     Parameters
     ----------
     enum: System.Enum
-        A Enum instance.
+        An Enum instance.
 
     Returns
     -------
-    Series
-        A Series containing the enum data.
+    namedtuple
+        A namedtuple containing the enum data.
 
     """
     label = enum.__name__
     names = system_get_enum_names(enum)
     values = system_get_enum_values(enum)
 
-    return Series(data=values, index=names, name=label)
+    # Rename None to NONE
+    if "None" in names:
+        names[names.index("None")] = "None_"
+
+    return namedtuple(label, names)._make(values)  # noqa
 
 
 def system_datetime_to_datetime(sdt):
     """Converts a System.DateTime into a datetime.datetime instance.
 
     N.B.: As the System.DateTime does not contain info on the timezone, there might be an error if these do not match
     between the supplied DateTime instance and the current computer
@@ -134,10 +140,16 @@
         An System.DateTime instance
 
     Returns
     -------
     datetime.datetime
         The pyton datetime instance
     """
-    return dt(year=sdt.Year, month=sdt.Month, day=sdt.Day,
-              hour=sdt.Hour, minute=sdt.Minute, second=sdt.Second,
-              microsecond=sdt.Millisecond*1000)
+    return dt(
+        year=sdt.Year,
+        month=sdt.Month,
+        day=sdt.Day,
+        hour=sdt.Hour,
+        minute=sdt.Minute,
+        second=sdt.Second,
+        microsecond=sdt.Millisecond * 1000,
+    )
```

### Comparing `zospy-0.6.2/zospy/utils/pyutils.py` & `zospy-1.0.0/zospy/utils/pyutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     val
         The value to which the attribute is set
 
     Returns
     -------
         None
     """
-    pre, _, post = attr.rpartition('.')
+    pre, _, post = attr.rpartition(".")
     return setattr(rgetattr(obj, pre) if pre else obj, post, val)
 
 
 def rgetattr(obj, attr, *args):
     """Wrapper for the getattr() function that handles nested strings.
 
     Parameters
@@ -44,8 +44,8 @@
     AttributeError
         When the attribute does not exist and no default is supplied in the *args
     """
 
     def _getattr(subobj, subattr, *subargs):
         return getattr(subobj, subattr, *subargs)
 
-    return functools.reduce(lambda x, y: _getattr(x, y, *args), [obj] + attr.split('.'))
+    return functools.reduce(lambda x, y: _getattr(x, y, *args), [obj] + attr.split("."))
```

### Comparing `zospy-0.6.2/zospy/zpcore.py` & `zospy-1.0.0/zospy/zpcore.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,240 +1,237 @@
+from __future__ import annotations
+
 import logging
 import warnings
 import weakref
 
-from zospy.analyses import mtf, reports, wavefront, psf
-from zospy.api import constants
-from zospy.api.apisupport import load_zosapi_nethelper, load_zosapi
-from zospy.functions.lde import get_pupil
-from zospy.utils.zputils import proc_constant
+from zospy.api import _ZOSAPI, constants
+from zospy.api.apisupport import load_zosapi, load_zosapi_nethelper
 
 logger = logging.getLogger(__name__)
 
 
 class OpticStudioSystem:
-    """Wrapper for OpticStudio System instances"""
+    """Wrapper for OpticStudio System instances."""
+
     def __init__(self, zos_instance, system_instance):
         """Initiates the OpticStudioSystem.
 
         Parameters
         ----------
         zos_instance: ZOS
             A ZOS instance
         system_instance: ZOS.Application.PrimarySystem
             A PrimarySystem instance obtained from the zos_instance.
         """
-        self._ZOS = zos_instance
+        self._ZOS: ZOS = zos_instance
 
-        self._System = system_instance
+        self._System: _ZOSAPI.IOpticalSystem = system_instance
         self._OpenFile = None
 
     @property
-    def SystemName(self): # noqa
+    def SystemName(self) -> str:
         return self._System.SystemName
 
     @SystemName.setter
-    def SystemName(self, value): # noqa
+    def SystemName(self, value: str):
         self._System.SystemName = value
 
     @property
-    def SystemID(self): # noqa
+    def SystemID(self) -> int:
         return self._System.SystemID
 
     @property
-    def Mode(self): # noqa
-        return constants.get_constantname_by_value(constants.SystemType, self._System.Mode)
+    def Mode(self) -> str:
+        return str(self._System.Mode)
 
     @property
-    def SystemFile(self): # noqa
+    def SystemFile(self) -> str:
         return self._System.SystemFile
 
     @property
-    def IsNonAxial(self): # noqa
+    def IsNonAxial(self) -> bool:
         return self._System.IsNonAxial
 
     @property
-    def NeedsSave(self): # noqa
+    def NeedsSave(self) -> bool:
         return self._System.NeedsSave
 
     @property
-    def SystemData(self): # noqa
+    def SystemData(self) -> _ZOSAPI.SystemData.ISystemData:
         return self._System.SystemData
 
     @property
-    def LDE(self):  # noqa
+    def LDE(self) -> _ZOSAPI.Editors.LDE.ILensDataEditor:
         return self._System.LDE
 
     @property
-    def NCE(self):  # noqa
+    def NCE(self) -> _ZOSAPI.Editors.NCE.INonSeqEditor:
         return self._System.NCE
 
     @property
-    def MFE(self):  # noqa
+    def MFE(self) -> _ZOSAPI.Editors.MFE.IMeritFunctionEditor:
         return self._System.MFE
 
     @property
-    def TDE(self):  # noqa
+    def TDE(self) -> _ZOSAPI.Editors.TDE.IToleranceDataEditor:
         return self._System.TDE
 
     @property
-    def MCE(self):  # noqa
+    def MCE(self) -> _ZOSAPI.Editors.MCE.IMultiConfigEditor:
         return self._System.MCE
 
     @property
-    def Analyses(self): # noqa
+    def Analyses(self) -> _ZOSAPI.Analysis.I_Analyses:
         return self._System.Analyses
 
     @property
-    def Tools(self): # noqa
+    def Tools(self) -> _ZOSAPI.Tools.IOpticalSystemTools:
         return self._System.Tools
 
     @property
-    def TheApplication(self): # noqa
+    def TheApplication(self) -> _ZOSAPI.IZOSAPI_Application:
         return self._System.TheApplication
 
     @property
-    def LensUpdateMode(self): # noqa
-        return constants.get_constantname_by_value(constants.LensUpdateMode, self._System.LensUpdateMode)
+    def LensUpdateMode(self) -> str:
+        return str(self._System.UpdateMode)
 
     @LensUpdateMode.setter
-    def LensUpdateMode(self, value): # noqa
+    def LensUpdateMode(self, value: _ZOSAPI.LensUpdateMode):
         """Sets the LensUpdateMode.
 
         Parameters
         ----------
         value: str or int
             The new mode. Should be one of ['None', 'EditorsOnly', 'AllWindows'] or int. The integer is interpreted as
             one of the zospy.constants.LensUpdateMode constants.
         """
-        self._System.LensUpdateMode = proc_constant(constants.LensUpdateMode, value)
+        self._System.LensUpdateMode = value
 
     @property
-    def SessionModes(self): # noqa
-
-        return constants.get_constantname_by_value(constants.SessionModes, self._System.SessionModes)
+    def SessionModes(self) -> str:
+        return str(self._System.SessionMode)
 
     @SessionModes.setter
-    def SessionModes(self, value): # noqa
+    def SessionModes(self, value: constants.SessionModes | str):
         """Sets the SessionMode.
 
         Parameters
         ----------
         value: str or int
-            The new mode. Should be one of ['FromPreferences', 'SessionOn', 'SessionOff'] or int. The integer is
-            interpreted as one of the zospy.constants.LensUpdateMode constants.
+            The new mode. Should be one of ['FromPreferences', 'SessionOn', 'SessionOff'].
         """
-        self._System.SessionModes = proc_constant(constants.SessionModes, value)
+        self._System.SessionMode = constants.process_constant(constants.SessionModes, value)
 
-    def get_current_status(self):
+    def get_current_status(self) -> str:
         return self._System.GetCurrentStatus()
 
-    def update_status(self):
+    def update_status(self) -> str:
         return self._System.UpdateStatus()
 
-    def make_sequential(self):
+    def make_sequential(self) -> bool:
         return self._System.MakeSequential()
 
-    def make_nonsequential(self):
+    def make_nonsequential(self) -> bool:
         return self._System.MakeNonSequential()
 
-    def load(self, filepath, saveifneeded=False):
-        """Loads an earlier defined zemax file
-
+    def load(self, filepath: str, saveifneeded: bool = False):
+        """Loads an earlier defined zemax file.
 
         Parameters
         ----------
         filepath: str
             The filepath that should be loaded
         saveifneeded: bool
             Defines if the current file is saved before opening the new file. Defaults to False.
         """
-        logger.debug('Opening {} with SaveIfNeeded set to {}'.format(filepath, saveifneeded))
+        logger.debug("Opening {} with SaveIfNeeded set to {}".format(filepath, saveifneeded))
 
         self._System.LoadFile(filepath, saveifneeded)
         self._OpenFile = filepath
 
-        logger.info('Opened {}'.format(filepath))
+        logger.info("Opened {}".format(filepath))
 
-    def new(self, saveifneeded=False):
+    def new(self, saveifneeded: bool = False):
         """Creates a new session file.
 
         Parameters
         ----------
         saveifneeded: bool
             Defines if the current file is saved before opening the new file. Defaults to False.
         """
-
-        logger.debug('Creating new file')
+        logger.debug("Creating new file")
 
         self._System.New(saveifneeded)
         self._OpenFile = None
 
-        logger.info('Opened new file')
+        logger.info("Opened new file")
 
-    def save_as(self, filepath):
+    def save_as(self, filepath: str):
         """Saves the current session under a specified name.
 
         Parameters
         ----------
         filepath: str
             The filepath where the system should be saved. Note that a partial path or relative path does not work.
         """
-
-        logger.debug('Saving open session as {}'.format(filepath))
+        logger.debug("Saving open session as {}".format(filepath))
 
         self._System.SaveAs(filepath)
         self._OpenFile = filepath
 
-        logger.info('File saved as {}'.format(filepath))
+        logger.info("File saved as {}".format(filepath))
 
-    def save(self):
+    def save(self) -> bool:
         """Saves the current optic studio session.
 
         If the file name for the current session is not known (e.g. when a new file was created), a warning is raised
         and the file is not saved. On these occurences, save_as() should be used once.
 
         Returns (bool): A boolean indicating if the saving was successful.
 
         """
-        logger.debug('Saving file')
+        logger.debug("Saving file")
 
         if self._OpenFile is None:
-            warnings.warn('No file name has been defined for the current system, the current session has not been '
-                          'saved. Please use the save_as() function before using save.')
-            logger.critical('Could not save file')
+            warnings.warn(
+                "No file name has been defined for the current system, the current session has not been "
+                "saved. Please use the save_as() function before using save."
+            )
+            logger.critical("Could not save file")
 
             return False
         else:
             self._System.Save()
-            logger.info('File saved')
+            logger.info("File saved")
             return True
 
-    def close(self, saveifneeded=False):
-        """Closes the optical system. Only works on secondary systems (See OpticStudio documentation)
+    def close(self, saveifneeded: bool = False) -> bool:
+        """Closes the optical system. Only works on secondary systems (See OpticStudio documentation).
 
         Parameters
         ----------
         saveifneeded: bool
             Defines if the current file is saved before opening the new file. Defaults to False.
         """
         return self._System.Close(saveifneeded)
 
-    def copy_system(self):
+    def copy_system(self) -> OpticStudioSystem:
         """Copies the current OpticStudioSystem instance.
 
         Returns
         -------
         zospy.core.OpticStudioSystem
             A ZOSPy OpticStudioSystem instance. Should be sequential.
         """
         return OpticStudioSystem(self._ZOS, self._System.CopySystem())
 
-    def _ensure_correct_mode(self, required):
-        """Ensures that the system is in the required type
+    def _ensure_correct_mode(self, required: str):
+        """Ensures that the system is in the required type.
 
         Parameters
         ----------
         required: str
             The required system type. Either 'Sequential' or 'NonSequential'.
 
         Returns
@@ -242,30 +239,30 @@
         None
 
         Raises
         ------
         ValueError:
             When the system is in the incorrect type
         """
-        logger.debug('Ensuring correct mode')
+        logger.debug("Ensuring correct mode")
         if self.Mode != required:
-            err = 'Incorrect system type. System is in {} mode but {} mode is required'.format(self.Mode, required)
+            err = "Incorrect system type. System is in {} mode but {} mode is required".format(self.Mode, required)
             logger.critical(err)
             raise TypeError(err)
         else:
-            logger.debug('System is in correct mode')
+            logger.debug("System is in correct mode")
         # ToDo: Eveluate what happens in 'mixed mode'
 
     def __del__(self):
-        logger.debug('Closing connections with Zemax OpticStudio')
+        logger.debug("Closing connections with Zemax OpticStudio")
         # ToDo Add cleanup
 
 
 class ZOS:
-    """An Communication instance for Zemax OpticStudio.
+    """A Communication instance for Zemax OpticStudio.
 
     This class can be used to establish a link between Python and Zemax OpticStudio through .NET,
     and control OpticStudio. The connection is established as following:
 
     Simple:
     1. self.wakeup().
     2. self.create_new_session() or self.connect_as_extension().
@@ -275,71 +272,70 @@
     1. self._load_zos_dlls()
     2. self._update_constants()
     3. self.create_new_session() or self.connect_as_extension().
     4. self.get_primary_system()
 
     After connection, many OpticStudio functionalities are controllable through ZOS.ZOSAPI()
 
-    Attributes:
+    Attributes
+    ----------
         ZOSAPI (None | netModuleObject): The ZOSAPI interface or if loaded.
         ZOSAPI_NetHelper (None | netModuleObject): The ZOSAPI_NetHelper interface if loaded.
     """
 
     _OpticStudioSystem = OpticStudioSystem
 
     _instances = set()
 
     def __new__(cls, *args, **kwargs):
-
         if len(cls._instances) >= 1:
             # As the number of applications within runtime is limited to 1 by Zemax, it is logical to also limit the
             # number of ZOS instances
-            raise ValueError('Cannot have more than one active ZOS instance')
+            raise ValueError("Cannot have more than one active ZOS instance")
 
         instance = super(ZOS, cls).__new__(cls, *args, **kwargs)
 
         return instance
 
     def __init__(self):
         """Initiation of the ZOS Instance."""
-        logger.debug('Initializing ZOS instance')
+        logger.debug("Initializing ZOS instance")
 
-        self.ZOSAPI = None
+        self.ZOSAPI: _ZOSAPI = None
         self.ZOSAPI_NetHelper = None
-        self.Connection = None
-        self.Application = None
+        self.Connection: _ZOSAPI.IZOSAPI_Connection = None
+        self.Application: _ZOSAPI.IZOSAPI_Application = None
 
         # Register the instance and create a finalize code to remove it from ZOS._instances when deleted
         ZOS._instances.add(id(self))
         weakref.finalize(self, ZOS._instances.discard, id(self))
 
-        logger.info('ZOS instance initialized')
+        logger.info("ZOS instance initialized")
 
-    def wakeup(self, preload=False, zosapi_nethelper=None):
+    def wakeup(self, preload: bool = False, zosapi_nethelper: str = None):
         """Wakes the zosapi instance.
 
         The parameters are passed to self._load_zos_dlls()
 
-                Parameters
+        Parameters
         ----------
         preload: bool
             A boolean indicating if nested namespaces should be preloaded.
         zosapi_nethelper: str, optional
             Optional filepath to the ZOSAPI_NetHelper dll, if None, the windows registry will be used to find
             ZOSAPI_NetHelper dll. Defaults to None.
 
         Returns
         -------
         None
         """
-
         self._load_zos_dlls(preload=preload, zosapi_nethelper=zosapi_nethelper)
         self._assign_connection()
 
-    def _load_zos_dlls(self, preload=False, zosapi_nethelper=None):
+    def _load_zos_dlls(self, preload: bool = False, zosapi_nethelper: str = None):
         """Loads the ZOS-API DLLs and makes them available for usage through ZOS.ZOSAPI and ZOS.ZOSAPI_NetHelper.
 
         As there are many nested namespaces in the ZOSAPI DLLs that are always available after import but not
         preloaded, it can be chosen to do so. This should only be done for developmental reasons, as it likely slows
         down the code.
 
         Parameters
@@ -355,78 +351,96 @@
         FileNotFoundError:
             An error occurred in locating one of the DLLs.
         ModuleNotFoundError:
             One of the nested namespaces cannot be found. This error can only occur with preload set to True.
 
 
         """
-        logger.debug('Loading ZOS DLLs with preload set to {}'.format(preload))
+        logger.debug("Loading ZOS DLLs with preload set to {}".format(preload))
         self.ZOSAPI_NetHelper = load_zosapi_nethelper(filepath=zosapi_nethelper, preload=preload)
         self.ZOSAPI = load_zosapi(self.ZOSAPI_NetHelper, preload=preload)
 
     def _assign_connection(self):
-        """Assigns the ZOSAPI Connection to self.Connection"""
+        """Assigns the ZOSAPI Connection to self.Connection."""
         if not self.Connection:
-            logger.debug('Assigning ZOSAPI_Connection() to self.Connection')
+            logger.debug("Assigning ZOSAPI_Connection() to self.Connection")
             self.Connection = self.ZOSAPI.ZOSAPI_Connection()
         else:
-            logger.debug('ZOSAPI_Connection() already assigned self.Connection')
+            logger.debug("ZOSAPI_Connection() already assigned self.Connection")
 
-    def connect_as_extension(self, instancenumber=0):
+    def connect_as_extension(self, instancenumber: int = 0) -> bool:
         """Creates a standalone Zemax Opticstudio instance.
 
         The application will be assigned to self.Application.
 
         Returns
         -------
         bool
             True if a valid connection is made, else False
         """
-
         self._assign_connection()
 
         if self.Connection.IsAlive:  # ToDo ensure no memory leak
-            raise RuntimeError('Only one Zemax application can exist within runtime')
+            raise RuntimeError("Only one Zemax application can exist within runtime")
 
         self.Application = self.Connection.ConnectAsExtension(instancenumber)
 
         if self.Application.IsValidLicenseForAPI:
             return True
         else:
-            logger.critical('OpticStudio Licence is not valid for API, connection not established')
+            logger.critical("OpticStudio Licence is not valid for API, connection not established")
             return False
 
-    def create_new_application(self):
+    def create_new_application(self) -> bool:
         """Creates a standalone Zemax Opticstudio instance.
 
         The application will be assigned to self.Application.
 
         Returns
         -------
         bool
             True if a valid connection is made, else False
         """
         self._assign_connection()
 
         if self.Connection.IsAlive:  # ToDo ensure no memory leak
-            raise RuntimeError('Only one Zemax application can exist within runtime')
+            raise RuntimeError("Only one Zemax application can exist within runtime")
 
         self.Application = self.Connection.CreateNewApplication()
 
         if self.Application.IsValidLicenseForAPI:
             return True
         else:
-            logger.critical('OpticStudio Licence is not valid for API, connection not established')
+            logger.critical("OpticStudio Licence is not valid for API, connection not established")
             return False
 
-    def get_primary_system(self):
+    def create_new_system(self, system_mode: constants.SystemType | str = "Sequential") -> OpticStudioSystem:
+        """Creates a new OpticStudioSystem. This works only if ZOSPy is connected to a standalone application.
+
+        Parameters
+        ----------
+        system_mode : constants.SystemType | str
+            The mode of the new system, must be one of "Sequential", "NonSequential". Defaults to "Sequential".
+
+        Returns
+        -------
+        OpticStudioSystem
+            The new OpticStudioSystem.
+        """
+        if self.Application.Mode == constants.ZOSAPI_Mode.Server:
+            new_system = self.Application.CreateNewSystem(constants.process_constant(constants.SystemType, system_mode))
+            return self._OpticStudioSystem(zos_instance=self, system_instance=new_system)
+
+        raise ValueError("Can only create a new system when using a standalone connection.")
+
+    def get_primary_system(self) -> OpticStudioSystem:
         opticstudiosystem = self.Application.PrimarySystem
         return self._OpticStudioSystem(zos_instance=self, system_instance=opticstudiosystem)
 
-    def get_system(self, pos=0):
-        warnings.warn('ZOS.get_system() has not been tested yet')
+    def get_system(self, pos: int = 0) -> OpticStudioSystem:
+        warnings.warn("ZOS.get_system() has not been tested yet")
         # ToDo test
         opticstudiosystem = self.Application.PrimarySystem.GetSystemAt(pos)
         return self._OpticStudioSystem(zos_instance=self, system_instance=opticstudiosystem)
 
     def licence_check(self):
         pass
```

