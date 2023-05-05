# Comparing `tmp/vot-toolkit-0.5.3.tar.gz` & `tmp/vot-toolkit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vot-toolkit-0.5.3.tar", last modified: Fri Mar 25 11:28:54 2022, max compression
+gzip compressed data, was "vot-toolkit-0.6.0.tar", last modified: Fri May  5 11:13:24 2023, max compression
```

## Comparing `vot-toolkit-0.5.3.tar` & `vot-toolkit-0.6.0.tar`

### file list

```diff
@@ -1,105 +1,119 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.884220 vot-toolkit-0.5.3/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      211 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/MANIFEST.in
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3254 2022-03-25 11:28:54.884220 vot-toolkit-0.5.3/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2396 2022-03-11 09:30:24.000000 vot-toolkit-0.5.3/README.md
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      272 2022-03-11 09:29:31.000000 vot-toolkit-0.5.3/requirements.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2022-03-25 11:28:54.884220 vot-toolkit-0.5.3/setup.cfg
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/setup.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.856220 vot-toolkit-0.5.3/vot/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1867 2021-04-20 09:19:05.000000 vot-toolkit-0.5.3/vot/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      158 2021-04-20 09:19:05.000000 vot-toolkit-0.5.3/vot/__main__.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.856220 vot-toolkit-0.5.3/vot/analysis/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15786 2022-03-11 09:29:31.000000 vot-toolkit-0.5.3/vot/analysis/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21026 2021-06-16 14:19:04.000000 vot-toolkit-0.5.3/vot/analysis/_processor.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5845 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/analysis/basic.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12235 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/analysis/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8935 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/analysis/supervised.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8811 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/analysis/tpr.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.860220 vot-toolkit-0.5.3/vot/dataset/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15742 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/dataset/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/vot/dataset/cow.png
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2707 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/dataset/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5251 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/dataset/got10k.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11416 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/dataset/otb.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4216 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/dataset/proxy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3644 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/dataset/trackingnet.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10300 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/dataset/vot.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.864220 vot-toolkit-0.5.3/vot/document/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12139 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/document/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/vot/document/commands.tex
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5248 2022-03-11 09:29:31.000000 vot-toolkit-0.5.3/vot/document/common.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5217 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/document/html.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/vot/document/jquery.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5748 2022-03-11 09:29:31.000000 vot-toolkit-0.5.3/vot/document/latex.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/vot/document/pure.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      647 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/vot/document/report.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/vot/document/report.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/vot/document/table.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2022-03-23 08:48:42.000000 vot-toolkit-0.5.3/vot/document/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.864220 vot-toolkit-0.5.3/vot/experiment/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6255 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/experiment/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5347 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/experiment/multirun.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3083 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/experiment/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2648 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/experiment/transformer.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.868220 vot-toolkit-0.5.3/vot/region/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2398 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/region/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6517 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/region/io.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9101 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/region/raster.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10212 2022-03-11 09:29:31.000000 vot-toolkit-0.5.3/vot/region/shapes.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1006 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/vot/region/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.876220 vot-toolkit-0.5.3/vot/stack/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3059 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      253 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/otb100.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      251 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/otb50.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      625 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/testing.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      863 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      301 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/vot2013.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      324 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/vot2014.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      355 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/vot2015.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      493 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/vot2016.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      809 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/vot2017.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      747 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/vot2018.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      745 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/vot2019.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      817 2021-04-19 11:27:09.000000 vot-toolkit-0.5.3/vot/stack/vot2020.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      817 2021-04-20 09:19:05.000000 vot-toolkit-0.5.3/vot/stack/vot2021.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.876220 vot-toolkit-0.5.3/vot/stack/vot2022/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      566 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/vot2022/depth.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/vot2022/lt.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/vot2022/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/vot2022/stb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/stack/vot2022/sts.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      438 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/votlt2019.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      438 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/votlt2020.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      438 2021-04-20 09:19:05.000000 vot-toolkit-0.5.3/vot/stack/votlt2021.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      258 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/votrgbd2019.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      258 2021-04-19 11:27:22.000000 vot-toolkit-0.5.3/vot/stack/votrgbd2020.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      258 2021-04-20 09:19:05.000000 vot-toolkit-0.5.3/vot/stack/votrgbd2021.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      347 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/votrgbtir2020.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      259 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/vottir2015.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      259 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/stack/vottir2016.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.880220 vot-toolkit-0.5.3/vot/tracker/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14894 2022-03-11 09:30:24.000000 vot-toolkit-0.5.3/vot/tracker/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      694 2021-04-20 09:19:05.000000 vot-toolkit-0.5.3/vot/tracker/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4770 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/tracker/results.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      476 2021-04-20 09:19:05.000000 vot-toolkit-0.5.3/vot/tracker/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    18671 2022-03-11 09:30:24.000000 vot-toolkit-0.5.3/vot/tracker/trax.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.880220 vot-toolkit-0.5.3/vot/utilities/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12416 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/utilities/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15501 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/utilities/cli.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2635 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/utilities/data.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8255 2021-04-15 12:10:29.000000 vot-toolkit-0.5.3/vot/utilities/draw.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3609 2020-12-04 15:25:26.000000 vot-toolkit-0.5.3/vot/utilities/migration.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3798 2021-04-20 09:19:05.000000 vot-toolkit-0.5.3/vot/utilities/net.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8133 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/utilities/notebook.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2022-03-25 11:28:05.000000 vot-toolkit-0.5.3/vot/version.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.880220 vot-toolkit-0.5.3/vot/workspace/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6879 2022-03-11 09:29:31.000000 vot-toolkit-0.5.3/vot/workspace/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10073 2022-03-11 09:29:31.000000 vot-toolkit-0.5.3/vot/workspace/storage.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1782 2022-03-11 09:29:31.000000 vot-toolkit-0.5.3/vot/workspace/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2022-03-25 11:28:54.884220 vot-toolkit-0.5.3/vot_toolkit.egg-info/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3254 2022-03-25 11:28:54.000000 vot-toolkit-0.5.3/vot_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2131 2022-03-25 11:28:54.000000 vot-toolkit-0.5.3/vot_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2022-03-25 11:28:54.000000 vot-toolkit-0.5.3/vot_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2022-03-25 11:28:54.000000 vot-toolkit-0.5.3/vot_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      273 2022-03-25 11:28:54.000000 vot-toolkit-0.5.3/vot_toolkit.egg-info/requires.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2022-03-25 11:28:54.000000 vot-toolkit-0.5.3/vot_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.603696 vot-toolkit-0.6.0/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      211 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/MANIFEST.in
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-05 11:13:24.603696 vot-toolkit-0.6.0/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2716 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/README.md
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/requirements.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2023-05-05 11:13:24.603696 vot-toolkit-0.6.0/setup.cfg
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-05 11:11:52.000000 vot-toolkit-0.6.0/setup.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.575696 vot-toolkit-0.6.0/vot/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1867 2021-04-20 09:19:05.000000 vot-toolkit-0.6.0/vot/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      158 2021-04-20 09:19:05.000000 vot-toolkit-0.6.0/vot/__main__.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.579696 vot-toolkit-0.6.0/vot/analysis/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15920 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21427 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/_processor.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7608 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/accuracy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2517 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/failures.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16706 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/longterm.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12235 2023-04-18 14:33:10.000000 vot-toolkit-0.6.0/vot/analysis/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8824 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/analysis/supervised.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.579696 vot-toolkit-0.6.0/vot/dataset/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16723 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/dataset/cow.png
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3079 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5356 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/got10k.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11511 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/otb.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4924 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/proxy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3753 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/trackingnet.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9243 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/dataset/vot.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.583696 vot-toolkit-0.6.0/vot/document/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12362 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/document/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/commands.tex
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5273 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/document/common.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5217 2021-04-15 12:10:29.000000 vot-toolkit-0.6.0/vot/document/html.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/jquery.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5748 2022-03-11 09:29:31.000000 vot-toolkit-0.6.0/vot/document/latex.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/pure.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      647 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/report.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/report.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/document/table.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2022-03-23 08:48:42.000000 vot-toolkit-0.6.0/vot/document/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.583696 vot-toolkit-0.6.0/vot/experiment/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7508 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      798 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/helpers.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7180 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/multirun.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3044 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3214 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/experiment/transformer.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.587696 vot-toolkit-0.6.0/vot/region/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2373 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8674 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/io.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9593 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/raster.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10172 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/shapes.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/region/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.587696 vot-toolkit-0.6.0/vot/stack/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3047 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      253 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/otb100.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      251 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/otb50.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/tests/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      183 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/tests/basic.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      550 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/tests/multiobject.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/tests/segmentation.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      863 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2013.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2014.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2015/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2015/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2015/tir.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2016/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      540 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2016/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2016/tir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2017.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2018/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2018/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2018/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2019/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2019/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2019/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2019/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2019/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2020/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2020/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2020/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2020/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2020/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.591696 vot-toolkit-0.6.0/vot/stack/vot2021/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2021/lt.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2021/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2021/st.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.595696 vot-toolkit-0.6.0/vot/stack/vot2022/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/stack/vot2022/depth.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/vot2022/lt.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/vot2022/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/vot2022/stb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/stack/vot2022/sts.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      388 2023-05-04 11:42:13.000000 vot-toolkit-0.6.0/vot/stack/vots2023.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.595696 vot-toolkit-0.6.0/vot/tracker/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19651 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/tracker/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      763 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/tracker/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6642 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/tracker/results.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      476 2021-04-20 09:19:05.000000 vot-toolkit-0.6.0/vot/tracker/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19771 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/tracker/trax.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.599696 vot-toolkit-0.6.0/vot/utilities/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12508 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/utilities/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16157 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/utilities/cli.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2635 2021-04-15 12:10:29.000000 vot-toolkit-0.6.0/vot/utilities/data.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8255 2021-04-15 12:10:29.000000 vot-toolkit-0.6.0/vot/utilities/draw.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3609 2020-12-04 15:25:26.000000 vot-toolkit-0.6.0/vot/utilities/migration.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3798 2021-04-20 09:19:05.000000 vot-toolkit-0.6.0/vot/utilities/net.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8133 2022-03-25 11:28:05.000000 vot-toolkit-0.6.0/vot/utilities/notebook.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/version.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.599696 vot-toolkit-0.6.0/vot/workspace/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7013 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/workspace/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10512 2023-05-05 11:01:43.000000 vot-toolkit-0.6.0/vot/workspace/storage.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1782 2022-03-11 09:29:31.000000 vot-toolkit-0.6.0/vot/workspace/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-05 11:13:24.603696 vot-toolkit-0.6.0/vot_toolkit.egg-info/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2409 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2023-05-05 11:13:24.000000 vot-toolkit-0.6.0/vot_toolkit.egg-info/top_level.txt
```

### Comparing `vot-toolkit-0.5.3/PKG-INFO` & `vot-toolkit-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.5.3
+Version: 0.6.0
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         The VOT evaluation toolkit
         ==========================
         
         This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
         
-        For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://service.ait.ac.at/mailman/listinfo/votchallenge) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
+        For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
         
         Developers
         ----------
         
-        * [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana (lead developer)
+        The VOT toolkit is developed and maintained by  [Luka Čehovin Zajc](https://vicos.si/lukacu) with the help of the VOT innitiative members and the VOT community.
+        
+        Contributors:
+        
+        * [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana
         * [Alan Lukežič](https://vicos.si/people/alan_lukezic/), University of Ljubljana
         * Yan Song, Tampere University
         
+        Acknowledgements
+        ----------------
+        
+        The development of this package was supported by Sloveninan research agency (ARRS) projects Z2-1866 and J2-316.
+        
         License
         -------
         
         Copyright (C) 2021 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
         
         This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
         
@@ -39,9 +48,9 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `vot-toolkit-0.5.3/README.md` & `vot-toolkit-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 
 The VOT evaluation toolkit
 ==========================
 
 This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
 
-For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://service.ait.ac.at/mailman/listinfo/votchallenge) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
+For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
 
 Developers
 ----------
 
-* [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana (lead developer)
+The VOT toolkit is developed and maintained by  [Luka Čehovin Zajc](https://vicos.si/lukacu) with the help of the VOT innitiative members and the VOT community.
+
+Contributors:
+
+* [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana
 * [Alan Lukežič](https://vicos.si/people/alan_lukezic/), University of Ljubljana
 * Yan Song, Tampere University
 
+Acknowledgements
+----------------
+
+The development of this package was supported by Sloveninan research agency (ARRS) projects Z2-1866 and J2-316.
+
 License
 -------
 
 Copyright (C) 2021 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
```

### Comparing `vot-toolkit-0.5.3/setup.py` & `vot-toolkit-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,13 +31,13 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     entry_points={
         'console_scripts': ['vot=vot.utilities.cli:main'],
     },
 )
```

### Comparing `vot-toolkit-0.5.3/vot/__init__.py` & `vot-toolkit-0.6.0/vot/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/analysis/__init__.py` & `vot-toolkit-0.6.0/vot/analysis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 from vot.utilities.data import Grid
 
 analysis_registry = ClassRegistry("vot_analysis")
 
 class MissingResultsException(ToolkitException):
     """Exception class that denotes missing results during analysis
     """
-    pass
-
+    def __init__(self, *args: object) -> None:
+        if not args:
+            args = ["Missing results"]
+        super().__init__(*args)
+        
 class Sorting(Enum):
     """Sorting direction enumeration class
     """
     UNSORTABLE = auto()
     DESCENDING = auto()
     ASCENDING = auto()
 
@@ -425,10 +428,9 @@
 
 def is_special(region: Region, code=None) -> bool:
     if code is None:
         return region.type == RegionType.SPECIAL
     return region.type == RegionType.SPECIAL and region.code == code
 
 from ._processor import process_stack_analyses, AnalysisProcessor, AnalysisError
-
-for module in ["vot.analysis.multistart", "vot.analysis.supervised", "vot.analysis.basic", "vot.analysis.tpr"]:
-    importlib.import_module(module)
+for module in [".multistart", ".supervised", ".accuracy", ".failures", ".longterm"]:
+    importlib.import_module(module, package="vot.analysis")
```

### Comparing `vot-toolkit-0.5.3/vot/analysis/_processor.py` & `vot-toolkit-0.6.0/vot/analysis/_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 
 import logging
+import sys
 import threading
-from collections import Iterable, OrderedDict, namedtuple
+from collections import OrderedDict, namedtuple
+if sys.version_info >= (3, 3):
+    from collections.abc import Iterable
+else:
+    from collections import Iterable
 from functools import partial
 from typing import List, Union, Mapping, Tuple, Any
 from concurrent.futures import Executor, Future, ThreadPoolExecutor
 from threading import RLock, Condition
 from queue import Queue, Empty
 
 from cachetools import Cache
@@ -603,36 +608,37 @@
 
 def process_stack_analyses(workspace: "Workspace", trackers: List[Tracker]):
 
     processor = AnalysisProcessor.default()
 
     results = dict()
     condition = Condition()
+    errors = []
 
     def insert_result(container: dict, key):
         def insert(future: Future):
             try:
                 container[key] = future.result()
             except AnalysisError as e:
-                e.print(logger)
+                errors.append(e)
             except Exception as e:
                 logger.exception(e)
             with condition:
                 condition.notify()
         return insert
 
     for experiment in workspace.stack:
 
         logger.debug("Traversing experiment %s", experiment.identifier)
 
         experiment_results = dict()
 
         results[experiment] = experiment_results
 
-        sequences = [experiment.transform(sequence) for sequence in workspace.dataset]
+        sequences = experiment.transform(workspace.dataset)
 
         for analysis in experiment.analyses:
 
             if not analysis.compatible(experiment):
                 continue
 
             logger.debug("Traversing analysis %s", class_fullname(analysis))
@@ -661,8 +667,16 @@
 
         except KeyboardInterrupt:
             processor.cancel()
             progress.close()
             logger.info("Analysis interrupted by user, aborting.")
             return None
 
+    if len(errors) > 0:
+        logger.info("Errors occured during analysis, incomplete.")
+        for e in errors:
+            logger.info("Failed task {}: {}".format(e.task, e.root_cause))
+            if logger.isEnabledFor(logging.DEBUG):
+                e.print(logger)
+        return None
+
     return results
```

### Comparing `vot-toolkit-0.5.3/vot/analysis/basic.py` & `vot-toolkit-0.6.0/vot/analysis/accuracy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,61 @@
 from typing import List, Tuple, Any
 
 import numpy as np
 
-from attributee import Boolean, Integer, Include
+from attributee import Boolean, Integer, Include, Float
 
 from vot.analysis import (Measure,
                           MissingResultsException,
                           SequenceAggregator, Sorting,
                           is_special, SeparableAnalysis,
-                          analysis_registry)
+                          analysis_registry, Curve)
 from vot.dataset import Sequence
 from vot.experiment import Experiment
-from vot.experiment.multirun import (MultiRunExperiment, SupervisedExperiment)
-from vot.region import Region, Special, calculate_overlaps
-from vot.tracker import Tracker
+from vot.experiment.multirun import (MultiRunExperiment)
+from vot.region import Region, calculate_overlaps
+from vot.tracker import Tracker, Trajectory
 from vot.utilities.data import Grid
 
-def compute_accuracy(trajectory: List[Region], sequence: Sequence, burnin: int = 10, 
-    ignore_unknown: bool = True, bounded: bool = True) -> float:
+def gather_overlaps(trajectory: List[Region], groundtruth: List[Region], burnin: int = 10, 
+    ignore_unknown: bool = True, ignore_invisible: bool = False, bounds = None, threshold: float = None) -> float:
 
-    overlaps = np.array(calculate_overlaps(trajectory, sequence.groundtruth(), (sequence.size) if bounded else None))
+    overlaps = np.array(calculate_overlaps(trajectory, groundtruth, bounds))
     mask = np.ones(len(overlaps), dtype=bool)
 
-    for i, region in enumerate(trajectory):
-        if is_special(region, Special.UNKNOWN) and ignore_unknown:
+    if threshold is None: threshold = -1
+
+    for i, (region_tr, region_gt) in enumerate(zip(trajectory, groundtruth)):
+        # Skip if groundtruth is unknown
+        if is_special(region_gt, Sequence.UNKNOWN):
+            mask[i] = False
+        elif ignore_invisible and region_gt.is_empty():
+            mask[i] = False
+        # Skip if predicted is unknown
+        elif is_special(region_tr, Trajectory.UNKNOWN) and ignore_unknown:
             mask[i] = False
-        elif is_special(region, Special.INITIALIZATION):
+        # Skip if predicted is initialization frame
+        elif is_special(region_tr, Trajectory.INITIALIZATION):
             for j in range(i, min(len(trajectory), i + burnin)):
                 mask[j] = False
-        elif is_special(region, Special.FAILURE):
+        elif is_special(region_tr, Trajectory.FAILURE):
+            mask[i] = False
+        elif overlaps[i] <= threshold:
             mask[i] = False
-    
-    if any(mask):
-        return np.mean(overlaps[mask]), np.sum(mask)
-    else:
-        return 0, 0
-
-def compute_eao_partial(overlaps: List, success: List[bool], curve_length: int):
-    phi = curve_length * [float(0)]
-    active = curve_length * [float(0)]
-
-    for o, success in zip(overlaps, success):
-
-        o_array = np.array(o)
-
-        for j in range(1, curve_length):
-
-            if j < len(o):
-                phi[j] += np.mean(o_array[1:j+1])
-                active[j] += 1
-            elif not success:
-                phi[j] += np.sum(o_array[1:len(o)]) / (j - 1)
-                active[j] += 1
-
-    phi = [p / a if a > 0 else 0 for p, a in zip(phi, active)]
-    return phi, active
 
-def count_failures(trajectory: List[Region]) -> Tuple[int, int]:
-    return len([region for region in trajectory if is_special(region, Special.FAILURE)]), len(trajectory)
+    return overlaps[mask]
 
 @analysis_registry.register("accuracy")
 class SequenceAccuracy(SeparableAnalysis):
 
     burnin = Integer(default=10, val_min=0)
     ignore_unknown = Boolean(default=True)
+    ignore_invisible = Boolean(default=False)    
     bounded = Boolean(default=True)
+    threshold = Float(default=None, val_min=0, val_max=1)
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiRunExperiment)
 
     @property
     def title(self):
         return "Sequence accurarcy"
@@ -76,38 +63,47 @@
     def describe(self):
         return Measure("Accuracy", "AUC", 0, 1, Sorting.DESCENDING),
 
     def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
 
         assert isinstance(experiment, MultiRunExperiment)
 
-        trajectories = experiment.gather(tracker, sequence)
-
-        if len(trajectories) == 0:
-            raise MissingResultsException()
+        objects = sequence.objects()
+        objects_accuracy = 0
+        bounds = (sequence.size) if self.bounded else None
+
+        for object in objects:
+            trajectories = experiment.gather(tracker, sequence, objects=[object])
+            if len(trajectories) == 0:
+                raise MissingResultsException()
+
+            cummulative = 0
+
+            for trajectory in trajectories:
+                overlaps = gather_overlaps(trajectory.regions(), sequence.object(object), self.burnin, 
+                                        ignore_unknown=self.ignore_unknown, ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold)
+                if overlaps.size > 0:
+                    cummulative += np.mean(overlaps)
 
-        cummulative = 0
-        for trajectory in trajectories:
-            accuracy, _ = compute_accuracy(trajectory.regions(), sequence, self.burnin, self.ignore_unknown, self.bounded)
-            cummulative = cummulative + accuracy
+            objects_accuracy += cummulative / len(trajectories)
 
-        return cummulative / len(trajectories),
+        return objects_accuracy / len(objects),
 
 @analysis_registry.register("average_accuracy")
 class AverageAccuracy(SequenceAggregator):
 
     analysis = Include(SequenceAccuracy)
     weighted = Boolean(default=True)
 
     def compatible(self, experiment: Experiment):
         return isinstance(experiment, MultiRunExperiment)
 
     @property
     def title(self):
-        return "Average accurarcy"
+        return "Accurarcy"
 
     def dependencies(self):
         return self.analysis,
 
     def describe(self):
         return Measure("Accuracy", "AUC", 0, 1, Sorting.DESCENDING),
 
@@ -124,61 +120,96 @@
                 frames += len(sequence)
             else:
                 accuracy += results[i, 0][0]
                 frames += 1
 
         return accuracy / frames,
 
-@analysis_registry.register("failures")
-class FailureCount(SeparableAnalysis):
+@analysis_registry.register("success_plot")
+class SuccessPlot(SeparableAnalysis):
+
+    ignore_unknown = Boolean(default=True)
+    ignore_invisible = Boolean(default=False)
+    burnin = Integer(default=0, val_min=0)
+    bounded = Boolean(default=True)
+    threshold = Float(default=None, val_min=0, val_max=1)
+    resolution = Integer(default=100, val_min=2)
 
     def compatible(self, experiment: Experiment):
-        return isinstance(experiment, SupervisedExperiment)
+        return isinstance(experiment, MultiRunExperiment)
 
     @property
     def title(self):
-        return "Number of failures"
+        return "Sequence success plot"
 
     def describe(self):
-        return Measure("Failures", "F", 0, None, Sorting.ASCENDING),
+        return Curve("Success plot", 2, "Success", minimal=(0, 0), maximal=(1, 1), labels=("Threshold", "Success"), trait="success"),
 
     def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
 
-        assert isinstance(experiment, SupervisedExperiment)
+        assert isinstance(experiment, MultiRunExperiment)
 
-        trajectories = experiment.gather(tracker, sequence)
+        objects = sequence.objects()
+        bounds = (sequence.size) if self.bounded else None
 
-        if len(trajectories) == 0:
-            raise MissingResultsException()
+        axis_x = np.linspace(0, 1, self.resolution)
+        axis_y = np.zeros_like(axis_x)
 
-        failures = 0
-        for trajectory in trajectories:
-            failures = failures + count_failures(trajectory.regions())[0]
+        for object in objects:
+            trajectories = experiment.gather(tracker, sequence, objects=[object])
+            if len(trajectories) == 0:
+                raise MissingResultsException()
 
-        return failures / len(trajectories), len(trajectories[0])
+            object_y = np.zeros_like(axis_x) 
 
+            for trajectory in trajectories:
+                overlaps = gather_overlaps(trajectory.regions(), sequence.object(object), burnin=self.burnin, ignore_unknown=self.ignore_unknown, ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold)
 
-@analysis_registry.register("cumulative_failures")
-class CumulativeFailureCount(SequenceAggregator):
+                for i, threshold in enumerate(axis_x):
+                    if threshold == 1:
+                        # Nicer handling of the edge case
+                        object_y[i] += np.sum(overlaps >= threshold) / len(overlaps)
+                    else:
+                        object_y[i] += np.sum(overlaps > threshold) / len(overlaps)
 
-    analysis = Include(FailureCount)
+            axis_y += object_y / len(trajectories)
 
-    def compatible(self, experiment: Experiment):
-        return isinstance(experiment, SupervisedExperiment)
+        axis_y /= len(objects)
+
+        return [(x, y) for x, y in zip(axis_x, axis_y)],
+
+
+@analysis_registry.register("average_success_plot")
+class AverageSuccessPlot(SequenceAggregator):
+
+    resolution = Integer(default=100, val_min=2)
+    analysis = Include(SuccessPlot)
 
     def dependencies(self):
         return self.analysis,
 
+    def compatible(self, experiment: Experiment):
+        return isinstance(experiment, MultiRunExperiment)
+
     @property
     def title(self):
-        return "Number of failures"
+        return "Sequence success plot"
 
     def describe(self):
-        return Measure("Failures", "F", 0, None, Sorting.ASCENDING), 
+        return Curve("Success plot", 2, "Success", minimal=(0, 0), maximal=(1, 1), labels=("Threshold", "Success"), trait="success"),
 
     def aggregate(self, _: Tracker, sequences: List[Sequence], results: Grid):
-        failures = 0
+        axis_x = np.linspace(0, 1, self.resolution)
+        axis_y = np.zeros_like(axis_x)
+
+        for i, _ in enumerate(sequences):
+            if results[i, 0] is None:
+                continue
+
+            curve = results[i, 0][0]
+
+            for j, (_, y) in enumerate(curve):
+                axis_y[j] += y
 
-        for a in results:
-            failures = failures + a[0]
+        axis_y /= len(sequences)
 
-        return failures,
+        return [(x, y) for x, y in zip(axis_x, axis_y)],
```

### Comparing `vot-toolkit-0.5.3/vot/analysis/multistart.py` & `vot-toolkit-0.6.0/vot/analysis/multistart.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/analysis/supervised.py` & `vot-toolkit-0.6.0/vot/analysis/supervised.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,50 +7,48 @@
 
 import numpy as np
 
 from attributee import Integer, Boolean, Float, Include
 
 from vot.tracker import Tracker, Trajectory
 from vot.dataset import Sequence
-from vot.dataset.proxy import FrameMapSequence
 from vot.experiment import Experiment
 from vot.experiment.multirun import SupervisedExperiment
-from vot.experiment.multistart import MultiStartExperiment, find_anchors
-from vot.region import Region, Special, calculate_overlaps
+from vot.region import Region, calculate_overlaps
 from vot.analysis import MissingResultsException, Measure, Point, is_special, Plot, Analysis, \
     Sorting, SeparableAnalysis, SequenceAggregator, analysis_registry, TrackerSeparableAnalysis, Axes
 from vot.utilities.data import Grid
 
 def compute_accuracy(trajectory: List[Region], sequence: Sequence, burnin: int = 10, 
     ignore_unknown: bool = True, bounded: bool = True) -> float:
 
     overlaps = np.array(calculate_overlaps(trajectory, sequence.groundtruth(), (sequence.size) if bounded else None))
     mask = np.ones(len(overlaps), dtype=bool)
 
     for i, region in enumerate(trajectory):
-        if is_special(region, Special.UNKNOWN) and ignore_unknown:
+        if is_special(region, Trajectory.UNKNOWN) and ignore_unknown:
             mask[i] = False
-        elif is_special(region, Special.INITIALIZATION):
+        elif is_special(region, Trajectory.INITIALIZATION):
             for j in range(i, min(len(trajectory), i + burnin)):
                 mask[j] = False
-        elif is_special(region, Special.FAILURE):
+        elif is_special(region, Trajectory.FAILURE):
             mask[i] = False
     
     if any(mask):
         return np.mean(overlaps[mask]), np.sum(mask)
     else:
         return 0, 0
 
 def count_failures(trajectory: List[Region]) -> Tuple[int, int]:
-    return len([region for region in trajectory if is_special(region, Special.FAILURE)]), len(trajectory)
+    return len([region for region in trajectory if is_special(region, Trajectory.FAILURE)]), len(trajectory)
 
 
 def locate_failures_inits(trajectory: List[Region]) -> Tuple[int, int]:
-    return [i for i, region in enumerate(trajectory) if is_special(region, Special.FAILURE)], \
-            [i for i, region in enumerate(trajectory) if is_special(region, Special.INITIALIZATION)]
+    return [i for i, region in enumerate(trajectory) if is_special(region, Trajectory.FAILURE)], \
+            [i for i, region in enumerate(trajectory) if is_special(region, Trajectory.INITIALIZATION)]
 
 def compute_eao_curve(overlaps: List, weights: List[float], success: List[bool]):
     max_length = max([len(el) for el in overlaps])
     total_runs = len(overlaps)
     
     overlaps_array = np.zeros((total_runs, max_length), dtype=np.float32)
     mask_array = np.zeros((total_runs, max_length), dtype=np.float32)  # mask out frames which are not considered in EAO calculation
```

### Comparing `vot-toolkit-0.5.3/vot/dataset/__init__.py` & `vot-toolkit-0.6.0/vot/dataset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import logging
 
 from numbers import Number
+from collections import namedtuple
 from abc import abstractmethod, ABC
 from typing import List, Mapping, Optional, Set, Tuple
 
 from PIL.Image import Image
 import numpy as np
 from trax import Region
 
@@ -87,21 +88,32 @@
 
     def image(self, channel: Optional[str] = None):
         channelobj = self._sequence.channel(channel)
         if channelobj is None:
             return None
         return channelobj.frame(self._index)
 
+    def objects(self):
+        objects = {}
+        for o in self._sequence.objects():
+            region = self._sequence.object(o, self._index)
+            if region is not None:
+                objects[o] = region
+        return objects
+
+    def object(self, id: str):
+        return self._sequence.object(id, self._index)
+
     def groundtruth(self):
         return self._sequence.groundtruth(self._index)
 
-    def tags(self, index = None):
+    def tags(self):
         return self._sequence.tags(self._index)
 
-    def values(self, index=None):
+    def values(self):
         return self._sequence.values(self._index)
 
 class SequenceIterator(object):
 
     def __init__(self, sequence: "Sequence"):
         self._position = 0
         self._sequence = sequence
@@ -246,14 +258,17 @@
 
     def filename(self, index):
         if index < 0 or index >= self.length:
             return None
 
         return os.path.join(self.base, self._files[index])
 
+    def __len__(self):
+        return self.length
+
 class FrameList(ABC):
     """Abstract base for all sequences, just a list of frame objects
     """
 
     def __iter__(self):
         return SequenceIterator(self)
 
@@ -266,14 +281,17 @@
         pass
 
 class Sequence(FrameList):
     """_summary_
 
     """
 
+    UNKNOWN = 0
+    INVISIBLE = 1
+
     def __init__(self, name: str, dataset: "Dataset" = None):
         self._name = name
         self._dataset = dataset
 
     def __len__(self) -> int:
         return self.length
 
@@ -298,14 +316,22 @@
         pass
 
     @abstractmethod
     def channels(self) -> Set[str]:
         pass
 
     @abstractmethod
+    def objects(self) -> Set[str]:
+        pass
+
+    @abstractmethod
+    def object(self, id, index=None):
+        pass
+
+    @abstractmethod
     def groundtruth(self, index: int) -> Region:
         pass
 
     @abstractmethod
     def tags(self, index=None) -> List[str]:
         pass
 
@@ -371,66 +397,83 @@
         """Returns a list of unique sequence names
 
         Returns:
             List[str]: List of sequence names
         """
         return self.list()
 
+SequenceData = namedtuple("SequenceData", ["channels", "objects", "tags", "values", "length"])
+
 class BaseSequence(Sequence):
 
     def __init__(self, name, dataset=None):
         super().__init__(name, dataset)
         self._metadata = self._read_metadata()
         self._data = None
 
     @abstractmethod
     def _read_metadata(self):
         raise NotImplementedError
 
     @abstractmethod
-    def _read(self):
+    def _read(self) -> SequenceData:
         raise NotImplementedError
 
     def __preload(self):
         if self._data is None:
             self._data = self._read()
 
     def metadata(self, name, default=None):
         return self._metadata.get(name, default)
 
     def channels(self):
         self.__preload()
-        return self._data[0]
+        return self._data.channels.keys()
 
     def channel(self, channel=None):
         self.__preload()
         if channel is None:
             channel = self.metadata("channel.default")
-        return self._data[0].get(channel, None)
+        return self._data.channels.get(channel, None)
 
     def frame(self, index):
         return Frame(self, index)
 
-    def groundtruth(self, index=None):
+    def objects(self):
+        self.__preload()
+        return self._data.objects.keys()
+
+    def object(self, id, index=None):
         self.__preload()
+        obj = self._data.objects.get(id, None)
         if index is None:
-            return self._data[1]
-        return self._data[1][index]
+            return obj
+        if obj is None:
+            return None
+        return obj[index]
+
+    def groundtruth(self, index=None):
+        self.__preload()
+        if len(self.objects()) != 1:
+            raise DatasetException("More than one object in sequence")
+
+        id = next(iter(self._data.objects))
+        return self.object(id, index)
 
     def tags(self, index=None):
         self.__preload()
         if index is None:
-            return self._data[2].keys()
-        return [t for t, sq in self._data[2].items() if sq[index]]
+            return self._data.tags.keys()
+        return [t for t, sq in self._data.tags.items() if sq[index]]
 
     def values(self, index=None):
         self.__preload()
         if index is None:
-            return self._data[3].keys()
-        return {v: sq[index] for v, sq in self._data[3].items()}
+            return self._data.values.keys()
+        return {v: sq[index] for v, sq in self._data.values.items()}
 
     @property
     def size(self):
         return self.channel().size
 
     @property
     def width(self):
@@ -439,30 +482,30 @@
     @property
     def height(self):
         return self.channel().height
 
     @property
     def length(self):
         self.__preload()
-        return len(self._data[1])
+        return self._data.length
 
 class InMemorySequence(BaseSequence):
 
     def __init__(self, name, channels):
         super().__init__(name, None)
         self._channels = {c: InMemoryChannel() for c in channels}
         self._tags = {}
         self._values = {}
         self._groundtruth = []
 
     def _read_metadata(self):
         return dict()
 
     def _read(self):
-        return self._channels, self._groundtruth, self._tags, self._values
+        return SequenceData(self._channels, {"object" : self._groundtruth}, self._tags, self._values)
 
     def append(self, images: dict, region: "Region", tags: list = None, values: dict = None):
 
         if not set(images.keys()).issuperset(self._channels.keys()):
             raise DatasetException("Images not provided for all channels")
 
         for k, channel in self._channels.items():
@@ -531,18 +574,15 @@
         DatasetException: If the dataset is not found or a network error occured
     """
     from urllib.parse import urlsplit
 
     try:
         res = urlsplit(url)
 
-        if not res.scheme or res.scheme == "vot":
-            from .vot import resolve_dataset_alias
-            download_dataset(resolve_dataset_alias(res.path), path)
-        elif res.scheme in ["http", "https"]:
+        if res.scheme in ["http", "https"]:
             if res.path.endswith(".json"):
                 from .vot import download_dataset_meta
                 download_dataset_meta(url, path)
             else:
                 download_bundle(url, path)
         elif res.scheme == "otb":
             from .otb import download_dataset as download_otb
```

### Comparing `vot-toolkit-0.5.3/vot/dataset/cow.png` & `vot-toolkit-0.6.0/vot/dataset/cow.png`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/dataset/dummy.py` & `vot-toolkit-0.6.0/vot/dataset/dummy.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 from vot.utilities import write_properties
 
 from PIL import Image
 import numpy as np
 
 class DummySequence(VOTSequence):
 
-    def __init__(self, length=100, size=(640, 480)):
-        base = os.path.join(tempfile.gettempdir(), "vot_dummy_%d_%d_%d" % (length, size[0], size[1]))
-        if not os.path.isdir(base) or not os.path.isfile(os.path.join(base, "groundtruth.txt")):
-            DummySequence._generate(base, length, size)
+    def __init__(self, length=100, size=(640, 480), objects=1):
+        base = os.path.join(tempfile.gettempdir(), "vot_dummy_%d_%d_%d_%d" % (length, size[0], size[1], objects))
+        if not os.path.isdir(base) or not os.path.isfile(os.path.join(base, "sequence")):
+            DummySequence._generate(base, length, size, objects)
         super().__init__(base, None)
 
     @staticmethod
-    def _generate(base, length, size):
+    def _generate(base, length, size, objects):
 
         background_color = Image.fromarray(np.random.normal(15, 5, (size[1], size[0], 3)).astype(np.uint8))
         background_depth = Image.fromarray(np.ones((size[1], size[0]), dtype=np.uint8) * 200)
         background_ir = Image.fromarray(np.zeros((size[1], size[0]), dtype=np.uint8))
 
         template = Image.open(os.path.join(os.path.dirname(__file__), "cow.png"))
 
@@ -36,39 +36,47 @@
         os.makedirs(dir_depth, exist_ok=True)
         os.makedirs(dir_ir, exist_ok=True)
 
         path_color = os.path.join(dir_color, "%08d.jpg")
         path_depth = os.path.join(dir_depth, "%08d.png")
         path_ir = os.path.join(dir_ir, "%08d.png")
 
-        groundtruth = []
+        groundtruth = {i : [] for i in range(objects)}
 
         center_x = size[0] / 2
         center_y = size[1] / 2
 
         radius = min(center_x - template.size[0], center_y - template.size[1])
 
         speed = (math.pi * 2) / length
+        offset = (math.pi * 2) / objects
 
         for i in range(length):
             frame_color = background_color.copy()
             frame_depth = background_depth.copy()
             frame_ir = background_ir.copy()
 
-            x = int(center_x + math.cos(i * speed) * radius - template.size[0] / 2)
-            y = int(center_y + math.sin(i * speed) * radius - template.size[1] / 2)
+            for o in range(objects):
 
-            frame_color.paste(template, (x, y), template)
-            frame_depth.paste(10, (x, y), template)
-            frame_ir.paste(240, (x, y), template)
+                x = int(center_x + math.cos(i * speed + offset * o) * radius - template.size[0] / 2)
+                y = int(center_y + math.sin(i * speed + offset * o) * radius - template.size[1] / 2)
+
+                frame_color.paste(template, (x, y), template)
+                frame_depth.paste(10, (x, y), template)
+                frame_ir.paste(240, (x, y), template)
+
+                groundtruth[o].append(Rectangle(x, y, template.size[0], template.size[1]))
 
             frame_color.save(path_color % (i + 1))
             frame_depth.save(path_depth % (i + 1))
             frame_ir.save(path_ir % (i + 1))
 
-            groundtruth.append(Rectangle(x, y, template.size[0], template.size[1]))
+        if objects == 1:
+            write_trajectory(os.path.join(base, "groundtruth.txt"), groundtruth[0])
+        else:
+            for i, g in groundtruth.items():
+                write_trajectory(os.path.join(base, "groundtruth_%03d.txt" % i), g)
 
-        write_trajectory(os.path.join(base, "groundtruth.txt"), groundtruth)
         metadata = {"name": "dummy", "fps" : 30, "format" : "dummy",
                           "channel.default": "color"}
         write_properties(os.path.join(base, "sequence"), metadata)
```

### Comparing `vot-toolkit-0.5.3/vot/dataset/got10k.py` & `vot-toolkit-0.6.0/vot/dataset/got10k.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import logging
 from collections import OrderedDict
 import configparser
 
 import six
 
 from vot import get_logger
-from vot.dataset import Dataset, DatasetException, BaseSequence, PatternFileListChannel
+from vot.dataset import Dataset, DatasetException, BaseSequence, \
+     PatternFileListChannel, SequenceData, Sequence
 from vot.region import Special
 from vot.region.io import read_trajectory
 from vot.utilities import Progress
 
 logger = get_logger()
 
 def load_channel(source):
@@ -61,15 +62,15 @@
 
         groundtruth_file = os.path.join(self._base, self.metadata("groundtruth", "groundtruth.txt"))
         groundtruth = read_trajectory(groundtruth_file)
 
         if len(groundtruth) == 1 and channels["color"].length > 1:
             # We are dealing with testing dataset, only first frame is available, so we pad the
             # groundtruth with unknowns. Only unsupervised experiment will work, but it is ok
-            groundtruth.extend([Special(Special.UNKNOWN)] * (channels["color"].length - 1))
+            groundtruth.extend([Special(Sequence.UNKNOWN)] * (channels["color"].length - 1))
 
         self._metadata["length"] = len(groundtruth)
 
         tagfiles = glob.glob(os.path.join(self._base, '*.label'))
 
         for tagfile in tagfiles:
             with open(tagfile, 'r') as filehandle:
@@ -99,15 +100,17 @@
                 tag_tmp[:len(tag)] = tag
                 tag = tag_tmp
 
         for name, value in values.items():
             if not len(value) == len(groundtruth):
                 raise DatasetException("Length mismatch for value %s" % name)
 
-        return channels, groundtruth, tags, values
+        objects = {"object" : groundtruth}
+
+        return SequenceData(channels, objects, tags, values, len(groundtruth)) 
 
 class GOT10kDataset(Dataset):
 
     def __init__(self, path, sequence_list="list.txt"):
         super().__init__(path)
 
         if not os.path.isabs(sequence_list):
```

### Comparing `vot-toolkit-0.5.3/vot/dataset/otb.py` & `vot-toolkit-0.6.0/vot/dataset/otb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from collections import OrderedDict
 import os
 import logging
 import six
 
 from vot import get_logger
-from vot.dataset import BaseSequence, Dataset, DatasetException, PatternFileListChannel
+from vot.dataset import BaseSequence, Dataset, DatasetException, PatternFileListChannel, SequenceData
 from vot.utilities import Progress
 from vot.region.io import parse_region
 
 logger = get_logger()
 
 _BASE_URL = "http://cvlab.hanyang.ac.kr/tracker_benchmark/seq/"
 
@@ -157,16 +157,18 @@
             for region in filehandle.readlines():
                 groundtruth.append(parse_region(region.replace("\t", ",").replace(" ", ",")))
 
         self._metadata["length"] = len(groundtruth)
 
         if not channels["color"].length == len(groundtruth):
             raise DatasetException("Length mismatch between groundtruth and images %d != %d" % (channels["color"].length, len(groundtruth)))
+        
+        objects = {"object" : groundtruth}
 
-        return channels, groundtruth, {}, {}
+        return SequenceData(channels, objects, {}, {}, len(groundtruth)) 
 
 class OTBDataset(Dataset):
 
     def __init__(self, path):
         super().__init__(path)
 
         dataset = _SEQUENCES
```

### Comparing `vot-toolkit-0.5.3/vot/dataset/proxy.py` & `vot-toolkit-0.6.0/vot/dataset/proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 from vot.dataset import Channel, Sequence, Frame
 
 class ProxySequence(Sequence):
     """A proxy sequence base that forwards requests to undelying source sequence. Meant as a base class.
     """
 
-    def __init__(self, source: Sequence):
+    def __init__(self, source: Sequence, name: str = None):
         """Creates a proxy sequence.
 
         Args:
             source (Sequence): Source sequence object
         """
-        super().__init__(source.name, source.dataset)
+        if name is None:
+            name = source.name
+        super().__init__(name, source.dataset)
         self._source = source
 
-    
     def __len__(self):
         return self.length
 
     def frame(self, index: int) -> Frame:
         return Frame(self, index)
 
     def metadata(self, name, default=None):
@@ -30,14 +31,20 @@
 
     def channel(self, channel=None):
         return self._source.channel(channel)
 
     def channels(self):
         return self._source.channels()
 
+    def objects(self):
+        return self._source.objects()
+
+    def object(self, id, index=None):
+        return self._source.object(id, index)
+
     def groundtruth(self, index: int = None) -> List[Region]:
         return self._source.groundtruth(index)
 
     def tags(self, index=None):
         return self._source.tags(index)
 
     def values(self, index=None):
@@ -136,17 +143,31 @@
     def __init__(self, source: Sequence, channels: Set[str]):
         super().__init__(source)
         self._filter = [i for i in channels if i in source.channels()]
 
     def channel(self, channel=None):
         if channel not in self._filter:
             return None
+        return self._source.channel(channel)
 
-        sourcechannel = self._source.channel(channel)
+    def channels(self):
+        return set(self._filter)
 
-        if sourcechannel is None:
-            return None
+class ObjectFilterSequence(ProxySequence):
+    """A proxy sequence that only makes specific object visible.
+    """
 
-        return FrameMapChannel(sourcechannel, self._map)
+    def __init__(self, source: Sequence, id: str, trim: bool=False):
+        super().__init__(source, "%s_%s" % (source.name, id))
+        self._id = id
+    
+    def objects(self):
+        objects = self._source.objects()
+        return {self._id: objects[id]}
 
-    def channels(self):
-        return list(self._channels)
+    def object(self, id, index=None):
+        if id != self._id:
+            return None
+        return self._source.object(id, index)
+
+    def groundtruth(self, index: int = None) -> List[Region]:
+        return self._source.object(self._id, index)
```

### Comparing `vot-toolkit-0.5.3/vot/dataset/trackingnet.py` & `vot-toolkit-0.6.0/vot/dataset/trackingnet.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import os
 import glob
 import logging
 from collections import OrderedDict
 
 import six
 
-from vot.dataset import Dataset, DatasetException, BaseSequence, PatternFileListChannel
+from vot.dataset import Dataset, DatasetException, \
+    BaseSequence, PatternFileListChannel, SequenceData, \
+    Sequence
 from vot.region import Special
 from vot.region.io import read_trajectory
 from vot.utilities import Progress
 
 logger = logging.getLogger("vot")
 
 def load_channel(source):
@@ -53,19 +55,21 @@
         self._metadata["width"], self._metadata["height"] = six.next(six.itervalues(channels)).size
 
         groundtruth = read_trajectory(self._base)
 
         if len(groundtruth) == 1 and channels["color"].length > 1:
             # We are dealing with testing dataset, only first frame is available, so we pad the
             # groundtruth with unknowns. Only unsupervised experiment will work, but it is ok
-            groundtruth.extend([Special(Special.UNKNOWN)] * (channels["color"].length - 1))
+            groundtruth.extend([Special(Sequence.UNKNOWN)] * (channels["color"].length - 1))
 
         self._metadata["length"] = len(groundtruth)
 
-        return channels, groundtruth, tags, values
+        objects = {"object" : groundtruth}
+
+        return SequenceData(channels, objects, tags, values, len(groundtruth))
 
 class TrackingNetDataset(Dataset):
 
     def __init__(self, path, splits=False):
         super().__init__(path)
 
         if not splits and not TrackingNetDataset.check(path):
```

### Comparing `vot-toolkit-0.5.3/vot/dataset/vot.py` & `vot-toolkit-0.6.0/vot/dataset/vot.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import logging
 from collections import OrderedDict
 
 import six
 
 import cv2
 
-from vot.dataset import Dataset, DatasetException, Sequence, BaseSequence, PatternFileListChannel
+from vot.dataset import Dataset, DatasetException, Sequence, BaseSequence, PatternFileListChannel, SequenceData
 from vot.region.io import write_trajectory, read_trajectory
+from vot.region import Special
 from vot.utilities import Progress, localize_path, read_properties, write_properties
 
 logger = logging.getLogger("vot")
 
 def load_channel(source):
 
     extension = os.path.splitext(source)[1]
@@ -44,69 +45,79 @@
         return metadata
 
     def _read(self):
 
         channels = {}
         tags = {}
         values = {}
-        groundtruth = []
 
         for c in ["color", "depth", "ir"]:
             channel_path = self.metadata("channels.%s" % c, None)
             if not channel_path is None:
                 channels[c] = load_channel(os.path.join(self._base, localize_path(channel_path)))
 
         # Load default channel if no explicit channel data available
         if len(channels) == 0:
             channels["color"] = load_channel(os.path.join(self._base, "color", "%08d.jpg"))
         else:
             self._metadata["channel.default"] = next(iter(channels.keys()))
 
         self._metadata["width"], self._metadata["height"] = six.next(six.itervalues(channels)).size
 
-        groundtruth_file = os.path.join(self._base, self.metadata("groundtruth", "groundtruth.txt"))
-        groundtruth = read_trajectory(groundtruth_file)
+        lenghts = [len(t) for t in channels.values()]
+        assert all([x == lenghts[0] for x in lenghts]), "Sequence channels have different lengths"
+        length = lenghts[0]
+
+        objectsfiles = glob.glob(os.path.join(self._base, 'groundtruth_*.txt'))
+        if len(objectsfiles) > 0:
+            objects = {}
+            for objectfile in objectsfiles:
+                groundtruth = read_trajectory(os.path.join(objectfile))
+                if len(groundtruth) < length: groundtruth += [Special(Sequence.UNKNOWN)] * (length - len(groundtruth))
+                objectid = os.path.basename(objectfile)[12:-4]
+                objects[objectid] = groundtruth
+        else:
+            groundtruth_file = os.path.join(self._base, self.metadata("groundtruth", "groundtruth.txt"))
+            groundtruth = read_trajectory(groundtruth_file)
+            if len(groundtruth) < length: groundtruth += [Special(Sequence.UNKNOWN)] * (length - len(groundtruth))
+            objects["object"] = groundtruth
 
-        self._metadata["length"] = len(groundtruth)
+        self._metadata["length"] = length
 
         tagfiles = glob.glob(os.path.join(self._base, '*.tag')) + glob.glob(os.path.join(self._base, '*.label'))
 
         for tagfile in tagfiles:
             with open(tagfile, 'r') as filehandle:
                 tagname = os.path.splitext(os.path.basename(tagfile))[0]
                 tag = [line.strip() == "1" for line in filehandle.readlines()]
-                while not len(tag) >= len(groundtruth):
+                while not len(tag) >= length:
                     tag.append(False)
                 tags[tagname] = tag
 
         valuefiles = glob.glob(os.path.join(self._base, '*.value'))
 
         for valuefile in valuefiles:
             with open(valuefile, 'r') as filehandle:
                 valuename = os.path.splitext(os.path.basename(valuefile))[0]
                 value = [float(line.strip()) for line in filehandle.readlines()]
-                while not len(value) >= len(groundtruth):
+                while not len(value) >= length:
                     value.append(0.0)
                 values[valuename] = value
 
-        for name, channel in channels.items():
-            if not channel.length == len(groundtruth):
-                raise DatasetException("Length mismatch for channel %s (%d != %d)" % (name, channel.length, len(groundtruth)))
-
         for name, tag in tags.items():
-            if not len(tag) == len(groundtruth):
-                tag_tmp = len(groundtruth) * [False]
+            if not len(tag) == length:
+                tag_tmp = length * [False]
                 tag_tmp[:len(tag)] = tag
                 tag = tag_tmp
 
         for name, value in values.items():
-            if not len(value) == len(groundtruth):
+            if not len(value) == length:
                 raise DatasetException("Length mismatch for value %s" % name)
 
-        return channels, groundtruth, tags, values
+        return SequenceData(channels, objects, tags, values, length) 
 
 class VOTDataset(Dataset):
 
     def __init__(self, path):
         super().__init__(path)
 
         if not os.path.isfile(os.path.join(path, "list.txt")):
@@ -229,34 +240,7 @@
     for value in sequence.values():
         data = "\n".join([ str(sequence.values(i).get(value, "")) for i in range(sequence.length)])
         with open(os.path.join(directory, "%s.value" % value), "w") as fp:
             fp.write(data)
 
     write_trajectory(os.path.join(directory, "groundtruth.txt"), [f.groundtruth() for f in sequence])
     write_properties(os.path.join(directory, "sequence"), metadata)
-
-
-_VOT_DATASETS = {
-    "vot2013" : "http://data.votchallenge.net/vot2013/dataset/description.json",
-    "vot2014" : "http://data.votchallenge.net/vot2014/dataset/description.json",
-    "vot2015" : "http://data.votchallenge.net/vot2015/dataset/description.json",
-    "vot-tir2015" : "http://www.cvl.isy.liu.se/research/datasets/ltir/version1.0/ltir_v1_0_8bit.zip",
-    "vot2016" : "http://data.votchallenge.net/vot2016/main/description.json",
-    "vot-tir2016" : "http://data.votchallenge.net/vot2016/vot-tir2016.zip",
-    "vot2017" : "http://data.votchallenge.net/vot2017/main/description.json",
-    "vot-st2018" : "http://data.votchallenge.net/vot2018/main/description.json",
-    "vot-lt2018" : "http://data.votchallenge.net/vot2018/longterm/description.json",
-    "vot-st2019" : "http://data.votchallenge.net/vot2019/main/description.json",
-    "vot-lt2019" : "http://data.votchallenge.net/vot2019/longterm/description.json",
-    "vot-rgbd2019" : "http://data.votchallenge.net/vot2019/rgbd/description.json",
-    "vot-rgbd2022" : "http://data.votchallenge.net/vot2022/rgbd/description.json",
-    "vot-rgbt2019" : "http://data.votchallenge.net/vot2019/rgbtir/meta/description.json",
-    "vot-st2020" : "https://data.votchallenge.net/vot2020/shortterm/description.json",
-    "vot-rgbt2020" : "http://data.votchallenge.net/vot2020/rgbtir/meta/description.json",
-    "vot-st2021": "https://data.votchallenge.net/vot2021/shortterm/description.json",
-    "test" : "http://data.votchallenge.net/toolkit/test.zip"
-}
-
-def resolve_dataset_alias(name):
-    if not name in _VOT_DATASETS:
-        raise ValueError("Unknown dataset")
-    return _VOT_DATASETS[name]
```

### Comparing `vot-toolkit-0.5.3/vot/document/__init__.py` & `vot-toolkit-0.6.0/vot/document/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 
 import os
 import typing
 from abc import ABC, abstractmethod
 import json
-import math
 import inspect
 import threading
-import logging
-import tempfile
 import datetime
 import collections
+import collections.abc
+import sys
 from asyncio import wait
 from asyncio.futures import wrap_future
 
 import numpy as np
 import yaml
 
 from matplotlib.cm import get_cmap
 from matplotlib.figure import Figure
 from matplotlib.axes import Axes as PlotAxes
 import matplotlib.colors as colors
 
 from attributee import Attributee, Object, Nested, String, Callable, Integer, List
 
 from vot import __version__ as version
-from vot import check_debug, get_logger
+from vot import get_logger
 from vot.dataset import Sequence
 from vot.tracker import Tracker
 from vot.analysis import Axes
-from vot.experiment import Experiment, analysis_resolver
 from vot.utilities import class_fullname
 from vot.utilities.data import Grid
 
 class Plot(object):
 
     def __init__(self, identifier: str, xlabel: str, ylabel: str,
         xlimits: typing.Tuple[float, float], ylimits: typing.Tuple[float, float], trait = None):
@@ -313,42 +311,52 @@
 class TrackerSorter(Attributee):
 
     experiment = String(default=None)
     analysis = String(default=None)
     result = Integer(val_min=0, default=0)
 
     def __call__(self, experiments, trackers, sequences):
+        from vot.analysis import AnalysisError
+
         if self.experiment is None or self.analysis is None:
             return range(len(trackers))
 
         experiment = next(filter(lambda x: x.identifier == self.experiment, experiments), None)
 
         if experiment is None:
             raise RuntimeError("Experiment not found")
 
         analysis = next(filter(lambda x: x.name == self.analysis, experiment.analyses), None)
 
         if analysis is None:
             raise RuntimeError("Analysis not found")
 
-        future = analysis.commit(experiment, trackers, sequences)
-        result = future.result()
+        try:
+
+            future = analysis.commit(experiment, trackers, sequences)
+            result = future.result()
+        except AnalysisError as e:
+            raise RuntimeError("Unable to sort trackers", e)
 
         scores = [x[self.result] for x in result]
         indices = [i[0] for i in sorted(enumerate(scores), reverse=True, key=lambda x: x[1])]
 
         return indices
 
 class Generator(Attributee):
 
     async def generate(self, experiments, trackers, sequences):
         raise NotImplementedError
 
     async def process(self, analyses, experiment, trackers, sequences):
-        if not isinstance(analyses, collections.Iterable):
+        if sys.version_info >= (3, 3):
+            _Iterable = collections.abc.Iterable
+        else:
+            _Iterable = collections.Iterable
+        if not isinstance(analyses, _Iterable):
             analyses = [analyses]
 
         futures = []
 
         for analysis in analyses:
             futures.append(wrap_future(analysis.commit(experiment, trackers, sequences)))
```

### Comparing `vot-toolkit-0.5.3/vot/document/common.py` & `vot-toolkit-0.6.0/vot/document/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 from vot.analysis import Measure, Point, Plot, Curve, Sorting, Axes
 
 def read_resource(name):
     path = os.path.join(os.path.dirname(__file__), name)
     with open(path, "r") as filehandle:
         return filehandle.read()
 
+def per_tracker(a):
+    return a.axes == Axes.TRACKERS
+
 def extract_measures_table(trackers, results):
     table_header = [[], [], []]
     table_data = dict()
     column_order = []
 
     for experiment, eresults in results.items():
         for analysis, aresults in eresults.items():
             descriptions = analysis.describe()
 
             # Ignore all non per-tracker results
-            if analysis.axes != Axes.TRACKERS:
+            if not per_tracker(analysis):
                 continue
 
             for i, description in enumerate(descriptions):
                 if description is None:
                     continue
                 if isinstance(description, Measure):
                     table_header[0].append(experiment)
@@ -72,15 +75,15 @@
 
     for experiment, eresults in results.items():
         experiment_plots = list()
         for analysis, aresults in eresults.items():
             descriptions = analysis.describe()
 
             # Ignore all non per-tracker results
-            if analysis.axes != Axes.TRACKERS:
+            if not per_tracker(analysis):
                 continue
 
             for i, description in enumerate(descriptions):
                 if description is None:
                     continue
 
                 plot_identifier = "%s_%s_%d" % (experiment.identifier, analysis.name, j)
@@ -101,15 +104,14 @@
                     xlabel = description.label(0)
                     ylabel = description.label(1)
                     plot = LinePlot(plot_identifier, xlabel, ylabel, xlim, ylim, description.trait)
                 else:
                     continue
 
                 for t in order if order is not None else range(len(trackers)):
-                    
                     tracker = trackers[t]
                     values = aresults[t, 0]
                     data = values[i] if not values is None else None
                     plot(tracker, data)
 
                 experiment_plots.append((description.name, plot))
```

### Comparing `vot-toolkit-0.5.3/vot/document/html.py` & `vot-toolkit-0.6.0/vot/document/html.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/document/jquery.js` & `vot-toolkit-0.6.0/vot/document/jquery.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/document/latex.py` & `vot-toolkit-0.6.0/vot/document/latex.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/document/pure.css` & `vot-toolkit-0.6.0/vot/document/pure.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/document/report.css` & `vot-toolkit-0.6.0/vot/document/report.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/document/report.js` & `vot-toolkit-0.6.0/vot/document/report.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/document/table.js` & `vot-toolkit-0.6.0/vot/document/table.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/experiment/__init__.py` & `vot-toolkit-0.6.0/vot/experiment/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from datetime import datetime
 from abc import abstractmethod
 
 from class_registry import ClassRegistry
 
 from attributee import Attributee, Object, Integer, Float, Nested, List
 
-from vot.tracker import RealtimeTrackerRuntime, TrackerException
+from vot.tracker import TrackerException
 from vot.utilities import Progress, to_number, import_class
 
 experiment_registry = ClassRegistry("vot_experiment")
-
 transformer_registry = ClassRegistry("vot_transformer")
 
 class RealtimeConfig(Attributee):
     """Config proxy for real-time experiment.
     """
 
     grace = Integer(val_min=0, default=0)
@@ -61,14 +60,17 @@
     return analysis
 
 class Experiment(Attributee):
     """Experiment abstract base class. 
 
     """
 
+    UNKNOWN = 0
+    INITIALIZATION = 1
+
     realtime = Nested(RealtimeConfig, default=None, description="Realtime modifier config")
     noise = Nested(NoiseConfig, default=None)
     inject = Nested(InjectConfig, default=None)
     transformers = List(Object(transformer_resolver), default=[])
     analyses = List(Object(analysis_resolver), default=[])
 
     def __init__(self, _identifier: str, _storage: "LocalStorage", **kwargs):
@@ -78,52 +80,83 @@
         # TODO: validate analysis names
 
     @property
     def identifier(self) -> str:
         return self._identifier
 
     @property
+    def _multiobject(self) -> bool:
+        # TODO: at some point this may be a property for all experiments
+        return False
+
+    @property
     def storage(self) -> "Storage":
         return self._storage
 
-    def _get_initialization(self, sequence: "Sequence", index: int):
-        return sequence.groundtruth(index)
+    def _get_initialization(self, sequence: "Sequence", index: int, id: str = None):
+        if not self._multiobject and id is None:
+            return sequence.groundtruth(index)
+        else:
+            return sequence.frame(index).object(id)
+
+    def _get_runtime(self, tracker: "Tracker", sequence: "Sequence", multiobject=False):
+        from ..tracker import SingleObjectTrackerRuntime, RealtimeTrackerRuntime, MultiObjectTrackerRuntime
+
+        runtime = tracker.runtime()
+
+        if multiobject:
+            if not runtime.multiobject:
+                runtime = MultiObjectTrackerRuntime(runtime)
+        else:
+            runtime = SingleObjectTrackerRuntime(runtime)
 
-    def _get_runtime(self, tracker: "Tracker", sequence: "Sequence"):
         if not self.realtime is None:
             grace = to_number(self.realtime.grace, min_n=0)
             fps = to_number(self.realtime.fps, min_n=0, conversion=float)
             interval = 1 / float(sequence.metadata("fps", fps))
-            runtime = RealtimeTrackerRuntime(tracker.runtime(), grace, interval)
-        else:
-            runtime = tracker.runtime()
+            runtime = RealtimeTrackerRuntime(runtime, grace, interval)
+
         return runtime
 
     @abstractmethod
     def execute(self, tracker: "Tracker", sequence: "Sequence", force: bool = False, callback: typing.Callable = None):
         raise NotImplementedError
 
     @abstractmethod
     def scan(self, tracker: "Tracker", sequence: "Sequence"):
+        """ Scan results for a given tracker and sequence. """
         raise NotImplementedError
 
     def results(self, tracker: "Tracker", sequence: "Sequence") -> "Results":
-        from vot.tracker import Results
-        from vot.workspace import LocalStorage
         if tracker.storage is not None:
             return tracker.storage.results(tracker, self, sequence)
         return self._storage.results(tracker, self, sequence)
 
     def log(self, identifier: str):
         return self._storage.substorage("logs").write("{}_{:%Y-%m-%dT%H-%M-%S.%f%z}.log".format(identifier, datetime.now()))
 
-    def transform(self, sequence: "Sequence"):
-        for transformer in self.transformers:
-            sequence = transformer(sequence)
-        return sequence
+    def transform(self, sequences):
+        from vot.dataset import Sequence
+        from vot.experiment.transformer import SingleObject
+        if isinstance(sequences, Sequence):
+            sequences = [sequences]
+        
+        transformers = list(self.transformers)
+
+        if not self._multiobject:
+            transformers.insert(0, SingleObject())
+
+        # Process sequences one transformer at the time. The number of sequences may grow
+        for transformer in transformers:
+            transformed = []
+            for sequence in sequences:
+                transformed.extend(transformer(sequence))
+            sequences = transformed
+
+        return sequences
 
 from .multirun import UnsupervisedExperiment, SupervisedExperiment
 from .multistart import MultiStartExperiment
 
 def run_experiment(experiment: Experiment, tracker: "Tracker", sequences: typing.List["Sequence"], force: bool = False, persist: bool = False):
     """A helper function that performs a given experiment with a given tracker on a list of sequences.
 
@@ -147,25 +180,33 @@
         def __call__(self, progress):
             self.bar.absolute(self._finished + min(1, max(0, progress)))
 
         def push(self):
             self._finished = self._finished + 1
             self.bar.absolute(self._finished)
 
+        def close(self):
+            self.bar.close()
+
     logger = logging.getLogger("vot")
 
+    transformed = []
+    for sequence in sequences:
+        transformed.extend(experiment.transform(sequence))
+    sequences = transformed
+
     progress = EvaluationProgress("{}/{}".format(tracker.identifier, experiment.identifier), len(sequences))
     for sequence in sequences:
-        sequence = experiment.transform(sequence)
         try:
             experiment.execute(tracker, sequence, force=force, callback=progress)
         except TrackerException as te:
             logger.error("Tracker %s encountered an error: %s", te.tracker.identifier, te)
             logger.debug(te, exc_info=True)
             if not te.log is None:
                 with experiment.log(te.tracker.identifier) as flog:
                     flog.write(te.log)
                     logger.error("Tracker output written to file: %s", flog.name)
             if not persist:
                 raise TrackerException("Experiment interrupted", te, tracker=tracker)
         progress.push()
 
+    progress.close()
```

### Comparing `vot-toolkit-0.5.3/vot/experiment/multirun.py` & `vot-toolkit-0.6.0/vot/experiment/multirun.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,103 +4,143 @@
 
 from vot.dataset import Sequence
 from vot.region import Special, calculate_overlap
 
 from attributee import Boolean, Integer, Float, List, String
 
 from vot.experiment import Experiment, experiment_registry
-from vot.tracker import Tracker, Trajectory
+from vot.tracker import Tracker, Trajectory, ObjectStatus
 
 class MultiRunExperiment(Experiment):
 
     repetitions = Integer(val_min=1, default=1)
     early_stop = Boolean(default=True)
 
     def _can_stop(self, tracker: Tracker, sequence: Sequence):
         if not self.early_stop:
             return False
-        trajectories = self.gather(tracker, sequence)
-        if len(trajectories) < 3:
-            return False
-
-        for trajectory in trajectories[1:]:
-            if not trajectory.equals(trajectories[0]):
+        
+        for o in sequence.objects():
+            trajectories = self.gather(tracker, sequence, objects=[o])
+            if len(trajectories) < 3:
                 return False
+            for trajectory in trajectories[1:]:
+                if not trajectory.equals(trajectories[0]):
+                    return False
 
         return True
 
     def scan(self, tracker: Tracker, sequence: Sequence):
         
         results = self.results(tracker, sequence)
 
         files = []
         complete = True
+        multiobject = len(sequence.objects()) > 1
+        assert self._multiobject or not multiobject
 
-        for i in range(1, self.repetitions+1):
-            name = "%s_%03d" % (sequence.name, i)
-            if Trajectory.exists(results, name):
-                files.extend(Trajectory.gather(results, name))
-            elif self._can_stop(tracker, sequence):
-                break
-            else:
-                complete = False
-                break
+        for o in sequence.objects():
+            prefix = sequence.name if not multiobject else "%s_%s" % (sequence.name, o)
+            for i in range(1, self.repetitions+1):
+                name = "%s_%03d" % (prefix, i)
+                if Trajectory.exists(results, name):
+                    files.extend(Trajectory.gather(results, name))
+                elif self._can_stop(tracker, sequence):
+                    break
+                else:
+                    complete = False
+                    break
 
         return complete, files, results
 
-    def gather(self, tracker: Tracker, sequence: Sequence):
+    def gather(self, tracker: Tracker, sequence: Sequence, objects = None, pad = False):
         trajectories = list()
+
+        multiobject = len(sequence.objects()) > 1
+
+        assert self._multiobject or not multiobject
         results = self.results(tracker, sequence)
-        for i in range(1, self.repetitions+1):
-            name = "%s_%03d" % (sequence.name, i)
-            if Trajectory.exists(results, name):
-                trajectories.append(Trajectory.read(results, name))
+
+        if objects is None:
+            objects = list(sequence.objects())
+
+        for o in objects:
+            prefix = sequence.name if not multiobject else "%s_%s" % (sequence.name, o)
+            for i in range(1, self.repetitions+1):
+                name =  "%s_%03d" % (prefix, i)
+                if Trajectory.exists(results, name):
+                    trajectories.append(Trajectory.read(results, name))
+                elif pad:
+                    trajectories.append(None)
         return trajectories
 
 @experiment_registry.register("unsupervised")
 class UnsupervisedExperiment(MultiRunExperiment):
 
+    multiobject = Boolean(default=False)
+
+    @property
+    def _multiobject(self) -> bool:
+        return self.multiobject
+
     def execute(self, tracker: Tracker, sequence: Sequence, force: bool = False, callback: Callable = None):
 
+        from .helpers import MultiObjectHelper
+
         results = self.results(tracker, sequence)
 
-        with self._get_runtime(tracker, sequence) as runtime:
+        multiobject = len(sequence.objects()) > 1
+        assert self._multiobject or not multiobject
+
+        helper = MultiObjectHelper(sequence)
+
+        def result_name(sequence, o, i):
+            return "%s_%s_%03d" % (sequence.name, o, i) if multiobject else "%s_%03d" % (sequence.name, i)
+
+        with self._get_runtime(tracker, sequence, self._multiobject) as runtime:
 
             for i in range(1, self.repetitions+1):
-                name = "%s_%03d" % (sequence.name, i)
 
-                if Trajectory.exists(results, name) and not force:
+                trajectories = {}
+
+                for o in helper.all(): trajectories[o] = Trajectory(sequence.length)
+
+                if all([Trajectory.exists(results, result_name(sequence, o, i)) for o in trajectories.keys()]) and not force:
                     continue
 
                 if self._can_stop(tracker, sequence):
                     return
 
-                trajectory = Trajectory(sequence.length)
-
-                _, properties, elapsed = runtime.initialize(sequence.frame(0), self._get_initialization(sequence, 0))
-
-                properties["time"] = elapsed
+                _, elapsed = runtime.initialize(sequence.frame(0), [ObjectStatus(self._get_initialization(sequence, 0, x), {}) for x in helper.new(0)])
 
-                trajectory.set(0, Special(Special.INITIALIZATION), properties)
+                for x in helper.new(0):
+                    trajectories[x].set(0, Special(Trajectory.INITIALIZATION), {"time": elapsed})
 
                 for frame in range(1, sequence.length):
-                    region, properties, elapsed = runtime.update(sequence.frame(frame))
+                    state, elapsed = runtime.update(sequence.frame(frame), [ObjectStatus(self._get_initialization(sequence, 0, x), {}) for x in helper.new(frame)])
 
-                    properties["time"] = elapsed
+                    if not isinstance(state, list):
+                        state = [state]
 
-                    trajectory.set(frame, region, properties)
+                    for x, object in zip(helper.objects(frame), state):
+                        object.properties["time"] = elapsed # TODO: what to do with time stats?
+                        trajectories[x].set(frame, object.region, object.properties)
 
-                trajectory.write(results, name)
+                    if callback:
+                        callback(float(i-1) / self.repetitions + (float(frame) / (self.repetitions * len(sequence))))
+
+                for o, trajectory in trajectories.items():
+                    trajectory.write(results, result_name(sequence, o, i))
 
-                if callback:
-                    callback(i / self.repetitions)
 
 @experiment_registry.register("supervised")
 class SupervisedExperiment(MultiRunExperiment):
 
+    FAILURE = 2
+
     skip_initialize = Integer(val_min=1, default=1)
     skip_tags = List(String(), default=[])
     failure_overlap = Float(val_min=0, val_max=1, default=0)
 
     def execute(self, tracker: Tracker, sequence: Sequence, force: bool = False, callback: Callable = None):
 
         results = self.results(tracker, sequence)
@@ -117,39 +157,37 @@
                     return
 
                 trajectory = Trajectory(sequence.length)
 
                 frame = 0
                 while frame < sequence.length:
 
-                    _, properties, elapsed = runtime.initialize(sequence.frame(frame), self._get_initialization(sequence, frame))
-
-                    properties["time"] = elapsed
+                    _, elapsed = runtime.initialize(sequence.frame(frame), self._get_initialization(sequence, frame))
 
-                    trajectory.set(frame, Special(Special.INITIALIZATION), properties)
+                    trajectory.set(frame, Special(Trajectory.INITIALIZATION), {"time" : elapsed})
 
                     frame = frame + 1
 
                     while frame < sequence.length:
 
-                        region, properties, elapsed = runtime.update(sequence.frame(frame))
+                        object, elapsed = runtime.update(sequence.frame(frame))
 
-                        properties["time"] = elapsed
+                        object.properties["time"] = elapsed
 
-                        if calculate_overlap(region, sequence.groundtruth(frame), sequence.size) <= self.failure_overlap:
-                            trajectory.set(frame, Special(Special.FAILURE), properties)
+                        if calculate_overlap(object.region, sequence.groundtruth(frame), sequence.size) <= self.failure_overlap:
+                            trajectory.set(frame, Special(SupervisedExperiment.FAILURE), object.properties)
                             frame = frame + self.skip_initialize
  
                             if self.skip_tags:
                                 while frame < sequence.length:
                                     if not [t for t in sequence.tags(frame) if t in self.skip_tags]:
                                         break
                                     frame = frame + 1
                             break
                         else:
-                            trajectory.set(frame, region, properties)
+                            trajectory.set(frame, object.region, object.properties)
                         frame = frame + 1
 
                 if  callback:
                     callback(i / self.repetitions)
 
                 trajectory.write(results, name)
```

### Comparing `vot-toolkit-0.5.3/vot/experiment/multistart.py` & `vot-toolkit-0.6.0/vot/experiment/multistart.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,25 +71,23 @@
                 if reverse:
                     proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
                 else:
                     proxy = FrameMapSequence(sequence, list(range(i, sequence.length)))
 
                 trajectory = Trajectory(proxy.length)
 
-                _, properties, elapsed = runtime.initialize(proxy.frame(0), self._get_initialization(proxy, 0))
+                _, elapsed = runtime.initialize(proxy.frame(0), self._get_initialization(proxy, 0))
 
-                properties["time"] = elapsed
-
-                trajectory.set(0, Special(Special.INITIALIZATION), properties)
+                trajectory.set(0, Special(Trajectory.INITIALIZATION), {"time": elapsed})
 
                 for frame in range(1, proxy.length):
-                    region, properties, elapsed = runtime.update(proxy.frame(frame))
+                    object, elapsed = runtime.update(proxy.frame(frame))
 
-                    properties["time"] = elapsed
+                    object.properties["time"] = elapsed
 
-                    trajectory.set(frame, region, properties)
+                    trajectory.set(frame, object.region, object.properties)
 
                 trajectory.write(results, name)
 
                 current = current + 1
                 if  callback:
                     callback(current / total)
```

### Comparing `vot-toolkit-0.5.3/vot/experiment/transformer.py` & `vot-toolkit-0.6.0/vot/experiment/transformer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from abc import abstractmethod
+from typing import List
 
 from PIL import Image
 
-from attributee import Attributee, Integer, Float
+from attributee import Attributee, Integer, Float, Boolean
 
 from vot.dataset import Sequence, VOTSequence, InMemorySequence
 from vot.dataset.proxy import FrameMapSequence
 from vot.dataset.vot import write_sequence
 from vot.region import RegionType
 from vot.utilities import arg_hash
 from vot.experiment import transformer_registry
@@ -15,26 +16,39 @@
 class Transformer(Attributee):
 
     def __init__(self, cache: "LocalStorage", **kwargs):
         super().__init__(**kwargs)
         self._cache = cache
 
     @abstractmethod
-    def __call__(self, sequence: Sequence) -> Sequence:
+    def __call__(self, sequence: Sequence) -> List[Sequence]:
         raise NotImplementedError
 
+@transformer_registry.register("singleobject")
+class SingleObject(Transformer):
+
+    trim = Boolean(default=False, description="Trim each generated sequence to a visible subsection for the selected object")
+
+    def __call__(self, sequence: Sequence) -> List[Sequence]:
+        from vot.dataset.proxy import ObjectFilterSequence
+        
+        if len(sequence.objects()) == 1:
+            return [sequence]
+        
+        return [ObjectFilterSequence(sequence, id, self.trim) for id in sequence.objects()]
+        
 @transformer_registry.register("redetection")
 class Redetection(Transformer):
 
     length = Integer(default=100, val_min=1)
     initialization = Integer(default=5, val_min=1)
     padding = Float(default=2, val_min=0)
     scaling = Float(default=1, val_min=0.1, val_max=10)
 
-    def __call__(self, sequence: Sequence) -> Sequence:
+    def __call__(self, sequence: Sequence) -> List[Sequence]:
 
         chache_dir = self._cache.directory(self, arg_hash(sequence.name, **self.dump()))
 
         if not os.path.isfile(os.path.join(chache_dir, "sequence")):
             generated = InMemorySequence(sequence.name, sequence.channels())
             size = (int(sequence.size[0] * self.scaling), int(sequence.size[1] * self.scaling))
 
@@ -59,8 +73,8 @@
             generated.append(initial_images, sequence.frame(0).groundtruth())
             generated.append(redetect_images, sequence.frame(0).groundtruth().move(size[0] - template.width, size[1] - template.height))
 
             write_sequence(chache_dir, generated)
 
         source = VOTSequence(chache_dir, name=sequence.name)
         mapping = [0] * self.initialization + [1] * (self.length - self.initialization)
-        return FrameMapSequence(source, mapping)
+        return [FrameMapSequence(source, mapping)]
```

### Comparing `vot-toolkit-0.5.3/vot/region/__init__.py` & `vot-toolkit-0.6.0/vot/region/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import abstractmethod, ABC
-from typing import Tuple
 from enum import Enum
 
 from vot import ToolkitException
 from vot.utilities.draw import DrawHandle
 
 class RegionException(ToolkitException):
     """General region exception"""
@@ -53,23 +52,19 @@
     @abstractmethod
     def is_empty(self):
         """Check if region is empty (not annotated or not reported)
         """
 
 class Special(Region):
     """
-    Special region
+    Special region, meaning of the code can change depending on the context
 
     :var code: Code value
     """
 
-    UNKNOWN = 0
-    INITIALIZATION = 1
-    FAILURE = 2
-
     def __init__(self, code):
         """ Constructor
 
         :param code: Special code
         """
         super().__init__()
         self._code = int(code)
@@ -99,11 +94,11 @@
         """
         return self._code
 
     def draw(self, handle: DrawHandle):
         pass
 
     def is_empty(self):
-        return False
+        return True
 
 from .raster import calculate_overlap, calculate_overlaps
 from .shapes import Rectangle, Polygon, Mask
```

### Comparing `vot-toolkit-0.5.3/vot/region/io.py` & `vot-toolkit-0.6.0/vot/region/io.py`

 * *Files 23% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     rle = np.array([el for el in elements[4:]], dtype=np.int32)
 
     # create mask from RLE within target region
     mask = rle_to_mask(rle, region_w, region_h)
 
     return mask, (tl_x, tl_y)
 
+
 from vot.region.raster import mask_bounds
 
 def encode_mask(mask):
     """
     mask: input binary mask, type: uint8
     output: full RLE encoding in the format: (x0, y0, w, h), RLE
     first get minimal axis-aligned region which contains all positive pixels
@@ -143,31 +144,90 @@
         elif len(tokens) % 2 == 0 and len(tokens) > 4:
             if any([math.isnan(el) for el in tokens]):
                 return Special(0)
             else:
                 return Polygon([(x_, y_) for x_, y_ in zip(tokens[::2], tokens[1::2])])
     return None
 
+def read_trajectory_binary(fp: io.RawIOBase):
+    import struct
+    from cachetools import LRUCache, cached
+    from vot.region import Special
+    from vot.region.shapes import Rectangle, Polygon, Mask
+
+    buffer = dict(data=fp.read(), offset = 0)
+
+    @cached(cache=LRUCache(maxsize=32))
+    def calcsize(format):
+        return struct.calcsize(format)
+
+    def read(format: str):
+        unpacked = struct.unpack_from(format, buffer["data"], buffer["offset"])
+        buffer["offset"] += calcsize(format)
+        return unpacked
+
+    _, length = read("<hI")
+
+    trajectory = []
+
+    for _ in range(length):
+        type, = read("<B")
+        if type == 0: r = Special(*read("<I"))
+        elif type == 1: r = Rectangle(*read("<ffff"))
+        elif type == 2:
+            n, = read("<H")
+            values = read("<%df" % (2 * n))
+            r = Polygon(list(zip(values[0::2], values[1::2])))
+        elif type == 3:
+            tl_x, tl_y, region_w, region_h, n = read("<hhHHH")
+            rle = read("<%dH" % (n))
+            r = Mask(rle_to_mask(rle, region_w, region_h), (tl_x, tl_y))
+        else:
+            raise IOError("Wrong region type")
+        trajectory.append(r)
+    return trajectory
+
+def write_trajectory_binary(fp: io.RawIOBase, data: List["Region"]):
+    import struct
+    from vot.region import Special
+    from vot.region.shapes import Rectangle, Polygon, Mask
+
+    fp.write(struct.pack("<hI", 1, len(data)))
+
+    for r in data:
+        if isinstance(r, Special): fp.write(struct.pack("<BI", 0, r.code))
+        elif isinstance(r, Rectangle): fp.write(struct.pack("<Bffff", 1, r.x, r.y, r.width, r.height))
+        elif isinstance(r, Polygon): fp.write(struct.pack("<BH%df" % (2 * r.size), 2, r.size, *[item for sublist in r.points() for item in sublist]))
+        elif isinstance(r, Mask): 
+            rle = mask_to_rle(r.mask)
+            fp.write(struct.pack("<BhhHHH%dH" % len(rle), 3, r.offset[0], r.offset[1], r.mask.shape[1], r.mask.shape[0], len(rle), *rle))
+        else:
+            raise IOError("Wrong region type")
+
 def read_trajectory(fp: Union[str, TextIO]):
     if isinstance(fp, str):
-        binary = fp.endswith(".tra")
+        try:
+            import struct
+            with open(fp, "r+b") as tfp:
+                v, = struct.unpack("<h", tfp.read(struct.calcsize("<h")))
+                binary = v == 1
+                # TODO: we can use the same file handle in case of binary format
+        except Exception as e:
+            binary = False
+
         fp = open(fp, "rb" if binary else "r")
         close = True
     else:
         binary = isinstance(fp, (io.RawIOBase, io.BufferedIOBase)) 
         close = False
 
-    regions = []
-    # iterate over all lines in the file
-
-    from vot.region import RegionException
-
     if binary:
-        raise RegionException("Binary format not supported at the moment")
+        regions = read_trajectory_binary(fp)
     else:
+        regions = []
         for line in fp.readlines():
             regions.append(parse_region(line.strip()))
 
     if close:
         fp.close()
 
     return regions
@@ -181,24 +241,22 @@
     Args:
         fp (Union[str, TextIO]): File handle or file name
         data (List[Region]): Trajectory, a list of region objects
 
     """
 
     if isinstance(fp, str):
-        binary = fp.endswith(".tra")
+        binary = fp.endswith(".bin")
         close = True
         fp = open(fp, "wb" if binary else "w")
     else:
         binary = isinstance(fp, (io.RawIOBase, io.BufferedIOBase)) 
         close = False
 
-    from vot.region import RegionException
-
     if binary:
-        raise RegionException("Binary format not supported at the moment")
+        write_trajectory_binary(fp, data)
     else:
         for region in data:
-            fp.write('%s\n' % str(region))
+            fp.write(str(region) + "\n")
     
     if close:
         fp.close()
```

### Comparing `vot-toolkit-0.5.3/vot/region/raster.py` & `vot-toolkit-0.6.0/vot/region/raster.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Tuple, Optional
 
 import numba
 import numpy as np
 
+_TYPE_EMPTY = 0
 _TYPE_RECTANGLE = 1
 _TYPE_POLYGON = 2
 _TYPE_MASK = 3
 
 @numba.njit()
 def mask_bounds(mask: np.ndarray):
     """
@@ -23,14 +24,17 @@
         for j in range(mask.shape[1]):
             if mask[i, j] != 0:
                 top = min(top, i)
                 bottom = max(bottom, i)
                 left = min(left, j)
                 right = max(right, j)
 
+    if top == ii32.max:
+        return (0, 0, 0, 0)
+
     return (left, top, right, bottom)
 
 
 @numba.njit()
 def rasterize_rectangle(data: np.ndarray, bounds: Tuple[int, int, int, int]):
     width = bounds[2] - bounds[0] + 1
     height = bounds[3] - bounds[1] + 1
@@ -186,30 +190,37 @@
 
     if t == _TYPE_RECTANGLE:
         return rasterize_rectangle(a, bounds)
     elif t == _TYPE_POLYGON:
         return rasterize_polygon(a, bounds)
     elif t == _TYPE_MASK:
         return copy_mask(a, o, bounds)
+    
+    return np.zeros((bounds[3] - bounds[1] + 1, bounds[2] - bounds[0] + 1), dtype=np.uint8)
 
 @numba.njit(cache=True)
 def _calculate_overlap(a: np.ndarray, b: np.ndarray, at: int, bt: int, ao: Optional[Tuple[int, int]] = None,
         bo: Optional[Tuple[int, int]] = None, bounds: Optional[Tuple[int, int]] = None):
 
     bounds1 = _region_bounds(a, at, ao)
     bounds2 = _region_bounds(b, bt, bo)
 
     union = (min(bounds1[0], bounds2[0]), min(bounds1[1], bounds2[1]), max(bounds1[2], bounds2[2]), max(bounds1[3], bounds2[3]))
 
+    if union[0] >= union[2] or union[1] >= union[3]:
+        # Two empty regons are considered to be identical
+        return float(1)
+
     if not bounds is None:
         raster_bounds = (max(0, union[0]), max(0, union[1]), min(bounds[0] - 1, union[2]), min(bounds[1] - 1, union[3]))
     else:
         raster_bounds = union
 
     if raster_bounds[0] >= raster_bounds[2] or raster_bounds[1] >= raster_bounds[3]:
+        # Regions are not identical, but are outside rasterization bounds.
         return float(0)
 
     m1 = _region_raster(a, raster_bounds, at, ao)
     m2 = _region_raster(b, raster_bounds, bt, bo)
 
     a1 = m1.ravel()
     a2 = m2.ravel()
@@ -224,53 +235,60 @@
                 intersection += 1
 
     return float(intersection) / float(union_) if union_ > 0 else float(0)
 
 from vot.region import Region, RegionException
 from vot.region.shapes import Shape, Rectangle, Polygon, Mask
 
-def calculate_overlap(reg1: Shape, reg2: Shape, bounds: Optional[Tuple[int, int]] = None):
+Bounds = Tuple[int, int]
+
+def calculate_overlap(reg1: Shape, reg2: Shape, bounds: Optional[Bounds] = None):
     """
     Inputs: reg1 and reg2 are Region objects (Rectangle, Polygon or Mask)
     bounds: size of the image, format: [width, height]
     function first rasterizes both regions to 2-D binary masks and calculates overlap between them
     """
 
-    if not isinstance(reg1, Shape) or not isinstance(reg2, Shape):
-        return float(0)
-
     if isinstance(reg1, Rectangle):
         data1 = np.round(reg1._data)
         offset1 = (0, 0)
         type1 = _TYPE_RECTANGLE
     elif isinstance(reg1, Polygon):
         data1 = np.round(reg1._points)
         offset1 = (0, 0)
         type1 = _TYPE_POLYGON
     elif isinstance(reg1, Mask):
         data1 = reg1.mask
         offset1 = reg1.offset
         type1 = _TYPE_MASK
+    else:
+        data1 = np.zeros((1, 1))
+        offset1 = (0, 0)
+        type1 = _TYPE_EMPTY
 
     if isinstance(reg2, Rectangle):
         data2 = np.round(reg2._data)
         offset2 = (0, 0)
         type2 = _TYPE_RECTANGLE
     elif isinstance(reg2, Polygon):
         data2 = np.round(reg2._points)
         offset2 = (0, 0)
         type2 = _TYPE_POLYGON
     elif isinstance(reg2, Mask):
         data2 = reg2.mask
         offset2 = reg2.offset
         type2 = _TYPE_MASK
+    else:
+        data2 = np.zeros((1, 1))
+        offset2 = (0, 0)
+        type2 = _TYPE_EMPTY
 
     return _calculate_overlap(data1, data2, type1, type2, offset1, offset2, bounds)
 
-def calculate_overlaps(first: List[Region], second: List[Region], bounds: Optional[Tuple[int, int]]):
+def calculate_overlaps(first: List[Region], second: List[Region], bounds: Optional[Bounds] = None):
     """
     first and second are lists containing objects of type Region
     bounds is in the format [width, height]
     output: list of per-frame overlaps (floats)
     """
     if not len(first) == len(second):
         raise RegionException("List not of the same size {} != {}".format(len(first), len(second)))
```

### Comparing `vot-toolkit-0.5.3/vot/region/shapes.py` & `vot-toolkit-0.6.0/vot/region/shapes.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         offset_str = '%d,%d' % self.offset
         region_sz_str = '%d,%d' % (self.mask.shape[1], self.mask.shape[0])
         rle_str = ','.join([str(el) for el in mask_to_rle(self.mask)])
         return 'm%s,%s,%s' % (offset_str, region_sz_str, rle_str)
 
     def _optimize(self):
         bounds = mask_bounds(self.mask)
-        if bounds[0] is None:
+        if bounds[2] == 0:
             # mask is empty
             self._mask = np.zeros((0, 0), dtype=np.uint8)
             self._offset = (0, 0)
         else:
             self._mask = np.copy(self.mask[bounds[1]:bounds[3], bounds[0]:bounds[2]])
             self._offset = (bounds[0] + self.offset[0], bounds[1] + self.offset[1])
 
@@ -278,18 +278,16 @@
         handle.mask(self._mask, self.offset)
 
     def rasterize(self, bounds: Tuple[int, int, int, int]):
         from vot.region.raster import copy_mask
         return copy_mask(self._mask, self._offset, np.array(bounds))
 
     def is_empty(self):
-        if self.mask.shape[1] > 0 and self.mask.shape[0] > 0:
-            return False
-        else:
-            return True
+        bounds = mask_bounds(self.mask)
+        return bounds[2] == 0 or bounds[3] == 0
 
     def resize(self, factor=1):
 
         offset = (int(self.offset[0] * factor), int(self.offset[1] * factor))
         height = max(1, int(self.mask.shape[0] * factor))
         width = max(1, int(self.mask.shape[1] * factor))
```

### Comparing `vot-toolkit-0.5.3/vot/stack/__init__.py` & `vot-toolkit-0.6.0/vot/stack/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from typing import List, Mapping
 
 import yaml
 
 from attributee import Attributee, String, Boolean, Map, Object
 
 from vot.experiment import Experiment, experiment_registry
-from vot.experiment.transformer import Transformer
 from vot.utilities import import_class
-from vot.analysis import Analysis
 
 def experiment_resolver(typename, context, **kwargs):
 
     identifier = context.key
     storage = None
 
     if getattr(context.parent, "workspace", None) is not None:
@@ -28,16 +26,16 @@
     else:
         experiment_class = import_class(typename)
         assert issubclass(experiment_class, Experiment)
         return experiment_class(_identifier=identifier, _storage=storage, **kwargs)
 
 class Stack(Attributee):
 
-    title = String()
-    dataset = String(default="")
+    title = String(default="Stack")
+    dataset = String(default=None)
     url = String(default="")
     deprecated = Boolean(default=False)
     experiments = Map(Object(experiment_resolver))
 
     def __init__(self, name: str, workspace: "Workspace", **kwargs):
         self._workspace = workspace
         self._name = name
@@ -94,11 +92,13 @@
 
     stacks = {}
     root = Path(os.path.join(os.path.dirname(__file__)))
 
     for stack_path in root.rglob("*.yaml"):
         with open(stack_path, 'r') as fp:
             stack_metadata = yaml.load(fp, Loader=yaml.BaseLoader)
+        if stack_metadata is None:
+            continue
         key = str(stack_path.relative_to(root).with_name(os.path.splitext(stack_path.name)[0]))
         stacks[key] = stack_metadata.get("title", "")
 
     return stacks
```

### Comparing `vot-toolkit-0.5.3/vot/stack/testing.yaml` & `vot-toolkit-0.6.0/vot/stack/tests/segmentation.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-title: VOT testing
+title: VOT Segmentation testing
 url: http://www.votchallenge.net/
 dataset: http://box.vicos.si/tracking/vot20_test_dataset.zip
 experiments:
   baseline:
     type: multistart
     analyses:
       - type: multistart_average_ar
```

### Comparing `vot-toolkit-0.5.3/vot/stack/tests.py` & `vot-toolkit-0.6.0/vot/stack/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/stack/vot2017.yaml` & `vot-toolkit-0.6.0/vot/stack/vot2017.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 title: VOT2017 challenge
-dataset: vot:vot2017
+dataset: http://data.votchallenge.net/vot2017/main/description.json
 url: http://www.votchallenge.net/vot2017/
 experiments:
   baseline:
     type: supervised
     repetitions: 15
     skip_initialize: 5
     analyses:
```

### Comparing `vot-toolkit-0.5.3/vot/stack/vot2018.yaml` & `vot-toolkit-0.6.0/vot/stack/vot2018/shortterm.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 title: VOT-ST2018 challenge
-dataset: vot:vot-st2018
+dataset: http://data.votchallenge.net/vot2018/main/description.json
 url: http://www.votchallenge.net/vot2018/
 experiments:
   baseline:
     type: supervised
     repetitions: 15
     skip_initialize: 5
     analyses:
```

### Comparing `vot-toolkit-0.5.3/vot/stack/vot2019.yaml` & `vot-toolkit-0.6.0/vot/stack/vot2019/shortterm.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 title: VOT-ST2019 challenge
-dataset: vot:vot-st2019
+dataset: http://data.votchallenge.net/vot2019/main/description.json
 url: http://www.votchallenge.net/vot2019/
 experiments:
   baseline:
     type: supervised
     repetitions: 15
     skip_initialize: 5
     analyses:
```

### Comparing `vot-toolkit-0.5.3/vot/stack/vot2020.yaml` & `vot-toolkit-0.6.0/vot/stack/vot2021/st.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-title: VOT-ST2020 challenge
-dataset: vot:vot-st2020
-url: http://www.votchallenge.net/vot2020/
+title: VOT-ST2021 challenge
+dataset: https://data.votchallenge.net/vot2021/shortterm/description.json
+url: http://www.votchallenge.net/vot2021/
 experiments:
   baseline:
     type: multistart
     analyses:
       - type: multistart_eao_score
         name: eaoscore
         low: 115
```

### Comparing `vot-toolkit-0.5.3/vot/stack/vot2021.yaml` & `vot-toolkit-0.6.0/vot/stack/vot2022/stb.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-title: VOT-ST2021 challenge
-dataset: vot:vot-st2021
-url: http://www.votchallenge.net/vot2021/
+title: VOT-ST2022 bounding-box challenge
+dataset: https://data.votchallenge.net/vot2022/stb/description.json
+url: https://www.votchallenge.net/vot2022/
 experiments:
   baseline:
     type: multistart
     analyses:
       - type: multistart_eao_score
         name: eaoscore
         low: 115
```

### Comparing `vot-toolkit-0.5.3/vot/stack/vot2022/sts.yaml` & `vot-toolkit-0.6.0/vot/stack/vot2022/sts.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/tracker/__init__.py` & `vot-toolkit-0.6.0/vot/tracker/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,80 @@
 
 import os
 import re
 import configparser
 import logging
 import copy
-from typing import Tuple
-from collections import OrderedDict
+from typing import Tuple, List, Union
+from collections import OrderedDict, namedtuple
 from abc import abstractmethod, ABC
 
 import yaml
 
 from vot import ToolkitException
 from vot.dataset import Frame
 from vot.region import Region
 from vot.utilities import to_string
 
 logger = logging.getLogger("vot")
 
 class TrackerException(ToolkitException):
+    """ Base class for all tracker related exceptions."""
+
     def __init__(self, *args, tracker, tracker_log=None):
+        """ Initialize the exception.
+
+        Args:
+            tracker (Tracker): Tracker that caused the exception.
+            tracker_log (str, optional): Optional log message. Defaults to None.
+        """
         super().__init__(*args)
         self._tracker_log = tracker_log
         self._tracker = tracker
 
     @property
-    def log(self):
+    def log(self) -> str:
+        """ Returns the log message of the tracker.
+
+        Returns:
+            sts: Log message of the tracker.
+        """
         return self._tracker_log
 
     @property
     def tracker(self):
+        """ Returns the tracker that caused the exception."""
         return self._tracker
 
 class TrackerTimeoutException(TrackerException):
     pass
 
 VALID_IDENTIFIER = re.compile("^[a-zA-Z0-9-_]+$")
 
 VALID_REFERENCE = re.compile("^([a-zA-Z0-9-_]+)(@[a-zA-Z0-9-_]*)?$")
 
 def is_valid_identifier(identifier):
+    """Checks if the identifier is valid."""
     return not VALID_IDENTIFIER.match(identifier) is None
 
 def is_valid_reference(reference):
+    """Checks if the reference is valid."""
     return not VALID_REFERENCE.match(reference) is None
 
 def parse_reference(reference):
+    """Parses the reference into identifier and version."""
     matches = VALID_REFERENCE.match(reference)
     if not matches:
         return None, None
     return matches.group(1), matches.group(2)[1:] if not matches.group(2) is None else None
 
 _runtime_protocols = {}
 
 class Registry(object):
+    """ Repository of known trackers. Trackers are loaded from a manifest files in one or more directories. """
 
     def __init__(self, directories, root=os.getcwd()):
         trackers = dict()
         registries = []
 
         for directory in directories:
             if not os.path.isabs(directory):
@@ -103,27 +121,43 @@
 
                     trackers[section] = Tracker(_identifier=section, _source=registry, **config[section])
 
         self._trackers = OrderedDict(sorted(trackers.items(), key=lambda t: t[0]))
         logger.debug("Found %d trackers", len(self._trackers))
 
     def __getitem__(self, reference) -> "Tracker":
+        """ Returns the tracker for the given reference. """
+
         return self.resolve(reference, skip_unknown=False, resolve_plural=False)[0]
 
     def __contains__(self, reference) -> bool:
+        """ Checks if the tracker is registered. """
         identifier, _ = parse_reference(reference)
         return identifier in self._trackers
 
     def __iter__(self):
         return iter(self._trackers.values())
 
     def __len__(self):
         return len(self._trackers)
 
     def resolve(self, *references, storage=None, skip_unknown=True, resolve_plural=True):
+        """ Resolves the references to trackers.
+
+        Args:
+            storage (_type_, optional): Sto . Defaults to None.
+            skip_unknown (bool, optional): _description_. Defaults to True.
+            resolve_plural (bool, optional): _description_. Defaults to True.
+
+        Raises:
+            ToolkitException: _description_
+
+        Returns:
+            _type_: _description_
+        """        """"""
 
         trackers = []
 
         for reference in references:
 
             if resolve_plural and reference.startswith("#"):
                 tag = reference[1:]
@@ -169,14 +203,15 @@
     def references(self):
         return [t.reference for t in self._trackers.values()]
 
     def identifiers(self):
         return [t.identifier for t in self._trackers.values()]
 
 class Tracker(object):
+    """ Tracker definition class. """
 
     @staticmethod
     def _collect_envvars(**kwargs):
         envvars = dict()
         other = dict()
 
         if "env" in kwargs:
@@ -263,14 +298,15 @@
         if self.version == version or version is None:
             return self
         tracker = copy.copy(self)
         tracker._version = version
         return tracker
 
     def runtime(self, log=False) -> "TrackerRuntime":
+        """Creates a new runtime instance for this tracker instance."""
         if not self._command:
             raise TrackerException("Tracker does not have an attached executable", tracker=self)
 
         if not self._protocol in _runtime_protocols:
             raise TrackerException("Runtime protocol '{}' not available".format(self._protocol), tracker=self)
 
         return _runtime_protocols[self._protocol](self, self._command, log=log, envvars=self._envvars, arguments=self._arguments, **self._args)
@@ -315,107 +351,122 @@
         if self._version is None:
             return self._identifier
         else:
             return self._identifier + "@" + self._version
 
     @property
     def protocol(self) -> str:
+        """Returns the communication protocol used by this tracker.
+
+        Returns:
+            str: Communication protocol
+        """
         return self._protocol
 
     def describe(self):
         data = dict(command=self._command, label=self.label, protocol=self.protocol, arguments=self._arguments, env=self._envvars)
         data.update(self._args)
         return data
 
     def metadata(self, key):
+        """Returns the metadata value for specified key."""
         if not key in self._metadata:
             return None
         return self._metadata[key]
 
     def tagged(self, tag):
+        """Returns true if the tracker is tagged with specified tag."""
+
         return tag in self._tags
 
+ObjectStatus = namedtuple("ObjectStatus", ["region", "properties"])
+
+Objects = Union[List[ObjectStatus], ObjectStatus]
 class TrackerRuntime(ABC):
+    """Base class for tracker runtime implementations. """
 
     def __init__(self, tracker: Tracker):
         self._tracker = tracker
 
     @property
     def tracker(self) -> Tracker:
         return self._tracker
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
 
+    @property
+    def multiobject(self):
+        return False
+
     @abstractmethod
     def stop(self):
         pass
 
     @abstractmethod
     def restart(self):
+        """Restarts the tracker runtime, usually stars a new process."""
         pass
 
     @abstractmethod
-    def initialize(self, frame: Frame, region: Region, properties: dict = None) -> Tuple[Region, dict, float]:
+    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
         pass
 
     @abstractmethod
-    def update(self, frame: Frame, properties: dict = None) -> Tuple[Region, dict, float]:
+    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
         pass
 
 class RealtimeTrackerRuntime(TrackerRuntime):
 
     def __init__(self, runtime: TrackerRuntime, grace: int = 1, interval: float = 0.1):
         super().__init__(runtime.tracker)
         self._runtime = runtime
         self._grace = grace
         self._interval = interval
         self._countdown = 0
         self._time = 0
         self._out = None
 
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.stop()
+    @property
+    def multiobject(self):
+        return self._runtime.multiobject
 
     def stop(self):
         self._runtime.stop()
         self._time = 0
         self._out = None
 
     def restart(self):
         self._runtime.restart()
         self._time = 0
         self._out = None
 
-    def initialize(self, frame: Frame, region: Region, properties: dict = None) -> Tuple[Region, dict, float]:
+    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
         self._countdown = self._grace
         self._out = None
 
-        out, prop, time = self._runtime.initialize(frame, region, properties)
+        out, prop, time = self._runtime.initialize(frame, new, properties)
 
         if time > self._interval:
             if self._countdown > 0:
                 self._countdown = self._countdown - 1
                 self._time = 0
             else:
                 self._time = time - self._interval
                 self._out = out
         else:
             self._time = 0
 
         return out, prop, time
 
 
-    def update(self, frame: Frame, properties: dict = None) -> Tuple[Region, dict, float]:
+    def update(self, frame: Frame, _: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
 
         if self._time > self._interval:
             self._time = self._time - self._interval
             return self._out, dict(), 0
         else:
             self._out = None
             self._time = 0
@@ -436,41 +487,120 @@
 class PropertyInjectorTrackerRuntime(TrackerRuntime):
 
     def __init__(self, runtime: TrackerRuntime, **kwargs):
         super().__init__(runtime.tracker)
         self._runtime = runtime
         self._properties = {k : str(v) for k, v in kwargs.items()}
 
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.stop()
+    @property
+    def multiobject(self):
+        return self._runtime.multiobject
 
     def stop(self):
         self._runtime.stop()
 
     def restart(self):
         self._runtime.restart()
 
-    def initialize(self, frame: Frame, region: Region, properties: dict = None) -> Tuple[Region, dict, float]:
+    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
 
         if not properties is None:
             tproperties = dict(properties)
         else:
             tproperties = dict()
 
         tproperties.update(self._properties)
 
-        return self._runtime.initialize(frame, region, tproperties)
+        return self._runtime.initialize(frame, new, tproperties)
 
 
-    def update(self, frame: Frame, properties: dict = None) -> Tuple[Region, dict, float]:
-        return self._runtime.update(frame, properties)
+    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
+        return self._runtime.update(frame, new, properties)
+
+
+class SingleObjectTrackerRuntime(TrackerRuntime):
+
+    def __init__(self, runtime: TrackerRuntime):
+        super().__init__(runtime.tracker)
+        self._runtime = runtime
+
+    @property
+    def multiobject(self):
+        return False
+
+    def stop(self):
+        self._runtime.stop()
+
+    def restart(self):
+        self._runtime.restart()
+
+    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
+
+        if isinstance(new, list) and len(new) != 1: raise TrackerException("Only supports single object tracking", tracker=self.tracker)
+        status = self._runtime.initialize(frame, new, properties)
+        if isinstance(status, list): status = status[0]
+        return status
+
+    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
+
+        if not new is None: raise TrackerException("Only supports single object tracking", tracker=self.tracker)
+        status = self._runtime.update(frame, new, properties)
+        if isinstance(status, list): status = status[0]
+        return status
+
+class MultiObjectTrackerRuntime(TrackerRuntime):
+
+    def __init__(self, runtime: TrackerRuntime):
+        super().__init__(runtime.tracker)
+        if self._runtime.multiobject:
+            self._runtime = runtime
+        else:
+            self._runtime = [runtime]
+            self._used = 0
+
+    @property
+    def multiobject(self):
+        return True
+
+    def stop(self):
+        if isinstance(self._runtime, TrackerRuntime):
+            self._runtime.stop()
+        else:
+            for r in self._runtime:
+                r.stop()
+
+    def restart(self):
+        if isinstance(self._runtime, TrackerRuntime):
+            self._runtime.restart()
+        else:
+            for r in self._runtime:
+                r.restart()
 
+    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
+        if isinstance(self._runtime, TrackerRuntime):
+            return self._runtime.initialize(frame, new, properties)
+        if isinstance(new, ObjectStatus):
+            new = [new]
+
+        self._used = 0
+        status = []
+        for i, o in enumerate(new):
+            if i >= len(self._runtime):
+                self._runtime.append(self._tracker.runtime())
+                self._runtime.initialize(frame, new, properties)
+
+        if isinstance(status, list): status = status[0]
+        return status
+
+    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
+
+        if not new is None: raise TrackerException("Only supports single object tracking")
+        status = self._runtime.update(frame, new, properties)
+        if isinstance(status, list): status = status[0]
+        return status
 
 try:
 
     from vot.tracker.trax import TraxTrackerRuntime, trax_matlab_adapter, trax_python_adapter, trax_octave_adapter
 
     _runtime_protocols["trax"] = TraxTrackerRuntime
     _runtime_protocols["traxmatlab"] = trax_matlab_adapter
```

### Comparing `vot-toolkit-0.5.3/vot/tracker/dummy.py` & `vot-toolkit-0.6.0/vot/tracker/dummy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import absolute_import
 import os
 from sys import path
 import time
 
-from trax import Image, Region, Server, TraxStatus
-
 def _main():
-    region = None
+    """ Dummy tracker main function for testing purposes."""
+    from trax import Image, Region, Server, TraxStatus
+
+    objects = None
     with Server([Region.RECTANGLE], [Image.PATH]) as server:
         while True:
             request = server.wait()
             if request.type in [TraxStatus.QUIT, TraxStatus.ERROR]:
                 break
             if request.type == TraxStatus.INITIALIZE:
-                region = request.region
-            server.status(region)
+                objects = request.objects
+            server.status(objects)
             time.sleep(0.1)
 
 if __name__ == '__main__':
     _main()
 else:
     from . import Tracker
```

### Comparing `vot-toolkit-0.5.3/vot/tracker/trax.py` & `vot-toolkit-0.6.0/vot/tracker/trax.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from trax.region import Region as TraxRegion
 from trax.region import Polygon as TraxPolygon
 from trax.region import Mask as TraxMask
 from trax.region import Rectangle as TraxRectangle
 
 from vot.dataset import Frame, DatasetException
 from vot.region import Region, Polygon, Rectangle, Mask
-from vot.tracker import Tracker, TrackerRuntime, TrackerException
+from vot.tracker import Tracker, TrackerRuntime, TrackerException, Objects, ObjectStatus
 from vot.utilities import to_logical, to_number, normalize_path
 
 PORT_POOL_MIN = 9090
 PORT_POOL_MAX = 65535
 
 logger = logging.getLogger("vot")
 
@@ -84,26 +84,43 @@
 def convert_region(region: Region) -> TraxRegion:
     if isinstance(region, Rectangle):
         return TraxRectangle.create(region.x, region.y, region.width, region.height)
     elif isinstance(region, Polygon):
         return TraxPolygon.create([region[i] for i in range(region.size)])
     elif isinstance(region, Mask):
         return TraxMask.create(region.mask, x=region.offset[0], y=region.offset[1])
-
     return None
 
 def convert_traxregion(region: TraxRegion) -> Region:
     if region.type == TraxRegion.RECTANGLE:
         x, y, width, height = region.bounds()
         return Rectangle(x, y, width, height)
     elif region.type == TraxRegion.POLYGON:
         return Polygon(list(region))
     elif region.type == TraxRegion.MASK:
         return Mask(region.array(), region.offset(), optimize=True)
+    return None
 
+def convert_objects(objects: Objects) -> TraxRegion:
+    if objects is None: return []
+    if isinstance(objects, (list, )):
+        return [(convert_region(o.region), dict(o.properties)) for o in objects]
+    if isinstance(objects, (ObjectStatus, )):
+        return [(convert_region(objects.region), dict(objects.properties))]
+    else:
+        return [(convert_region(objects), dict())]
+
+def convert_traxobjects(region: TraxRegion) -> Region:
+    if region.type == TraxRegion.RECTANGLE:
+        x, y, width, height = region.bounds()
+        return Rectangle(x, y, width, height)
+    elif region.type == TraxRegion.POLYGON:
+        return Polygon(list(region))
+    elif region.type == TraxRegion.MASK:
+        return Mask(region.array(), region.offset(), optimize=True)
     return None
 
 class TestRasterMethods(unittest.TestCase):
 
     def test_convert_traxregion(self):
         convert_traxregion(TraxRectangle.create(0, 0, 10, 10))
         convert_traxregion(TraxPolygon.create([(0, 0), (10, 0), (10, 10), (0, 10)]))
@@ -184,21 +201,23 @@
         try:
             if socket:
                 self._client = Client(stream=self._socket.fileno(), timeout=30, log=log)
             else:
                 self._client = Client(
                     stream=(self._process.stdin.fileno(), self._process.stdout.fileno()), log=log
                 )
+                
         except TraxException as e:
             self.terminate()
             self._watchdog_reset(False)
             raise e
         self._watchdog_reset(False)
 
         self._has_vot_wrapper = not self._client.get("vot") is None
+        self._multiobject = self._client.get("multiobject")
 
     def _watchdog_reset(self, enable=True):
         if self._watchdog_counter == 0:
             return
 
         if enable:
             self._watchdog_counter = self._timeout * 10
@@ -236,48 +255,54 @@
     @property
     def alive(self):
         if self._process is None:
             return False
         self._returncode = self._process.returncode
         return self._returncode is None
 
-    def initialize(self, frame: Frame, region: Region, properties: dict = None) -> Tuple[Region, dict, float]:
+    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
 
         if not self.alive:
             raise TraxException("Tracker not alive")
 
         if properties is None:
             properties = dict()
 
         tlist = convert_frame(frame, self._client.channels)
-        tregion = convert_region(region)
+        tobjects = convert_objects(new)
 
         self._watchdog_reset(True)
 
-        region, properties, elapsed = self._client.initialize(tlist, tregion, properties)
+        status, elapsed = self._client.initialize(tlist, tobjects, properties)
 
         self._watchdog_reset(False)
 
-        return convert_traxregion(region), properties.dict(), elapsed
+        status = [ObjectStatus(convert_traxregion(region), properties) for region, properties in status]
+
+        return status, elapsed
 
 
-    def frame(self, frame: Frame, properties: dict = dict()) -> Tuple[Region, dict, float]:
+    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
 
         if not self.alive:
             raise TraxException("Tracker not alive")
 
         tlist = convert_frame(frame, self._client.channels)
 
+        tobjects = convert_objects(new)
+
         self._watchdog_reset(True)
 
-        region, properties, elapsed = self._client.frame(tlist, properties)
+        status, elapsed = self._client.frame(tlist, properties, tobjects)
 
         self._watchdog_reset(False)
 
-        return convert_traxregion(region), properties.dict(), elapsed
+        status = [ObjectStatus(convert_traxregion(region), properties) for region, properties in status]
+
+        return status, elapsed
 
     def terminate(self):
         with self._watchdog_lock:
 
             if not self.alive:
                 return
 
@@ -363,14 +388,19 @@
 
         self._envvars = envvars
 
     @property
     def tracker(self) -> Tracker:
         return self._tracker
 
+    @property
+    def multiobject(self):
+        self._connect()
+        return self._process._multiobject
+
     def _connect(self):
         if not self._process:
             if not self._output is None:
                 log = self._output
             else:
                 log = ColorizedOutput()
             self._process = TrackerProcess(self._command, self._envvars, log=log, socket=self._socket, timeout=self._timeout)
@@ -411,46 +441,44 @@
     def restart(self):
         try:
             self.stop()
             self._connect()
         except TraxException as e:
             self._error(e)
 
-    def initialize(self, frame: Frame, region: Region, properties: dict = None) -> Tuple[Region, dict, float]:
+    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
         try:
             if self._restart:
                 self.stop()
             self._connect()
 
             tproperties = dict(self._arguments)
 
             if not properties is None:
                 tproperties.update(properties)
 
-            return self._process.initialize(frame, region, tproperties)
+            return self._process.initialize(frame, new, tproperties)
         except TraxException as e:
             self._error(e)
 
-    def update(self, frame: Frame, properties: dict = None) -> Tuple[Region, dict, float]:
+    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
         try:
             if properties is None:
                 properties = dict()
-            return self._process.frame(frame, properties)
+            return self._process.update(frame, new, properties)
         except TraxException as e:
             self._error(e)
 
     def stop(self):
         if not self._process is None:
             self._process.terminate()
             self._process = None
 
     def __del__(self):
-        if not self._process is None:
-            self._process.terminate()
-            self._process = None
+        self.stop()
 
 def escape_path(path):
     if sys.platform.startswith("win"):
         return path.replace("\\\\", "\\").replace("\\", "\\\\")
     else:
         return path
```

### Comparing `vot-toolkit-0.5.3/vot/utilities/__init__.py` & `vot-toolkit-0.6.0/vot/utilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,17 @@
         return kls.__name__  # Avoid reporting __builtin__
     else:
         return module + '.' + kls.__name__
 
 def flip(size: Tuple[Number, Number]) -> Tuple[Number, Number]:
     return (size[1], size[0])
 
+def flatten(nested_list):
+    return [item for sublist in nested_list for item in sublist]
+
 from vot.utilities.notebook import is_notebook
 
 if is_notebook():
     try:
         from ipywidgets import IntProgress
         from tqdm._tqdm_notebook import tqdm_notebook as tqdm
     except ImportError:
```

### Comparing `vot-toolkit-0.5.3/vot/utilities/cli.py` & `vot-toolkit-0.6.0/vot/utilities/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,18 @@
 def do_test(config: argparse.Namespace):
     """Run a test for a tracker
 
     Args:
         config (argparse.Namespace): Configuration
     """
     from vot.dataset.dummy import DummySequence
-    from vot.dataset import load_sequence
+    from vot.dataset import load_sequence, Frame
+    from vot.tracker import ObjectStatus
+    from vot.experiment.helpers import MultiObjectHelper
+
     trackers = Registry(config.registry)
 
     if not config.tracker:
         logger.error("Unable to continue without a tracker")
         logger.error("List of found trackers: ")
         for k in trackers.identifiers():
             logger.error(" * %s", k)
@@ -53,65 +56,80 @@
 
     if not config.tracker in trackers:
         logger.error("Tracker does not exist")
         return
 
     tracker = trackers[config.tracker]
 
-    logger.info("Generating dummy sequence")
-
-    if config.sequence is None:
-        sequence = DummySequence(50)
-    else:
-        sequence = load_sequence(normalize_path(config.sequence))
-
-    logger.info("Obtaining runtime for tracker %s", tracker.identifier)
-
-    if config.visualize:
-        import matplotlib.pylab as plt
-        from vot.utilities.draw import MatplotlibDrawHandle
-        figure = plt.figure()
-        figure.canvas.set_window_title('VOT Test')
-        axes = figure.add_subplot(1, 1, 1)
-        axes.set_aspect("equal")
-        handle = MatplotlibDrawHandle(axes, size=sequence.size)
-        handle.style(fill=False)
-        figure.show()
-
-    runtime = None
-
+    def visualize(axes, frame: Frame, reference, state):
+        axes.clear()
+        handle.image(frame.channel())
+        if not isinstance(state, list):
+            state = [state]
+        for gt, st in zip(reference, state):
+            handle.style(color="green").region(gt)
+            handle.style(color="red").region(st.region)
+        
     try:
 
         runtime = tracker.runtime(log=True)
 
-        for repeat in range(1, 4):
+        logger.info("Generating dummy sequence")
+
+        if config.sequence is None:
+            sequence = DummySequence(50, objects=3 if runtime.multiobject else 1)
+        else:
+            sequence = load_sequence(normalize_path(config.sequence))
 
-            logger.info("Initializing tracker ({}/{})".format(repeat, 3))
+        logger.info("Obtaining runtime for tracker %s", tracker.identifier)
 
-            region, _, _ = runtime.initialize(sequence.frame(0), sequence.groundtruth(0))
+        context = {"continue" : True}
+
+        def on_press(event):
+            if event.key == 'q':
+                context["continue"] = False
+
+        if config.visualize:
+            import matplotlib.pylab as plt
+            from vot.utilities.draw import MatplotlibDrawHandle
+            figure = plt.figure()
+            figure.canvas.set_window_title('VOT Test')
+            axes = figure.add_subplot(1, 1, 1)
+            axes.set_aspect("equal")
+            handle = MatplotlibDrawHandle(axes, size=sequence.size)
+            context["click"] = figure.canvas.mpl_connect('key_press_event', on_press)
+            handle.style(fill=False)
+            figure.show()
+
+        helper = MultiObjectHelper(sequence)
+
+        logger.info("Initializing tracker")
+
+        frame = sequence.frame(0)
+        state, _ = runtime.initialize(frame, [ObjectStatus(frame.object(x), {}) for x in helper.new(0)])
+
+        if config.visualize:
+            visualize(axes, frame, [frame.object(x) for x in helper.objects(0)], state)
+            figure.canvas.draw()
+
+        for i in range(1, len(sequence)):
+            
+            logger.info("Processing frame %d/%d", i, sequence.length-1)
+            frame = sequence.frame(i)
+            state, _ = runtime.update(frame, [ObjectStatus(frame.object(x), {}) for x in helper.new(i)])
 
             if config.visualize:
-                axes.clear()
-                handle.image(sequence.frame(0).channel())
-                handle.style(color="green").region(sequence.frame(0).groundtruth())
-                handle.style(color="red").region(region)
+                visualize(axes, frame, [frame.object(x) for x in helper.objects(i)], state)
                 figure.canvas.draw()
+                figure.canvas.flush_events()
 
-            for i in range(1, sequence.length):
-                logger.info("Updating on frame %d/%d", i, sequence.length-1)
-                region, _, _ = runtime.update(sequence.frame(i))
-
-                if config.visualize:
-                    axes.clear()
-                    handle.image(sequence.frame(i).channel())
-                    handle.style(color="green").region(sequence.frame(i).groundtruth())
-                    handle.style(color="red").region(region)
-                    figure.canvas.draw()
+            if not context["continue"]:
+                break
 
-            logger.info("Stopping tracker")
+        logger.info("Stopping tracker")
 
         runtime.stop()
 
         logger.info("Test concluded successfuly")
 
     except TrackerException as te:
         logger.error("Error during tracker execution: {}".format(te))
@@ -154,34 +172,34 @@
 
 def do_evaluate(config: argparse.Namespace):
 
     from vot.experiment import run_experiment
 
     workspace = Workspace.load(config.workspace)
 
-    logger.info("Loaded workspace in '%s'", config.workspace)
+    logger.debug("Loaded workspace in '%s'", config.workspace)
 
     global_registry = [os.path.abspath(x) for x in config.registry]
 
     registry = Registry(list(workspace.registry) + global_registry, root=config.workspace)
 
-    logger.info("Found data for %d trackers", len(registry))
+    logger.debug("Found data for %d trackers", len(registry))
 
     trackers = registry.resolve(*config.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
 
     if len(trackers) == 0:
         logger.error("Unable to continue without at least on tracker")
         logger.error("List of available found trackers: ")
         for k in registry.identifiers():
             logger.error(" * %s", k)
         return
 
     try:
         for tracker in trackers:
-            logger.info("Evaluating tracker %s", tracker.identifier)
+            logger.debug("Evaluating tracker %s", tracker.identifier)
             for experiment in workspace.stack:
                 run_experiment(experiment, tracker, workspace.dataset, config.force, config.persist)
 
         logger.info("Evaluation concluded successfuly")
 
     except KeyboardInterrupt:
         logger.info("Evaluation interrupted by the user")
@@ -191,21 +209,21 @@
 def do_analysis(config: argparse.Namespace):
 
     from vot.analysis import AnalysisProcessor, process_stack_analyses
     from vot.document import generate_document
 
     workspace = Workspace.load(config.workspace)
 
-    logger.info("Loaded workspace in '%s'", config.workspace)
+    logger.debug("Loaded workspace in '%s'", config.workspace)
 
     global_registry = [os.path.abspath(x) for x in config.registry]
 
     registry = Registry(list(workspace.registry) + global_registry, root=config.workspace)
 
-    logger.info("Found data for %d trackers", len(registry))
+    logger.debug("Found data for %d trackers", len(registry))
 
     if not config.trackers:
         trackers = workspace.list_results(registry)
     else:
         trackers = registry.resolve(*config.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
 
     if not trackers:
@@ -264,47 +282,46 @@
 
     Args:
         config ([type]): [description]
     """
 
     import zipfile, io
     from shutil import copyfileobj
+    from vot.utilities import flatten
 
     workspace = Workspace.load(config.workspace)
 
-    logger.info("Loaded workspace in '%s'", config.workspace)
+    logger.debug("Loaded workspace in '%s'", config.workspace)
 
     registry = Registry(list(workspace.registry) + config.registry, root=config.workspace)
 
-    logger.info("Found data for %d trackers", len(registry))
-
     tracker = registry[config.tracker]
 
     logger.info("Packaging results for tracker %s", tracker.identifier)
 
     all_files = []
     can_finish = True
 
     with Progress("Scanning", len(workspace.dataset) * len(workspace.stack)) as progress:
 
         for experiment in workspace.stack:
-            for sequence in workspace.dataset:
-                sequence = experiment.transform(sequence)
+            sequences = experiment.transform(workspace.dataset)
+            for sequence in sequences:
                 complete, files, results = experiment.scan(tracker, sequence)
                 all_files.extend([(f, experiment.identifier, sequence.name, results) for f in files])
                 if not complete:
                     logger.error("Results are not complete for experiment %s, sequence %s", experiment.identifier, sequence.name)
                     can_finish = False
                 progress.relative(1)
 
     if not can_finish:
         logger.error("Unable to continue, experiments not complete")
         return
 
-    logger.info("Collected %d files, compressing to archive ...", len(all_files))
+    logger.debug("Collected %d files, compressing to archive ...", len(all_files))
 
     timestamp = datetime.now()
 
     archive_name = "{}_{:%Y-%m-%dT%H-%M-%S.%f%z}.zip".format(tracker.identifier, timestamp)
 
     with Progress("Compressing", len(all_files)) as progress:
 
@@ -369,15 +386,15 @@
 
     try:
 
         args = parser.parse_args()
 
         logger.setLevel(logging.INFO)
 
-        if args.debug or check_debug:
+        if args.debug or check_debug():
             logger.setLevel(logging.DEBUG)
 
         update, version = check_updates()
         if update:
             logger.warning("A newer version of the VOT toolkit is available (%s), please update.", version)
 
         if args.action == "test":
```

### Comparing `vot-toolkit-0.5.3/vot/utilities/data.py` & `vot-toolkit-0.6.0/vot/utilities/data.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/utilities/draw.py` & `vot-toolkit-0.6.0/vot/utilities/draw.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/utilities/migration.py` & `vot-toolkit-0.6.0/vot/utilities/migration.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/utilities/net.py` & `vot-toolkit-0.6.0/vot/utilities/net.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/utilities/notebook.py` & `vot-toolkit-0.6.0/vot/utilities/notebook.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot/workspace/__init__.py` & `vot-toolkit-0.6.0/vot/workspace/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 
 import os
 import typing
 import importlib
 
 import yaml
+from lazy_object_proxy import Proxy
 
 from attributee import Attribute, Attributee, Nested, List, String, CoerceContext
 
 from .. import ToolkitException, get_logger
 from ..dataset import Dataset, load_dataset
 from ..tracker import Registry, Tracker
 from ..stack import Stack, resolve_stack
-from ..utilities import normalize_path, class_fullname
+from ..utilities import normalize_path
 from ..document import ReportConfiguration
-from .storage import LocalStorage, Storage, NullStorage
+from .storage import LocalStorage, Storage, NullStorage, StorageConfiguration
+
 
 _logger = get_logger()
 
 class WorkspaceException(ToolkitException):
     """Errors related to workspace raise this exception
     """
     pass
@@ -53,14 +55,15 @@
     given experiments on a provided dataset.
     """
 
     registry = List(String(transformer=lambda x, ctx: normalize_path(x, ctx.parent.directory)))
     stack = StackLoader()
     sequences = String(default="sequences")
     report = Nested(ReportConfiguration)
+    results = Nested(StorageConfiguration)
 
     @staticmethod
     def initialize(directory: str, config: typing.Optional[typing.Dict] = None, download: bool = True) -> None:
         """Initialize a new workspace in a given directory with the given config
 
         Args:
             directory (str): Root for workspace storage
@@ -143,17 +146,20 @@
         """Do not call this constructor directly unless you know what you are doing, 
         instead use the static Workspace.load method.
 
         Args:
             directory ([type]): [description]
         """
         self._directory = directory
-        self._storage = LocalStorage(directory) if directory is not None else NullStorage()
 
+        self._storage = Proxy(lambda: LocalStorage(directory, self.results) if directory is not None else NullStorage())
+        
         super().__init__(**kwargs)
+
+        
         dataset_directory = normalize_path(self.sequences, directory)
 
         if not self.stack.dataset is None:
             Workspace.download_dataset(self.stack.dataset, dataset_directory)
 
         self._dataset = load_dataset(dataset_directory)
```

### Comparing `vot-toolkit-0.5.3/vot/workspace/storage.py` & `vot-toolkit-0.6.0/vot/workspace/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 from attributee.object import class_fullname
 
 from ..experiment import Experiment
 from ..dataset import Sequence
 from ..tracker import Tracker, Results
 
+from attributee import Attributee, Boolean
+
+class StorageConfiguration(Attributee):
+    binary = Boolean(default=True)
+
 class Storage(ABC):
     """Abstract superclass for workspace storage abstraction
     """
 
     @abstractmethod
     def results(self, tracker: Tracker, experiment: Experiment, sequence: Sequence) -> Results:
         """Returns results object for the given tracker, experiment, sequence combination
@@ -24,14 +29,18 @@
         Args:
             tracker (Tracker): Selected tracker
             experiment (Experiment): Selected experiment
             sequence (Sequence): Selected sequence
         """
         pass
 
+    @property
+    def config(self) -> StorageConfiguration:
+        return StorageConfiguration()
+
     @abstractmethod
     def documents(self) -> typing.List[str]:
         """Lists documents in the storage.
         """
         pass
 
     @abstractmethod
@@ -169,22 +178,27 @@
     def copy(self, localfile, destination):
         return
 
 class LocalStorage(Storage):
     """Storage backed by the local filesystem.
     """
 
-    def __init__(self, root: str):
+    def __init__(self, root: str, config: StorageConfiguration = None):
         self._root = root
         self._results = os.path.join(root, "results")
+        self._config = config if config is not None else StorageConfiguration()
 
     def __repr__(self) -> str:
         return "<Local storage: {}>".format(self._root)
 
     @property
+    def config(self) -> StorageConfiguration:
+        return self._config
+
+    @property
     def base(self) -> str:
         return self._root
 
     def results(self, tracker: Tracker, experiment: Experiment, sequence: Sequence):
         storage = LocalStorage(os.path.join(self._results, tracker.reference, experiment.identifier, sequence.name))
         return Results(storage)
 
@@ -221,15 +235,15 @@
     def isdocument(self, name):
         return os.path.isfile(os.path.join(self._root, name))
 
     def isfolder(self, name):
         return os.path.isdir(os.path.join(self._root, name))
 
     def substorage(self, name):
-        return LocalStorage(os.path.join(self.base, name))
+        return LocalStorage(os.path.join(self.base, name), self._config)
 
     def copy(self, localfile, destination):
         import shutil
         if os.path.isabs(destination):
             raise IOError("Only relative paths allowed")
 
         full = os.path.join(self.base, destination)
```

### Comparing `vot-toolkit-0.5.3/vot/workspace/tests.py` & `vot-toolkit-0.6.0/vot/workspace/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.5.3/vot_toolkit.egg-info/PKG-INFO` & `vot-toolkit-0.6.0/vot_toolkit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.5.3
+Version: 0.6.0
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         The VOT evaluation toolkit
         ==========================
         
         This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
         
-        For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://service.ait.ac.at/mailman/listinfo/votchallenge) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
+        For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
         
         Developers
         ----------
         
-        * [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana (lead developer)
+        The VOT toolkit is developed and maintained by  [Luka Čehovin Zajc](https://vicos.si/lukacu) with the help of the VOT innitiative members and the VOT community.
+        
+        Contributors:
+        
+        * [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana
         * [Alan Lukežič](https://vicos.si/people/alan_lukezic/), University of Ljubljana
         * Yan Song, Tampere University
         
+        Acknowledgements
+        ----------------
+        
+        The development of this package was supported by Sloveninan research agency (ARRS) projects Z2-1866 and J2-316.
+        
         License
         -------
         
         Copyright (C) 2021 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
         
         This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
         
@@ -39,9 +48,9 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `vot-toolkit-0.5.3/vot_toolkit.egg-info/SOURCES.txt` & `vot-toolkit-0.6.0/vot_toolkit.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 requirements.txt
 setup.py
 vot/__init__.py
 vot/__main__.py
 vot/version.py
 vot/analysis/__init__.py
 vot/analysis/_processor.py
-vot/analysis/basic.py
+vot/analysis/accuracy.py
+vot/analysis/failures.py
+vot/analysis/longterm.py
 vot/analysis/multistart.py
 vot/analysis/supervised.py
-vot/analysis/tpr.py
 vot/dataset/__init__.py
 vot/dataset/cow.png
 vot/dataset/dummy.py
 vot/dataset/got10k.py
 vot/dataset/otb.py
 vot/dataset/proxy.py
 vot/dataset/trackingnet.py
@@ -27,45 +28,51 @@
 vot/document/latex.py
 vot/document/pure.css
 vot/document/report.css
 vot/document/report.js
 vot/document/table.js
 vot/document/tests.py
 vot/experiment/__init__.py
+vot/experiment/helpers.py
 vot/experiment/multirun.py
 vot/experiment/multistart.py
 vot/experiment/transformer.py
 vot/region/__init__.py
 vot/region/io.py
 vot/region/raster.py
 vot/region/shapes.py
 vot/region/tests.py
 vot/stack/__init__.py
 vot/stack/otb100.yaml
 vot/stack/otb50.yaml
-vot/stack/testing.yaml
 vot/stack/tests.py
 vot/stack/vot2013.yaml
 vot/stack/vot2014.yaml
-vot/stack/vot2015.yaml
-vot/stack/vot2016.yaml
 vot/stack/vot2017.yaml
-vot/stack/vot2018.yaml
-vot/stack/vot2019.yaml
-vot/stack/vot2020.yaml
-vot/stack/vot2021.yaml
-vot/stack/votlt2019.yaml
-vot/stack/votlt2020.yaml
-vot/stack/votlt2021.yaml
-vot/stack/votrgbd2019.yaml
-vot/stack/votrgbd2020.yaml
-vot/stack/votrgbd2021.yaml
-vot/stack/votrgbtir2020.yaml
-vot/stack/vottir2015.yaml
-vot/stack/vottir2016.yaml
+vot/stack/vots2023.yaml
+vot/stack/tests/basic.yaml
+vot/stack/tests/multiobject.yaml
+vot/stack/tests/segmentation.yaml
+vot/stack/vot2015/rgb.yaml
+vot/stack/vot2015/tir.yaml
+vot/stack/vot2016/rgb.yaml
+vot/stack/vot2016/tir.yaml
+vot/stack/vot2018/longterm.yaml
+vot/stack/vot2018/shortterm.yaml
+vot/stack/vot2019/longterm.yaml
+vot/stack/vot2019/rgbd.yaml
+vot/stack/vot2019/rgbtir.yaml
+vot/stack/vot2019/shortterm.yaml
+vot/stack/vot2020/longterm.yaml
+vot/stack/vot2020/rgbd.yaml
+vot/stack/vot2020/rgbtir.yaml
+vot/stack/vot2020/shortterm.yaml
+vot/stack/vot2021/lt.yaml
+vot/stack/vot2021/rgbd.yaml
+vot/stack/vot2021/st.yaml
 vot/stack/vot2022/depth.yaml
 vot/stack/vot2022/lt.yaml
 vot/stack/vot2022/rgbd.yaml
 vot/stack/vot2022/stb.yaml
 vot/stack/vot2022/sts.yaml
 vot/tracker/__init__.py
 vot/tracker/dummy.py
```

