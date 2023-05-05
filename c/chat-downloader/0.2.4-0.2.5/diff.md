# Comparing `tmp/chat-downloader-0.2.4.tar.gz` & `tmp/chat-downloader-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-downloader-0.2.4.tar", last modified: Wed Feb 22 12:30:12 2023, max compression
+gzip compressed data, was "chat-downloader-0.2.5.tar", last modified: Fri May  5 21:15:16 2023, max compression
```

## Comparing `chat-downloader-0.2.4.tar` & `chat-downloader-0.2.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.819456 chat-downloader-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-02-22 12:30:12.819456 chat-downloader-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.815456 chat-downloader-0.2.4/chat_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/chat_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.815456 chat-downloader-0.2.4/chat_downloader/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/formatting/custom_formats.json
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/formatting/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.815456 chat-downloader-0.2.4/chat_downloader/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/output/continuous_write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.815456 chat-downloader-0.2.4/chat_downloader/sites/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/sites/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30461 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/sites/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    57648 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/sites/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    81549 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/sites/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/sites/zoom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.815456 chat-downloader-0.2.4/chat_downloader/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/chat_downloader/utils/timed_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.815456 chat-downloader-0.2.4/chat_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-02-22 12:30:12.000000 chat-downloader-0.2.4/chat_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-02-22 12:30:12.000000 chat-downloader-0.2.4/chat_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 12:30:12.000000 chat-downloader-0.2.4/chat_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 12:30:12.000000 chat-downloader-0.2.4/chat_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 12:30:12.000000 chat-downloader-0.2.4/chat_downloader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-22 12:30:12.000000 chat-downloader-0.2.4/chat_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 12:30:12.000000 chat-downloader-0.2.4/chat_downloader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.819456 chat-downloader-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/items.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/options.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.819456 chat-downloader-0.2.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/source/chat_downloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/docs/source/sites.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-22 12:30:12.819456 chat-downloader-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 12:30:12.819456 chat-downloader-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   136131 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/other youtube actions
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/test_chat_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/test_init_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/test_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/test_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)    67588 2023-02-22 12:29:59.000000 chat-downloader-0.2.4/tests/youtube_actions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.643220 chat-downloader-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-05 21:15:16.643220 chat-downloader-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.627220 chat-downloader-0.2.5/chat_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/chat_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.631220 chat-downloader-0.2.5/chat_downloader/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/formatting/custom_formats.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/formatting/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.631220 chat-downloader-0.2.5/chat_downloader/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/output/continuous_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.635220 chat-downloader-0.2.5/chat_downloader/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30461 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57721 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81549 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/sites/zoom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.635220 chat-downloader-0.2.5/chat_downloader/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/chat_downloader/utils/timed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.631220 chat-downloader-0.2.5/chat_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 21:15:16.000000 chat-downloader-0.2.5/chat_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.639220 chat-downloader-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/items.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/options.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.639220 chat-downloader-0.2.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/source/chat_downloader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/docs/source/sites.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 21:15:16.647220 chat-downloader-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:15:16.643220 chat-downloader-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136131 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/other youtube actions
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_chat_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_init_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/test_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67588 2023-05-05 21:15:02.000000 chat-downloader-0.2.5/tests/youtube_actions.json
```

### Comparing `chat-downloader-0.2.4/LICENSE` & `chat-downloader-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/PKG-INFO` & `chat-downloader-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-downloader
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple tool used to retrieve chat messages from livestreams, videos, clips and past broadcasts. No authentication needed!
 Home-page: https://github.com/xenova/chat-downloader
 Author: xenova
 Author-email: admin@xenova.com
 License: MIT license
 Keywords: python chat downloader youtube twitch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chat-downloader-0.2.4/README.rst` & `chat-downloader-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/chat_downloader.py` & `chat-downloader-0.2.5/chat_downloader/chat_downloader.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/cli.py` & `chat-downloader-0.2.5/chat_downloader/cli.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/debugging.py` & `chat-downloader-0.2.5/chat_downloader/debugging.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/errors.py` & `chat-downloader-0.2.5/chat_downloader/errors.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/formatting/custom_formats.json` & `chat-downloader-0.2.5/chat_downloader/formatting/custom_formats.json`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/formatting/format.py` & `chat-downloader-0.2.5/chat_downloader/formatting/format.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/output/continuous_write.py` & `chat-downloader-0.2.5/chat_downloader/output/continuous_write.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/sites/__init__.py` & `chat-downloader-0.2.5/chat_downloader/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/sites/common.py` & `chat-downloader-0.2.5/chat_downloader/sites/common.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/sites/facebook.py` & `chat-downloader-0.2.5/chat_downloader/sites/facebook.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/sites/twitch.py` & `chat-downloader-0.2.5/chat_downloader/sites/twitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,16 @@
                                 (?:(?:www|go|m)\.)?twitch\.tv/|
                                 player\.twitch\.tv/\?.*?\bchannel=
                             )
                             (?P<id>[^/#?]+)
                         '''
     }
 
-    _CLIENT_ID = 'kimne78kx3ncx6brgo4mv6wki5h1ko'  # public client id
+    # _CLIENT_ID = 'kimne78kx3ncx6brgo4mv6wki5h1ko'  # public client id
+    _CLIENT_ID = 'kd1unb4b3q4t58fwlpcbzcbnm76a8fp'  # public client id
 
     _GQL_API_URL = 'https://gql.twitch.tv/gql'
 
     _PING_TEXT = 'PING :tmi.twitch.tv'
     _PONG_TEXT = 'PONG :tmi.twitch.tv'
 
     _SUBSCRIPTION_TYPES = {
```

### Comparing `chat-downloader-0.2.4/chat_downloader/sites/youtube.py` & `chat-downloader-0.2.5/chat_downloader/sites/youtube.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/sites/zoom.py` & `chat-downloader-0.2.5/chat_downloader/sites/zoom.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     BaseChatDownloader,
     Chat,
     Remapper as r
 )
 from ..utils.core import (
     time_to_seconds,
     regex_search,
-    ensure_seconds
+    ensure_seconds,
+    multi_get,
 )
 from ..errors import (
     SiteError,
     ParsingError
 )
 
 # TODO add debugging options
@@ -30,24 +31,25 @@
 
 
 class ZoomChatDownloader(BaseChatDownloader):
     _NAME = 'zoom.us'
 
     _ZOOM_HOMEPAGE = 'https://zoom.us/'
     _ZOOM_PATH_TEMPLATE = 'rec/play/{id}'
+    _ZOOM_API_TEMPLATE = 'nws/recording/1.0/play/info/{file_id}'
 
     _INITIAL_INFO_REGEX = r'(?s)window\.__data__\s*=\s*({.+?});'
     _CHAT_MESSAGES_REGEX = r'window\.__data__\.chatList\.push\((\{[\s\S]+?\})\)'
 
     _SITE_DEFAULT_PARAMS = {
         'format': 'default',  # TODO create zoom format
     }
 
     _REMAPPING = {
-        'username': 'author_name',
+        'userName': 'author_name',
         'time': 'time_text',
         'content': 'message',
     }
 
     _TESTS = [
         {
             'name': 'Get chat messages from past broadcast #1',
@@ -112,40 +114,57 @@
             error_message = regex_search(page_data, self._ERROR_MESSAGE_REGEX)
             if error_message:
                 raise ZoomError(error_message.split('\n')[0])
             else:
                 raise ParsingError('Error parsing video')
 
         initial_info = self._parse_js_dict(json_string)
-
         video_type = 'video' if initial_info.get('isVideo') else 'not_video'
 
-        return Chat(
-            self._get_chat_messages(page_data, params),
+        file_id = initial_info.get('fileId')
+        if not file_id:
+            raise ParsingError('Error parsing video. Unable to find file ID.')
+
+        api_url = base_url + self._ZOOM_API_TEMPLATE.format(file_id=file_id)
+
+        api_data = self._session_get_json(api_url)
 
-            title=initial_info.get('topic'),
+        if api_data.get('errorCode') != 0:
+            raise ZoomError(
+                f'An error occured: {api_data.get("errorMessage")} ({api_data.get("errorCode")})')
+
+        result = api_data.get('result')
+        if not result:
+            raise ZoomError(
+                f'Unable to find chat messages for video {video_id}')
+
+        chat_messages = result.get('meetingChatList') or []
+        title = multi_get(result, 'meet', 'topic')
+        return Chat(
+            self._get_chat_messages(chat_messages, params),
+            title=title,
             video_type=video_type,
-            start_time=initial_info.get('fileStartTime'),
-            id=initial_info.get('recordingId'),
+            start_time=result.get('fileStartTime'),
+            id=video_id,
+            duration=result.get('duration'),
         )
 
     def _parse_js_dict(self, json_string):
         # Helper method to parse JS dictionary format
         result = re.sub(r"^([^:\s]+):\s+", r'"\g<1>": ',
                         json_string, 0, re.MULTILINE)
         result = result.replace(r"\'", "'")
         result = re.sub(r":\s+'(.*)'", ": \"\\g<1>\"", result, 0, re.MULTILINE)
         return json.loads(result)
 
-    def _get_chat_messages(self, page_data, params):
+    def _get_chat_messages(self, messages, params):
         start_time = ensure_seconds(params.get('start_time'), 0)
         end_time = ensure_seconds(params.get('end_time'), float('inf'))
 
-        for item in re.findall(self._CHAT_MESSAGES_REGEX, page_data):
-            data = self._parse_js_dict(item)
+        for data in messages:
             data = r.remap_dict(data, self._REMAPPING)
 
             # Process time inforamtion
             data['time_in_seconds'] = time_to_seconds(data['time_text'])
             if data['time_in_seconds'] < start_time:
                 continue
```

### Comparing `chat-downloader-0.2.4/chat_downloader/utils/core.py` & `chat-downloader-0.2.5/chat_downloader/utils/core.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader/utils/timed_utils.py` & `chat-downloader-0.2.5/chat_downloader/utils/timed_utils.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/chat_downloader.egg-info/PKG-INFO` & `chat-downloader-0.2.5/chat_downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-downloader
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple tool used to retrieve chat messages from livestreams, videos, clips and past broadcasts. No authentication needed!
 Home-page: https://github.com/xenova/chat-downloader
 Author: xenova
 Author-email: admin@xenova.com
 License: MIT license
 Keywords: python chat downloader youtube twitch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chat-downloader-0.2.4/chat_downloader.egg-info/SOURCES.txt` & `chat-downloader-0.2.5/chat_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/Makefile` & `chat-downloader-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/README.rst` & `chat-downloader-0.2.5/docs/README.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/changelog.rst` & `chat-downloader-0.2.5/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/cli.rst` & `chat-downloader-0.2.5/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/conf.py` & `chat-downloader-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/contributing.rst` & `chat-downloader-0.2.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/items.rst` & `chat-downloader-0.2.5/docs/items.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/options.rst` & `chat-downloader-0.2.5/docs/options.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/source/chat_downloader.rst` & `chat-downloader-0.2.5/docs/source/chat_downloader.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/docs/source/sites.rst` & `chat-downloader-0.2.5/docs/source/sites.rst`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/setup.py` & `chat-downloader-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/tests/other youtube actions` & `chat-downloader-0.2.5/tests/other youtube actions`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/tests/test_chat_downloader.py` & `chat-downloader-0.2.5/tests/test_chat_downloader.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/tests/test_formatting.py` & `chat-downloader-0.2.5/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/tests/test_generators.py` & `chat-downloader-0.2.5/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/tests/test_init_params.py` & `chat-downloader-0.2.5/tests/test_init_params.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/tests/test_sites.py` & `chat-downloader-0.2.5/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/tests/test_utils.py` & `chat-downloader-0.2.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/tests/test_writers.py` & `chat-downloader-0.2.5/tests/test_writers.py`

 * *Files identical despite different names*

### Comparing `chat-downloader-0.2.4/tests/youtube_actions.json` & `chat-downloader-0.2.5/tests/youtube_actions.json`

 * *Files identical despite different names*

