# Comparing `tmp/uphill-0.1.1.1.tar.gz` & `tmp/uphill-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uphill-0.1.1.1.tar", last modified: Fri May  5 09:45:11 2023, max compression
+gzip compressed data, was "uphill-0.1.2.tar", last modified: Fri May  5 11:07:45 2023, max compression
```

## Comparing `uphill-0.1.1.1.tar` & `uphill-0.1.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/
--rw-rw-r--   0 root         (0) root         (0)      164 2023-04-28 07:46:55.000000 uphill-0.1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-05 09:45:11.395990 uphill-0.1.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1436 2023-05-04 11:27:36.000000 uphill-0.1.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      158 2023-03-22 13:11:45.000000 uphill-0.1.1.1/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)      149 2023-05-05 09:45:11.395990 uphill-0.1.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2035 2023-03-22 08:56:54.000000 uphill-0.1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.391990 uphill-0.1.1.1/uphill/
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 09:44:01.000000 uphill-0.1.1.1/uphill/VERSION
--rw-r--r--   0 root         (0) root         (0)     1141 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/apply/
--rw-r--r--   0 root         (0) root         (0)       66 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/apply/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6283 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/apply/aishell.py
--rw-r--r--   0 root         (0) root         (0)     5431 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/apply/aishell2.py
--rw-r--r--   0 root         (0) root         (0)     3091 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/apply/musan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/array/
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/array/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20668 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/array/document_array.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/array/mixins/
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/array/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4797 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/array/mixins/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/array/mixins/auto_compress.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/array/mixins/serialization.py
--rw-r--r--   0 root         (0) root         (0)     5842 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/array/supervision_array.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/bin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/bin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/bin/download.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/bin/main.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/bin/parser.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-04 08:56:07.000000 uphill-0.1.1.1/uphill/bin/parser_base.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/bin/prepare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/core/audio/
--rw-r--r--   0 root         (0) root         (0)      597 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/audio/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10373 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/audio/augment.py
--rw-r--r--   0 root         (0) root         (0)     8468 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/audio/io.py
--rw-r--r--   0 root         (0) root         (0)    11152 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/audio/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/core/text/
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/text/__init__.py
--rw-r--r--   0 root         (0) root         (0)  2509660 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/text/lang.model
--rw-r--r--   0 root         (0) root         (0)     9838 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/text/own_langid.py
--rw-r--r--   0 root         (0) root         (0)     2899 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/text/utils.py
--rw-r--r--   0 root         (0) root         (0)    12582 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/text/vocab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/core/utils/
--rw-r--r--   0 root         (0) root         (0)      963 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/utils/constant.py
--rw-r--r--   0 root         (0) root         (0)     2757 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/utils/download.py
--rw-r--r--   0 root         (0) root         (0)    16263 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     4070 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/utils/module.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/utils/parallel.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/core/utils/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/document/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/document/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26028 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/document/document.py
--rw-r--r--   0 root         (0) root         (0)     2745 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/document/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill/document/mixins/
--rw-r--r--   0 root         (0) root         (0)      261 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/document/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/document/mixins/internal.py
--rw-r--r--   0 root         (0) root         (0)     2336 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/document/mixins/plot.py
--rw-r--r--   0 root         (0) root         (0)     1289 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/document/mixins/serialization.py
--rw-r--r--   0 root         (0) root         (0)    19783 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/document/source.py
--rw-r--r--   0 root         (0) root         (0)     2130 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/document/supervision.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/errors.py
--rw-r--r--   0 root         (0) root         (0)     6211 2023-04-27 12:32:00.000000 uphill-0.1.1.1/uphill/logx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:45:11.395990 uphill-0.1.1.1/uphill.egg-info/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-05 09:45:11.000000 uphill-0.1.1.1/uphill.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1546 2023-05-05 09:45:11.000000 uphill-0.1.1.1/uphill.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 09:45:11.000000 uphill-0.1.1.1/uphill.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-05 09:45:11.000000 uphill-0.1.1.1/uphill.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-05 09:45:11.000000 uphill-0.1.1.1/uphill.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 09:45:11.000000 uphill-0.1.1.1/uphill.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.530447 uphill-0.1.2/
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-04-28 07:46:55.000000 uphill-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      628 2023-05-05 11:07:45.530447 uphill-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1436 2023-05-04 11:27:36.000000 uphill-0.1.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-03-22 13:11:45.000000 uphill-0.1.2/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      149 2023-05-05 11:07:45.530447 uphill-0.1.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2035 2023-03-22 08:56:54.000000 uphill-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.526447 uphill-0.1.2/uphill/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/VERSION
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.526447 uphill-0.1.2/uphill/apply/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/apply/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6283 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/apply/aishell.py
+-rw-r--r--   0 root         (0) root         (0)     5431 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/apply/aishell2.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/apply/musan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.526447 uphill-0.1.2/uphill/array/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/array/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20668 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/array/document_array.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.526447 uphill-0.1.2/uphill/array/mixins/
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/array/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/array/mixins/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/array/mixins/auto_compress.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-05-05 11:03:33.000000 uphill-0.1.2/uphill/array/mixins/serialization.py
+-rw-r--r--   0 root         (0) root         (0)     5842 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/array/supervision_array.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.526447 uphill-0.1.2/uphill/bin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/bin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/bin/download.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/bin/main.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/bin/parser.py
+-rw-r--r--   0 root         (0) root         (0)      842 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/bin/parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/bin/prepare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.526447 uphill-0.1.2/uphill/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.530447 uphill-0.1.2/uphill/core/audio/
+-rw-r--r--   0 root         (0) root         (0)      597 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/audio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10373 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/audio/augment.py
+-rw-r--r--   0 root         (0) root         (0)     8468 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/audio/io.py
+-rw-r--r--   0 root         (0) root         (0)    11152 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/audio/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.530447 uphill-0.1.2/uphill/core/text/
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2509660 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/text/lang.model
+-rw-r--r--   0 root         (0) root         (0)     9838 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/text/own_langid.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/text/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12582 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/text/vocab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.530447 uphill-0.1.2/uphill/core/utils/
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/utils/constant.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/utils/download.py
+-rw-r--r--   0 root         (0) root         (0)    16263 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     4070 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/utils/module.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/utils/parallel.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/core/utils/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.530447 uphill-0.1.2/uphill/document/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/document/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26028 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/document/document.py
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/document/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.530447 uphill-0.1.2/uphill/document/mixins/
+-rw-r--r--   0 root         (0) root         (0)      261 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/document/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/document/mixins/internal.py
+-rw-r--r--   0 root         (0) root         (0)     2336 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/document/mixins/plot.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/document/mixins/serialization.py
+-rw-r--r--   0 root         (0) root         (0)    19783 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/document/source.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/document/supervision.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-05-05 11:03:09.000000 uphill-0.1.2/uphill/logx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:07:45.526447 uphill-0.1.2/uphill.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      628 2023-05-05 11:07:45.000000 uphill-0.1.2/uphill.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-05-05 11:07:45.000000 uphill-0.1.2/uphill.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 11:07:45.000000 uphill-0.1.2/uphill.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-05 11:07:45.000000 uphill-0.1.2/uphill.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-05 11:07:45.000000 uphill-0.1.2/uphill.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 11:07:45.000000 uphill-0.1.2/uphill.egg-info/top_level.txt
```

### Comparing `uphill-0.1.1.1/PKG-INFO` & `uphill-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uphill
-Version: 0.1.1.1
+Version: 0.1.2
 Summary: make data preparation more friendly
 Home-page: https://github.com/yinanxu0/uphill
 Author: yinanxu
 Author-email: yinanxu0@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `uphill-0.1.1.1/README.md` & `uphill-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/setup.py` & `uphill-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/__init__.py` & `uphill-0.1.2/uphill/__init__.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/apply/aishell.py` & `uphill-0.1.2/uphill/apply/aishell.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/apply/aishell2.py` & `uphill-0.1.2/uphill/apply/aishell2.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/apply/musan.py` & `uphill-0.1.2/uphill/apply/musan.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/array/document_array.py` & `uphill-0.1.2/uphill/array/document_array.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/array/mixins/algorithm.py` & `uphill-0.1.2/uphill/array/mixins/algorithm.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/array/mixins/auto_compress.py` & `uphill-0.1.2/uphill/array/mixins/auto_compress.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/array/mixins/serialization.py` & `uphill-0.1.2/uphill/array/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/array/supervision_array.py` & `uphill-0.1.2/uphill/array/supervision_array.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/bin/download.py` & `uphill-0.1.2/uphill/bin/download.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/bin/main.py` & `uphill-0.1.2/uphill/bin/main.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/bin/parser.py` & `uphill-0.1.2/uphill/bin/parser.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/bin/parser_base.py` & `uphill-0.1.2/uphill/bin/parser_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 def add_arg_group(parser, title):
     return parser.add_argument_group(title)
 
 
 def set_base_parser():
     parser = argparse.ArgumentParser(
-        epilog='%s, a toolkit to process dataset easily. '
+        epilog='%s, a toolkit based on pytorch. '
         'Visit %s for tutorials and documents.' % (
             colored('uphill v%s' % __version__, 'green'),
             colored(
                 'https://github.com/yinanxu0/uphill',
                 'cyan',
                 attrs=['underline'],
             ),
         ),
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        description='Uphill Line Interface',
+        description='MountainTop Line Interface',
     )
 
     parser.add_argument(
         '-v',
         '--version',
         action='version',
         version=__version__,
```

### Comparing `uphill-0.1.1.1/uphill/bin/prepare.py` & `uphill-0.1.2/uphill/bin/prepare.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/audio/__init__.py` & `uphill-0.1.2/uphill/core/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/audio/augment.py` & `uphill-0.1.2/uphill/core/audio/augment.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/audio/io.py` & `uphill-0.1.2/uphill/core/audio/io.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/audio/utils.py` & `uphill-0.1.2/uphill/core/audio/utils.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/text/lang.model` & `uphill-0.1.2/uphill/core/text/lang.model`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/text/own_langid.py` & `uphill-0.1.2/uphill/core/text/own_langid.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/text/utils.py` & `uphill-0.1.2/uphill/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/text/vocab.py` & `uphill-0.1.2/uphill/core/text/vocab.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/utils/__init__.py` & `uphill-0.1.2/uphill/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/utils/download.py` & `uphill-0.1.2/uphill/core/utils/download.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/utils/io.py` & `uphill-0.1.2/uphill/core/utils/io.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/utils/module.py` & `uphill-0.1.2/uphill/core/utils/module.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/utils/parallel.py` & `uphill-0.1.2/uphill/core/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/utils/timing.py` & `uphill-0.1.2/uphill/core/utils/timing.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/core/utils/typing.py` & `uphill-0.1.2/uphill/core/utils/typing.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/document/document.py` & `uphill-0.1.2/uphill/document/document.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/document/helper.py` & `uphill-0.1.2/uphill/document/helper.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/document/mixins/internal.py` & `uphill-0.1.2/uphill/document/mixins/internal.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/document/mixins/plot.py` & `uphill-0.1.2/uphill/document/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/document/mixins/serialization.py` & `uphill-0.1.2/uphill/document/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/document/source.py` & `uphill-0.1.2/uphill/document/source.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/document/supervision.py` & `uphill-0.1.2/uphill/document/supervision.py`

 * *Files identical despite different names*

### Comparing `uphill-0.1.1.1/uphill/logx.py` & `uphill-0.1.2/uphill/logx.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 def get_logger(
     filepath: Optional[Union[Path, str]] = None,
     detail_level: int = 1
 ) -> logging.Logger:
     logger = logging.getLogger("uphill")
     logger.setLevel(logging.DEBUG)
+    # remove existed handler
+    if len(logger.handlers) > 0:
+        for handler in logger.handlers:
+            logger.removeHandler(handler)
     logger.addHandler(
         stream_handler(
             level=logging.INFO,
             detail_level=detail_level
         )
     )
     if filepath is not None:
@@ -91,102 +95,77 @@
 
 
 ###############
 # LoggerX
 ###############
 class LoggerX(object):
     def __init__(self):
-        self._initialized = False
         self.detail_level = int(os.environ.get("DETAIL_LEVEL", 1))
+        self.logger = get_logger(filepath=None, detail_level=self.detail_level)
 
     def initialize(
         self, 
         logdir: Optional[Union[str, Path]] = None, 
         to_file: bool = False, 
         detail_level: Optional[int] = None
     ):
         '''
         Initialize LoggerX
 
-        inputs
-        - logdir - where to write logfiles
-        - to_file - whether to write log to files
-        - debug - write full details to log record
+        params
+            - logdir - where to write logfiles
+            - to_file - whether to write log to files
+            - debug - write full details to log record
         '''
-        if self._initialized:
-            self.logger.warning(
-                "loggerx has been initialized, cannot initialize again", 
-                stacklevel=3
-            )
-            return
         self.detail_level = self.detail_level if detail_level is None else detail_level
         log_path = None
         if to_file:
             assert logdir is not None, "write to file but no place decleared, "\
                 "set `to_file` to False or set `logdir` a valid path"
             logdir = Path(logdir) if isinstance(logdir, str) else logdir
             # confirm target log directory exists
             if not logdir.exists():
                 logdir.mkdir(parents=True, exist_ok=True)
             from uphill.core.utils.timing import current_datetime
             log_path = logdir / f'uphill.{current_datetime()}.log'
         self.logger = get_logger(filepath=log_path, detail_level=self.detail_level)
-        self._initialized = True
 
     def __del__(self):
         return
 
-    def __check_msg(self, msg: Any=""):
+    def _check_msg(self, msg: Any=""):
         if msg is None or len(msg) == 0:
             self.logger.warning(
                 "empty message for logger is not recommended, skip", 
                 stacklevel=3
             )
             return False
         return True
     
-    def __check_initialized(self):
-        if not self._initialized:
-            print(
-                colored(
-                    "using loggerx before `initialize` is not recommended, "\
-                    "here initialize to console logger automatically",
-                    "red"
-                )
-            )
-            self.initialize()
-        return
-    
     #### logger functions
-    def debug(self, msg: Any="", *args, **kwargs):
-        self.__check_initialized()
-        if not self.__check_msg(msg):
+    def debug(self, msg: Any, stacklevel=2, *args, **kwargs):
+        if not self._check_msg(msg):
             return
-        self.logger.debug(msg, stacklevel=2, *args, **kwargs)
+        self.logger.debug(msg, stacklevel=stacklevel, *args, **kwargs)
     
-    def info(self, msg: Any="", *args, **kwargs):
-        self.__check_initialized()
-        if not self.__check_msg(msg):
+    def info(self, msg: Any, stacklevel=2, *args, **kwargs):
+        if not self._check_msg(msg):
             return
-        self.logger.info(msg, stacklevel=2, *args, **kwargs)
+        self.logger.info(msg, stacklevel=stacklevel, *args, **kwargs)
     
-    def warning(self, msg: Any="", *args, **kwargs):
-        self.__check_initialized()
-        if not self.__check_msg(msg):
+    def warning(self, msg: Any, stacklevel=2, *args, **kwargs):
+        if not self._check_msg(msg):
             return
-        self.logger.warning(msg, stacklevel=2, *args, **kwargs)
+        self.logger.warning(msg, stacklevel=stacklevel, *args, **kwargs)
     
-    def error(self, msg: Any="", *args, **kwargs):
-        self.__check_initialized()
-        if not self.__check_msg(msg):
+    def error(self, msg: Any, stacklevel=2, *args, **kwargs):
+        if not self._check_msg(msg):
             return
-        self.logger.error(msg, stacklevel=2, *args, **kwargs)
+        self.logger.error(msg, stacklevel=stacklevel, *args, **kwargs)
     
-    def critical(self, msg: Any="", *args, **kwargs):
-        self.__check_initialized()
-        if not self.__check_msg(msg):
+    def critical(self, msg: Any, stacklevel=2, *args, **kwargs):
+        if not self._check_msg(msg):
             return
-        self.logger.critical(msg, stacklevel=2, *args, **kwargs)
+        self.logger.critical(msg, stacklevel=stacklevel, *args, **kwargs)
 
 
-global loggerx 
 loggerx = LoggerX()
```

### Comparing `uphill-0.1.1.1/uphill.egg-info/PKG-INFO` & `uphill-0.1.2/uphill.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uphill
-Version: 0.1.1.1
+Version: 0.1.2
 Summary: make data preparation more friendly
 Home-page: https://github.com/yinanxu0/uphill
 Author: yinanxu
 Author-email: yinanxu0@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `uphill-0.1.1.1/uphill.egg-info/SOURCES.txt` & `uphill-0.1.2/uphill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

