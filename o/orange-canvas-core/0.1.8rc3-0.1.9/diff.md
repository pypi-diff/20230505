# Comparing `tmp/orange-canvas-core-0.1.8rc3.tar.gz` & `tmp/orange-canvas-core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orange-canvas-core-0.1.8rc3.tar", last modified: Thu Nov  7 08:43:46 2019, max compression
+gzip compressed data, was "dist/orange-canvas-core-0.1.9.tar", last modified: Mon Nov 18 14:03:40 2019, max compression
```

## Comparing `orange-canvas-core-0.1.8rc3.tar` & `orange-canvas-core-0.1.9.tar`

### file list

```diff
@@ -1,262 +1,263 @@
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1886 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/PKG-INFO
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/
--rw-r--r--   0 aleserjavec   (501) staff       (20)    13081 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/link.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     7046 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/events.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     6873 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_readwrite.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1093 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_nodes.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2700 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4111 2019-07-25 07:12:27.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_scheme.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1426 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_annotations.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     7186 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_widgetmanager.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2785 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_links.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     8823 2019-11-07 08:38:08.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_signalmanager.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1008 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    26098 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/readwrite.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      612 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/errors.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    11088 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/node.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    25024 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/widgetmanager.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    37823 2019-11-07 08:38:08.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/signalmanager.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     7044 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/annotations.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    25208 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/scheme/scheme.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    16212 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/config.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/__init__.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/
--rw-r--r--   0 aleserjavec   (501) staff       (20)    27764 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/overlay.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      193 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/redirect.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    10082 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/propertybindings.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)      748 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_resources.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      523 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_utils.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4345 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_overlay.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      776 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_shtools.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     6299 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_propertybindings.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4637 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_settings.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      761 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_markup.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3519 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/shtools.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     5309 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2296 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/markup.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      683 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/qtcompat.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    12332 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/utils/settings.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4161 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/suggestions.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    86161 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/schemeedit.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    30768 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/editlinksdialog.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2586 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/tests/test_quickmenu.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2013 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/tests/test_editlinksdialog.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    11411 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/tests/test_schemeedit.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      400 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    59513 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/quickmenu.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     9570 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/usagestatistics.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    58878 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/interactions.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     9256 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/document/commands.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     5782 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/layout.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2637 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/tests/test_layout.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     8931 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/tests/test_scene.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      313 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    30910 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/scene.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     7355 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/view.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4065 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/graphicspathobject.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1817 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_utils.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     5267 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_nodeitem.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      738 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1961 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_annotationitem.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3577 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_linkitem.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2033 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_graphicspathobject.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1851 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_controlpoints.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    50303 2019-11-06 16:08:10.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/nodeitem.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      288 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4988 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/utils.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    28672 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/annotationitem.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    15842 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/controlpoints.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    25090 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/linkitem.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/
--rw-r--r--   0 aleserjavec   (501) staff       (20)      193 2019-10-29 11:49:06.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/darkorange.qss
--rw-r--r--   0 aleserjavec   (501) staff       (20)       27 2019-10-23 09:21:16.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     8643 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange.qss
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2251 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Grid.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4870 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Search.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1991 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Arrow.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1420 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Info.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      862 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Text Size.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3321 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Document Info.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      538 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Dropdown.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      573 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Pause.svg
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1314 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Grid.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3045 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Search.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2413 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Examples.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      578 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Arrow.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)    11315 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Get Started.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      835 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/default-widget.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)    35907 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/orange-splash-screen.png
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1149 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Recent.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1953 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Documentation.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      405 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/arrow-right.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      845 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/default-category.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1407 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Info.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1346 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Tutorials.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     9836 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/orange-canvas.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      653 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Back.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      581 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Maximize Toolbar.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      849 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Text Size.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1157 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Document Info.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1397 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Open.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1879 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/YouTube.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1104 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/New.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      525 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Dropdown.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      580 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Minimize Toolbar.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      243 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/orange-canvas-core-splash.svg
--rw-r--r--   0 aleserjavec   (501) staff       (20)      560 2019-10-23 09:30:39.000000 orange-canvas-core-0.1.8rc3/orangecanvas/icons/Pause.svg
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4912 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/splashscreen.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    21398 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/toolbox.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     7557 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/lineedit.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1474 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_lineedit.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2224 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_toolbox.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1585 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_dock.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2937 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_dropshadow.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)       31 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      456 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_framelesswindow.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2309 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_stackedwidget.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1199 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_toolbar.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1227 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_splashscreen.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2937 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_toolgrid.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2612 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_tooltree.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      163 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     9117 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/dock.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2960 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/textlabel.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2491 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/test.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    11138 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/dropshadow.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    13296 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/tooltree.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    11878 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/stackedwidget.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    16729 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/toolgrid.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3464 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/toolbar.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    15982 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/utils.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3406 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/iconview.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2617 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/framelesswindow.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4683 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/quickhelp.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1540 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/itemmodels.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2432 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/gui/svgiconengine.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/
--rw-r--r--   0 aleserjavec   (501) staff       (20)    15401 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/description.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    17326 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/discovery.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    12080 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/qt.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     6278 2019-07-25 07:19:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2314 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/tests/test_discovery.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4573 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/tests/test_base.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1558 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/cache.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2737 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     5393 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/utils.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     7065 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/registry/base.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     5752 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/resources.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4991 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/scanner.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1456 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/tests/test_scanner.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1163 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/tests/test_previewbrowser.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      726 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/tests/test_previewdialog.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)       92 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4867 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/previewmodel.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     9381 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/previewbrowser.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3876 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/preview/previewdialog.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/
--rw-r--r--   0 aleserjavec   (501) staff       (20)    16139 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/widgettoolbox.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    77848 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/canvasmain.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    10092 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/outputview.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    49021 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/addons.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    23247 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/canvastooldock.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2319 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_widgettoolbox.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      624 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_schemeinfo.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2643 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_canvastooldock.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     4534 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_mainwindow.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3409 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_addons.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1088 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_welcomedialog.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3985 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_outputview.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1829 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_settings.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)       64 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1420 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/aboutdialog.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      670 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/application.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     5951 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/schemeinfo.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     3602 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/examples.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    18113 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/settings.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     8543 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/application/welcomedialog.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    16186 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/main.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      104 2019-10-28 09:51:35.000000 orange-canvas-core-0.1.8rc3/orangecanvas/__main__.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/help/
--rw-r--r--   0 aleserjavec   (501) staff       (20)    12594 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/orangecanvas/help/provider.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2262 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/help/intersphinx.py
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orangecanvas/help/tests/
--rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/help/tests/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2177 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/help/tests/test_provider.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)       68 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/orangecanvas/help/__init__.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)    14154 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/orangecanvas/help/manager.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)       57 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/MANIFEST.in
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/docs/
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/docs/source/
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/
--rw-r--r--   0 aleserjavec   (501) staff       (20)      632 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/application.welcomedialog.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      267 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.splashscreen.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      491 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/document.quickmenu.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      608 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.node.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      186 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/index.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      462 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.tooltree.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      235 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/application.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      172 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/document.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2189 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.events.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      193 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.readwrite.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      827 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/canvas.items.nodeitem.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      688 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.annotation.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      662 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.stackedwidget.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      311 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)     2094 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/overview.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      763 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/registry.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      603 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/application.canvasmain.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      358 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.toolbox.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      235 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.toolbar.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      315 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.framelesswindow.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      197 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.signalmanager.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      412 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.lineedit.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      240 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.quickhelp.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1456 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.scheme.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      237 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/canvas.items.linkitem.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      395 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.link.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1153 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/canvas.scene.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      211 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/canvas.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      714 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/document.schemeedit.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      279 2019-11-04 16:34:07.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      618 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.widgetmanager.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      343 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.dock.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      478 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/canvas.items.annotationitem.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      447 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.toolgrid.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      272 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.dropshadow.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)      506 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/source/index.rst
--rw-r--r--   0 aleserjavec   (501) staff       (20)     9729 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/source/conf.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)       81 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/docs/requirements-rtd.txt
--rw-r--r--   0 aleserjavec   (501) staff       (20)     7273 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/docs/make.bat
--rwxr-xr-x   0 aleserjavec   (501) staff       (20)     2134 2019-11-07 08:38:22.000000 orange-canvas-core-0.1.8rc3/setup.py
--rw-r--r--   0 aleserjavec   (501) staff       (20)      283 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/setup.cfg
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1041 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.8rc3/README.rst
-drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orange_canvas_core.egg-info/
--rw-r--r--   0 aleserjavec   (501) staff       (20)     1886 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orange_canvas_core.egg-info/PKG-INFO
--rw-r--r--   0 aleserjavec   (501) staff       (20)     8679 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orange_canvas_core.egg-info/SOURCES.txt
--rw-r--r--   0 aleserjavec   (501) staff       (20)      149 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orange_canvas_core.egg-info/requires.txt
--rw-r--r--   0 aleserjavec   (501) staff       (20)       13 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orange_canvas_core.egg-info/top_level.txt
--rw-r--r--   0 aleserjavec   (501) staff       (20)        1 2019-11-07 08:43:46.000000 orange-canvas-core-0.1.8rc3/orange_canvas_core.egg-info/dependency_links.txt
--rw-r--r--   0 aleserjavec   (501) staff       (20)    35147 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.8rc3/LICENSE.txt
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1883 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/PKG-INFO
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    13081 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/link.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     7046 2019-11-12 13:36:28.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/events.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     6873 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_readwrite.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1093 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_nodes.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2700 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4111 2019-07-25 07:12:27.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_scheme.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1426 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_annotations.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     7186 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_widgetmanager.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2785 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_links.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     8823 2019-11-15 09:44:05.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_signalmanager.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1008 2019-11-11 11:05:46.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    26098 2019-11-18 13:34:58.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/readwrite.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      612 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/errors.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    11088 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/node.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    25024 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/widgetmanager.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    37823 2019-11-18 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/signalmanager.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     7044 2019-11-07 09:53:01.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/annotations.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    25208 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/scheme/scheme.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    16212 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/config.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/__init__.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/utils/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    27764 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/utils/overlay.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      193 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/utils/redirect.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    10082 2019-11-07 09:53:01.000000 orange-canvas-core-0.1.9/orangecanvas/utils/propertybindings.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/utils/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      748 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_resources.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      523 2019-11-07 09:53:01.000000 orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_utils.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4345 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_overlay.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      776 2019-11-12 15:21:47.000000 orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_shtools.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/utils/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     6299 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_propertybindings.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4637 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_settings.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      761 2019-11-11 11:05:46.000000 orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_markup.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3519 2019-11-12 15:21:47.000000 orange-canvas-core-0.1.9/orangecanvas/utils/shtools.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     5309 2019-11-18 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/utils/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2296 2019-11-11 11:05:46.000000 orange-canvas-core-0.1.9/orangecanvas/utils/markup.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      683 2019-11-11 11:50:18.000000 orange-canvas-core-0.1.9/orangecanvas/utils/qtcompat.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    12332 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/utils/settings.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/document/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4161 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/document/suggestions.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    87018 2019-11-18 13:35:04.000000 orange-canvas-core-0.1.9/orangecanvas/document/schemeedit.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    30768 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/document/editlinksdialog.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/document/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1729 2019-11-18 13:35:04.000000 orange-canvas-core-0.1.9/orangecanvas/document/tests/test_usagestatistics.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2586 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/document/tests/test_quickmenu.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/document/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2013 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/document/tests/test_editlinksdialog.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    11411 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/document/tests/test_schemeedit.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      400 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/document/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    59513 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/document/quickmenu.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    12936 2019-11-18 13:35:04.000000 orange-canvas-core-0.1.9/orangecanvas/document/usagestatistics.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    57251 2019-11-18 13:35:04.000000 orange-canvas-core-0.1.9/orangecanvas/document/interactions.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     9256 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/document/commands.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     5782 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/layout.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2637 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/tests/test_layout.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     8931 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/tests/test_scene.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      313 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    30910 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/scene.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     7355 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/view.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4065 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/graphicspathobject.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1817 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_utils.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     5267 2019-11-08 15:53:41.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_nodeitem.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      738 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1961 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_annotationitem.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3577 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_linkitem.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2033 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_graphicspathobject.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1851 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_controlpoints.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    51070 2019-11-18 13:35:04.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/nodeitem.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      288 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4988 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/utils.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    28672 2019-11-11 11:05:46.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/annotationitem.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    15842 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/controlpoints.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    25090 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/canvas/items/linkitem.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/styles/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      193 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/styles/darkorange.qss
+-rw-r--r--   0 aleserjavec   (501) staff       (20)       27 2019-11-11 08:55:50.000000 orange-canvas-core-0.1.9/orangecanvas/styles/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     8643 2019-11-11 08:55:50.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange.qss
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2251 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange/Grid.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4870 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange/Search.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1991 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange/Arrow.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1420 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange/Info.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      862 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange/Text Size.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3321 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange/Document Info.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      538 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange/Dropdown.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      573 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/styles/orange/Pause.svg
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/icons/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1314 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Grid.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3045 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Search.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2413 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Examples.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      578 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Arrow.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    11315 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Get Started.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      835 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/icons/default-widget.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    35907 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/orange-splash-screen.png
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1149 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Recent.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1953 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Documentation.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      405 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/arrow-right.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      845 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/default-category.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1407 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Info.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1346 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Tutorials.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     9836 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/orange-canvas.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      653 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Back.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      581 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Maximize Toolbar.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      849 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Text Size.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1157 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Document Info.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1397 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Open.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1879 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/icons/YouTube.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1104 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/New.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      525 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Dropdown.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      580 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Minimize Toolbar.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      243 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/icons/orange-canvas-core-splash.svg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      560 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/icons/Pause.svg
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/gui/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4912 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/splashscreen.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    21398 2019-11-11 11:05:46.000000 orange-canvas-core-0.1.9/orangecanvas/gui/toolbox.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     7557 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/gui/lineedit.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1474 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_lineedit.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2224 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_toolbox.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1585 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_dock.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2937 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_dropshadow.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)       31 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      456 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_framelesswindow.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2309 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_stackedwidget.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1199 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_toolbar.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1227 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_splashscreen.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2937 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_toolgrid.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2612 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_tooltree.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      163 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/gui/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     9117 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/gui/dock.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2960 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/textlabel.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2491 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/test.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    11138 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/dropshadow.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    13296 2019-11-11 10:02:22.000000 orange-canvas-core-0.1.9/orangecanvas/gui/tooltree.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    11878 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/gui/stackedwidget.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    16729 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/toolgrid.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3464 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/toolbar.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    15982 2019-11-18 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/utils.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3406 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/iconview.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2617 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/framelesswindow.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4683 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/quickhelp.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1540 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/itemmodels.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2432 2019-11-07 14:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/gui/svgiconengine.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/registry/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    15401 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/registry/description.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    17326 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/registry/discovery.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    12080 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/registry/qt.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/registry/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     6278 2019-07-25 07:19:18.000000 orange-canvas-core-0.1.9/orangecanvas/registry/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2314 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/registry/tests/test_discovery.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4573 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/registry/tests/test_base.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1558 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/registry/cache.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2737 2019-11-07 09:53:01.000000 orange-canvas-core-0.1.9/orangecanvas/registry/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     5393 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/registry/utils.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     7065 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/registry/base.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     5752 2019-11-07 09:53:01.000000 orange-canvas-core-0.1.9/orangecanvas/resources.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/preview/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4991 2019-11-07 09:53:01.000000 orange-canvas-core-0.1.9/orangecanvas/preview/scanner.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/preview/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1456 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/preview/tests/test_scanner.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/preview/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1163 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/preview/tests/test_previewbrowser.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      726 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/preview/tests/test_previewdialog.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)       92 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/preview/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4867 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/preview/previewmodel.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     9381 2019-11-07 09:53:01.000000 orange-canvas-core-0.1.9/orangecanvas/preview/previewbrowser.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3876 2019-11-07 09:53:01.000000 orange-canvas-core-0.1.9/orangecanvas/preview/previewdialog.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/application/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    16139 2019-11-11 10:09:43.000000 orange-canvas-core-0.1.9/orangecanvas/application/widgettoolbox.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    77874 2019-11-18 13:35:04.000000 orange-canvas-core-0.1.9/orangecanvas/application/canvasmain.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    10092 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/application/outputview.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    49071 2019-11-18 13:35:04.000000 orange-canvas-core-0.1.9/orangecanvas/application/addons.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    23247 2019-11-11 10:09:43.000000 orange-canvas-core-0.1.9/orangecanvas/application/canvastooldock.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2319 2019-10-17 15:56:02.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/test_widgettoolbox.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      624 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/test_schemeinfo.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2643 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/test_canvastooldock.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     4534 2019-11-18 13:34:58.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/test_mainwindow.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3409 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/test_addons.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1088 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/test_welcomedialog.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3985 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/test_outputview.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1829 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/application/tests/test_settings.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)       64 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/application/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1420 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/application/aboutdialog.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      670 2019-11-11 10:09:43.000000 orange-canvas-core-0.1.9/orangecanvas/application/application.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     5951 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/application/schemeinfo.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     3602 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/application/examples.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    18113 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/application/settings.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     8543 2019-11-07 14:45:58.000000 orange-canvas-core-0.1.9/orangecanvas/application/welcomedialog.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    16186 2019-11-12 15:21:47.000000 orange-canvas-core-0.1.9/orangecanvas/main.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      104 2019-11-12 15:21:47.000000 orange-canvas-core-0.1.9/orangecanvas/__main__.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/help/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    12594 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/help/provider.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2262 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/orangecanvas/help/intersphinx.py
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orangecanvas/help/tests/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)        0 2019-11-07 09:53:00.000000 orange-canvas-core-0.1.9/orangecanvas/help/tests/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2177 2019-11-07 09:53:01.000000 orange-canvas-core-0.1.9/orangecanvas/help/tests/test_provider.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)       68 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/orangecanvas/help/__init__.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    14154 2019-11-12 13:35:00.000000 orange-canvas-core-0.1.9/orangecanvas/help/manager.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)       57 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/MANIFEST.in
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/docs/
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/docs/source/
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      632 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/application.welcomedialog.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      267 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.splashscreen.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      491 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/document.quickmenu.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      608 2019-11-11 11:05:46.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.node.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      186 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/index.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      462 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.tooltree.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      235 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/application.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      172 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/document.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2189 2019-11-11 11:05:46.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.events.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      193 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.readwrite.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      827 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/canvas.items.nodeitem.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      688 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.annotation.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      662 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.stackedwidget.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      311 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     2094 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/overview.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      763 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/registry.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      603 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/application.canvasmain.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      358 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.toolbox.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      235 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.toolbar.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      315 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.framelesswindow.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      197 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.signalmanager.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      412 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.lineedit.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      240 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.quickhelp.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1456 2019-11-11 11:05:46.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.scheme.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      237 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/canvas.items.linkitem.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      395 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.link.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1153 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/canvas.scene.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      211 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/canvas.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      714 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/document.schemeedit.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      279 2019-11-11 11:05:46.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      618 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.widgetmanager.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      343 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.dock.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      478 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/canvas.items.annotationitem.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      447 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.toolgrid.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      272 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.dropshadow.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      506 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/source/index.rst
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     9729 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/source/conf.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)       81 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/docs/requirements-rtd.txt
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     7273 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/docs/make.bat
+-rwxr-xr-x   0 aleserjavec   (501) staff       (20)     2131 2019-11-18 13:57:36.000000 orange-canvas-core-0.1.9/setup.py
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      283 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/setup.cfg
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1041 2019-10-29 13:55:02.000000 orange-canvas-core-0.1.9/README.rst
+drwxr-xr-x   0 aleserjavec   (501) staff       (20)        0 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orange_canvas_core.egg-info/
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     1883 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orange_canvas_core.egg-info/PKG-INFO
+-rw-r--r--   0 aleserjavec   (501) staff       (20)     8731 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orange_canvas_core.egg-info/SOURCES.txt
+-rw-r--r--   0 aleserjavec   (501) staff       (20)      149 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orange_canvas_core.egg-info/requires.txt
+-rw-r--r--   0 aleserjavec   (501) staff       (20)       13 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orange_canvas_core.egg-info/top_level.txt
+-rw-r--r--   0 aleserjavec   (501) staff       (20)        1 2019-11-18 14:03:40.000000 orange-canvas-core-0.1.9/orange_canvas_core.egg-info/dependency_links.txt
+-rw-r--r--   0 aleserjavec   (501) staff       (20)    35147 2019-07-03 12:45:18.000000 orange-canvas-core-0.1.9/LICENSE.txt
```

### Comparing `orange-canvas-core-0.1.8rc3/PKG-INFO` & `orange-canvas-core-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-canvas-core
-Version: 0.1.8rc3
+Version: 0.1.9
 Summary: Core component of Orange Canvas
 Home-page: http://orange.biolab.si/
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/biolab/orange-canvas-core/issues
 Project-URL: Source, https://github.com/biolab/orange-canvas-core/
```

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/link.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/link.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/events.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/events.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_readwrite.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_readwrite.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_nodes.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/__init__.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_scheme.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_scheme.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_annotations.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_widgetmanager.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_widgetmanager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_links.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/tests/test_signalmanager.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/tests/test_signalmanager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/__init__.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/readwrite.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/readwrite.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/errors.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/errors.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/node.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/node.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/widgetmanager.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/widgetmanager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/signalmanager.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/signalmanager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/annotations.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/annotations.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/scheme/scheme.py` & `orange-canvas-core-0.1.9/orangecanvas/scheme/scheme.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/config.py` & `orange-canvas-core-0.1.9/orangecanvas/config.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/overlay.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/overlay.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/propertybindings.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/propertybindings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_resources.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_utils.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_overlay.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_overlay.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_shtools.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_shtools.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_propertybindings.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_propertybindings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_settings.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/tests/test_markup.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/tests/test_markup.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/shtools.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/shtools.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/__init__.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/markup.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/markup.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/qtcompat.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/qtcompat.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/utils/settings.py` & `orange-canvas-core-0.1.9/orangecanvas/utils/settings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/suggestions.py` & `orange-canvas-core-0.1.9/orangecanvas/document/suggestions.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/schemeedit.py` & `orange-canvas-core-0.1.9/orangecanvas/document/schemeedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 )
 from AnyQt.QtGui import (
     QKeySequence, QCursor, QFont, QPainter, QPixmap, QColor, QIcon,
     QWhatsThisClickedEvent, QKeyEvent, QPalette
 )
 from AnyQt.QtCore import (
     Qt, QObject, QEvent, QSignalMapper, QCoreApplication, QPoint, QPointF,
-    QMimeData
-)
+    QMimeData, Slot)
 from AnyQt.QtCore import pyqtProperty as Property, pyqtSignal as Signal
 
 from ..registry import WidgetDescription, WidgetRegistry
 from .suggestions import Suggestions
 from .usagestatistics import UsageStatistics
 from ..registry.qt import whats_this_helper, QtWidgetRegistry
 from ..gui.quickhelp import QuickHelpTipEvent
@@ -67,14 +66,36 @@
 
 
 class NoWorkflowError(RuntimeError):
     def __init__(self, message: str = "No workflow model is set", **kwargs):
         super().__init__(message, *kwargs)
 
 
+class UndoStack(QUndoStack):
+    def __init__(self, parent, statistics: UsageStatistics):
+        QUndoStack.__init__(self, parent)
+        self._statistics = statistics
+
+    @Slot()
+    def undo(self):
+        self._statistics.begin_action(UsageStatistics.Undo)
+        super().undo()
+        self._statistics.end_action()
+
+    @Slot()
+    def redo(self):
+        self._statistics.begin_action(UsageStatistics.Redo)
+        super().redo()
+        self._statistics.end_action()
+
+    def push(self, macro):
+        super().push(macro)
+        self._statistics.end_action()
+
+
 class SchemeEditWidget(QWidget):
     """
     A widget for editing a :class:`~.scheme.Scheme` instance.
 
     """
     #: Undo command has become available/unavailable.
     undoAvailable = Signal(bool)
@@ -123,15 +144,17 @@
         self.__possibleMouseItemsMove = False
         self.__itemsMoving = {}
         self.__contextMenuTarget = None  # type: Optional[SchemeLink]
         self.__dropTarget = None  # type: Optional[items.LinkItem]
         self.__quickMenu = None   # type: Optional[quickmenu.QuickMenu]
         self.__quickTip = ""
 
-        self.__undoStack = QUndoStack(self)
+        self.__statistics = UsageStatistics(self)
+
+        self.__undoStack = UndoStack(self, self.__statistics)
         self.__undoStack.cleanChanged[bool].connect(self.__onCleanChanged)
 
         # Preferred position for paste command. Updated on every mouse button
         # press and copy operation.
         self.__pasteOrigin = QPointF(20, 20)
 
         # scheme node properties when set to a clean state
@@ -183,15 +206,14 @@
         self.__linkMenu.addSeparator()
         self.__linkMenu.addAction(self.__nodeInsertAction)
         self.__linkMenu.addSeparator()
         self.__linkMenu.addAction(self.__linkRemoveAction)
         self.__linkMenu.addAction(self.__linkResetAction)
 
         self.__suggestions = Suggestions()
-        self.__statistics = UsageStatistics()
 
     def __setupActions(self):
         self.__cleanUpAction = QAction(
             self.tr("Clean Up"), self,
             objectName="cleanup-action",
             shortcut=QKeySequence("Shift+A"),
             toolTip=self.tr("Align widgets to a grid (Shift+A)"),
@@ -684,27 +706,39 @@
                 self.__scheme.removeEventFilter(self)
                 sm = self.__scheme.findChild(signalmanager.SignalManager)
                 if sm:
                     sm.stateChanged.disconnect(
                         self.__signalManagerStateChanged)
                 self.__widgetManager = None
 
+                self.__scheme.node_added.disconnect(self.__statistics.log_node_add)
+                self.__scheme.node_removed.disconnect(self.__statistics.log_node_remove)
+                self.__scheme.link_added.disconnect(self.__statistics.log_link_add)
+                self.__scheme.link_removed.disconnect(self.__statistics.log_link_remove)
+                self.__statistics.write_statistics()
+
             self.__scheme = scheme
             self.__suggestions.set_scheme(self)
 
             self.setPath("")
 
             if self.__scheme:
                 self.__scheme.title_changed.connect(self.titleChanged)
                 self.titleChanged.emit(scheme.title)
                 self.__cleanProperties = node_properties(scheme)
                 sm = scheme.findChild(signalmanager.SignalManager)
                 if sm:
                     sm.stateChanged.connect(self.__signalManagerStateChanged)
                 self.__widgetManager = getattr(scheme, "widget_manager", None)
+
+                self.__scheme.node_added.connect(self.__statistics.log_node_add)
+                self.__scheme.node_removed.connect(self.__statistics.log_node_remove)
+                self.__scheme.link_added.connect(self.__statistics.log_link_add)
+                self.__scheme.link_removed.connect(self.__statistics.log_link_remove)
+                self.__statistics.log_scheme(self.__scheme)
             else:
                 self.__cleanProperties = []
 
             self.__teardownScene(self.__scene)
             self.__scene.deleteLater()
 
             self.__undoStack.clear()
@@ -836,15 +870,14 @@
     def addNode(self, node):
         # type: (SchemeNode) -> None
         """
         Add a new node (:class:`.SchemeNode`) to the document.
         """
         if self.__scheme is None:
             raise NoWorkflowError()
-        self.__statistics.log_node_add(node.description.name)
         command = commands.AddNodeCommand(self.__scheme, node)
         self.__undoStack.push(command)
 
     def createNewNode(self, description, title=None, position=None):
         # type: (WidgetDescription, Optional[str], Optional[Pos]) -> SchemeNode
         """
         Create a new :class:`.SchemeNode` and add it to the document.
@@ -966,15 +999,14 @@
 
         new_links = (
             SchemeLink(source_node, old_link.source_channel,
                        new_node, first_link_sink_channel),
             SchemeLink(new_node, second_link_source_channel,
                        sink_node, old_link.sink_channel))
 
-        self.usageStatistics().log_node_add(new_node.description.name)
         command = commands.InsertNodeCommand(self.__scheme, new_node, old_link, new_links)
         self.__undoStack.push(command)
 
     def onNewLink(self, func):
         """
         Runs function when new link is added to current scheme.
         """
@@ -1013,17 +1045,14 @@
         for item in selected:
             assert self.__scheme is not None
             if isinstance(item, items.NodeItem):
                 node = self.scene().node_for_item(item)
                 self.__undoStack.push(
                     commands.RemoveNodeCommand(self.__scheme, node)
                 )
-                statistics = self.usageStatistics()
-                statistics.set_action_type(UsageStatistics.NodeRemove)
-                statistics.log_node_remove(node.description.name)
             elif isinstance(item, items.annotationitem.Annotation):
                 if item.hasFocus() or item.isAncestorOf(scene.focusItem()):
                     # Clear input focus from the item to be removed.
                     scene.focusItem().clearFocus()
                 annot = self.scene().annotation_for_item(item)
                 self.__undoStack.push(
                     commands.RemoveAnnotationCommand(self.__scheme, annot)
@@ -1189,23 +1218,24 @@
                 data = event.mimeData()
                 qname = data.data(MIME_TYPE)
                 try:
                     desc = self.__registry.widget(bytes(qname).decode("utf-8"))
                 except KeyError:
                     log.error("Unknown qualified name '%s'", qname)
                 else:
-                    self.__statistics.set_action_type(UsageStatistics.NodeAddDrag)
+                    statistics = self.usageStatistics()
                     pos = event.scenePos()
                     item = self.__scene.item_at(event.scenePos(), items.LinkItem)
                     link = self.scene().link_for_item(item) if item else None
                     if link and can_insert_node(desc, link):
+                        statistics.begin_insert_action(True, link)
                         node = self.newNodeHelper(desc, position=(pos.x(), pos.y()))
-                        self.usageStatistics().set_action_type(UsageStatistics.NodeAddInsertDrag)
                         self.insertNode(node, link)
                     else:
+                        statistics.begin_action(UsageStatistics.ToolboxDrag)
                         self.createNewNode(desc, position=(pos.x(), pos.y()))
                 return True
 
             elif etype == QEvent.GraphicsSceneMousePress:
                 self.__pasteOrigin = event.scenePos()
                 return self.sceneMousePressEvent(event)
             elif etype == QEvent.GraphicsSceneMouseMove:
@@ -1243,14 +1273,21 @@
         if anchor_item and event.button() == Qt.LeftButton:
             # Start a new link starting at item
             scene.clearSelection()
             handler = interactions.NewLinkAction(self)
             self._setUserInteractionHandler(handler)
             return handler.mousePressEvent(event)
 
+        link_item = scene.item_at(pos, items.LinkItem)
+        if link_item and event.button() == Qt.MiddleButton:
+            link = self.scene().link_for_item(link_item)
+            self.removeLink(link)
+            event.accept()
+            return True
+
         any_item = scene.item_at(pos)
         if not any_item:
             self.__emptyClickButtons |= event.button()
 
         if not any_item and event.button() == Qt.LeftButton:
             # Create a RectangleSelectionAction but do not set in on the scene
             # just yet (instead wait for the mouse move event).
@@ -1352,16 +1389,15 @@
             with disable_undo_stack_actions(
                     self.__undoAction, self.__redoAction, self.__undoStack):
                 action.create_new(event.screenPos())
 
             event.accept()
             return True
 
-        item = scene.item_at(event.scenePos(), items.LinkItem,
-                             buttons=Qt.LeftButton)
+        item = scene.item_at(event.scenePos(), items.LinkItem)
 
         if item is not None and event.button() == Qt.LeftButton:
             link = self.scene().link_for_item(item)
             action = interactions.EditNodeLinksAction(self, link.source_node,
                                                       link.sink_node)
             action.edit_links()
             event.accept()
@@ -1449,16 +1485,15 @@
                     menu.addAction(a)
                 menu.setAttribute(Qt.WA_DeleteOnClose)
             else:
                 menu = self.__widgetMenu
             menu.popup(globalPos)
             return True
 
-        item = self.scene().item_at(scenePos, items.LinkItem,
-                                    buttons=Qt.RightButton)
+        item = self.scene().item_at(scenePos, items.LinkItem)
         if item is not None:
             link = self.scene().link_for_item(item)
             self.__linkEnableAction.setChecked(link.enabled)
             self.__contextMenuTarget = link
             self.__linkMenu.popup(globalPos)
             return True
 
@@ -1768,22 +1803,14 @@
         # type: () -> None
         """
         Remove link was requested from the context menu.
         """
         if self.__contextMenuTarget:
             self.removeLink(self.__contextMenuTarget)
 
-            statistics = self.usageStatistics()
-            statistics.set_action_type(UsageStatistics.LinkRemove)
-            statistics.log_link_remove(self.__contextMenuTarget.source_node.description.name,
-                                       self.__contextMenuTarget.sink_node.description.name,
-                                       self.__contextMenuTarget.source_channel.name,
-                                       self.__contextMenuTarget.sink_channel.name)
-            statistics.clear_action_type()
-
     def __linkReset(self):
         # type: () -> None
         """
         Link reset from the context menu was requested.
         """
         if self.__contextMenuTarget:
             link = self.__contextMenuTarget
@@ -1827,16 +1854,17 @@
         if action:
             item = action.property("item")
             desc = item.data(QtWidgetRegistry.WIDGET_DESC_ROLE)
         else:
             return
 
         if can_insert_node(desc, original_link):
+            statistics = self.usageStatistics()
+            statistics.begin_insert_action(False, original_link)
             new_node = self.newNodeHelper(desc, position=(x, y))
-            self.usageStatistics().set_action_type(UsageStatistics.NodeAddInsertMenu)
             self.insertNode(new_node, original_link)
         else:
             log.info("Cannot insert node: links not possible.")
 
     def __duplicateSelected(self):
         # type: () -> None
         """
@@ -1955,14 +1983,16 @@
         for nodedup in nodedups:
             macrocommands.append(
                 commands.AddNodeCommand(scheme, nodedup, parent=command))
         for linkdup in linkdups:
             macrocommands.append(
                 commands.AddLinkCommand(scheme, linkdup, parent=command))
 
+        statistics = self.usageStatistics()
+        statistics.begin_action(UsageStatistics.Duplicate)
         self.__undoStack.push(command)
         scene = self.__scene
 
         # deselect selected
         selected = self.scene().selectedItems()
         for item in selected:
             item.setSelected(False)
```

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/editlinksdialog.py` & `orange-canvas-core-0.1.9/orangecanvas/document/editlinksdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/tests/test_quickmenu.py` & `orange-canvas-core-0.1.9/orangecanvas/document/tests/test_quickmenu.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/tests/test_editlinksdialog.py` & `orange-canvas-core-0.1.9/orangecanvas/document/tests/test_editlinksdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/tests/test_schemeedit.py` & `orange-canvas-core-0.1.9/orangecanvas/document/tests/test_schemeedit.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/quickmenu.py` & `orange-canvas-core-0.1.9/orangecanvas/document/quickmenu.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/usagestatistics.py` & `orange-canvas-core-0.1.9/orangecanvas/document/usagestatistics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,95 @@
 import enum
-import sys
+import itertools
 from datetime import datetime
 import platform
 import json
 import logging
 import os
 from typing import List
 
-import requests
-
-from AnyQt.QtCore import QCoreApplication, QSettings
+from AnyQt.QtCore import QCoreApplication
 
 from orangecanvas import config
+from orangecanvas.scheme import SchemeNode, SchemeLink, Scheme
 
 log = logging.getLogger(__name__)
 
 
+class EventType(enum.IntEnum):
+    NodeAdd = 0
+    NodeRemove = 1
+    LinkAdd = 2
+    LinkRemove = 3
+
+
 class ActionType(enum.IntEnum):
-    Invalid = -1
-    NodeAddClick = 0
-    NodeAddDrag = 1
-    NodeAddMenu = 2
-    NodeAddInsertDrag = 3
-    NodeAddInsertMenu = 4
-    NodeAddExtendFromSink = 5
-    NodeAddExtendFromSource = 6
-    NodeRemove = 7
-    LinkAdd = 8
-    LinkRemove = 9
-    LinkEdit = 10  # ends up transformed into LinkAdd and LinkRemove events
+    Unclassified = 0
+    ToolboxClick = 1
+    ToolboxDrag = 2
+    QuickMenu = 3
+    ExtendFromSource = 4
+    ExtendFromSink = 5
+    InsertDrag = 6
+    InsertMenu = 7
+    Undo = 8
+    Redo = 9
+    Duplicate = 10
+    Load = 11
 
 
 class UsageStatistics:
     """
     Tracks usage statistics if enabled (is disabled by default).
 
     Data is tracked and stored in application data directory in
     'usage-statistics.json' file.
 
     It is the application's responsibility to ask for permission and
     appropriately handle the collected statistics.
 
-    In certain situations it is not simple to discern user-intended actions
-    from ones done automatically. For this purpose ActionType is employed,
-    set when the user explicitly performs an action.
-
-    The stored action type is automatically cleared after node actions,
-    but should be manually cleared for link actions with the clear_action_type() method.
-
     Data tracked per canvas session:
         date,
         application version,
         operating system,
         anaconda boolean,
-        UUID,
-        a sequence of the following actions:
-            node addition,
-            node removal,
-            link addition,
-            link removal
+        UUID (in Orange3),
+        a sequence of actions of type ActionType
+
+    An action consists of one or more events of type EventType.
+    Events refer to nodes according to a unique integer ID.
+    Each node is also associated with a widget name, assigned in a NodeAdd event.
+    Link events also reference corresponding source/sink channel names.
+
+    Some actions carry metadata (e.g. search query for QuickMenu, Extend).
+
+    Parameters
+    ----------
+    parent: SchemeEditWidget
     """
     _is_enabled = False
+    statistics_sessions = []
+    last_search_query = None
 
-    Invalid, NodeAddClick, NodeAddDrag, NodeAddMenu, NodeAddInsertDrag, NodeAddInsertMenu, \
-    NodeAddExtendFromSink, NodeAddExtendFromSource, NodeRemove, LinkAdd, LinkRemove, LinkEdit \
+    Unclassified, ToolboxClick, ToolboxDrag, QuickMenu, ExtendFromSink, ExtendFromSource, \
+    InsertDrag, InsertMenu, Undo, Redo, Duplicate, Load \
         = list(ActionType)
 
-    last_search_query = None
+    def __init__(self, parent):
+        self.parent = parent
 
-    def __init__(self):
         self._actions = []
-        self._action_type = UsageStatistics.Invalid
+        self._events = []
+        self._widget_ids = {}
+        self._id_iter = itertools.count()
+
+        self._action_type = ActionType.Unclassified
+        self._metadata = None
+
+        UsageStatistics.statistics_sessions.append(self)
 
     @classmethod
     def is_enabled(cls) -> bool:
         """
         Returns
         -------
         enabled : bool
@@ -87,208 +102,312 @@
         """
         Enable/disable usage collection.
 
         Parameters
         ----------
         state : bool
         """
+        if cls._is_enabled == state:
+            return
+
         cls._is_enabled = state
         log.info("{} usage statistics tracking".format(
             "Enabling" if state else "Disabling"
         ))
+        for session in UsageStatistics.statistics_sessions:
+            if state:
+                # log current scheme state after enabling of statistics
+                scheme = session.parent.scheme()
+                session.log_scheme(scheme)
+            else:
+                session.drop_statistics()
 
-    def log_node_add(self, widget_name, extended_widget=None):
+    def begin_action(self, action_type):
         """
-        Logs an node addition action, based on the currently set action type.
+        Sets the type of action that will be logged upon next call to a log method.
+
+        Each call to begin_action() should be matched with a call to end_action().
+
+        Parameters
+        ----------
+        action_type : ActionType
+        """
+        if not self.is_enabled():
+            return
+
+        if self._action_type != self.Unclassified:
+            raise ValueError("Tried to set " + str(action_type) + \
+                             " but " + str(self._action_type) + " was already set.")
+
+        self._prepare_action(action_type)
+
+    def begin_extend_action(self, from_sink, extended_widget):
+        """
+        Sets the type of action to widget extension in the specified direction,
+        noting the extended widget and query.
+
+        Each call to begin_extend_action() should be matched with a call to end_action().
 
         Parameters
         ----------
-        widget_name : str
-        extended_widget : str
+        from_sink : bool
+        extended_widget : SchemeNode
         """
         if not self.is_enabled():
             return
 
-        node_add_action_types = {self.NodeAddClick, self.NodeAddDrag, self.NodeAddMenu,
-                                 self.NodeAddInsertDrag, self.NodeAddInsertMenu,
-                                 self.NodeAddExtendFromSink, self.NodeAddExtendFromSource}
-
-        if self._action_type not in node_add_action_types:
-            log.info("Invalid action type registered for node addition logging. "
-                     "No action was logged.")
+        if self._events:
+            log.error("Tried to start extend action while current action already has events")
             return
 
-        action = {
-            "Type": self._action_type,
-            "Widget Name": widget_name,
-        }
+        # set action type
+        if from_sink:
+            action_type = ActionType.ExtendFromSink
+        else:
+            action_type = ActionType.ExtendFromSource
 
-        if self._action_type == UsageStatistics.NodeAddMenu:
-            action["Query"] = UsageStatistics.last_search_query
+        # set metadata
+        if extended_widget not in self._widget_ids:
+            log.error("Attempted to extend widget before it was logged. No action type was set.")
+            return
+        extended_id = self._widget_ids[extended_widget]
 
-        elif self._action_type == UsageStatistics.NodeAddExtendFromSink or \
-                self._action_type == UsageStatistics.NodeAddExtendFromSource:
-            action["Extended Widget"] = extended_widget
-            action["Query"] = UsageStatistics.last_search_query
-
-        elif self._action_type == UsageStatistics.LinkAdd or \
-                self._action_type == UsageStatistics.LinkRemove:
-            action["Connected Widget"] = extended_widget
+        metadata = {"Extended Widget": extended_id}
 
-        self._action_type = UsageStatistics.Invalid
-        self._actions.append(action)
+        self._prepare_action(action_type, metadata)
 
-    def log_node_remove(self, widget_name):
+    def begin_insert_action(self, via_drag, original_link):
         """
-        Logs an node removal action.
+        Sets the type of action to widget insertion via the specified way,
+        noting the old link's source and sink widgets.
+
+        Each call to begin_insert_action() should be matched with a call to end_action().
 
         Parameters
         ----------
-        widget_name : str
+        via_drag : bool
+        original_link : SchemeLink
         """
         if not self.is_enabled():
             return
 
-        if self._action_type is not UsageStatistics.NodeRemove:
-            log.info("Invalid action type registered for node removal logging. "
-                     "No action was logged.")
+        if self._events:
+            log.error("Tried to start insert action while current action already has events")
+            return
+
+        source_widget = original_link.source_node
+        sink_widget = original_link.sink_node
+
+        # set action type
+        if via_drag:
+            action_type = ActionType.InsertDrag
+        else:
+            action_type = ActionType.InsertMenu
+
+        # set metadata
+        if source_widget not in self._widget_ids or sink_widget not in self._widget_ids:
+            log.error("Attempted to log insert action between unknown widgets. "
+                      "No action was logged.")
+            self._clear_action()
+            return
+        src_id, sink_id = self._widget_ids[source_widget], self._widget_ids[sink_widget]
+
+        metadata = {"Source Widget": src_id,
+                    "Sink Widget": sink_id}
+
+        self._prepare_action(action_type, metadata)
+
+    def _prepare_action(self, action_type, metadata=None):
+        """
+        Sets the type of action and metadata that will be logged upon next call to a log method.
+
+        Parameters
+        ----------
+        action_type : ActionType
+        metadata : Dict[str, Any]
+        """
+        self._action_type = action_type
+        self._metadata = metadata
+
+    def end_action(self):
+        """
+        Ends the started action, concatenating the relevant events and adding it to
+        the list of actions.
+        """
+        if not self.is_enabled():
+            return
+
+        if not self._events:
+            log.info("End action called but no events were logged.")
+            self._clear_action()
             return
 
         action = {
             "Type": self._action_type,
-            "Widget Name": widget_name
+            "Events": self._events
         }
 
-        self._action_type = UsageStatistics.Invalid
+        # add metadata
+        if self._metadata:
+            action.update(self._metadata)
+
+        # add search query if relevant
+        if self._action_type in {ActionType.ExtendFromSource, ActionType.ExtendFromSink,
+                                 ActionType.QuickMenu}:
+            action["Query"] = self.last_search_query
+
         self._actions.append(action)
+        self._clear_action()
 
-    def log_link_add(self, source_widget, sink_widget, source_channel, sink_channel):
+    def _clear_action(self):
         """
-        Logs an link addition action.
+        Clear the current action.
+        """
+        self._events = []
+        self._action_type = ActionType.Unclassified
+        self._metadata = None
+        self.last_search_query = ""
+
+    def log_node_add(self, widget):
+        """
+        Logs an node addition action, based on the currently set action type.
 
         Parameters
         ----------
-        source_widget : str
-        sink_widget : str
-        source_channel : str
-        sink_channel : str
+        widget : SchemeNode
         """
         if not self.is_enabled():
             return
 
-        if self._action_type not in {UsageStatistics.LinkAdd, UsageStatistics.LinkEdit}:
-            log.info("Invalid action type registered for link add logging. "
-                     "No action was logged.")
-            return
+        # get or generate id for widget
+        if widget in self._widget_ids:
+            widget_id = self._widget_ids[widget]
+        else:
+            widget_id = next(self._id_iter)
+            self._widget_ids[widget] = widget_id
 
-        self._log_link(UsageStatistics.LinkAdd, source_widget, sink_widget, source_channel,
-                       sink_channel)
+        event = {
+            "Type": EventType.NodeAdd,
+            "Widget Name": widget.description.id,
+            "Widget": widget_id
+        }
+
+        self._events.append(event)
 
-    def log_link_remove(self, source_widget, sink_widget, source_channel, sink_channel):
+    def log_node_remove(self, widget):
         """
-        Logs an link removal action.
+        Logs an node removal action.
 
         Parameters
         ----------
-        source_widget : str
-        sink_widget : str
-        source_channel : str
-        sink_channel : str
+        widget : SchemeNode
         """
         if not self.is_enabled():
             return
 
-        if self._action_type not in {UsageStatistics.LinkRemove, UsageStatistics.LinkEdit}:
-            log.info("Invalid action type registered for link remove logging. "
-                     "No action was logged.")
+        # get id for widget
+        if widget not in self._widget_ids:
+            log.error("Attempted to log node removal before its addition. No action was logged.")
+            self._clear_action()
             return
+        widget_id = self._widget_ids[widget]
 
-        self._log_link(UsageStatistics.LinkRemove, source_widget, sink_widget, source_channel,
-                       sink_channel)
-
-    def _log_link(self, action_type, source_widget, sink_widget, source_channel, sink_channel):
-        action = {
-            "Type": action_type,
-            "Source Widget": source_widget,
-            "Sink Widget": sink_widget,
-            "Source Channel": source_channel,
-            "Sink Channel": sink_channel
+        event = {
+            "Type": EventType.NodeRemove,
+            "Widget": widget_id
         }
 
-        self._actions.append(action)
+        self._events.append(event)
 
-    def set_action_type(self, action_type):
+    def log_link_add(self, link):
         """
-        Sets the type of action that will be logged upon next call to log_action.
+        Logs a link addition action.
 
         Parameters
         ----------
-        action_type : ActionType
+        link : SchemeLink
         """
-        self._action_type = action_type
+        if not self.is_enabled():
+            return
 
-    def clear_action_type(self):
-        """
-        Clear the currently set action type by setting it to Invalid.
-        """
-        self._action_type = UsageStatistics.Invalid
+        self._log_link(EventType.LinkAdd, link)
 
-    def filename(self) -> str:
+    def log_link_remove(self, link):
         """
-        Return the filename path where the statistics are saved
+        Logs a link removal action.
+
+        Parameters
+        ----------
+        link : SchemeLink
         """
-        return os.path.join(config.data_dir(), "usage-statistics.json")
+        if not self.is_enabled():
+            return
 
-    def load(self) -> 'List[dict]':
+        self._log_link(EventType.LinkRemove, link)
+
+    def _log_link(self, action_type, link):
+        source_widget = link.source_node
+        sink_widget = link.sink_node
+
+        # get id for widgets
+        if source_widget not in self._widget_ids or sink_widget not in self._widget_ids:
+            log.error("Attempted to log link action between unknown widgets. No action was logged.")
+            self._clear_action()
+            return
+
+        src_id, sink_id = self._widget_ids[source_widget], self._widget_ids[sink_widget]
+
+        event = {
+            "Type": action_type,
+            "Source Widget": src_id,
+            "Sink Widget": sink_id,
+            "Source Channel": link.source_channel.name,
+            "Sink Channel": link.sink_channel.name
+        }
+
+        self._events.append(event)
+
+    def log_scheme(self, scheme):
         """
-        Load and return the usage statistics data.
+        Log all nodes and links in a scheme.
 
-        Returns
-        -------
-        data : dict
+        Parameters
+        ----------
+        scheme : Scheme
         """
         if not self.is_enabled():
-            return []
-        try:
-            with open(self.filename(), "r", encoding="utf-8") as f:
-                return json.load(f)
-        except (FileNotFoundError, PermissionError, IsADirectoryError,
-                UnicodeDecodeError, json.JSONDecodeError):
-            return []
+            return
 
-    def send_statistics(self, url: str) -> None:
-        """
-        Send the statistics to the remote at `url`.
+        if not scheme or not scheme.nodes:
+            return
 
-        The contents are send via POST file upload (multipart/form-data)
+        self.begin_action(ActionType.Load)
 
-        Does nothing if not enabled.
+        # first log nodes
+        for node in scheme.nodes:
+            self.log_node_add(node)
 
-        Parameters
-        ----------
-        url : str
+        # then log links
+        for link in scheme.links:
+            self.log_link_add(link)
+
+        self.end_action()
+
+    def drop_statistics(self):
+        """
+        Clear all data in the statistics session.
         """
-        if self.is_enabled():
-            data = self.load()
-            try:
-                r = requests.post(url, files={'file': json.dumps(data)})
-                if r.status_code != 200:
-                    log.warning("Error communicating with server while attempting to send "
-                                "usage statistics.")
-                    return
-                # success - wipe statistics file
-                log.info("Usage statistics sent.")
-                with open(self.filename(), 'w', encoding="utf-8") as f:
-                    json.dump([], f)
-            except (ConnectionError, requests.exceptions.RequestException):
-                log.warning("Connection error while attempting to send usage statistics.")
-            except Exception:
-                log.warning("Failed to send usage statistics.")
+        self._actions = []
+        self._widget_ids = {}
+        self._id_iter = itertools.count()
 
     def write_statistics(self):
+        """
+        Write the statistics session to file, and clear it.
+        """
         if not self.is_enabled():
             return
 
         statistics_path = self.filename()
         statistics = {
             "Date": str(datetime.now().date()),
             "Application Version": QCoreApplication.applicationVersion(),
@@ -303,10 +422,47 @@
             data = []
 
         data.append(statistics)
 
         with open(statistics_path, 'w') as f:
             json.dump(data, f)
 
+        self.drop_statistics()
+
+    def close(self):
+        """
+        Close statistics session, effectively not updating it upon
+        toggling statistics tracking.
+        """
+        UsageStatistics.statistics_sessions.remove(self)
+
     @staticmethod
     def set_last_search_query(query):
+        if not UsageStatistics.is_enabled():
+            return
+
         UsageStatistics.last_search_query = query
+
+    @staticmethod
+    def filename() -> str:
+        """
+        Return the filename path where the statistics are saved
+        """
+        return os.path.join(config.data_dir(), "usage-statistics.json")
+
+    @staticmethod
+    def load() -> 'List[dict]':
+        """
+        Load and return the usage statistics data.
+
+        Returns
+        -------
+        data : dict
+        """
+        if not UsageStatistics.is_enabled():
+            return []
+        try:
+            with open(UsageStatistics.filename(), "r", encoding="utf-8") as f:
+                return json.load(f)
+        except (FileNotFoundError, PermissionError, IsADirectoryError,
+                UnicodeDecodeError, json.JSONDecodeError):
+            return []
```

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/interactions.py` & `orange-canvas-core-0.1.9/orangecanvas/document/interactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,16 +461,14 @@
             stack = self.document.undoStack()
 
             self.macro = QUndoCommand(self.tr("Add link"))
 
             if item:
                 # If the release was over a node item then connect them
                 node = self.scene.node_for_item(item)
-                statistics = self.document.usageStatistics()
-                statistics.set_action_type(UsageStatistics.LinkAdd)
             else:
                 # Release on an empty canvas part
                 # Show a quick menu popup for a new widget creation.
                 try:
                     node = self.create_new(event)
                 except Exception:
                     log.error("Failed to create a new node, ending.",
@@ -514,15 +512,16 @@
 
         def is_compatible(source, sink):
             # type: (WidgetDescription, WidgetDescription) -> bool
             return any(scheme.compatible_channels(output, input)
                        for output in source.outputs
                        for input in sink.inputs)
 
-        if self.direction == self.FROM_SINK:
+        from_sink = self.direction == self.FROM_SINK
+        if from_sink:
             # Reverse the argument order.
             is_compatible = reversed_arguments(is_compatible)
             suggestion_sort = self.suggestions.get_source_suggestions(from_desc.name)
         else:
             suggestion_sort = self.suggestions.get_sink_suggestions(from_desc.name)
 
         def sort(left, right):
@@ -549,45 +548,38 @@
             item = action.property("item")
             desc = item.data(QtWidgetRegistry.WIDGET_DESC_ROLE)
             pos = event.scenePos()
             # a new widget should be placed so that the connection
             # stays as it was
             offset = 31 * (-1 if self.direction == self.FROM_SINK else
                            1 if self.direction == self.FROM_SOURCE else 0)
+            statistics = self.document.usageStatistics()
+            statistics.begin_extend_action(from_sink, node)
             node = self.document.newNodeHelper(desc,
                                                position=(pos.x() + offset,
                                                          pos.y()))
-            statistics = self.document.usageStatistics()
-            if self.direction == self.FROM_SINK:
-                statistics.set_action_type(UsageStatistics.NodeAddExtendFromSink)
-            else:
-                statistics.set_action_type(UsageStatistics.NodeAddExtendFromSource)
-            statistics.log_node_add(node.description.name, from_desc.name)
             return node
         else:
             return None
 
     def connect_nodes(self, source_node, sink_node):
         # type: (Node, Node) -> None
         """
         Connect `source_node` to `sink_node`. If there are more then one
         equally weighted and non conflicting links possible present a
         detailed dialog for link editing.
 
         """
-        stat = self.document.usageStatistics()
         try:
             possible = self.scheme.propose_links(source_node, sink_node)
 
             log.debug("proposed (weighted) links: %r",
                       [(s1.name, s2.name, w) for s1, s2, w in possible])
 
             if not possible:
-                # should action_type have been set to LinkAdd, reset it, as no link is possible
-                stat.clear_action_type()
                 raise NoPossibleLinksError
 
             source, sink, w = possible[0]
 
             # just a list of signal tuples for now, will be converted
             # to SchemeLinks later
             links_to_add = []     # type: List[Link]
@@ -623,48 +615,41 @@
                     )
                 except Exception:
                     log.error("Failed to edit the links",
                               exc_info=True)
                     raise
                 if rstatus == EditLinksDialog.Rejected:
                     raise UserCanceledError
-                stat.set_action_type(UsageStatistics.LinkEdit)
             else:
                 # links_to_add now needs to be a list of actual SchemeLinks
                 links_to_add = [
                     scheme.SchemeLink(source_node, source, sink_node, sink)
                 ]
                 links_to_add, links_to_remove = \
                     add_links_plan(self.scheme, links_to_add)
 
             # Remove temp items before creating any new links
             self.cleanup()
 
             for link in links_to_remove:
-                stat.log_link_add(source_node.description.name, sink_node.description.name,
-                                  link.source_channel.name, link.sink_channel.name)
                 commands.RemoveLinkCommand(self.scheme, link,
                                            parent=self.macro)
 
             for link in links_to_add:
                 # Check if the new requested link is a duplicate of an
                 # existing link
                 duplicate = self.scheme.find_links(
                     link.source_node, link.source_channel,
                     link.sink_node, link.sink_channel
                 )
 
                 if not duplicate:
-                    stat.log_link_add(source_node.description.name, sink_node.description.name,
-                                      link.source_channel.name, link.sink_channel.name)
                     commands.AddLinkCommand(self.scheme, link,
                                             parent=self.macro)
 
-            stat.clear_action_type()
-
         except scheme.IncompatibleChannelTypeError:
             log.info("Cannot connect: invalid channel types.")
             self.cancel()
         except scheme.SchemeTopologyError:
             log.info("Cannot connect: connection creates a cycle.")
             self.cancel()
         except NoPossibleLinksError:
@@ -898,17 +883,18 @@
         if action:
             item = action.property("item")
             desc = item.data(QtWidgetRegistry.WIDGET_DESC_ROLE)
             # Get the scene position
             view = self.document.view()
             pos = view.mapToScene(view.mapFromGlobal(pos))
 
+            statistics = self.document.usageStatistics()
+            statistics.begin_action(UsageStatistics.QuickMenu)
             node = self.document.newNodeHelper(desc,
                                                position=(pos.x(), pos.y()))
-            self.document.usageStatistics().set_action_type(UsageStatistics.NodeAddMenu)
             self.document.addNode(node)
             return node
         else:
             return None
 
 
 class RectangleSelectionAction(UserInteraction):
@@ -1106,16 +1092,14 @@
         dlg.setNodes(self.source_node, self.sink_node)
         dlg.setLinks(initial_links)
 
         log.info("Executing a Link Editor Dialog.")
         rval = dlg.exec_()
 
         if rval == EditLinksDialog.Accepted:
-            statistics = self.document.usageStatistics()
-            statistics.set_action_type(UsageStatistics.LinkEdit)
             links_spec = dlg.links()
 
             links_to_add = set(links_spec) - set(existing_links)
             links_to_remove = set(existing_links) - set(links_spec)
 
             stack = self.document.undoStack()
             stack.beginMacro("Edit Links")
@@ -1140,28 +1124,21 @@
             for source_channel, sink_channel in links_to_remove:
                 links = self.scheme.find_links(source_node=self.source_node,
                                                source_channel=source_channel,
                                                sink_node=self.sink_node,
                                                sink_channel=sink_channel)
                 assert len(links) == 1
                 self.document.removeLink(links[0])
-                statistics.log_link_remove(links[0].source_node.description.name,
-                                           links[0].sink_node.description.name,
-                                           links[0].source_channel.name, links[0].sink_channel.name)
 
             for source_channel, sink_channel in links_to_add:
                 link = scheme.SchemeLink(self.source_node, source_channel,
                                          self.sink_node, sink_channel)
 
                 self.document.addLink(link)
-                statistics.log_link_add(link.source_node.description.name,
-                                        link.sink_node.description.name,
-                                        link.source_channel.name, link.sink_channel.name)
 
-            statistics.clear_action_type()
             stack.endMacro()
 
 
 def point_to_tuple(point):
     # type: (QPointF) -> Tuple[float, float]
     """
     Convert a QPointF into a (x, y) tuple.
```

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/document/commands.py` & `orange-canvas-core-0.1.9/orangecanvas/document/commands.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/layout.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/layout.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/tests/test_layout.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/tests/test_scene.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/tests/test_scene.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/scene.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/scene.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/view.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/view.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/graphicspathobject.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/graphicspathobject.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_utils.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_nodeitem.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_nodeitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/__init__.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_annotationitem.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_annotationitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_linkitem.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_linkitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_graphicspathobject.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_graphicspathobject.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/tests/test_controlpoints.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/tests/test_controlpoints.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/nodeitem.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/nodeitem.py`

 * *Files 2% similar despite different names*

```diff
@@ -842,32 +842,30 @@
 class NameTextItem(QGraphicsTextItem):
     def __init__(self, *args, **kwargs):
         # type: (Any, Any) -> None
         super().__init__(*args, **kwargs)
         self.__selected = False
         self.__palette = None  # type: Optional[QPalette]
         self.__content = ""
+        #: The cached text background shape when this item is selected
+        self.__cachedBackgroundPath = None  # type: Optional[QPainterPath]
+        self.document().documentLayoutChanged.connect(self.__onLayoutChanged)
+
+    def __onLayoutChanged(self):
+        self.__cachedBackgroundPath = None
+        self.update()
 
     def paint(self, painter, option, widget=None):
         # type: (QPainter, QStyleOptionGraphicsItem, Optional[QWidget]) -> None
         if self.__selected:
+            path = self.__textBackgroundPath()
             painter.save()
             painter.setPen(QPen(Qt.NoPen))
             painter.setBrush(self.palette().color(QPalette.Highlight))
-            doc = self.document()
-            margin = doc.documentMargin()
-            painter.translate(margin, margin)
-            offset = min(margin, 2)
-            for line in self._lines(doc):
-                rect = line.naturalTextRect()
-                painter.drawRoundedRect(
-                    rect.adjusted(-offset, -offset, offset, offset),
-                    3, 3
-                )
-
+            painter.drawPath(path)
             painter.restore()
 
         super().paint(painter, option, widget)
 
     def _blocks(self, doc):
         # type: (QTextDocument) -> Iterable[QTextBlock]
         block = doc.begin()
@@ -878,14 +876,31 @@
     def _lines(self, doc):
         # type: (QTextDocument) -> Iterable[QTextLine]
         for block in self._blocks(doc):
             blocklayout = block.layout()
             for i in range(blocklayout.lineCount()):
                 yield blocklayout.lineAt(i)
 
+    def __textBackgroundPath(self) -> QPainterPath:
+        # return a path outlining all the text lines.
+        if self.__cachedBackgroundPath is None:
+            doc = self.document()
+            margin = doc.documentMargin()
+            path = QPainterPath()
+            offset = min(margin, 2)
+            for line in self._lines(doc):
+                rect = line.naturalTextRect()
+                rect.translate(margin, margin)
+                rect = rect.adjusted(-offset, -offset, offset, offset)
+                p = QPainterPath()
+                p.addRoundedRect(rect, 3, 3)
+                path = path.united(p)
+            self.__cachedBackgroundPath = path
+        return self.__cachedBackgroundPath
+
     def setSelectionState(self, state):
         # type: (bool) -> None
         if self.__selected != state:
             self.__selected = state
             self.__updateDefaultTextColor()
             self.update()
 
@@ -915,14 +930,15 @@
             role = QPalette.WindowText
         self.setDefaultTextColor(self.palette().color(role))
 
     def setHtml(self, contents):
         # type: (str) -> None
         if contents != self.__content:
             self.__content = contents
+            self.__cachedBackgroundPath = None
             super().setHtml(contents)
 
 
 class NodeItem(QGraphicsWidget):
     """
     An widget node item in the canvas.
     """
```

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/utils.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/annotationitem.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/annotationitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/controlpoints.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/controlpoints.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/canvas/items/linkitem.py` & `orange-canvas-core-0.1.9/orangecanvas/canvas/items/linkitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange.qss` & `orange-canvas-core-0.1.9/orangecanvas/styles/orange.qss`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Grid.svg` & `orange-canvas-core-0.1.9/orangecanvas/styles/orange/Grid.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Search.svg` & `orange-canvas-core-0.1.9/orangecanvas/styles/orange/Search.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Arrow.svg` & `orange-canvas-core-0.1.9/orangecanvas/styles/orange/Arrow.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Info.svg` & `orange-canvas-core-0.1.9/orangecanvas/styles/orange/Info.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Text Size.svg` & `orange-canvas-core-0.1.9/orangecanvas/styles/orange/Text Size.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Document Info.svg` & `orange-canvas-core-0.1.9/orangecanvas/styles/orange/Document Info.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Dropdown.svg` & `orange-canvas-core-0.1.9/orangecanvas/styles/orange/Dropdown.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/styles/orange/Pause.svg` & `orange-canvas-core-0.1.9/orangecanvas/styles/orange/Pause.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Grid.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Grid.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Search.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Search.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Examples.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Examples.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Arrow.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Arrow.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Get Started.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Get Started.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/default-widget.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/default-widget.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/orange-splash-screen.png` & `orange-canvas-core-0.1.9/orangecanvas/icons/orange-splash-screen.png`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Recent.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Recent.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Documentation.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Documentation.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/default-category.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/default-category.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Info.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Info.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Tutorials.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Tutorials.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/orange-canvas.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/orange-canvas.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Back.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Back.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Maximize Toolbar.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Maximize Toolbar.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Text Size.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Text Size.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Document Info.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Document Info.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Open.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Open.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/YouTube.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/YouTube.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/New.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/New.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Dropdown.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Dropdown.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Minimize Toolbar.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Minimize Toolbar.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/icons/Pause.svg` & `orange-canvas-core-0.1.9/orangecanvas/icons/Pause.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/splashscreen.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/splashscreen.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/toolbox.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/toolbox.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/lineedit.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/lineedit.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_lineedit.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_lineedit.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_toolbox.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_toolbox.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_dock.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_dock.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_dropshadow.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_dropshadow.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_stackedwidget.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_stackedwidget.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_toolbar.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_toolbar.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_splashscreen.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_splashscreen.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_toolgrid.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_toolgrid.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tests/test_tooltree.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tests/test_tooltree.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/dock.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/dock.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/textlabel.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/textlabel.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/test.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/test.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/dropshadow.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/dropshadow.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/tooltree.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/tooltree.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/stackedwidget.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/stackedwidget.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/toolgrid.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/toolgrid.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/toolbar.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/toolbar.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/utils.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/iconview.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/iconview.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/framelesswindow.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/framelesswindow.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/quickhelp.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/quickhelp.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/itemmodels.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/itemmodels.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/gui/svgiconengine.py` & `orange-canvas-core-0.1.9/orangecanvas/gui/svgiconengine.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/description.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/description.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/discovery.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/discovery.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/qt.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/qt.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/tests/__init__.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/tests/test_discovery.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/tests/test_base.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/cache.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/cache.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/__init__.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/utils.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/registry/base.py` & `orange-canvas-core-0.1.9/orangecanvas/registry/base.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/resources.py` & `orange-canvas-core-0.1.9/orangecanvas/resources.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/preview/scanner.py` & `orange-canvas-core-0.1.9/orangecanvas/preview/scanner.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/preview/tests/test_scanner.py` & `orange-canvas-core-0.1.9/orangecanvas/preview/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/preview/tests/test_previewbrowser.py` & `orange-canvas-core-0.1.9/orangecanvas/preview/tests/test_previewbrowser.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/preview/tests/test_previewdialog.py` & `orange-canvas-core-0.1.9/orangecanvas/preview/tests/test_previewdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/preview/previewmodel.py` & `orange-canvas-core-0.1.9/orangecanvas/preview/previewmodel.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/preview/previewbrowser.py` & `orange-canvas-core-0.1.9/orangecanvas/preview/previewbrowser.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/preview/previewdialog.py` & `orange-canvas-core-0.1.9/orangecanvas/preview/previewdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/widgettoolbox.py` & `orange-canvas-core-0.1.9/orangecanvas/application/widgettoolbox.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/canvasmain.py` & `orange-canvas-core-0.1.9/orangecanvas/application/canvasmain.py`

 * *Files 0% similar despite different names*

```diff
@@ -885,15 +885,16 @@
     def on_tool_box_widget_activated(self, action):
         """A widget action in the widget toolbox has been activated.
         """
         widget_desc = action.data()
         if isinstance(widget_desc, WidgetDescription):
             scheme_widget = self.current_document()
             if scheme_widget:
-                scheme_widget.usageStatistics().set_action_type(UsageStatistics.NodeAddClick)
+                statistics = scheme_widget.usageStatistics()
+                statistics.begin_action(UsageStatistics.ToolboxClick)
                 scheme_widget.createNewNode(widget_desc)
 
     def on_quick_category_action(self, action):
         """The quick category menu action triggered.
         """
         category = action.text()
         settings = QSettings()
@@ -1852,24 +1853,24 @@
         document = self.current_document()
         if document.isModifiedStrict():
             if self.ask_save_changes() == QDialog.Rejected:
                 # Reject the event
                 event.ignore()
                 return
 
-        document.usageStatistics().write_statistics()
-
         old_scheme = document.scheme()
 
         # Set an empty scheme to clear the document
         document.setScheme(config.workflow_constructor(parent=self))
         if old_scheme is not None:
             QApplication.sendEvent(old_scheme, QEvent(QEvent.Close))
             old_scheme.deleteLater()
 
+        document.usageStatistics().close()
+
         geometry = self.saveGeometry()
         state = self.saveState(version=self.SETTINGS_VERSION)
         settings = QSettings()
         settings.beginGroup("mainwindow")
         settings.setValue("geometry", geometry)
         settings.setValue("state", state)
         settings.setValue("canvasdock/expanded",
```

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/outputview.py` & `orange-canvas-core-0.1.9/orangecanvas/application/outputview.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/addons.py` & `orange-canvas-core-0.1.9/orangecanvas/application/addons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1044,15 +1044,15 @@
             msg_box.setInformativeText('Press OK to close Orange now.')
 
             msg_box.button(QMessageBox.Cancel).setText('Close later')
             return msg_box.exec_()
 
         if QMessageBox.Ok == message_restart(self):
             self.accept()
-            self.parent().close()
+            QApplication.closeAllWindows()
         else:
             self.reject()
 
 
 PYPI_API_JSON = "https://pypi.org/pypi/{name}/json"
 
 
@@ -1243,14 +1243,16 @@
         fn = os.path.join(sysconfig.get_path("purelib"), "test_write_" + str(os.getpid()))
         with open(fn, "w"):
             pass
         os.remove(fn)
         return True
     except PermissionError:
         return False
+    except OSError:
+        return False
 
 
 class Command(enum.Enum):
     Install = "Install"
     Upgrade = "Upgrade"
     Uninstall = "Uninstall"
```

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/canvastooldock.py` & `orange-canvas-core-0.1.9/orangecanvas/application/canvastooldock.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_widgettoolbox.py` & `orange-canvas-core-0.1.9/orangecanvas/application/tests/test_widgettoolbox.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_schemeinfo.py` & `orange-canvas-core-0.1.9/orangecanvas/application/tests/test_schemeinfo.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_canvastooldock.py` & `orange-canvas-core-0.1.9/orangecanvas/application/tests/test_canvastooldock.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_mainwindow.py` & `orange-canvas-core-0.1.9/orangecanvas/application/tests/test_mainwindow.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_addons.py` & `orange-canvas-core-0.1.9/orangecanvas/application/tests/test_addons.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_welcomedialog.py` & `orange-canvas-core-0.1.9/orangecanvas/application/tests/test_welcomedialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_outputview.py` & `orange-canvas-core-0.1.9/orangecanvas/application/tests/test_outputview.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/tests/test_settings.py` & `orange-canvas-core-0.1.9/orangecanvas/application/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/aboutdialog.py` & `orange-canvas-core-0.1.9/orangecanvas/application/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/application.py` & `orange-canvas-core-0.1.9/orangecanvas/application/application.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/schemeinfo.py` & `orange-canvas-core-0.1.9/orangecanvas/application/schemeinfo.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/examples.py` & `orange-canvas-core-0.1.9/orangecanvas/application/examples.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/settings.py` & `orange-canvas-core-0.1.9/orangecanvas/application/settings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/application/welcomedialog.py` & `orange-canvas-core-0.1.9/orangecanvas/application/welcomedialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/main.py` & `orange-canvas-core-0.1.9/orangecanvas/main.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/help/provider.py` & `orange-canvas-core-0.1.9/orangecanvas/help/provider.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/help/intersphinx.py` & `orange-canvas-core-0.1.9/orangecanvas/help/intersphinx.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/help/tests/test_provider.py` & `orange-canvas-core-0.1.9/orangecanvas/help/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orangecanvas/help/manager.py` & `orange-canvas-core-0.1.9/orangecanvas/help/manager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/application.welcomedialog.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/application.welcomedialog.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.node.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.node.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.events.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.events.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/canvas.items.nodeitem.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/canvas.items.nodeitem.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.annotation.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.annotation.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/gui.stackedwidget.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/gui.stackedwidget.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/overview.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/overview.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/registry.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/registry.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/application.canvasmain.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/application.canvasmain.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.scheme.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.scheme.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/canvas.scene.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/canvas.scene.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/document.schemeedit.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/document.schemeedit.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/orangecanvas/scheme.widgetmanager.rst` & `orange-canvas-core-0.1.9/docs/source/orangecanvas/scheme.widgetmanager.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/source/conf.py` & `orange-canvas-core-0.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/docs/make.bat` & `orange-canvas-core-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/setup.py` & `orange-canvas-core-0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 from setuptools import setup, find_packages
 
 NAME = "orange-canvas-core"
-VERSION = "0.1.8rc3"
+VERSION = "0.1.9"
 DESCRIPTION = "Core component of Orange Canvas"
 
 with open("README.rst", "rt", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 URL = "http://orange.biolab.si/"
 AUTHOR = "Bioinformatics Laboratory, FRI UL"
```

### Comparing `orange-canvas-core-0.1.8rc3/README.rst` & `orange-canvas-core-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.1.8rc3/orange_canvas_core.egg-info/PKG-INFO` & `orange-canvas-core-0.1.9/orange_canvas_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-canvas-core
-Version: 0.1.8rc3
+Version: 0.1.9
 Summary: Core component of Orange Canvas
 Home-page: http://orange.biolab.si/
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/biolab/orange-canvas-core/issues
 Project-URL: Source, https://github.com/biolab/orange-canvas-core/
```

### Comparing `orange-canvas-core-0.1.8rc3/orange_canvas_core.egg-info/SOURCES.txt` & `orange-canvas-core-0.1.9/orange_canvas_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 orangecanvas/document/schemeedit.py
 orangecanvas/document/suggestions.py
 orangecanvas/document/usagestatistics.py
 orangecanvas/document/tests/__init__.py
 orangecanvas/document/tests/test_editlinksdialog.py
 orangecanvas/document/tests/test_quickmenu.py
 orangecanvas/document/tests/test_schemeedit.py
+orangecanvas/document/tests/test_usagestatistics.py
 orangecanvas/gui/__init__.py
 orangecanvas/gui/dock.py
 orangecanvas/gui/dropshadow.py
 orangecanvas/gui/framelesswindow.py
 orangecanvas/gui/iconview.py
 orangecanvas/gui/itemmodels.py
 orangecanvas/gui/lineedit.py
```

### Comparing `orange-canvas-core-0.1.8rc3/LICENSE.txt` & `orange-canvas-core-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

