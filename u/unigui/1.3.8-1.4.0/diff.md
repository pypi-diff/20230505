# Comparing `tmp/unigui-1.3.8.tar.gz` & `tmp/unigui-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unigui-1.3.8.tar", last modified: Sun Apr 30 19:55:19 2023, max compression
+gzip compressed data, was "dist/unigui-1.4.0.tar", last modified: Fri May  5 20:46:42 2023, max compression
```

## Comparing `unigui-1.3.8.tar` & `unigui-1.4.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.702103 unigui-1.3.8/
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.3.8/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.3.8/MANIFEST.in
--rw-r--r--   0 george    (1000) george    (1000)    19408 2023-04-30 19:55:19.702103 unigui-1.3.8/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)    19138 2023-04-30 19:49:37.000000 unigui-1.3.8/README.md
--rw-r--r--   0 george    (1000) george    (1000)       38 2023-04-30 19:55:19.702103 unigui-1.3.8/setup.cfg
--rw-r--r--   0 george    (1000) george    (1000)      565 2023-04-30 19:55:05.000000 unigui-1.3.8/setup.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.698769 unigui-1.3.8/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:50.000000 unigui-1.3.8/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     7695 2023-04-30 19:19:54.000000 unigui-1.3.8/unigui/guielements.py
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.3.8/unigui/manager.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:40.000000 unigui-1.3.8/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.3.8/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:22.000000 unigui-1.3.8/unigui/utils.py
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.698769 unigui-1.3.8/unigui/web/
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.698769 unigui-1.3.8/unigui/web/css/
--rw-r--r--   0 george    (1000) george    (1000)     3267 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/css/855.47c4761e.css
--rw-r--r--   0 george    (1000) george    (1000)        0 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/css/app.31d6cfe0.css
--rw-r--r--   0 george    (1000) george    (1000)   219590 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/css/vendor.49a52e8f.css
--rw-r--r--   0 george    (1000) george    (1000)    64483 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/favicon.ico
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.702103 unigui-1.3.8/unigui/web/fonts/
--rw-r--r--   0 george    (1000) george    (1000)    20436 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 george    (1000) george    (1000)    20544 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 george    (1000) george    (1000)    20416 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 george    (1000) george    (1000)    20408 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 george    (1000) george    (1000)    20424 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 george    (1000) george    (1000)    20344 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 george    (1000) george    (1000)   164912 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 george    (1000) george    (1000)   128360 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.702103 unigui-1.3.8/unigui/web/icons/
--rw-r--r--   0 george    (1000) george    (1000)    12324 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/icons/favicon-128x128.png
--rw-r--r--   0 george    (1000) george    (1000)      859 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/icons/favicon-16x16.png
--rw-r--r--   0 george    (1000) george    (1000)     2039 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/icons/favicon-32x32.png
--rw-r--r--   0 george    (1000) george    (1000)     9643 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/icons/favicon-96x96.png
--rw-r--r--   0 george    (1000) george    (1000)      907 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/index.html
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.702103 unigui-1.3.8/unigui/web/js/
--rw-r--r--   0 george    (1000) george    (1000)      763 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/193.b4cc3ffe.js
--rw-r--r--   0 george    (1000) george    (1000)     6560 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/430.4be6e8a8.js
--rw-r--r--   0 george    (1000) george    (1000)    39631 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/855.e620c0f1.js
--rw-r--r--   0 george    (1000) george    (1000)     5868 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/app.ed80a2d1.js
--rw-r--r--   0 george    (1000) george    (1000)   847622 2023-04-17 21:42:41.000000 unigui-1.3.8/unigui/web/js/vendor.c0de6c67.js
-drwxr-xr-x   0 george    (1000) george    (1000)        0 2023-04-30 19:55:19.698769 unigui-1.3.8/unigui.egg-info/
--rw-r--r--   0 george    (1000) george    (1000)    19408 2023-04-30 19:55:19.000000 unigui-1.3.8/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)     1194 2023-04-30 19:55:19.000000 unigui-1.3.8/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-04-30 19:55:19.000000 unigui-1.3.8/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.3.8/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-04-30 19:55:19.000000 unigui-1.3.8/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.0/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7695 2023-05-03 16:32:01.000000 unigui-1.4.0/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.0/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.0/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.0/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.0/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/css/702.ee87c168.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/vendor.c0de6c67.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/app.b57ab5bb.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/193.b4cc3ffe.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/430.4be6e8a8.js
+-rw-rw-r--   0 george    (1000) george    (1000)    39968 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/js/702.aec0d6a9.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-05 20:35:19.000000 unigui-1.4.0/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.0/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      565 2023-05-05 20:46:11.000000 unigui-1.4.0/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-05 20:46:42.000000 unigui-1.4.0/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-05 20:46:42.000000 unigui-1.4.0/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-03 16:32:01.000000 unigui-1.4.0/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.0/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.0/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1194 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-05 20:46:42.000000 unigui-1.4.0/unigui.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `unigui-1.3.8/LICENSE` & `unigui-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/PKG-INFO` & `unigui-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.3.8
+Version: 1.4.0
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # unigui #
 Universal GUI and App Browser
     Python connector
 
@@ -417,7 +418,9 @@
 Examples are in tests folder.
 
 The articles about Unigui and its protocol in details:
 
 in English https://docs.google.com/document/d/1G_9Ejt9ETDoXpTCD3YkR8CW508Idk9BaMlD72tlx8bc/edit?usp=sharing
 
 in Russian https://docs.google.com/document/d/1EleilkEX-m5XOZK5S9WytIGpImAzOhz7kW3EUaeow7Q/edit?usp=sharing
+
+
```

### Comparing `unigui-1.3.8/README.md` & `unigui-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/setup.py` & `unigui-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.3.8',      
+      version='1.4.0',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.3.8/unigui/guielements.py` & `unigui-1.4.0/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/manager.py` & `unigui-1.4.0/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/server.py` & `unigui-1.4.0/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/utils.py` & `unigui-1.4.0/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/css/855.47c4761e.css` & `unigui-1.4.0/unigui/web/css/702.ee87c168.css`

 * *Files 13% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-e163239e]{display:flex;justify-content:center}.custom-caption[data-v-e163239e]{padding:5px!important}.web-camera-container[data-v-e163239e]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-e163239e]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-e163239e]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-e163239e]{opacity:1}.web-camera-container .camera-shoot[data-v-e163239e]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-e163239e]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-e163239e]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-e163239e]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-e163239e]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-e163239e]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-e163239e]{animation:preload-e163239e 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-e163239e]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-e163239e]:nth-child(3){animation-delay:.4s}@keyframes preload-e163239e{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-e163239e]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-0440fa69]{display:flex;justify-content:center}.custom-caption[data-v-0440fa69]{padding:5px!important}.web-camera-container[data-v-0440fa69]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-0440fa69]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-0440fa69]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-0440fa69]{opacity:1}.web-camera-container .camera-shoot[data-v-0440fa69]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-0440fa69]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-0440fa69]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-0440fa69]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-0440fa69]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-0440fa69]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-0440fa69]{animation:preload-0440fa69 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-0440fa69]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-0440fa69]:nth-child(3){animation-delay:.4s}@keyframes preload-0440fa69{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-0440fa69]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.3.8/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.4.0/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/favicon.ico` & `unigui-1.4.0/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.4.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.4.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.4.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.4.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.4.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/icons/favicon-128x128.png` & `unigui-1.4.0/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/icons/favicon-16x16.png` & `unigui-1.4.0/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/icons/favicon-32x32.png` & `unigui-1.4.0/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/icons/favicon-96x96.png` & `unigui-1.4.0/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/index.html` & `unigui-1.4.0/unigui/web/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.ed80a2d1.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.b57ab5bb.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.3.8/unigui/web/js/193.b4cc3ffe.js` & `unigui-1.4.0/unigui/web/js/193.b4cc3ffe.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/js/430.4be6e8a8.js` & `unigui-1.4.0/unigui/web/js/430.4be6e8a8.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui/web/js/855.e620c0f1.js` & `unigui-1.4.0/unigui/web/js/702.aec0d6a9.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [855], {
-        9855: (e, t, a) => {
+    [702], {
+        9702: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Qt
+                default: () => Wt
             });
             var l = a(3673),
                 s = a(2323);
-            const o = (0, l._)("div", {
+            const i = (0, l._)("div", {
                 class: "q-pa-lg"
             }, null, -1);
 
-            function i(e, t, a, i, n, d) {
+            function o(e, t, a, o, n, d) {
                 const r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-tab"),
                     h = (0, l.up)("q-tabs"),
                     u = (0, l.up)("q-toolbar"),
                     p = (0, l.up)("q-header"),
                     g = (0, l.up)("zone"),
                     m = (0, l.up)("q-page"),
@@ -29,15 +29,15 @@
                     }, {
                         default: (0, l.w5)((() => [(0, l.Wm)(u, null, {
                             default: (0, l.w5)((() => [(0, l.Wm)(r, {
                                 class: "text-h5"
                             }, {
                                 default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.screen.header ? e.screen.header : ""), 1)])),
                                 _: 1
-                            }), o, (0, l.Wm)(h, {
+                            }), i, (0, l.Wm)(h, {
                                 class: "text-teal",
                                 align: "center",
                                 "inline-label": "",
                                 dense: "",
                                 modelValue: e.tab,
                                 "onUpdate:modelValue": t[0] || (t[0] = t => e.tab = t),
                                 style: {
@@ -68,15 +68,15 @@
                         _: 1
                     })])),
                     _: 1
                 })
             }
             a(71);
 
-            function n(e, t, a, o, i, n) {
+            function n(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-item-section"),
                     c = (0, l.up)("q-item-label"),
                     h = (0, l.up)("q-item");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     clickable: "",
                     tag: "a",
@@ -128,16 +128,16 @@
 
             function j(e) {
                 for (var t in e) e.hasOwnProperty(t) && delete e[t]
             }
 
             function S(e, t, a, l = "?") {
                 let s = ++_,
-                    o = [e.pdata.name, e.data.name, l, t, s];
-                C(o), p[s] = a
+                    i = [e.pdata.name, e.data.name, l, t, s];
+                C(i), p[s] = a
             }
 
             function A() {
                 j(y), j(b)
             }
 
             function Z(e, t) {
@@ -190,78 +190,78 @@
 
             function W(e) {
                 Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), g && console.log("------------------recalc design");
                 const t = V(e),
                     a = H(e);
                 for (let [l, s] of Object.entries(t)) {
                     let e = b[l];
-                    const [t, o] = a[l];
-                    let i, n = e.geom().el,
+                    const [t, i] = a[l];
+                    let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = y[d];
                     for (let a of r.data.childs)
                         if (Array.isArray(a)) {
                             if (a.find((t => t.name == e.data.name))) {
                                 let e = a[a.length - 1],
                                     t = `${e.name}@${d}`;
-                                i = b[t];
+                                o = b[t];
                                 break
                             }
                         } else if (a.name == e.data.name) {
-                        i = e;
+                        o = e;
                         break
                     }
-                    let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (i ? i.geom().right : e.geom().right);
-                    c /= o;
+                    let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
+                    c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
                     e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
             function V(e) {
                 const t = u.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
-                    o = {};
-                for (let [d, r] of Object.entries(y)) o[r.name] = r.$el.getBoundingClientRect().height;
-                let i = [];
+                    i = {};
+                for (let [d, r] of Object.entries(y)) i[r.name] = r.$el.getBoundingClientRect().height;
+                let o = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
                         n = t ? z(d) : [
                             [d]
                         ];
                     for (let a of n) {
                         let e = 0;
-                        for (let t of a) e += o[t.name] + 8;
-                        i.push([e, a])
+                        for (let t of a) e += i[t.name] + 8;
+                        o.push([e, a])
                     }
-                    i.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
-                    for (let l of i) {
+                    o.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
+                    for (let l of o) {
                         let t = l[1];
                         (0, r.hu)(Array.isArray(t));
-                        const o = [];
+                        const i = [];
                         for (let [e, a] of Object.entries(b))
                             if (a.expanding_height) {
-                                let [l, i] = e.split("@");
-                                if (t.find((e => e.name == i))) {
+                                let [l, o] = e.split("@");
+                                if (t.find((e => e.name == o))) {
                                     let e = !0;
                                     const t = a.geom();
-                                    for (let [l, i] of o.entries()) {
-                                        let n = i.geom();
-                                        if (i !== a && n.top == t.top) {
-                                            n.scrollHeight < t.scrollHeight && (o[l] = a), e = !1, s.set(a.fullname, i.fullname);
+                                    for (let [l, o] of i.entries()) {
+                                        let n = o.geom();
+                                        if (o !== a && n.top == t.top) {
+                                            n.scrollHeight < t.scrollHeight && (i[l] = a), e = !1, s.set(a.fullname, o.fullname);
                                             break
                                         }
                                     }
-                                    e && o.push(a)
+                                    e && i.push(a)
                                 }
-                            } o.length && e.push([a - l[0] - 64, o])
+                            } i.length && e.push([a - l[0] - 64, i])
                     }
                     for (let [a, s] of e) {
                         s.sort(((e, t) => e.geom().scrollHeight < t.geom().scrollHeight));
                         let e = s.length;
                         for (let t of s) t.fullname in l && (e--, a -= l[t.fullname]);
                         for (let t of s) t.fullname in l || ("docviewer" == t.type ? l[t.fullname] = a / e + 4 : l[t.fullname] = a / e)
                     }
@@ -291,56 +291,56 @@
                         for (let t of n)
                             for (let a of l) e.push(Array.isArray(t) ? a.concat(t) : [...a, t]);
                     else
                         for (let t of l) e.push([...t, n]);
                     l = e
                 }
                 l.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
-                const o = [];
-                let i = new Map;
+                const i = [];
+                let o = new Map;
                 for (let n of l) {
                     let e = Array.isArray(n) ? n[n.length - 1] : n,
                         t = y[e.name].$el.getBoundingClientRect().right;
                     e = Array.isArray(n) ? n[0] : n;
                     let l = y[e.name].$el.getBoundingClientRect().left,
                         s = a - t + l - 10;
                     const d = [];
-                    for (let [a, o] of Object.entries(b))
-                        if (o.expanding_width) {
+                    for (let [a, i] of Object.entries(b))
+                        if (i.expanding_width) {
                             let e = a.split("@")[1];
                             if (n.find((t => t.name == e))) {
                                 let e = !0,
-                                    t = o.geom().left;
+                                    t = i.geom().left;
                                 for (let [a, l] of d.entries())
-                                    if (l !== o && l.geom().left == t) {
-                                        l.geom().scrollWidth < o.geom().scrollWidth ? (d[a] = o, i.set(l.fullname, o.fullname)) : i.set(o.fullname, l.fullname), e = !1;
+                                    if (l !== i && l.geom().left == t) {
+                                        l.geom().scrollWidth < i.geom().scrollWidth ? (d[a] = i, o.set(l.fullname, i.fullname)) : o.set(i.fullname, l.fullname), e = !1;
                                         break
-                                    } e && d.push(o)
+                                    } e && d.push(i)
                             }
-                        } d.length && o.push([s, d])
+                        } d.length && i.push([s, d])
                 }
-                for (let [n, d] of o) {
+                for (let [n, d] of i) {
                     d.sort(((e, t) => e.geom().scrollWidth - t.geom().scrollWidth));
                     let e = d.length,
                         t = {};
                     for (let a of d) {
                         let l = s[a.fullname];
                         l && (e--, n -= l[0] / l[1]);
-                        let o = a.pdata ? a.pdata.name : a.name;
-                        t[o] ? t[o]++ : t[o] = 1
+                        let i = a.pdata ? a.pdata.name : a.name;
+                        t[i] ? t[i]++ : t[i] = 1
                     }
                     for (let a of d) {
                         let l = s[a.fullname];
                         if (void 0 === l) {
                             let l = a.pdata ? a.pdata.name : a.name;
                             s[a.fullname] = [Math.floor(n / e), t[l]]
                         }
                     }
                 }
-                for (let [n, d] of i.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
+                for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
                 return s
             }
             const E = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
                         C(["root", this.name])
@@ -370,30 +370,30 @@
                 B = L;
             R()(E, "components", {
                 QItem: T.Z,
                 QItemSection: K.Z,
                 QIcon: P.Z,
                 QItemLabel: N.Z
             });
-            const Y = {
+            const F = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
-                F = {
+                Y = {
                     class: "q-col-gutter-sm q-py-sm"
                 },
                 X = {
                     key: 0,
                     class: "column q-col-gutter-sm q-py-sm"
                 };
 
-            function J(e, t, a, s, o, i) {
+            function J(e, t, a, s, i, o) {
                 const n = (0, l.up)("zone", !0),
                     d = (0, l.up)("block");
-                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", Y, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", F, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", X, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
+                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", F, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", Y, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", X, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
                     data: e
                 }, null, 8, ["data"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e.data
@@ -416,15 +416,15 @@
                 },
                 le = ["data", "pdata"],
                 se = {
                     key: 0,
                     class: "row"
                 };
 
-            function oe(e, t, a, o, i, n) {
+            function ie(e, t, a, i, o, n) {
                 const d = (0, l.up)("element"),
                     r = (0, l.up)("q-icon"),
                     c = (0, l.up)("q-scroll-area"),
                     h = (0, l.up)("q-card");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     class: "my-card q-ma-xs"
                 }, {
@@ -476,16 +476,16 @@
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
                     _: 1
                 })
             }
-            var ie = a(8880);
-            const ne = e => ((0, l.dD)("data-v-e163239e"), e = e(), (0, l.Cn)(), e),
+            var oe = a(8880);
+            const ne = e => ((0, l.dD)("data-v-0440fa69"), e = e(), (0, l.Cn)(), e),
                 de = ["width", "height"],
                 re = ["src"],
                 ce = {
                     key: 15,
                     class: "web-camera-container"
                 },
                 he = {
@@ -515,15 +515,15 @@
                 }, null, -1))),
                 ve = [ke],
                 Ce = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function xe(e, t, a, o, i, n) {
+            function xe(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-img"),
                     c = (0, l.up)("q-badge"),
                     h = (0, l.up)("q-select"),
                     u = (0, l.up)("q-checkbox"),
                     p = (0, l.up)("q-toggle"),
                     g = (0, l.up)("q-btn-toggle"),
@@ -535,22 +535,22 @@
                     k = (0, l.up)("q-uploader"),
                     v = (0, l.up)("cgraph"),
                     C = (0, l.up)("q-btn");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
-                    onClick: (0, ie.iM)(e.switchValue, ["stop"]),
+                    onClick: (0, oe.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, s.j5)(e.elemSize)
                 }, {
                     default: (0, l.w5)((() => [e.data.header ? ((0, l.wg)(), (0, l.iD)("div", {
                         key: 0,
                         class: "absolute-bottom-right text-subtitle2 custom-caption",
-                        onClick: t[0] || (t[0] = (0, ie.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
+                        onClick: t[0] || (t[0] = (0, oe.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
                     }, (0, s.zw)(e.data.header), 1)) : (0, l.kq)("", !0), e.value ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "absolute all-pointer-events",
                         size: "32px",
                         name: "check_circle",
                         color: "gray",
                         style: {
@@ -623,15 +623,15 @@
                     key: 6,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
-                    onKeyup: (0, ie.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, l.wg)(), (0, l.j4)(h, {
                     key: 7,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     "use-input": "",
@@ -640,15 +640,15 @@
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
-                    onKeyup: (0, ie.D2)(e.pressedEnter, ["enter"])
+                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"])
                 }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(y, {
                     key: 8,
                     style: (0, s.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(w, {
@@ -666,15 +666,15 @@
                     key: 9,
                     class: "textarea",
                     "onUpdate:modelValue": t[9] || (t[9] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, s.j5)(e.elemSize)
                 }, null, 4)), [
-                    [ie.nr, e.value]
+                    [oe.nr, e.value]
                 ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(b, {
                     key: 10,
                     color: "green"
                 })) : "video" == e.type ? ((0, l.wg)(), (0, l.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
@@ -712,15 +712,15 @@
                     class: (0, s.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[10] || (t[10] = (...t) => e.toggleCamera && e.toggleCamera(...t))
                 }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", pe, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", ue, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", ge, fe, 512), [
-                    [ie.F8, e.isCameraOpen && e.isLoading]
+                    [oe.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("div", {
                     key: 0,
                     class: (0, s.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, l._)("div", {
                     class: (0, s.C_)(["camera-shutter", {
@@ -728,24 +728,24 @@
                     }])
                 }, null, 2), (0, l.wy)((0, l._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
                 }, null, 8, we), [
-                    [ie.F8, !e.isPhotoTaken]
+                    [oe.F8, !e.isPhotoTaken]
                 ]), (0, l.wy)((0, l._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
                 }, null, 8, ye), [
-                    [ie.F8, e.isPhotoTaken]
+                    [oe.F8, e.isPhotoTaken]
                 ])], 2)), [
-                    [ie.F8, !e.isLoading]
+                    [oe.F8, !e.isLoading]
                 ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", be, [(0, l._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.takePhoto && e.takePhoto(...t))
                 }, ve)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", Ce, [(0, l.Wm)(C, {
                     onClick: e.downloadImage,
                     label: "Send"
@@ -767,15 +767,15 @@
                     key: 0
                 },
                 _e = {
                     class: "row"
                 },
                 je = ["onClick"];
 
-            function Se(e, t, a, o, i, n) {
+            function Se(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-input"),
                     c = (0, l.up)("q-tooltip"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-th"),
                     p = (0, l.up)("q-tr"),
                     g = (0, l.up)("q-checkbox"),
@@ -928,25 +928,25 @@
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props"])])),
                     body: (0, l.w5)((t => [(0, l.Wm)(p, {
                         props: t,
                         onClick: e => t.selected = !t.selected
                     }, {
-                        default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.columns, ((a, o) => ((0, l.wg)(), (0, l.j4)(f, {
+                        default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.columns, ((a, i) => ((0, l.wg)(), (0, l.j4)(f, {
                             key: a.name,
                             props: t
                         }, {
                             default: (0, l.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, l.wg)(), (0, l.j4)(g, {
                                 key: 0,
                                 modelValue: t.row[a.name],
-                                "onUpdate:modelValue": [e => t.row[a.name] = e, l => e.change_switcher(t.row, a.name, o)],
+                                "onUpdate:modelValue": [e => t.row[a.name] = e, l => e.change_switcher(t.row, a.name, i)],
                                 dense: "",
                                 disable: !e.editMode
-                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && o == e.cedit && e.redit == t.row.iiid ? ((0, l.wg)(), (0, l.j4)(m, {
+                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && i == e.cedit && e.redit == t.row.iiid ? ((0, l.wg)(), (0, l.j4)(m, {
                                 key: 1,
                                 dense: "",
                                 "model-value": t.row[a.name],
                                 "use-input": "",
                                 "hide-selected": "",
                                 "fill-input": "",
                                 autofocus: "",
@@ -954,71 +954,76 @@
                                 borderless: "",
                                 onInputValue: e.change,
                                 "hide-dropdown-icon": "",
                                 "input-debounce": "0",
                                 options: e.options,
                                 onFilter: e.complete,
                                 onKeydown: e.keyInput
-                            }, null, 8, ["model-value", "onInputValue", "options", "onFilter", "onKeydown"])) : e.editMode && o == e.cedit && e.redit == t.row.iiid ? ((0, l.wg)(), (0, l.j4)(r, {
+                            }, null, 8, ["model-value", "onInputValue", "options", "onFilter", "onKeydown"])) : e.editMode && i == e.cedit && e.redit == t.row.iiid ? ((0, l.wg)(), (0, l.j4)(r, {
                                 key: 2,
                                 modelValue: t.row[a.name],
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, l.wg)(), (0, l.iD)("div", {
                                 key: 3,
-                                onClick: a => e.select(t.row.iiid, o)
+                                onClick: a => e.select(t.row.iiid, i)
                             }, (0, s.zw)(t.row[a.name]), 9, je))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
             var Ae = a(1959);
-            const Ze = (0, l.aZ)({
+
+            function Ze(e, t) {
+                return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
+            }
+            const Me = (0, l.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
                     } = (0, Ae.BK)(e);
                     let s = (0, l.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const l = a.headers,
                                 s = l.length,
-                                o = a.rows,
-                                i = o.length;
-                            for (var n = 0, d = 0; d < i; d++) {
+                                i = a.rows,
+                                o = i.length;
+                            for (var n = 0, d = 0; d < o; d++) {
                                 const t = {},
-                                    a = o[d];
+                                    a = i[d];
                                 for (var r = 0; r < s; r++) t[l[r]] = a[r];
                                 t.iiid = s == a.length ? n : a[a.length - 1], e.push(t), n++
                             }
                             return e
                         })),
-                        o = () => {
-                            let e = t.value;
-                            return null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]]
+                        i = () => {
+                            let e = t.value,
+                                a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
+                            return a
                         },
-                        i = o(),
-                        n = (0, Ae.iH)(i),
+                        o = i(),
+                        n = (0, Ae.iH)(o),
                         d = (0, Ae.iH)(!Array.isArray(t.value.value)),
                         r = (e, l) => {
                             C([a.value.name, t.value.name, e, l])
                         },
                         c = (0, l.Fl)((() => d.value ? n.value.length > 0 ? n.value[0].iiid : null : n.value.map((e => e.iiid)))),
                         h = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
-                        n.value = o(), i = n.value
+                        n.value = i(), o = n.value
                     })), (0, l.YP)(t, ((e, a) => {
-                        g && console.log("data update", a.name), n.value = o(), i = n.value, d.value = !Array.isArray(t.value.value)
+                        g && console.log("data update", a.name), n.value = i(), o = n.value, d.value = !Array.isArray(t.value.value)
                     })), {
                         rows: s,
                         value: c,
                         selected: n,
                         singleMode: d,
                         sendMessage: r,
                         datavalue: h
@@ -1114,15 +1119,15 @@
                                 let e = a.rows;
                                 a.select(e[t], 0), a.showSelected()
                             }), 100)
                         }), "+")
                     },
                     showSelected() {
                         let e = this.$refs.table;
-                        if (this.selected) {
+                        if (this.selected.length) {
                             let t = e.computedRows.findIndex((e => e.iiid === this.selected[0].iiid));
                             e.scrollTo(t)
                         }
                     },
                     deselectAll() {
                         this.selected = [], this.sendMessage("=", this.value)
                     },
@@ -1143,15 +1148,18 @@
                             for (let t of this.selected) e.splice(t.iiid, 1)
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
-                        this.updated !== this.selected && (this.updated = this.selected, this.sendMessage("=", this.value)), this.data.show && this.showSelected()
+                        void 0 === this.updated ? this.updated = this.selected : Ze(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
+                    },
+                    data(e) {
+                        g && console.log("data update", this.name), this.updated = void 0
                     }
                 },
                 computed: {
                     redit() {
                         return console.log("redit", this.editMode && this.selected.length ? this.selected[0].iiid : null), this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
@@ -1172,52 +1180,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var Me = a(9267),
-                $e = a(4842),
-                ze = a(2165),
-                De = a(8870),
-                Oe = a(8186),
-                Qe = a(2414),
-                We = a(3884),
-                Ve = a(5735),
-                He = a(7208);
-            const Ee = (0, U.Z)(Ze, [
+            var $e = a(9267),
+                ze = a(4842),
+                De = a(2165),
+                Oe = a(8870),
+                Qe = a(8186),
+                We = a(2414),
+                Ve = a(3884),
+                He = a(5735),
+                Ee = a(7208);
+            const Ue = (0, U.Z)(Me, [
                     ["render", Se]
                 ]),
-                Ue = Ee;
-            R()(Ze, "components", {
-                QTable: Me.Z,
-                QInput: $e.Z,
+                Te = Ue;
+            R()(Me, "components", {
+                QTable: $e.Z,
+                QInput: ze.Z,
                 QIcon: P.Z,
-                QBtn: ze.Z,
-                QTooltip: De.Z,
-                QTr: Oe.Z,
-                QTh: Qe.Z,
-                QTd: We.Z,
-                QCheckbox: Ve.Z,
-                QSelect: He.Z
+                QBtn: De.Z,
+                QTooltip: Oe.Z,
+                QTr: Qe.Z,
+                QTh: We.Z,
+                QTd: Ve.Z,
+                QCheckbox: He.Z,
+                QSelect: Ee.Z
             });
-            const Te = ["nodes", "edges"];
+            const Ke = ["nodes", "edges"];
 
-            function Ke(e, t, a, o, i, n) {
+            function Pe(e, t, a, i, o, n) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Te)
+                }, null, 12, Ke)
             }
-            var Pe = a(2393),
-                Ne = a.n(Pe);
-            const Ie = Ne().stylesheet().selector("node").css({
+            var Ne = a(2393),
+                Ie = a.n(Ne);
+            const Re = Ie().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555"
                 }).selector("node[label]").css({
                     label: "data(label)",
@@ -1236,45 +1244,45 @@
                 }).selector("edge[label]").css({
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray"
                 }),
-                Re = {
+                Le = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Le(e, t) {
+            function Be(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id) return !0;
                 return !1
             }
-            const Be = (0, l.aZ)({
+            const Fe = (0, l.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Ie,
-                            layoutOptions: Re,
+                            style: Re,
+                            layoutOptions: Le,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: []
                         }
                     },
                     mounted() {
-                        let e = Ne()({
+                        let e = Ie()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1389,15 +1397,15 @@
                             }
                         },
                         data: {
                             handler(e, t) {
                                 console.log("wa gr");
                                 let a = e.value,
                                     l = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Le(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Le(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Be(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Be(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1414,38 +1422,38 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Ye = (0, U.Z)(Be, [
-                    ["render", Ke]
+                Ye = (0, U.Z)(Fe, [
+                    ["render", Pe]
                 ]),
-                Fe = Ye;
+                Xe = Ye;
 
-            function Xe(e) {
+            function Je(e) {
                 let t = e.minheight ? e.minheight : m,
                     a = e.minwidth ? e.minwidth : f;
                 return `height: ${t}px; width: ${a}px`
             }
 
-            function Je(e) {
+            function Ge(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const Ge = (0, l.aZ)({
+            const et = (0, l.aZ)({
                 name: "element",
                 components: {
-                    utable: Ue,
-                    cgraph: Fe
+                    utable: Te,
+                    cgraph: Xe
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
@@ -1507,18 +1515,19 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(Je, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(Ge, "image/jpeg")
                     },
                     geom() {
-                        const e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
+                        let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
+                        e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
                         let t = this.type;
                         const a = "docviewer" == t || "graph" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
                             l = e.getBoundingClientRect();
                         return {
                             el: e,
                             inner: a,
                             left: l.left,
@@ -1531,15 +1540,15 @@
                 },
                 mounted() {
                     b[this.fullname] = this, g && console.log("mounted", this.fullname)
                 },
                 data() {
                     return {
                         value: this.data.value,
-                        styleSize: Xe(this.data),
+                        styleSize: Je(this.data),
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
@@ -1607,25 +1616,25 @@
                     treeNodes() {
                         var e = [];
                         if ("list" == this.type) return this.data.options.map((e => ({
                             label: e,
                             children: []
                         })));
                         var t = {};
-                        for (const [s, o] of Object.entries(this.data.options)) {
+                        for (const [s, i] of Object.entries(this.data.options)) {
                             var a = t[s];
                             if (a || (a = {
                                     label: s,
                                     children: []
-                                }, t[s] = a), o) {
-                                var l = t[o];
+                                }, t[s] = a), i) {
+                                var l = t[i];
                                 l || (l = {
-                                    label: o,
+                                    label: i,
                                     children: []
-                                }, t[o] = l), l.children.push(a)
+                                }, t[i] = l), l.children.push(a)
                             } else e.push(a)
                         }
                         return e
                     }
                 },
                 props: {
                     data: {
@@ -1645,50 +1654,50 @@
                         g && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        g && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize = Xe(this.data), console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
+                        g && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize = Je(this.data), console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
                     }
                 }
             });
-            var et = a(4027),
-                tt = a(9721),
-                at = a(8886),
-                lt = a(8761),
-                st = a(1232),
+            var tt = a(4027),
+                at = a(9721),
+                lt = a(8886),
+                st = a(8761),
+                it = a(1232),
                 ot = a(5551),
-                it = a(5869),
-                nt = a(1745);
-            const dt = (0, U.Z)(Ge, [
+                nt = a(5869),
+                dt = a(1745);
+            const rt = (0, U.Z)(et, [
                     ["render", xe],
-                    ["__scopeId", "data-v-e163239e"]
+                    ["__scopeId", "data-v-0440fa69"]
                 ]),
-                rt = dt;
-            R()(Ge, "components", {
-                QImg: et.Z,
+                ct = rt;
+            R()(et, "components", {
+                QImg: tt.Z,
                 QIcon: P.Z,
-                QSelect: He.Z,
-                QBadge: tt.Z,
-                QCheckbox: Ve.Z,
-                QToggle: at.Z,
-                QBtnToggle: lt.Z,
-                QInput: $e.Z,
-                QScrollArea: st.Z,
+                QSelect: Ee.Z,
+                QBadge: at.Z,
+                QCheckbox: He.Z,
+                QToggle: lt.Z,
+                QBtnToggle: st.Z,
+                QInput: ze.Z,
+                QScrollArea: it.Z,
                 QTree: ot.Z,
-                QSeparator: it.Z,
-                QUploader: nt.Z,
-                QBtn: ze.Z
+                QSeparator: nt.Z,
+                QUploader: dt.Z,
+                QBtn: De.Z
             });
-            const ct = (0, l.aZ)({
+            const ht = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: rt
+                    element: ct
                 },
                 data() {
                     return {
                         styleSize: w,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -1755,42 +1764,51 @@
                 },
                 watch: {
                     data(e) {
                         g && console.log("data update", this.name), this.styleSize = w, y[this.name] = this, this.expanding && (b[this.fullname] = this)
                     }
                 }
             });
-            var ht = a(151);
-            const ut = (0, U.Z)(ct, [
-                    ["render", oe]
+            var ut = a(151);
+            const pt = (0, U.Z)(ht, [
+                    ["render", ie]
                 ]),
-                pt = ut;
-            R()(ct, "components", {
-                QCard: ht.Z,
+                gt = pt;
+            R()(ht, "components", {
+                QCard: ut.Z,
                 QIcon: P.Z,
-                QScrollArea: st.Z
+                QScrollArea: it.Z
             });
-            const gt = (0, l.aZ)({
+            const mt = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: pt
+                        block: gt
                     },
                     props: {
                         data: Object
+                    },
+                    updated(e) {
+                        (0, l.Y3)((() => {
+                            requestAnimationFrame((() => {
+                                requestAnimationFrame((() => {
+                                    W()
+                                }))
+                            }))
+                        }))
                     }
                 }),
-                mt = (0, U.Z)(gt, [
+                ft = (0, U.Z)(mt, [
                     ["render", J]
                 ]),
-                ft = mt,
-                wt = {
+                wt = ft,
+                yt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function yt(e, t, a, o, i, n) {
+            function bt(e, t, a, i, o, n) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
@@ -1806,32 +1824,32 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", wt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", yt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const bt = {
+            const kt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: pt
+                    block: gt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
@@ -1847,30 +1865,30 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var kt = a(5926),
-                vt = a(2025);
-            const Ct = (0, U.Z)(bt, [
-                    ["render", yt]
+            var vt = a(5926),
+                Ct = a(2025);
+            const xt = (0, U.Z)(kt, [
+                    ["render", bt]
                 ]),
-                xt = Ct;
-            R()(bt, "components", {
-                QDialog: kt.Z,
-                QCard: ht.Z,
+                qt = xt;
+            R()(kt, "components", {
+                QDialog: vt.Z,
+                QCard: ut.Z,
                 QItemLabel: N.Z,
-                QSpace: vt.Z,
-                QBtn: ze.Z
+                QSpace: Ct.Z,
+                QBtn: De.Z
             });
-            var qt = !0;
-            let _t = null;
-            const jt = (0, l.aZ)({
+            var _t = !0;
+            let jt = null;
+            const St = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         localServer: !0,
@@ -1879,15 +1897,15 @@
                             blocks: []
                         },
                         prevHeight: 0
                     }
                 },
                 components: {
                     menubar: B,
-                    zone: ft
+                    zone: wt
                 },
                 created() {
                     v(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
@@ -1904,15 +1922,15 @@
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: xt
+                                component: qt
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -1930,85 +1948,82 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == _t ? (l = {
+                        "progress" == t ? null == jt ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, _t = this.$q.notify(l)) : null == e ? (_t(), _t = null) : (l = {
+                        }, jt = this.$q.notify(l)) : null == e ? (jt(), jt = null) : (l = {
                             caption: e
-                        }, _t(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, jt(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if (qt) qt = !1, this.menu = e[0].map((e => ({
+                        if (_t) _t = !1, this.menu = e[0].map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), Q(), this.screen = e[1], this.tab = this.screen.name, g && console.log("init loading..");
-                        else if ("screen" == e.type) A(), Q(), this.screen = e;
+                        else if ("screen" == e.type) A(), this.screen = e;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = xt, t.componentProps = {
+                            t.component = qt, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
                         } else if (e.hasOwnProperty("answer")) $(e);
                         else {
                             e.update && M(e);
                             let t = !1;
                             for (let a of k) a in e && (this.notify(e[a], a), t = !0);
                             t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        _t && !e.progress && this.notify(null, "progress")
+                        jt && !e.progress && this.notify(null, "progress")
                     }
                 },
                 mounted() {
-                    Q(), window.addEventListener("resize", this.onResize)
-                },
-                updated() {
-                    g && console.log("before updated")
+                    window.addEventListener("resize", this.onResize)
                 }
             });
-            var St = a(9214),
-                At = a(3812),
-                Zt = a(9570),
-                Mt = a(7547),
-                $t = a(3269),
-                zt = a(2652),
-                Dt = a(4379);
-            const Ot = (0, U.Z)(jt, [
-                    ["render", i]
+            var At = a(9214),
+                Zt = a(3812),
+                Mt = a(9570),
+                $t = a(7547),
+                zt = a(3269),
+                Dt = a(2652),
+                Ot = a(4379);
+            const Qt = (0, U.Z)(St, [
+                    ["render", o]
                 ]),
-                Qt = Ot;
-            R()(jt, "components", {
-                QLayout: St.Z,
-                QHeader: At.Z,
-                QToolbar: Zt.Z,
-                QBtn: ze.Z,
+                Wt = Qt;
+            R()(St, "components", {
+                QLayout: At.Z,
+                QHeader: Zt.Z,
+                QToolbar: Mt.Z,
+                QBtn: De.Z,
                 QItemLabel: N.Z,
-                QTabs: Mt.Z,
-                QTab: $t.Z,
-                QPageContainer: zt.Z,
-                QPage: Dt.Z
+                QTabs: $t.Z,
+                QTab: zt.Z,
+                QPageContainer: Dt.Z,
+                QPage: Ot.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.3.8/unigui/web/js/app.ed80a2d1.js` & `unigui-1.4.0/unigui/web/js/app.b57ab5bb.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(855)]).then(r.bind(r, 9855)),
+                        component: () => Promise.all([r.e(736), r.e(702)]).then(r.bind(r, 9702)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -44,30 +44,30 @@
                                     top: 0
                                 }),
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
-                async function b(e, t) {
+                async function g(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
                         n = e(d);
                     return n.use(o.Z, t), {
                         app: n,
                         router: r
                     }
                 }
-                var g = r(6417),
+                var b = r(6417),
                     y = r(5597);
                 const w = {
                         config: {
                             notify: {}
                         },
                         plugins: {
-                            Notify: g.Z,
+                            Notify: b.Z,
                             Dialog: y.Z
                         }
                     },
                     O = "";
                 async function k({
                     app: e,
                     router: t
@@ -94,15 +94,15 @@
                             urlPath: i,
                             publicPath: O
                         })
                     } catch (l) {
                         return l && l.url ? void a(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== n && (e.use(t), e.mount("#q-app"))
                 }
-                b(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
+                g(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
                     const r = t.map((e => e.default)).filter((e => "function" === typeof e));
                     k(e, r)
                 }))))
             },
             2390: (e, t, r) => {
                 r.r(t), r.d(t, {
                     default: () => o
@@ -160,24 +160,24 @@
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "b4cc3ffe",
             430: "4be6e8a8",
-            855: "e620c0f1"
+            702: "aec0d6a9"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            736: "49a52e8f",
-            855: "47c4761e"
+            702: "ee87c168",
+            736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                855: 1
+                702: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.3.8/unigui/web/js/vendor.c0de6c67.js` & `unigui-1.4.0/unigui/web/js/vendor.c0de6c67.js`

 * *Files identical despite different names*

### Comparing `unigui-1.3.8/unigui.egg-info/PKG-INFO` & `unigui-1.4.0/unigui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.3.8
+Version: 1.4.0
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # unigui #
 Universal GUI and App Browser
     Python connector
 
@@ -417,7 +418,9 @@
 Examples are in tests folder.
 
 The articles about Unigui and its protocol in details:
 
 in English https://docs.google.com/document/d/1G_9Ejt9ETDoXpTCD3YkR8CW508Idk9BaMlD72tlx8bc/edit?usp=sharing
 
 in Russian https://docs.google.com/document/d/1EleilkEX-m5XOZK5S9WytIGpImAzOhz7kW3EUaeow7Q/edit?usp=sharing
+
+
```

### Comparing `unigui-1.3.8/unigui.egg-info/SOURCES.txt` & `unigui-1.4.0/unigui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/855.47c4761e.css
+unigui/web/css/702.ee87c168.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -28,10 +28,10 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.b4cc3ffe.js
 unigui/web/js/430.4be6e8a8.js
-unigui/web/js/855.e620c0f1.js
-unigui/web/js/app.ed80a2d1.js
+unigui/web/js/702.aec0d6a9.js
+unigui/web/js/app.b57ab5bb.js
 unigui/web/js/vendor.c0de6c67.js
```

