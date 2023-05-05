# Comparing `tmp/spyder-modelx-0.8.0.tar.gz` & `tmp/spyder-modelx-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\spyder-modelx-0.8.0.tar", last modified: Wed May 19 13:36:23 2021, max compression
+gzip compressed data, was "dist\spyder-modelx-0.9.0.tar", last modified: Fri Jul 23 02:25:58 2021, max compression
```

## Comparing `spyder-modelx-0.8.0.tar` & `spyder-modelx-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:23.000000 spyder-modelx-0.8.0/
--rw-rw-rw-   0        0        0        0 2018-08-13 13:21:38.000000 spyder-modelx-0.8.0/CHANGELOG.md
--rw-rw-rw-   0        0        0       28 2018-08-13 13:21:38.000000 spyder-modelx-0.8.0/CONTRIBUTORS.md
--rw-rw-rw-   0        0        0    35147 2017-09-09 01:33:52.000000 spyder-modelx-0.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0      116 2018-08-13 13:21:38.000000 spyder-modelx-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2701 2021-05-19 13:36:23.000000 spyder-modelx-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2021-04-24 03:31:59.000000 spyder-modelx-0.8.0/README.rst
--rw-rw-rw-   0        0        0       42 2021-05-19 13:36:23.000000 spyder-modelx-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     3094 2021-05-19 11:25:06.000000 spyder-modelx-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx/
--rw-rw-rw-   0        0        0      924 2019-03-17 14:07:40.000000 spyder-modelx-0.8.0/spyder_modelx/__init__.py
--rw-rw-rw-   0        0        0      773 2021-05-19 13:31:25.000000 spyder-modelx-0.8.0/spyder_modelx/_version.py
--rw-rw-rw-   0        0        0    16238 2021-05-19 11:25:06.000000 spyder-modelx-0.8.0/spyder_modelx/mxkernel.py
--rw-rw-rw-   0        0        0     2645 2019-06-15 03:46:41.000000 spyder-modelx-0.8.0/spyder_modelx/mxkernelspec.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx/plugins/
--rw-rw-rw-   0        0        0        0 2019-03-16 13:52:25.000000 spyder-modelx-0.8.0/spyder_modelx/plugins/__init__.py
--rw-rw-rw-   0        0        0     4055 2020-02-16 01:46:28.000000 spyder-modelx-0.8.0/spyder_modelx/plugins/analyzer_plugin.py
--rw-rw-rw-   0        0        0    12932 2021-05-07 07:14:53.000000 spyder-modelx-0.8.0/spyder_modelx/plugins/dataview_plugin.py
--rw-rw-rw-   0        0        0    16386 2021-05-07 14:50:23.000000 spyder-modelx-0.8.0/spyder_modelx/plugins/mxplugin.py
--rw-rw-rw-   0        0        0     5738 2020-01-02 09:23:12.000000 spyder-modelx-0.8.0/spyder_modelx/plugins/stacked_mixin.py
--rw-rw-rw-   0        0        0     4047 2019-03-23 09:21:22.000000 spyder-modelx-0.8.0/spyder_modelx/start_kernel.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx/tests/
--rw-rw-rw-   0        0        0      724 2019-03-17 14:07:41.000000 spyder-modelx-0.8.0/spyder_modelx/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx/tests/fromspyder/
--rw-rw-rw-   0        0        0     1346 2018-10-17 14:20:08.000000 spyder-modelx-0.8.0/spyder_modelx/tests/fromspyder/__init__.py
--rw-rw-rw-   0        0        0    18460 2021-03-17 13:28:39.000000 spyder-modelx-0.8.0/spyder_modelx/tests/fromspyder/test_mxdataview.py
--rw-rw-rw-   0        0        0     2581 2019-03-17 14:07:40.000000 spyder-modelx-0.8.0/spyder_modelx/tests/test_plugin.py
--rw-rw-rw-   0        0        0     1894 2019-06-15 03:15:55.000000 spyder-modelx-0.8.0/spyder_modelx/util.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx/utility/
--rw-rw-rw-   0        0        0        0 2020-04-02 08:56:04.000000 spyder-modelx-0.8.0/spyder_modelx/utility/__init__.py
--rw-rw-rw-   0        0        0    15692 2020-05-10 04:43:39.000000 spyder-modelx-0.8.0/spyder_modelx/utility/formula.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:23.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/
--rw-rw-rw-   0        0        0      729 2019-03-17 14:07:41.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/__init__.py
--rw-rw-rw-   0        0        0    20798 2021-05-19 11:25:06.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxanalyzer.py
--rw-rw-rw-   0        0        0     7625 2020-04-19 06:53:16.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxclient.py
--rw-rw-rw-   0        0        0     8922 2021-04-15 03:33:56.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxcodeeditor.py
--rw-rw-rw-   0        0        0     7354 2021-04-15 03:06:52.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxcodelist.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:23.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/
--rw-rw-rw-   0        0        0        0 2021-03-17 09:27:49.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/__init__.py
--rw-rw-rw-   0        0        0    35668 2021-05-07 08:00:38.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/arrayviewer.py
--rw-rw-rw-   0        0        0    69225 2021-05-07 14:46:29.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/collectionsviewer.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:23.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat32/
--rw-rw-rw-   0        0        0        0 2021-03-21 03:48:59.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat32/__init__.py
--rw-rw-rw-   0        0        0    32875 2021-03-21 07:09:15.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat32/arrayviewer.py
--rw-rw-rw-   0        0        0    59005 2021-03-21 07:25:26.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat32/collectionsviewer.py
--rw-rw-rw-   0        0        0    33122 2021-03-21 07:01:42.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat32/dataframeviewer.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:23.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat33/
--rw-rw-rw-   0        0        0        0 2021-03-21 03:48:59.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat33/__init__.py
--rw-rw-rw-   0        0        0    65006 2021-03-28 08:49:22.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat33/collectionsviewer.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:23.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat401/
--rw-rw-rw-   0        0        0        0 2021-03-21 03:48:59.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat401/__init__.py
--rw-rw-rw-   0        0        0    35518 2021-03-21 06:27:20.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat401/arrayviewer.py
--rw-rw-rw-   0        0        0    66926 2021-03-28 11:26:09.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat401/collectionsviewer.py
--rw-rw-rw-   0        0        0    27841 2021-03-21 13:17:25.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat401/dataframeviewer.py
--rw-rw-rw-   0        0        0    57367 2021-05-07 08:47:50.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/dataframeviewer.py
--rw-rw-rw-   0        0        0    41762 2021-04-22 15:21:43.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxexplorer.py
--rw-rw-rw-   0        0        0     1619 2021-03-17 13:28:39.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxlineedit.py
--rw-rw-rw-   0        0        0    12855 2021-03-08 13:57:21.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxproperty.py
--rw-rw-rw-   0        0        0    30949 2021-05-19 11:25:06.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxshell.py
--rw-rw-rw-   0        0        0     5327 2020-01-02 09:32:14.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxtoolbar.py
--rw-rw-rw-   0        0        0    16273 2021-04-16 08:41:42.000000 spyder-modelx-0.8.0/spyder_modelx/widgets/mxtreemodel.py
-drwxrwxrwx   0        0        0        0 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx.egg-info/
--rw-rw-rw-   0        0        0     2701 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2051 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-05-19 13:36:22.000000 spyder-modelx-0.8.0/spyder_modelx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/
+-rw-rw-rw-   0        0        0        0 2018-08-13 13:21:38.000000 spyder-modelx-0.9.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0       28 2018-08-13 13:21:38.000000 spyder-modelx-0.9.0/CONTRIBUTORS.md
+-rw-rw-rw-   0        0        0    35147 2017-09-09 01:33:52.000000 spyder-modelx-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      116 2018-08-13 13:21:38.000000 spyder-modelx-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2701 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2021-04-24 03:31:59.000000 spyder-modelx-0.9.0/README.rst
+-rw-rw-rw-   0        0        0       42 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     3094 2021-07-23 02:24:25.000000 spyder-modelx-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/
+-rw-rw-rw-   0        0        0      924 2019-03-17 14:07:40.000000 spyder-modelx-0.9.0/spyder_modelx/__init__.py
+-rw-rw-rw-   0        0        0      773 2021-07-23 02:24:25.000000 spyder-modelx-0.9.0/spyder_modelx/_version.py
+-rw-rw-rw-   0        0        0    16858 2021-07-07 08:18:41.000000 spyder-modelx-0.9.0/spyder_modelx/mxkernel.py
+-rw-rw-rw-   0        0        0     2645 2019-06-15 03:46:41.000000 spyder-modelx-0.9.0/spyder_modelx/mxkernelspec.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/plugins/
+-rw-rw-rw-   0        0        0        0 2021-07-03 15:27:02.000000 spyder-modelx-0.9.0/spyder_modelx/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4055 2021-07-06 16:24:43.000000 spyder-modelx-0.9.0/spyder_modelx/plugins/analyzer_plugin.py
+-rw-rw-rw-   0        0        0    13787 2021-07-09 02:33:14.000000 spyder-modelx-0.9.0/spyder_modelx/plugins/dataview_plugin.py
+-rw-rw-rw-   0        0        0    16386 2021-05-07 14:50:23.000000 spyder-modelx-0.9.0/spyder_modelx/plugins/mxplugin.py
+-rw-rw-rw-   0        0        0     5738 2021-07-07 02:24:47.000000 spyder-modelx-0.9.0/spyder_modelx/plugins/stacked_mixin.py
+-rw-rw-rw-   0        0        0     4047 2019-03-23 09:21:22.000000 spyder-modelx-0.9.0/spyder_modelx/start_kernel.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/tests/
+-rw-rw-rw-   0        0        0      724 2019-03-17 14:07:41.000000 spyder-modelx-0.9.0/spyder_modelx/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/tests/fromspyder/
+-rw-rw-rw-   0        0        0     1346 2018-10-17 14:20:08.000000 spyder-modelx-0.9.0/spyder_modelx/tests/fromspyder/__init__.py
+-rw-rw-rw-   0        0        0    18460 2021-03-17 13:28:39.000000 spyder-modelx-0.9.0/spyder_modelx/tests/fromspyder/test_mxdataview.py
+-rw-rw-rw-   0        0        0     2581 2019-03-17 14:07:40.000000 spyder-modelx-0.9.0/spyder_modelx/tests/test_plugin.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/utility/
+-rw-rw-rw-   0        0        0        0 2020-04-02 08:56:04.000000 spyder-modelx-0.9.0/spyder_modelx/utility/__init__.py
+-rw-rw-rw-   0        0        0    15692 2020-05-10 04:43:39.000000 spyder-modelx-0.9.0/spyder_modelx/utility/formula.py
+-rw-rw-rw-   0        0        0     1894 2021-07-03 15:27:31.000000 spyder-modelx-0.9.0/spyder_modelx/utility/tupleencoder.py
+-rw-rw-rw-   0        0        0     1847 2021-07-03 15:44:16.000000 spyder-modelx-0.9.0/spyder_modelx/utility/typeutil.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/
+-rw-rw-rw-   0        0        0      729 2019-03-17 14:07:41.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/__init__.py
+-rw-rw-rw-   0        0        0    20817 2021-07-07 08:35:44.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxanalyzer.py
+-rw-rw-rw-   0        0        0     7625 2020-04-19 06:53:16.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxclient.py
+-rw-rw-rw-   0        0        0     8922 2021-04-15 03:33:56.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxcodeeditor.py
+-rw-rw-rw-   0        0        0     7354 2021-04-15 03:06:52.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxcodelist.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/
+-rw-rw-rw-   0        0        0        0 2021-03-17 09:27:49.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/__init__.py
+-rw-rw-rw-   0        0        0    35668 2021-05-07 08:00:38.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/arrayviewer.py
+-rw-rw-rw-   0        0        0    69225 2021-05-07 14:46:29.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/collectionsviewer.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat32/
+-rw-rw-rw-   0        0        0        0 2021-03-21 03:48:59.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat32/__init__.py
+-rw-rw-rw-   0        0        0    32875 2021-03-21 07:09:15.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat32/arrayviewer.py
+-rw-rw-rw-   0        0        0    59005 2021-03-21 07:25:26.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat32/collectionsviewer.py
+-rw-rw-rw-   0        0        0    33122 2021-03-21 07:01:42.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat32/dataframeviewer.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat33/
+-rw-rw-rw-   0        0        0        0 2021-03-21 03:48:59.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat33/__init__.py
+-rw-rw-rw-   0        0        0    65006 2021-03-28 08:49:22.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat33/collectionsviewer.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat401/
+-rw-rw-rw-   0        0        0        0 2021-03-21 03:48:59.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat401/__init__.py
+-rw-rw-rw-   0        0        0    35518 2021-03-21 06:27:20.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat401/arrayviewer.py
+-rw-rw-rw-   0        0        0    66926 2021-03-28 11:26:09.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat401/collectionsviewer.py
+-rw-rw-rw-   0        0        0    27841 2021-03-21 13:17:25.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat401/dataframeviewer.py
+-rw-rw-rw-   0        0        0    57367 2021-05-07 08:47:50.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/dataframeviewer.py
+-rw-rw-rw-   0        0        0    41786 2021-07-23 01:51:29.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxexplorer.py
+-rw-rw-rw-   0        0        0     1619 2021-03-17 13:28:39.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxlineedit.py
+-rw-rw-rw-   0        0        0    12855 2021-03-08 13:57:21.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxproperty.py
+-rw-rw-rw-   0        0        0    31040 2021-07-07 07:25:53.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxshell.py
+-rw-rw-rw-   0        0        0     5364 2021-07-06 14:41:03.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxtoolbar.py
+-rw-rw-rw-   0        0        0    16460 2021-07-04 06:36:57.000000 spyder-modelx-0.9.0/spyder_modelx/widgets/mxtreemodel.py
+drwxrwxrwx   0        0        0        0 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx.egg-info/
+-rw-rw-rw-   0        0        0     2701 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2101 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2021-07-23 02:25:58.000000 spyder-modelx-0.9.0/spyder_modelx.egg-info/top_level.txt
```

### Comparing `spyder-modelx-0.8.0/LICENSE.txt` & `spyder-modelx-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/PKG-INFO` & `spyder-modelx-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: spyder-modelx
-Version: 0.8.0
+Version: 0.9.0
 Summary: Spyder plugin for modelx
 Home-page: https://github.com/fumitoh/spyder-modelx
 Author: Fumito Hamamura
 Author-email: fumito.ham@gmail.com
 License: LGPLv3
 Description: Spyder plugin for **modelx**
         ============================
```

### Comparing `spyder-modelx-0.8.0/README.rst` & `spyder-modelx-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/setup.py` & `spyder-modelx-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 def get_description():
     """Get long description."""
     with open(os.path.join(HERE, 'README.rst'), 'r') as f:
         data = f.read()
     return data
 
 
-REQUIREMENTS = ['spyder>=3.2.5', 'modelx>=0.15.0', 'asttokens']
+REQUIREMENTS = ['spyder>=3.2.5', 'modelx>=0.16.1', 'asttokens']
 
 
 setup(
     name='spyder-modelx',
     version=get_version(),
     keywords=['Spyder', 'Plugin'],
     url='https://github.com/fumitoh/spyder-modelx',
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx/__init__.py` & `spyder-modelx-0.9.0/spyder_modelx/__init__.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/_version.py` & `spyder-modelx-0.9.0/spyder_modelx/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
-version_info = (0, 8, 0)
+version_info = (0, 9, 0)
 __version__ = '.'.join(map(str, version_info))
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx/mxkernel.py` & `spyder-modelx-0.9.0/spyder_modelx/mxkernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,18 @@
 import spyder
 
 if spyder.version_info < (3, 3, 0):
     from spyder.utils.ipython.spyder_kernel import SpyderKernel
 else:
     from spyder_kernels.console.kernel import SpyderKernel
 
-from spyder_modelx.util import hinted_tuple_hook
+from spyder_modelx.utility.tupleencoder import hinted_tuple_hook
+from spyder_modelx.utility.typeutil import (
+    is_instance_of,
+    is_numpy_number, numpy_to_py)
 
 
 class ModelxKernel(SpyderKernel):
 
     def __init__(self, *args, **kwargs):
         super(ModelxKernel, self).__init__(*args, **kwargs)
 
@@ -386,46 +389,63 @@
         else:
             content = {'mx_obj': obj, 'mx_args': args, 'mx_adjacency': adjacency}
             self.send_mx_msg(msgtype, content=content, data=attrs)
 
     def _to_sendval(self, value):
         from modelx.core.cells import Interface
         from modelx.io.baseio import BaseDataClient
-        import pandas as pd
-        import numpy as np
-        import numpy.ma
 
         if isinstance(value, (Interface, str, BaseDataClient,
                               ModuleType)):
             return repr(value)
 
-        elif isinstance(value, (pd.DataFrame, pd.Index, pd.Series,
-                                np.ndarray, np.ma.MaskedArray,
-                                list, set, tuple, dict)):
+        elif any(
+                is_instance_of(value, c, "pandas") for c in [
+                    "DataFrame", "Index", "Series"
+                ]):
             return "Type: " + value.__class__.__name__
-        elif isinstance(value, np.float64):
-            return float(value)
+
+        elif any(
+            is_instance_of(value, c, "numpy") for c in [
+                "ndarray", "MaskedArray"
+            ]):
+            return "Type: " + value.__class__.__name__
+
+        elif isinstance(value, (list, set, tuple, dict)):
+            return "Type: " + value.__class__.__name__
+
+        elif is_numpy_number(value):
+            return numpy_to_py[type(value).__name__](value)
         else:
             return value
 
 
-    def mx_get_value(self, msgtype, fullname: str, argstr: str):
+    def mx_get_value(self, msgtype, fullname: str, argstr: str, calc: bool):
+        """Get value of modelx object
+
+        Returns a pair of the value and bool to indicate if the value is just
+        calculated
+
+        """
         import modelx as mx
         from modelx.core.reference import ReferenceProxy
         from modelx.core.base import Interface
 
         args = ast.literal_eval(argstr)
         obj = mx.get_object(fullname, as_proxy=True)
         if isinstance(obj, ReferenceProxy):
-            value = mx.get_object(fullname)
+            value = [mx.get_object(fullname), False]
         elif isinstance(obj, Interface):
             if args in obj:
-                value = obj(*args)
+                value = [obj(*args), False]
             else:
-                raise KeyError("value for %s not found" % argstr)
+                if calc:
+                    value = [obj(*args), True]
+                else:
+                    raise KeyError("value for %s not found" % argstr)
 
         if spyder.version_info > (4,):
             return value
         else:
             self.send_mx_msg(msgtype, content=None, data=value)
 
     def mx_get_allvalues(self, msgtype, fullname: str):
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx/mxkernelspec.py` & `spyder-modelx-0.9.0/spyder_modelx/mxkernelspec.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/plugins/analyzer_plugin.py` & `spyder-modelx-0.9.0/spyder_modelx/plugins/analyzer_plugin.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/plugins/dataview_plugin.py` & `spyder-modelx-0.9.0/spyder_modelx/plugins/dataview_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 import spyder
 try:
     from spyder.api.plugins import SpyderPluginWidget
 except ImportError:
     from spyder.plugins import SpyderPluginWidget  # Spyder3
 
-from spyder.utils.qthelpers import create_plugin_layout
+from spyder.utils.qthelpers import create_plugin_layout, create_action
 
 if spyder.version_info > (5,):
     from spyder_modelx.widgets.mxdataviewer.dataframeviewer import MxDataFrameViewer
     from spyder_modelx.widgets.mxdataviewer.arrayviewer import MxArrayViewer
     from spyder_modelx.widgets.mxdataviewer.collectionsviewer import MxCollectionsViewer
 elif spyder.version_info > (4,):
     from spyder_modelx.widgets.mxdataviewer.compat401.dataframeviewer import MxDataFrameViewer
@@ -191,14 +191,24 @@
         objbox_layout.setContentsMargins(5, 5, 0, 5)
 
         self.setLayout(layout)
 
         self.attrdict = None
         object_radio.setChecked(True)
 
+    def setup_option_actions(self, *args, **kwargs):
+
+        self.calc_on_update = create_action(self,
+           _("Calculate upon update"),
+           tip=_("Calculate the selected cells if not yet calculated"),
+           toggled=lambda state:
+           self.sig_option_changed.emit('calc_on_update', state))
+        self.calc_on_update.setChecked(True)
+        self.actions = [self.calc_on_update]
+
     def set_shellwidget(self, shellwidget):
         """Bind shellwidget instance to namespace browser"""
         self.shellwidget = shellwidget
         self.shellwidget.set_mxdataview(self)
 
     # MxToolBarMixin interface method
     def setup_toolbar(self):
@@ -230,25 +240,32 @@
         if self.object_radio.isChecked():
 
             argtxt = self.argbox.get_expr()
             args = "(" + argtxt + ("," if argtxt else "") + ")"
             # assert
             ast.literal_eval(args)
 
-            val = self.shellwidget.update_mxdataview(
+            calc = self.calc_on_update.isChecked()
+
+            val, is_calculated = self.shellwidget.update_mxdataview(
                 is_obj=True,
                 obj=self.attrdict["fullname"],
-                args=args
+                args=args,
+                calc=calc
             )
             self.update_value(val)
+            if is_calculated:
+                self.shellwidget.refresh_namespacebrowser()
+
         elif self.expr_radio.isChecked():
             self.shellwidget.update_mxdataview(
                 is_obj=False,
                 expr=self.exprbox.get_expr()
             )
+            self.shellwidget.refresh_namespacebrowser()
         else:
             raise RuntimeError("MxDataViewer: must not happen")
 
     def update_value(self, data):
 
         import pandas as pd
         import numpy as np
@@ -316,16 +333,21 @@
         return self.current_widget()
 
     def refresh_plugin(self):
         """Refresh MxExplorer widget."""
         pass
 
     def get_plugin_actions(self):
-        """Return a list of actions related to plugin."""
-        return []
+        """Return a list of actions related to plugin"""
+        widget = self.current_widget()
+        if isinstance(widget, self.MX_WIDGET_CLASS):
+            return widget.actions
+        else:
+            # Start-up Label
+            return []
 
     def register_plugin(self):
         """Register plugin in Spyder's main window."""
         if spyder.version_info < (4,):
             self.main.add_dockwidget(self)
         else:
             self.add_dockwidget()
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx/plugins/mxplugin.py` & `spyder-modelx-0.9.0/spyder_modelx/plugins/mxplugin.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/plugins/stacked_mixin.py` & `spyder-modelx-0.9.0/spyder_modelx/plugins/stacked_mixin.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/start_kernel.py` & `spyder-modelx-0.9.0/spyder_modelx/start_kernel.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/tests/__init__.py` & `spyder-modelx-0.9.0/spyder_modelx/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/tests/fromspyder/__init__.py` & `spyder-modelx-0.9.0/spyder_modelx/tests/fromspyder/__init__.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/tests/fromspyder/test_mxdataview.py` & `spyder-modelx-0.9.0/spyder_modelx/tests/fromspyder/test_mxdataview.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/tests/test_plugin.py` & `spyder-modelx-0.9.0/spyder_modelx/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/util.py` & `spyder-modelx-0.9.0/spyder_modelx/utility/tupleencoder.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/utility/formula.py` & `spyder-modelx-0.9.0/spyder_modelx/utility/formula.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/__init__.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxanalyzer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxanalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     from spyder.plugins.variableexplorer.widgets.dataframeeditor import DataFrameEditor
 else:
     from spyder.widgets.variableexplorer.arrayeditor import ArrayEditor
     from spyder.widgets.variableexplorer.collectionseditor import CollectionsEditor
     from spyder.widgets.variableexplorer.dataframeeditor import DataFrameEditor
 
 
-from spyder_modelx.util import TupleEncoder
+from spyder_modelx.utility.tupleencoder import TupleEncoder
 from spyder_modelx.widgets.mxlineedit import MxPyExprLineEdit
 from spyder_modelx.widgets.mxtoolbar import MxToolBarMixin
 from spyder_modelx.widgets.mxcodeeditor import BaseCodePane
 
 class NodeCols(enum.IntEnum):
     Node = 0
     Args = 1
@@ -583,15 +583,15 @@
 
         if index.isValid() and index.column() == NodeCols.Value:
 
             item = index.internalPointer()
             obj = item.node['obj']['fullname']
             args = str(item.node['args'])
 
-            data = self.shell.get_obj_value(
+            data, _ = self.shell.get_obj_value(
                 'analyze_getval', obj, args)
 
             if isinstance(data, (pd.DataFrame, pd.Index, pd.Series)):
                 dialog = DataFrameEditor(self)
                 dialog.setup_and_check(data)
             elif isinstance(data, (np.ndarray, np.ma.MaskedArray)):
                 dialog = ArrayEditor(self)
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxclient.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxclient.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxcodeeditor.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxcodeeditor.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxcodelist.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxcodelist.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/arrayviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/arrayviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/collectionsviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/collectionsviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat32/arrayviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat32/arrayviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat32/collectionsviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat32/collectionsviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat32/dataframeviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat32/dataframeviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat33/collectionsviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat33/collectionsviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat401/arrayviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat401/arrayviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat401/collectionsviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat401/collectionsviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/compat401/dataframeviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/compat401/dataframeviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxdataviewer/dataframeviewer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxdataviewer/dataframeviewer.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxexplorer.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxexplorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 class MxTreeView(QTreeView):
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         self.activated.connect(self.activated_callback)
-        self.doubleClicked.connect(self.doubleClicked_callback)
+        # self.doubleClicked.connect(self.doubleClicked_callback)
 
         self.plugin = parent.plugin
         self.shell = None
         self.reply = None  # To write dialog box result
         self.setAlternatingRowColors(False)
 
         # Context menu
@@ -122,19 +122,19 @@
     def activated_callback(self, index):
         if index.isValid():
             item = self.currentIndex().internalPointer()
             if not isinstance(item, ViewItem):
                 self.shell.update_mxproperty(item.itemData['fullname'])
                 # self.plugin.dataview.update_object(item.itemData['fullname'])
 
-    def doubleClicked_callback(self, index):
-        if index.isValid() and index.column() == TreeCol.IS_DERIVED:
-            answer = QMessageBox.warning(self.parent(), _("Warning"),
-                                         str(index.row()),
-                                         QMessageBox.Yes | QMessageBox.No)
+    # def doubleClicked_callback(self, index):
+    #     if index.isValid() and index.column() == TreeCol.IS_DERIVED:
+    #         answer = QMessageBox.warning(self.parent(), _("Warning"),
+    #                                      str(index.row()),
+    #                                      QMessageBox.Yes | QMessageBox.No)
 
 
     def contextMenuEvent(self, event):
         action = self.contextMenu.exec_(self.mapToGlobal(event.pos()))
 
         if action == self.action_update_formulas:
             index = self.currentIndex()
@@ -362,17 +362,17 @@
                         self, _("Delete Selected"),
                         _("Do you want to delete %s?" % item.name),
                         QMessageBox.Yes | QMessageBox.No)
 
                     if answer == QMessageBox.Yes:
                         self.shell.del_object(parent, item.name)
 
-                    QMessageBox.information(
-                        self, "Notice",
-                        "'%s' is deleted from '%s'" % (item.name, parent))
+                        QMessageBox.information(
+                            self, "Notice",
+                            "'%s' is deleted from '%s'" % (item.name, parent))
 
 
 class MxExplorer(QWidget):
     """modelx widget."""
 
     def __init__(self, parent):
         QWidget.__init__(self, parent)
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxlineedit.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxlineedit.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxproperty.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxproperty.py`

 * *Files identical despite different names*

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxshell.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxshell.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 if spyder.version_info < (4,):
     from spyder.widgets.ipythonconsole.client import ShellWidget
 else:
     from spyder.plugins.ipythonconsole.widgets.client import ShellWidget
 from spyder.utils import encoding
 from spyder.py3compat import PY2, to_text_string
 
-from spyder_modelx.util import TupleEncoder, hinted_tuple_hook
+from spyder_modelx.utility.tupleencoder import TupleEncoder, hinted_tuple_hook
 from spyder_modelx.utility.formula import (
     is_funcdef, is_lambda, replace_funcname, get_funcname)
 
 if spyder.version_info > (4,):
     from spyder.plugins.ipythonconsole.widgets.namespacebrowser import (
         CALL_KERNEL_TIMEOUT
     )
@@ -155,30 +155,31 @@
 
         # self.mxexprbox.editingFinished.connect(
         #     self.update_mxdataview)
 
         self.sig_mxdataview_eval.connect(self.mxdataviewer.update_value)
         self.sig_mxproperty.connect(self.mxdataviewer.update_object)
 
-    def get_obj_value(self, msgtype: str, obj: str, args: str):
+    def get_obj_value(self, msgtype: str, obj: str, args: str,
+                      calc: bool=False):
 
         # jsonargs = TupleEncoder(ensure_ascii=True).encode(args)
 
         if spyder.version_info > (4,):
             result = self.call_kernel(
                 interrupt=True,
                 blocking=True,
                 timeout=CALL_KERNEL_TIMEOUT).mx_get_value(
-                msgtype, obj, args
+                msgtype, obj, args, calc
             )
             return result
         else:
             code = (
-                    "get_ipython().kernel.mx_get_value('%s', '%s', '%s')"
-                    % (msgtype, obj, args)
+                    "get_ipython().kernel.mx_get_value('%s', '%s', '%s', %s)"
+                    % (msgtype, obj, args, calc)
             )
 
             # The code below is replaced with silent_exec_method
 
             # if self._reading:
             #     method = self.kernel_client.input
             #     code = u'!' + code
@@ -191,19 +192,19 @@
             elif msgtype == 'analyze_getval':
                 sig = self.sig_mxanalyzer_getval
             else:
                 raise RuntimeError('must not happen')
 
             return self._mx_wait_reply(code, sig)
 
-    def update_mxdataview(self, is_obj, obj=None, args=None, expr=None):
+    def update_mxdataview(self, is_obj, obj=None, args=None, expr=None, calc=False):
         """Update dataview"""
         # expr = self.mxdataviewer.exprbox.get_expr()
         if is_obj:
-            return self.get_obj_value('dataview_getval', obj, args)
+            return self.get_obj_value('dataview_getval', obj, args, calc)
         else:
             if expr:
                 method = "get_ipython().kernel.mx_get_evalresult('dataview', %s)" % expr
                 self.mx_silent_exec_method(method, msgtype='dataview')
 
             return None
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxtoolbar.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxtoolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         toolbar = self.setup_toolbar()
         if toolbar:
             for widget in toolbar:
                 self.tools_layout.addWidget(widget)
         else:
             self.tools_layout.addStretch()
 
+        self.setup_option_actions()
         self.setup_options_button()
 
     def get_actions(self):
         """Get actions of the widget."""
         return self.actions
 
     def setup_toolbar(self):
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx/widgets/mxtreemodel.py` & `spyder-modelx-0.9.0/spyder_modelx/widgets/mxtreemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,20 +179,17 @@
 
     def __hash__(self):
         return hash((self.parent().objid, self.attrid))
 
 
 class SpaceContainerItem(InterfaceItem):
     """Base Item class for Models and Spaces which inherit SpaceContainer."""
-    def updateChild(self):
-        self.childItems = self.newChildItems(self.itemData)
 
-    def newChildItems(self, data):
-        return [SpaceItem(space, self)
-                for space in data['spaces']['items'].values()]
+    def updateChild(self):
+        raise NotImplementedError
 
     def getSpaceContainerList(self):
         result = []
         result.append(self.itemData['fullname'])
         for child in self.childItems:
             if isinstance(child, SpaceContainerItem):
                 result.extend(child.getSpaceContainerList())
@@ -208,14 +205,22 @@
 
 
 class ModelItem(SpaceContainerItem):
     """Item class for a Model (root item)"""
     def __init__(self, data):
         super(ModelItem, self).__init__(data, parent=None)
 
+    def updateChild(self):
+        data = self.itemData
+        self.childItems.clear()
+        self.childItems.extend(SpaceItem(space, self)
+                               for space in data['spaces']['items'].values())
+        self.childItems.extend(RefItem(ref, self)
+                               for ref in data['refs']['items'].values())
+
     def getParams(self):
         return ''
 
 
 class SpaceItem(SpaceContainerItem):
     """Item class for Space objects."""
     def updateChild(self):
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx.egg-info/PKG-INFO` & `spyder-modelx-0.9.0/spyder_modelx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: spyder-modelx
-Version: 0.8.0
+Version: 0.9.0
 Summary: Spyder plugin for modelx
 Home-page: https://github.com/fumitoh/spyder-modelx
 Author: Fumito Hamamura
 Author-email: fumito.ham@gmail.com
 License: LGPLv3
 Description: Spyder plugin for **modelx**
         ============================
```

### Comparing `spyder-modelx-0.8.0/spyder_modelx.egg-info/SOURCES.txt` & `spyder-modelx-0.9.0/spyder_modelx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 setup.cfg
 setup.py
 spyder_modelx/__init__.py
 spyder_modelx/_version.py
 spyder_modelx/mxkernel.py
 spyder_modelx/mxkernelspec.py
 spyder_modelx/start_kernel.py
-spyder_modelx/util.py
 spyder_modelx.egg-info/PKG-INFO
 spyder_modelx.egg-info/SOURCES.txt
 spyder_modelx.egg-info/dependency_links.txt
 spyder_modelx.egg-info/requires.txt
 spyder_modelx.egg-info/top_level.txt
 spyder_modelx/plugins/__init__.py
 spyder_modelx/plugins/analyzer_plugin.py
@@ -23,14 +22,16 @@
 spyder_modelx/plugins/stacked_mixin.py
 spyder_modelx/tests/__init__.py
 spyder_modelx/tests/test_plugin.py
 spyder_modelx/tests/fromspyder/__init__.py
 spyder_modelx/tests/fromspyder/test_mxdataview.py
 spyder_modelx/utility/__init__.py
 spyder_modelx/utility/formula.py
+spyder_modelx/utility/tupleencoder.py
+spyder_modelx/utility/typeutil.py
 spyder_modelx/widgets/__init__.py
 spyder_modelx/widgets/mxanalyzer.py
 spyder_modelx/widgets/mxclient.py
 spyder_modelx/widgets/mxcodeeditor.py
 spyder_modelx/widgets/mxcodelist.py
 spyder_modelx/widgets/mxexplorer.py
 spyder_modelx/widgets/mxlineedit.py
```

