# Comparing `tmp/codefast-23.5.4.16.tar.gz` & `tmp/codefast-23.5.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefast-23.5.4.16.tar", last modified: Thu May  4 16:28:06 2023, max compression
+gzip compressed data, was "dist/codefast-23.5.5.11.tar", last modified: Fri May  5 03:21:24 2023, max compression
```

## Comparing `codefast-23.5.4.16.tar` & `codefast-23.5.5.11.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-04 16:27:53.000000 codefast-23.5.4.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 16:28:06.310782 codefast-23.5.4.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-04 16:27:53.000000 codefast-23.5.4.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/asyncio/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/asyncio/rabbitmq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/axe/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/axe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/axe/axe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/axe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/base/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/base/format_print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/betterargs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/betterargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/betterargs/abstractclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/cn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/concurrency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/concurrent/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/concurrent/fastapi_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/concurrent/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/decorators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/decorators/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2886 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/ds.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/experimental/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/experimental/nsq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/fio/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/fio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/fio/ffpb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/functools/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/functools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/functools/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/functools/subroutine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/io/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3328 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/dblite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/osdb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3857 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/network/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/curl.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/richdownloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1223 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/factory_method.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3320 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/responsibility_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/supercell/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/supercell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/types/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 16:28:05.000000 codefast-23.5.4.16/codefast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-04 16:28:06.000000 codefast-23.5.4.16/codefast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:28:05.000000 codefast-23.5.4.16/codefast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 16:28:05.000000 codefast-23.5.4.16/codefast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 16:28:05.000000 codefast-23.5.4.16/codefast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:28:06.310782 codefast-23.5.4.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-04 16:27:53.000000 codefast-23.5.4.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:27:53.000000 codefast-23.5.4.16/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 16:27:53.000000 codefast-23.5.4.16/tests/test_unique_session.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.904297 codefast-23.5.5.11/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1074 2021-08-14 02:45:04.000000 codefast-23.5.5.11/LICENSE
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1485 2023-05-05 03:21:24.904297 codefast-23.5.5.11/PKG-INFO
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1115 2021-08-14 02:45:04.000000 codefast-23.5.5.11/README.md
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.896297 codefast-23.5.5.11/codefast/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1605 2023-04-08 02:18:46.000000 codefast-23.5.5.11/codefast/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6075 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/argparser.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/asyncio/
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1368 2023-04-19 05:45:01.000000 codefast-23.5.5.11/codefast/asyncio/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1777 2023-05-04 16:26:49.000000 codefast-23.5.5.11/codefast/asyncio/rabbitmq.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/axe/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       34 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/axe/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2232 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/axe/axe.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1029 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/axe.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/base/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       31 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/base/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3880 2022-12-25 13:22:03.000000 codefast-23.5.5.11/codefast/base/format_print.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/betterargs/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       71 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/betterargs/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4719 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/betterargs/abstractclient.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      692 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/cn.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2646 2022-11-19 16:15:49.000000 codefast-23.5.5.11/codefast/concurrency.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/concurrent/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/concurrent/__init__.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2891 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/concurrent/fastapi_demo.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4328 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/concurrent/scheduler.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2108 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/constants.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      592 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/core.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/decorators/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3105 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/decorators/__init__.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)      440 2022-12-15 06:35:33.000000 codefast-23.5.5.11/codefast/decorators/log.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2886 2023-04-28 12:37:33.000000 codefast-23.5.5.11/codefast/decorators/retry.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)    11928 2023-01-09 08:00:38.000000 codefast-23.5.5.11/codefast/ds.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      112 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/exception.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/experimental/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2023-01-10 00:15:53.000000 codefast-23.5.5.11/codefast/experimental/__init__.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)      581 2023-01-10 02:42:34.000000 codefast-23.5.5.11/codefast/experimental/nsq.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/fio/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       23 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/fio/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     5951 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/fio/ffpb.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/frameworks/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1103 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/frameworks/__init__.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/functools/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       75 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/functools/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      485 2023-01-02 02:54:54.000000 codefast-23.5.5.11/codefast/functools/random.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1042 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/functools/subroutine.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/io/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      174 2023-02-05 03:01:40.000000 codefast-23.5.5.11/codefast/io/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3773 2023-03-29 03:50:19.000000 codefast-23.5.5.11/codefast/io/_json.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3328 2022-12-04 12:10:17.000000 codefast-23.5.5.11/codefast/io/dblite.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     7818 2023-03-29 13:37:50.000000 codefast-23.5.5.11/codefast/io/file.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     4411 2023-04-12 12:05:54.000000 codefast-23.5.5.11/codefast/io/osdb.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3857 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/io/sqlite.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3310 2022-12-28 09:45:27.000000 codefast-23.5.5.11/codefast/logger.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      716 2023-04-07 06:17:01.000000 codefast-23.5.5.11/codefast/math.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/network/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      135 2023-04-07 06:18:56.000000 codefast-23.5.5.11/codefast/network/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1213 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/network/curl.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      587 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/network/factory.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2681 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/network/richdownloader.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3778 2023-04-07 06:18:28.000000 codefast-23.5.5.11/codefast/network/tools.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/patterns/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       70 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/patterns/__init__.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1223 2022-12-10 01:39:19.000000 codefast-23.5.5.11/codefast/patterns/factory_method.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3320 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/patterns/observer.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1844 2023-04-12 13:39:31.000000 codefast-23.5.5.11/codefast/patterns/pipeline.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      773 2022-12-27 13:57:07.000000 codefast-23.5.5.11/codefast/patterns/responsibility_chain.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      395 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/patterns/singleton.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1303 2022-12-15 06:38:07.000000 codefast-23.5.5.11/codefast/reader.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/supercell/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       21 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/supercell/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      124 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/tmp.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/types/
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1064 2022-11-23 05:27:16.000000 codefast-23.5.5.11/codefast/types/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)    11921 2023-04-13 00:21:26.000000 codefast-23.5.5.11/codefast/utils.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast.egg-info/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1485 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/PKG-INFO
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1676 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       96 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/requires.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       15 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/top_level.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-05-05 03:21:24.904297 codefast-23.5.5.11/setup.cfg
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      878 2023-04-07 08:56:08.000000 codefast-23.5.5.11/setup.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/tests/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-04-18 12:52:35.000000 codefast-23.5.5.11/tests/__init__.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      825 2023-04-18 13:01:02.000000 codefast-23.5.5.11/tests/test_unique_session.py
```

### Comparing `codefast-23.5.4.16/LICENSE` & `codefast-23.5.5.11/LICENSE`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/README.md` & `codefast-23.5.5.11/README.md`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/__init__.py` & `codefast-23.5.5.11/codefast/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/argparser.py` & `codefast-23.5.5.11/codefast/argparser.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/asyncio/__init__.py` & `codefast-23.5.5.11/codefast/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/asyncio/rabbitmq.py` & `codefast-23.5.5.11/codefast/asyncio/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/axe/axe.py` & `codefast-23.5.5.11/codefast/axe/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/axe.py` & `codefast-23.5.5.11/codefast/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/base/format_print.py` & `codefast-23.5.5.11/codefast/base/format_print.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/betterargs/abstractclient.py` & `codefast-23.5.5.11/codefast/betterargs/abstractclient.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/cn.py` & `codefast-23.5.5.11/codefast/cn.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/concurrency.py` & `codefast-23.5.5.11/codefast/concurrency.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/concurrent/fastapi_demo.py` & `codefast-23.5.5.11/codefast/concurrent/fastapi_demo.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/concurrent/scheduler.py` & `codefast-23.5.5.11/codefast/concurrent/scheduler.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/constants.py` & `codefast-23.5.5.11/codefast/constants.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/core.py` & `codefast-23.5.5.11/codefast/core.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/decorators/__init__.py` & `codefast-23.5.5.11/codefast/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/decorators/retry.py` & `codefast-23.5.5.11/codefast/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/ds.py` & `codefast-23.5.5.11/codefast/ds.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/experimental/nsq.py` & `codefast-23.5.5.11/codefast/experimental/nsq.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/fio/ffpb.py` & `codefast-23.5.5.11/codefast/fio/ffpb.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/frameworks/__init__.py` & `codefast-23.5.5.11/codefast/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/functools/subroutine.py` & `codefast-23.5.5.11/codefast/functools/subroutine.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/io/_json.py` & `codefast-23.5.5.11/codefast/io/_json.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/io/dblite.py` & `codefast-23.5.5.11/codefast/io/dblite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/io/file.py` & `codefast-23.5.5.11/codefast/io/file.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/io/osdb.py` & `codefast-23.5.5.11/codefast/io/osdb.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/io/sqlite.py` & `codefast-23.5.5.11/codefast/io/sqlite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/logger.py` & `codefast-23.5.5.11/codefast/logger.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/math.py` & `codefast-23.5.5.11/codefast/math.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/network/curl.py` & `codefast-23.5.5.11/codefast/network/curl.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/network/factory.py` & `codefast-23.5.5.11/codefast/network/factory.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/network/richdownloader.py` & `codefast-23.5.5.11/codefast/network/richdownloader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/network/tools.py` & `codefast-23.5.5.11/codefast/network/tools.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/patterns/factory_method.py` & `codefast-23.5.5.11/codefast/patterns/factory_method.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/patterns/observer.py` & `codefast-23.5.5.11/codefast/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/patterns/pipeline.py` & `codefast-23.5.5.11/codefast/patterns/pipeline.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/patterns/responsibility_chain.py` & `codefast-23.5.5.11/codefast/patterns/responsibility_chain.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/reader.py` & `codefast-23.5.5.11/codefast/reader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/types/__init__.py` & `codefast-23.5.5.11/codefast/types/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast/utils.py` & `codefast-23.5.5.11/codefast/utils.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/codefast.egg-info/SOURCES.txt` & `codefast-23.5.5.11/codefast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/setup.py` & `codefast-23.5.5.11/setup.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.4.16/tests/test_unique_session.py` & `codefast-23.5.5.11/tests/test_unique_session.py`

 * *Files identical despite different names*

