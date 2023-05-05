# Comparing `tmp/vspreview-0.4.3.tar.gz` & `tmp/vspreview-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vspreview-0.4.3.tar", last modified: Sun Mar 26 17:41:17 2023, max compression
+gzip compressed data, was "vspreview-0.4.4.tar", last modified: Fri May  5 14:43:20 2023, max compression
```

## Comparing `vspreview-0.4.3.tar` & `vspreview-0.4.4.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.778879 vspreview-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-26 17:40:57.000000 vspreview-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-26 17:41:17.778879 vspreview-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-26 17:40:57.000000 vspreview-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-26 17:41:17.778879 vspreview-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-26 17:40:57.000000 vspreview-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.766879 vspreview-0.4.3/vspreview/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.770879 vspreview-0.4.3/vspreview/api/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/api/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/api/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/api/timecodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.770879 vspreview-0.4.3/vspreview/core/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.770879 vspreview-0.4.3/vspreview/core/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/custom/combobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/custom/dragnavigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/custom/edits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/custom/graphicsview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/custom/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/custom/notch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.774879 vspreview-0.4.3/vspreview/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/types/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/types/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/types/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/types/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    21305 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/types/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/types/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/core/vsenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.774879 vspreview-0.4.3/vspreview/main/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/main/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/main/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/main/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28792 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/main/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.774879 vspreview-0.4.3/vspreview/models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/models/generalmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/models/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/models/picture_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/models/scening.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.774879 vspreview-0.4.3/vspreview/toolbars/
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.774879 vspreview-0.4.3/vspreview/toolbars/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/benchmark/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9279 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/benchmark/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.774879 vspreview-0.4.3/vspreview/toolbars/comp/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/comp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/comp/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/comp/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.774879 vspreview-0.4.3/vspreview/toolbars/debug/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/debug/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/debug/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.774879 vspreview-0.4.3/vspreview/toolbars/main/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/main/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/main/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.774879 vspreview-0.4.3/vspreview/toolbars/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/misc/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/misc/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.778879 vspreview-0.4.3/vspreview/toolbars/pipette/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/pipette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/pipette/colorview.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/pipette/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/pipette/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.778879 vspreview-0.4.3/vspreview/toolbars/playback/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/playback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/playback/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    24853 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/playback/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.778879 vspreview-0.4.3/vspreview/toolbars/scening/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/scening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/scening/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/scening/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/toolbars/scening/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.778879 vspreview-0.4.3/vspreview/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-26 17:40:57.000000 vspreview-0.4.3/vspreview/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:17.770879 vspreview-0.4.3/vspreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-26 17:41:17.000000 vspreview-0.4.3/vspreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-26 17:41:17.000000 vspreview-0.4.3/vspreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:41:17.000000 vspreview-0.4.3/vspreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-26 17:41:17.000000 vspreview-0.4.3/vspreview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:41:10.000000 vspreview-0.4.3/vspreview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-26 17:41:17.000000 vspreview-0.4.3/vspreview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-26 17:41:17.000000 vspreview-0.4.3/vspreview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 14:42:57.000000 vspreview-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-05 14:43:20.431944 vspreview-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-05 14:42:57.000000 vspreview-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 14:43:20.435944 vspreview-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-05 14:42:57.000000 vspreview-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.423944 vspreview-0.4.4/vspreview/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/api/timecodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/core/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/combobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/dragnavigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/edits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/graphicsview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/custom/notch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21321 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/types/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/core/vsenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.427944 vspreview-0.4.4/vspreview/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/main/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/generalmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/picture_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/models/scening.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/benchmark/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9279 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/benchmark/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/comp/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/comp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/comp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20360 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/comp/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/debug/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/debug/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/main/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/main/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/misc/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/misc/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/pipette/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/pipette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/pipette/colorview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/pipette/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/pipette/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/playback/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/playback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/playback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24853 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/playback/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/toolbars/scening/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/scening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/scening/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/scening/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35883 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/toolbars/scening/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.431944 vspreview-0.4.4/vspreview/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-05 14:42:57.000000 vspreview-0.4.4/vspreview/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:20.423944 vspreview-0.4.4/vspreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:43:12.000000 vspreview-0.4.4/vspreview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 14:43:20.000000 vspreview-0.4.4/vspreview.egg-info/top_level.txt
```

### Comparing `vspreview-0.4.3/LICENSE` & `vspreview-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/PKG-INFO` & `vspreview-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.4.3
+Version: 0.4.4
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
```

### Comparing `vspreview-0.4.3/README.md` & `vspreview-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/setup.cfg` & `vspreview-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/setup.py` & `vspreview-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/api/other.py` & `vspreview-0.4.4/vspreview/api/other.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/api/output.py` & `vspreview-0.4.4/vspreview/api/output.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     if isinstance(node, vs.VideoNode):
         title, node_type = 'Clip', vs.VideoNode
     elif isinstance(node, vs.AudioNode):
         title, node_type = 'Audio', vs.AudioNode
     else:
         title, node_type = 'Node', vs.RawNode
 
-    if not name or name is True:
+    if (not name and name is not False) or name is True:
         name = f"{title} {index}"
 
         current_frame = inspect.currentframe()
 
         assert current_frame
         assert current_frame.f_back
```

### Comparing `vspreview-0.4.3/vspreview/core/abstracts.py` & `vspreview-0.4.4/vspreview/core/abstracts.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/bases.py` & `vspreview-0.4.4/vspreview/core/bases.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/custom/combobox.py` & `vspreview-0.4.4/vspreview/core/custom/combobox.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/custom/dragnavigator.py` & `vspreview-0.4.4/vspreview/core/custom/dragnavigator.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/custom/edits.py` & `vspreview-0.4.4/vspreview/core/custom/edits.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/custom/graphicsview.py` & `vspreview-0.4.4/vspreview/core/custom/graphicsview.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/custom/misc.py` & `vspreview-0.4.4/vspreview/core/custom/misc.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/custom/notch.py` & `vspreview-0.4.4/vspreview/core/custom/notch.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/logger.py` & `vspreview-0.4.4/vspreview/core/logger.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/types/audio.py` & `vspreview-0.4.4/vspreview/core/types/audio.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/types/misc.py` & `vspreview-0.4.4/vspreview/core/types/misc.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/types/scene.py` & `vspreview-0.4.4/vspreview/core/types/scene.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/types/units.py` & `vspreview-0.4.4/vspreview/core/types/units.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/types/video.py` & `vspreview-0.4.4/vspreview/core/types/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,15 +387,15 @@
             # we want a contiguous array, so we put in 0, 10 bits the R, 11 to 20 the G and 21 to 30 the B
             # R stays like it is + shift if it's 8 bits (gets applied to all clips), then G gets shifted
             # by 10 bits, (we multiply by 2 ** 10) and same for B but by 20 bits and it all gets summed
             shift = 2 ** (10 - PACKING_TYPE.vs_format.bits_per_sample)
 
             return vs.core.akarin.Expr(
                 clip.std.SplitPlanes(),
-                f'z {1048576 * shift} * y {1024 * shift} * + x {shift} * +', vs.GRAY32, True
+                f'z {shift * 0x100000}  * y {shift * 0x400} * x {shift} * + + 0xc0000000 +', vs.GRAY32, True
             )
 
         return clip
 
     def frame_to_qimage(self, frame: vs.VideoFrame, is_alpha: bool = False) -> QImage:
         from ctypes import POINTER
         from ctypes import cast as ccast
```

### Comparing `vspreview-0.4.3/vspreview/core/types/yaml.py` & `vspreview-0.4.4/vspreview/core/types/yaml.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/core/vsenv.py` & `vspreview-0.4.4/vspreview/core/vsenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from __future__ import annotations
 
+import sys
 import atexit
 import runpy
 from concurrent.futures import Future
 from threading import Lock
 from typing import Any, Callable, TypeVar
 
 from PyQt6.QtCore import QObject, QRunnable, QThreadPool, pyqtSignal
 from vsengine.loops import EventLoop, set_loop  # type: ignore[import]
 from vsengine.policy import GlobalStore, ManagedEnvironment, Policy  # type: ignore[import]
 
 from .logger import get_vs_logger
 
 __all__ = [
+    'PRELOADED_MODULES',
+
     '_monkey_runpy_dicts',
 
     'set_vsengine_loop',
     'get_current_environment',
     'make_environment'
 ]
 
+
+PRELOADED_MODULES = set(sys.modules.values())
+
 _monkey_runpy_dicts = {}
 
 orig_runpy_run_code = runpy._run_code  # type: ignore
 
 
 def _monkey_runpy_func(*args: Any, **kwargs: Any) -> Any:
     glob_dict = orig_runpy_run_code(*args, **kwargs)
```

### Comparing `vspreview-0.4.3/vspreview/init.py` & `vspreview-0.4.4/vspreview/init.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/main/dialog.py` & `vspreview-0.4.4/vspreview/main/dialog.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/main/settings.py` & `vspreview-0.4.4/vspreview/main/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/main/timeline.py` & `vspreview-0.4.4/vspreview/main/timeline.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/main/window.py` & `vspreview-0.4.4/vspreview/main/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 import io
 import logging
 import sys
 from fractions import Fraction
+from importlib import reload as reload_module
 from pathlib import Path
+from pkgutil import iter_modules
+from time import time
 from typing import Any, Iterable, Mapping, cast
 
 import vapoursynth as vs
 from PyQt6.QtCore import QByteArray, QEvent, QRectF, pyqtSignal
 from PyQt6.QtGui import QCloseEvent, QColorSpace, QMoveEvent, QPalette, QPixmap, QShowEvent
 from PyQt6.QtOpenGLWidgets import QOpenGLWidget
 from PyQt6.QtWidgets import QApplication, QGraphicsScene, QGraphicsView, QLabel, QMainWindow, QSizePolicy
 from vsengine import vpy  # type: ignore
 
 from ..core import (
-    AbstractQItem, DragNavigator, ExtendedWidget, Frame, GraphicsImageItem, GraphicsView, QAbstractYAMLObjectSingleton,
-    StatusBar, Time, Timer, VBoxLayout, VideoOutput, ViewMode, _monkey_runpy_dicts, get_current_environment,
-    make_environment, try_load
+    PRELOADED_MODULES, AbstractQItem, DragNavigator, ExtendedWidget, Frame, GraphicsImageItem, GraphicsView,
+    QAbstractYAMLObjectSingleton, StatusBar, Time, Timer, VBoxLayout, VideoOutput, ViewMode, _monkey_runpy_dicts,
+    get_current_environment, make_environment, try_load
 )
 from ..models import VideoOutputs
 from ..toolbars import Toolbars
 from ..utils import fire_and_forget, set_status_label
 from .dialog import ScriptErrorDialog, SettingsDialog
 from .settings import MainSettings, WindowSettings
 from .timeline import Timeline
@@ -99,14 +102,16 @@
         self.current_config_dir = config_dir / self.VSP_DIR_NAME
         self.global_config_dir = self.VSP_GLOBAL_DIR_NAME / self.VSP_DIR_NAME
         self.global_storage_path = self.global_config_dir / '.global.yml'
 
         self.app = cast(QApplication, QApplication.instance())
         assert self.app
 
+        self.last_reload_time = time()
+
         if self.settings.dark_theme_enabled:
             try:
                 from qdarkstyle import _load_stylesheet  # type: ignore[import]
             except ImportError:
                 self.settings.dark_theme_enabled = False
             else:
                 self.app.setStyleSheet(self.patch_dark_stylesheet(_load_stylesheet(qt_api='pyqt6')))
@@ -239,14 +244,61 @@
         try:
             argv_orig = sys.argv
             sys.argv = [script_path.name]
         except AttributeError:
             pass
 
         try:
+            if reloading:
+                std_path_lib = Path(logging.__file__).parent.parent
+                std_path_dlls = std_path_lib.parent / 'DLLs'
+
+                for module in set(sys.modules.values()) - PRELOADED_MODULES:
+                    if not hasattr(module, '__file__') or module.__file__ is None:
+                        continue
+
+                    mod_file = Path(module.__file__)
+
+                    if 'vspreview' in mod_file.parts:
+                        continue
+
+                    if std_path_lib in mod_file.parents or std_path_dlls in mod_file.parents:
+                        continue
+
+                    if not mod_file.exists() or not mod_file.is_file():
+                        continue
+
+                    parent = Path(module.__file__)
+
+                    def _traverse(path: Path) -> Iterable[bool]:
+                        for module in iter_modules([path]):
+                            newpath = Path(module.module_finder) / module.name
+
+                            if module.ispkg:
+                                if _traverse([newpath]):
+                                    return True
+
+                                continue
+
+                            newpath = newpath.with_suffix('.py')
+
+                            try:
+                                stats = newpath.stat()
+                            except FileNotFoundError:
+                                return False
+
+                            return stats.st_mtime > self.last_reload_time
+
+                    if _traverse(parent):
+                        try:
+                            logging.debug(f'Hot reloaded Python Package: "{module.__name__}"')
+                            reload_module(module)
+                        except Exception as e:
+                            logging.error(e)
+
             self.env = vpy.variables(
                 dict(self.external_args),
                 environment=vs.get_current_environment(),
                 module_name="__vspreview__"
             ).result()
             self.env.module.__dict__['_monkey_runpy'] = random()
             self.env = vpy.script(script_path, environment=self.env).result()
@@ -264,14 +316,15 @@
                     str(e), 'See console output for details.'
                 ])
             )
         finally:
             if argv_orig is not None:
                 sys.argv = argv_orig
             sys.path.pop()
+            self.last_reload_time = time()
 
         if len(vs.get_outputs()) == 0:
             logging.error('Script has no outputs set.')
             self.script_exec_failed = True
             self.handle_script_error('Script has no outputs set.')
             return
 
@@ -348,16 +401,17 @@
                     storage_contents += storage_file.read()
                     storage_contents += '\n'
 
                     if i == 0:
                         global_length = storage_contents.count('\n')
             except FileNotFoundError:
                 if self.settings.force_old_storages_removal or i == 0:
-                    storage_path.unlink()
-                    broken_storage = True
+                    if storage_path.exists():
+                        storage_path.unlink()
+                        broken_storage = True
                 else:
                     logging.warning(
                         '\n\tThe storage was created on an old version of VSPreview.'
                         '\n\tSave any scening or other important info and delete it.'
                         '\n\tIf you want the program to silently delete old storages, go into settings.'
                     )
                     sys.exit(1)
```

### Comparing `vspreview-0.4.3/vspreview/models/generalmodel.py` & `vspreview-0.4.4/vspreview/models/generalmodel.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/models/outputs.py` & `vspreview-0.4.4/vspreview/models/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         self.items = list(self._items)
 
     def switchToFFTSpectrumView(self, force_cache: bool = False) -> None:
         try:
             from vsdfft.spectrum import FFTSpectrum
         except ModuleNotFoundError:
             raise RuntimeError(
-                'vspreview: You can\'t chage to this view mode. You\'re missing the `vsdfft` package!'
+                'vspreview: You can\'t change to this view mode. You\'re missing the `vsdfft` package!'
             )
 
         if not self._fft_spectr_items or force_cache:
             max_width = max(*(x.width for x in self._items), 140)
             max_height = max(*(x.height for x in self._items), 140)
 
             self._fft_spectr_items = [
```

### Comparing `vspreview-0.4.3/vspreview/models/picture_types.py` & `vspreview-0.4.4/vspreview/models/picture_types.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/models/scening.py` & `vspreview-0.4.4/vspreview/models/scening.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/__init__.py` & `vspreview-0.4.4/vspreview/toolbars/__init__.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/benchmark/settings.py` & `vspreview-0.4.4/vspreview/toolbars/benchmark/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/benchmark/toolbar.py` & `vspreview-0.4.4/vspreview/toolbars/benchmark/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/comp/settings.py` & `vspreview-0.4.4/vspreview/toolbars/comp/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/comp/toolbar.py` & `vspreview-0.4.4/vspreview/toolbars/comp/toolbar.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,57 @@
     AbstractToolbar, CheckBox, ComboBox, FrameEdit, LineEdit, PictureType, ProgressBar, PushButton, VideoOutput,
     main_window
 )
 from ...models import PictureTypes
 from .settings import CompSettings
 
 if TYPE_CHECKING:
+    from requests import Session
+
     from ...main import MainWindow
 
 
 __all__ = [
     'CompToolbar'
 ]
 
 
 _MAX_ATTEMPTS_PER_PICTURE_TYPE: Final[int] = 50
 
 
+def _get_slowpic_headers(content_length: int, content_type: str, sess: Session) -> dict[str, str]:
+    return {
+        "Content-Length": str(content_length),
+        "Content-Type": content_type,
+        "Access-Control-Allow-Origin": "*",
+        "Origin": "https://slow.pics/",
+        "Referer": "https://slow.pics/comparison",
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/112.0",
+        "X-XSRF-TOKEN": sess.cookies.get_dict()["XSRF-TOKEN"]
+    }
+
+
+def _do_single_slowpic_upload(sess: Session, collection: str, imageUuid: str, image: Path, browser_id: str) -> None:
+    from uuid import uuid4
+
+    from requests_toolbelt import MultipartEncoder  # type: ignore
+
+    upload_info = MultipartEncoder({
+        "collectionUuid": collection,
+        "imageUuid": imageUuid,
+        "file": (image.name, image.read_bytes(), 'image/png'),
+        'browserId': browser_id,
+    }, str(uuid4()))
+
+    sess.post(
+        'https://slow.pics/upload/image', data=upload_info.to_string(),
+        headers=_get_slowpic_headers(upload_info.len, upload_info.content_type, sess)
+    )
+
+
 def select_frames(clip: vs.VideoNode, indices: list[int]) -> vs.VideoNode:
     return clip.std.BlankClip(length=len(indices)).std.FrameEval(lambda n: clip[indices[n]])
 
 
 def clear_filename(filename: str) -> str:
     import re
     import unicodedata
@@ -40,15 +72,15 @@
         'CON', 'PRN', 'AUX', 'NUL', 'COM1', 'COM2', 'COM3', 'COM4', 'COM5',
         'COM6', 'COM7', 'COM8', 'COM9', 'LPT1', 'LPT2', 'LPT3', 'LPT4', 'LPT5',
         'LPT6', 'LPT7', 'LPT8', 'LPT9',
     ]
 
     filename = ''.join(c for c in filename if c not in blacklist)
 
-    # Remove all charcters below code point 32
+    # Remove all characters below code point 32
     filename = ''.join(c for c in filename if 31 < ord(c))
     filename = unicodedata.normalize('NFKD', filename).rstrip('. ').strip()
 
     if all([x == '.' for x in filename]):
         filename = '__' + filename
 
     if filename in reserved:
@@ -107,14 +139,16 @@
 
     def isFinished(self) -> bool:
         return self.is_finished
 
     def run(self, conf: WorkerConfiguration) -> None:
         import os
         import shutil
+        from concurrent.futures import ThreadPoolExecutor
+        from uuid import uuid4
 
         try:
             from requests import Session
             from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor  # type: ignore
         except ModuleNotFoundError:
             raise ModuleNotFoundError(
                 'You are missing `requests` and `requests` toolbelt!\n'
@@ -157,78 +191,88 @@
                 if self.isFinished():
                     raise StopIteration
 
                 all_images.append(sorted(path_images))
         except StopIteration:
             return self.finished.emit()
 
+        total_images = 0
         fields = dict[str, Any]()
-
         for i, (output, images) in enumerate(zip(conf.outputs, all_images)):
             if self.isFinished():
                 return self.finished.emit()
             for j, (image, frame) in enumerate(zip(images, conf.frames)):
                 if self.isFinished():
                     return self.finished.emit()
                 fields[f'comparisons[{j}].name'] = str(frame)
-                fields[f'comparisons[{j}].images[{i}].name'] = output.name
-                fields[f'comparisons[{j}].images[{i}].file'] = (image.name, image.read_bytes(), 'image/png')
+                fields[f'comparisons[{j}].imageNames[{i}]'] = output.name
+                total_images += 1
 
         self.progress_status.emit('upload', 0, 0)
 
         with Session() as sess:
-            sess.get('https://slow.pics/api/comparison')
+            sess.get('https://slow.pics/comparison')
             if self.isFinished():
                 return self.finished.emit()
+
+            browser_id = str(uuid4())
+
             head_conf = {
                 'collectionName': conf.collection_name,
-                'public': str(conf.public).lower(),
-                'optimizeImages': str(conf.optimise).lower(),
                 'hentai': str(conf.nsfw).lower(),
+                'optimizeImages': str(conf.optimise).lower(),
+                'browserId': browser_id,
+                'public': str(conf.public).lower(),
             }
             if conf.remove_after is not None:
                 head_conf |= {'removeAfter': str(conf.remove_after)}
 
             def _monitor_cb(monitor: MultipartEncoderMonitor) -> None:
                 self._progress_update_func(monitor.bytes_read, monitor.len)
-
-            files = MultipartEncoder(head_conf | fields)
+            files = MultipartEncoder(head_conf | fields, str(uuid4()))
             monitor = MultipartEncoderMonitor(files, _monitor_cb)
-
-            response = sess.post(
-                'https://slow.pics/api/comparison',
-                cast(bytes, monitor.to_string()),
-                headers={
-                    "Accept": "*/*",
-                    "Accept-Encoding": "gzip, deflate, br",
-                    "Accept-Language": "en-US,en;q=0.5",
-                    "Content-Length": str(files.len),
-                    "Content-Type": files.content_type,
-                    "Origin": "https://slow.pics/",
-                    "Referer": "https://slow.pics/comparison",
-                    "Sec-Fetch-Mode": "cors",
-                    "Sec-Fetch-Site": "same-origin",
-                    "User-Agent": (
-                        "Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
-                        "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
-                    ),
-                    "X-XSRF-TOKEN": sess.cookies.get_dict()["XSRF-TOKEN"]  # noqa
-                }
-            )
-
+            comp_response = sess.post(
+                'https://slow.pics/upload/comparison', data=monitor.to_string(),
+                headers=_get_slowpic_headers(monitor.len, monitor.content_type, sess)
+            ).json()
+            collection = comp_response["collectionUuid"]
+            key = comp_response["key"]
+            image_ids = comp_response["images"]
+            images_done = 0
+            self._progress_update_func(0, total_images)
+            with ThreadPoolExecutor() as executor:
+                futures = []
+                for i, (output, images) in enumerate(zip(conf.outputs, all_images)):
+                    for j, (image, frame) in enumerate(zip(images, conf.frames)):
+                        if self.isFinished():
+                            return self.finished.emit()
+                        while len(futures) >= 5:
+                            for future in futures:
+                                if future.done():
+                                    futures.remove(future)
+                                    images_done += 1
+                                    self._progress_update_func(images_done, total_images)
+
+                        futures.append(
+                            executor.submit(
+                                _do_single_slowpic_upload,
+                                sess=sess, collection=collection, imageUuid=image_ids[j][i],
+                                image=image, browser_id=browser_id
+                            )
+                        )
+            self._progress_update_func(total_images, total_images)
         if conf.delete_cache:
             shutil.rmtree(conf.path, True)
 
-        url = f'https://slow.pics/c/{response.text}'
+        url = f'https://slow.pics/c/{key}'
 
         self.progress_status.emit(url, 0, 0)
 
         url_out = (
-            conf.path.parent / 'Old Comps'
-            / clear_filename(f'{conf.collection_name} - {response.text}')
+            conf.path.parent / 'Old Comps' / clear_filename(f'{conf.collection_name} - {key}')
         ).with_suffix('.url')
         url_out.parent.mkdir(parents=True, exist_ok=True)
         url_out.touch(exist_ok=True)
         url_out.write_text(f'[InternetShortcut]\nURL={url}')
 
         self.finished.emit()
 
@@ -454,21 +498,23 @@
 
         if len(frames):
             samples.extend(frames)
 
         if self.current_frame_checkbox.isChecked():
             samples.append(int(self.main.current_output.last_showed_frame))
 
-        collection_name = self.collection_name_lineedit.text()
+        collection_name = self.collection_name_lineedit.text().strip()
 
         if not collection_name:
             collection_name = self.settings.DEFAULT_COLLECTION_NAME
 
         if not collection_name:
             raise ValueError('You have to put a collection name!')
+        elif 5 > len(collection_name):
+            raise ValueError('Your collection name is too short!')
 
         collection_name = collection_name.format(
             script_name=self.main.script_path.stem
         )
 
         sample_frames = list(sorted(set(samples)))
```

### Comparing `vspreview-0.4.3/vspreview/toolbars/debug/toolbar.py` & `vspreview-0.4.4/vspreview/toolbars/debug/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/main/dialog.py` & `vspreview-0.4.4/vspreview/toolbars/main/dialog.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/main/toolbar.py` & `vspreview-0.4.4/vspreview/toolbars/main/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/misc/toolbar.py` & `vspreview-0.4.4/vspreview/toolbars/misc/toolbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,16 @@
         self.autosave_checkbox = CheckBox('Autosave', self, checked=True)
 
         self.copy_frame_button = PushButton('Copy Frame', self, clicked=self.copy_frame_to_clipboard)
 
         self.save_frame_as_button = PushButton('Save Frame as', self, clicked=self.on_save_frame_as_clicked)
 
         self.save_template_lineedit = LineEdit(
-            self.settings.SAVE_TEMPLATE, self, tooltip='''
+            self.settings.SAVE_TEMPLATE, self, text=self.settings.SAVE_TEMPLATE,
+            tooltip='''
                 Available placeholders:
                     {format}, {fps_den}, {fps_num}, {frame},
                     {height}, {index}, {matrix}, {primaries}, {range},
                     {script_name}, {total_frames}, {transfer}, {width}.
                 Frame props can be accessed as well using their names.
             '''.replace(' ' * 16, ' ').strip()
         )
```

### Comparing `vspreview-0.4.3/vspreview/toolbars/pipette/colorview.py` & `vspreview-0.4.4/vspreview/toolbars/pipette/colorview.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/pipette/toolbar.py` & `vspreview-0.4.4/vspreview/toolbars/pipette/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/playback/settings.py` & `vspreview-0.4.4/vspreview/toolbars/playback/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/playback/toolbar.py` & `vspreview-0.4.4/vspreview/toolbars/playback/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/scening/dialog.py` & `vspreview-0.4.4/vspreview/toolbars/scening/dialog.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/scening/settings.py` & `vspreview-0.4.4/vspreview/toolbars/scening/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/toolbars/scening/toolbar.py` & `vspreview-0.4.4/vspreview/toolbars/scening/toolbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,15 +480,15 @@
         cue_sheet.parse()
 
         for track in cue_sheet.tracks:
             if track.offset is None:
                 continue
             offset = offset_to_time(track.offset)
             if offset is None:
-                logging.warning(f"Scening import: INDEX timestamp '{track.offset}' format isn't suported.")
+                logging.warning(f"Scening import: INDEX timestamp '{track.offset}' format isn't supported.")
                 continue
             start = Frame(offset)
 
             end = None
             if track.duration is not None:
                 end = Frame(offset + Time(track.duration))
 
@@ -550,15 +550,15 @@
         from xml.etree import ElementTree
 
         timestamp_pattern = re.compile(r'(\d{2}):(\d{2}):(\d{2}(?:\.\d{3})?)')
 
         try:
             root = ElementTree.parse(str(path)).getroot()
         except ElementTree.ParseError as exc:
-            logging.warning(f"Scening import: error occured while parsing '{path.name}':")
+            logging.warning(f"Scening import: error occurred while parsing '{path.name}':")
             logging.warning(exc.msg)
             return
         for chapter in root.iter('ChapterAtom'):
             start_element = chapter.find('ChapterTimeStart')
             if start_element is None or start_element.text is None:
                 continue
             match = timestamp_pattern.match(start_element.text)
```

### Comparing `vspreview-0.4.3/vspreview/utils/debug.py` & `vspreview-0.4.4/vspreview/utils/debug.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview/utils/utils.py` & `vspreview-0.4.4/vspreview/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.4.3/vspreview.egg-info/PKG-INFO` & `vspreview-0.4.4/vspreview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.4.3
+Version: 0.4.4
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
```

### Comparing `vspreview-0.4.3/vspreview.egg-info/SOURCES.txt` & `vspreview-0.4.4/vspreview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

