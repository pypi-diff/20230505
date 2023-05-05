# Comparing `tmp/zimscraperlib-3.0.0.tar.gz` & `tmp/zimscraperlib-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimscraperlib-3.0.0.tar", last modified: Fri Mar 31 11:08:10 2023, max compression
+gzip compressed data, was "zimscraperlib-3.1.0.tar", last modified: Fri May  5 10:18:17 2023, max compression
```

## Comparing `zimscraperlib-3.0.0.tar` & `zimscraperlib-3.1.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:08:10.056135 zimscraperlib-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-03-31 11:08:10.056135 zimscraperlib-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 11:08:10.056135 zimscraperlib-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:08:10.048134 zimscraperlib-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:08:10.052135 zimscraperlib-3.0.0/src/zimscraperlib/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/filesystem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/fix_ogvjs_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:08:10.052135 zimscraperlib-3.0.0/src/zimscraperlib/image/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/image/convertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/image/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/image/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/image/probing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/image/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/image/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:08:10.056135 zimscraperlib-3.0.0/src/zimscraperlib/video/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/video/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/video/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/video/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/video/probing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:08:10.056135 zimscraperlib-3.0.0/src/zimscraperlib/zim/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/zim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/zim/_libkiwix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/zim/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/zim/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/zim/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/zim/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/zim/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-03-31 11:07:58.000000 zimscraperlib-3.0.0/src/zimscraperlib/zim/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:08:10.052135 zimscraperlib-3.0.0/src/zimscraperlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-03-31 11:08:10.000000 zimscraperlib-3.0.0/src/zimscraperlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-31 11:08:10.000000 zimscraperlib-3.0.0/src/zimscraperlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:08:10.000000 zimscraperlib-3.0.0/src/zimscraperlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-31 11:08:10.000000 zimscraperlib-3.0.0/src/zimscraperlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:08:10.000000 zimscraperlib-3.0.0/src/zimscraperlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-31 11:08:10.000000 zimscraperlib-3.0.0/src/zimscraperlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 11:08:10.000000 zimscraperlib-3.0.0/src/zimscraperlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.266518 zimscraperlib-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.274518 zimscraperlib-3.1.0/src/zimscraperlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/filesystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/fix_ogvjs_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.278519 zimscraperlib-3.1.0/src/zimscraperlib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/convertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/probing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/src/zimscraperlib/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/probing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/src/zimscraperlib/zim/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/_libkiwix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.278519 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/top_level.txt
```

### Comparing `zimscraperlib-3.0.0/CHANGELOG.md` & `zimscraperlib-3.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 ## Changelog
 
 All notable changes to this project are documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (as of version 1.5.0).
 
+## [3.1.0] - 2023-05-05
+
+### Changed
+
+- Using pylibzim `3.1.0`
+- ZIM metadata check now allows multiple values (comma-separated) for `Language`
+- Using `yt_dlp` instead of `youtube_dl`
+
+### Removed
+
+- Dropped support for Python 3.6
+
 ## [3.0.0] - 2023-03-31
 
 ⚠️ Warning: this release introduce several API changes to `zim.creator.Creator` and `zim.filesystem.make_zim_file`
 
 ### Added
 
 - `zim.creator.Creator.config_metadata` method (returning Self) exposing all mandatory Metdata, all standard ones and allowing extra text metdadata.
```

### Comparing `zimscraperlib-3.0.0/LICENSE` & `zimscraperlib-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/PKG-INFO` & `zimscraperlib-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: zimscraperlib
-Version: 3.0.0
+Version: 3.1.0
 Summary: Collection of python tools to re-use common code across scrapers
 Home-page: https://github.com/openzim/python_scraperlib
 Author: kiwix
 Author-email: reg@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 zimscraperlib
 =============
 
 [![Build Status](https://github.com/openzim/python-scraperlib/workflows/CI/badge.svg?query=branch%3Amain)](https://github.com/openzim/python-scraperlib/actions?query=branch%3Amain)
```

### Comparing `zimscraperlib-3.0.0/README.md` & `zimscraperlib-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/setup.py` & `zimscraperlib-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,16 @@
     entry_points={
         "console_scripts": ["fix_ogvjs_dist=zimscraperlib.fix_ogvjs_dist:run"]
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
```

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/constants.py` & `zimscraperlib-3.1.0/src/zimscraperlib/constants.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/download.py` & `zimscraperlib-3.1.0/src/zimscraperlib/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import io
 import pathlib
 import subprocess
 from concurrent.futures import Future, ThreadPoolExecutor
 from typing import Dict, Optional, Union
 
 import requests
-import youtube_dl
+import yt_dlp as youtube_dl
 
 from . import logger
 
 
 class YoutubeDownloader:
     """Download YT videos using youtube_dl on a ThreadPoolExecutor with nb_workers
```

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/filesystem.py` & `zimscraperlib-3.1.0/src/zimscraperlib/filesystem.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/fix_ogvjs_dist.py` & `zimscraperlib-3.1.0/src/zimscraperlib/fix_ogvjs_dist.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/html.py` & `zimscraperlib-3.1.0/src/zimscraperlib/html.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/i18n.py` & `zimscraperlib-3.1.0/src/zimscraperlib/i18n.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/image/convertion.py` & `zimscraperlib-3.1.0/src/zimscraperlib/image/convertion.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/image/optimization.py` & `zimscraperlib-3.1.0/src/zimscraperlib/image/optimization.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/image/presets.py` & `zimscraperlib-3.1.0/src/zimscraperlib/image/presets.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/image/probing.py` & `zimscraperlib-3.1.0/src/zimscraperlib/image/probing.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/image/transformation.py` & `zimscraperlib-3.1.0/src/zimscraperlib/image/transformation.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/inputs.py` & `zimscraperlib-3.1.0/src/zimscraperlib/inputs.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/logging.py` & `zimscraperlib-3.1.0/src/zimscraperlib/logging.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/types.py` & `zimscraperlib-3.1.0/src/zimscraperlib/types.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/uri.py` & `zimscraperlib-3.1.0/src/zimscraperlib/uri.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/video/config.py` & `zimscraperlib-3.1.0/src/zimscraperlib/video/config.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/video/encoding.py` & `zimscraperlib-3.1.0/src/zimscraperlib/video/encoding.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/video/presets.py` & `zimscraperlib-3.1.0/src/zimscraperlib/video/presets.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/video/probing.py` & `zimscraperlib-3.1.0/src/zimscraperlib/video/probing.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/zim/__init__.py` & `zimscraperlib-3.1.0/src/zimscraperlib/zim/__init__.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/zim/_libkiwix.py` & `zimscraperlib-3.1.0/src/zimscraperlib/zim/_libkiwix.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/zim/archive.py` & `zimscraperlib-3.1.0/src/zimscraperlib/zim/archive.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/zim/creator.py` & `zimscraperlib-3.1.0/src/zimscraperlib/zim/creator.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/zim/filesystem.py` & `zimscraperlib-3.1.0/src/zimscraperlib/zim/filesystem.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/zim/items.py` & `zimscraperlib-3.1.0/src/zimscraperlib/zim/items.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/zim/metadata.py` & `zimscraperlib-3.1.0/src/zimscraperlib/zim/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,16 +55,20 @@
                 datetime.date(**{k: int(v) for k, v in match.groupdict().items()})
             except Exception as exc:
                 raise ValueError(f"Invalid {name} format: {exc}")
 
 
 def validate_language(name: str, value: Union[Iterable[str], str]):
     """ensures Language metadata is a single or list of ISO-639-3 codes"""
-    if name == "Language" and not is_valid_iso_639_3(value):
-        raise ValueError(f"{value} is not ISO-639-3.")
+    if name == "Language":
+        if isinstance(value, str):
+            value = value.split(",")
+        for code in value:
+            if not is_valid_iso_639_3(code):
+                raise ValueError(f"{code} is not ISO-639-3.")
 
 
 def validate_counter(name: str, value: str):
     """ensures Counter metadata is not manually set"""
     if name == "Counter":
         raise ValueError(f"{name} cannot be set. libzim sets it.")
```

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib/zim/providers.py` & `zimscraperlib-3.1.0/src/zimscraperlib/zim/providers.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib.egg-info/PKG-INFO` & `zimscraperlib-3.1.0/src/zimscraperlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: zimscraperlib
-Version: 3.0.0
+Version: 3.1.0
 Summary: Collection of python tools to re-use common code across scrapers
 Home-page: https://github.com/openzim/python_scraperlib
 Author: kiwix
 Author-email: reg@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 zimscraperlib
 =============
 
 [![Build Status](https://github.com/openzim/python-scraperlib/workflows/CI/badge.svg?query=branch%3Amain)](https://github.com/openzim/python-scraperlib/actions?query=branch%3Amain)
```

### Comparing `zimscraperlib-3.0.0/src/zimscraperlib.egg-info/SOURCES.txt` & `zimscraperlib-3.1.0/src/zimscraperlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

