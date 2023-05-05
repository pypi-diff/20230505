# Comparing `tmp/ayugespidertools-2.0.1.tar.gz` & `tmp/ayugespidertools-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-2.0.1.tar", max compression
+gzip compressed data, was "ayugespidertools-2.0.2.tar", max compression
```

## Comparing `ayugespidertools-2.0.1.tar` & `ayugespidertools-2.0.2.tar`

### file list

```diff
@@ -1,115 +1,117 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/LICENSE
--rw-r--r--   0        0        0    13798 2023-04-27 03:19:49.000000 ayugespidertools-2.0.1/README.md
--rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-2.0.1/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-2.0.1/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      158 2023-04-25 08:54:15.594268 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      536 2023-04-25 08:55:28.881319 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0      685 2023-04-25 08:54:15.595268 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
--rw-r--r--   0        0        0     2871 2023-04-27 08:04:48.083361 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
--rw-r--r--   0        0        0     1086 2023-04-25 08:54:15.618268 ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-2.0.1/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     4050 2023-04-27 07:39:48.000000 ayugespidertools-2.0.1/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-2.0.1/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-2.0.1/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-2.0.1/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     3858 2023-04-25 02:55:36.000000 ayugespidertools-2.0.1/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    11765 2023-04-27 08:36:37.000000 ayugespidertools-2.0.1/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    13474 2023-04-25 02:55:56.000000 ayugespidertools-2.0.1/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-2.0.1/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-2.0.1/ayugespidertools/common/spiderdbconf.py
--rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-2.0.1/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-2.0.1/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    11325 2023-04-26 08:38:41.000000 ayugespidertools-2.0.1/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-2.0.1/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-2.0.1/ayugespidertools/config.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-2.0.1/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-2.0.1/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-2.0.1/ayugespidertools/items.py
--rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-2.0.1/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-2.0.1/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-2.0.1/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-2.0.1/ayugespidertools/oss.py
--rw-r--r--   0        0        0      694 2023-02-17 07:53:37.000000 ayugespidertools-2.0.1/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/processmanager.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-2.0.1/ayugespidertools/request.py
--rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-2.0.1/ayugespidertools/rpa.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/runjs.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0      356 2023-04-26 08:48:02.859698 ayugespidertools-2.0.1/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-25 08:54:13.045266 ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1068 2023-04-27 08:45:17.819120 ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0      981 2023-04-25 08:58:10.179432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-04-25 08:58:10.180432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
--rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0      475 2023-04-25 08:58:10.180432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7677 2023-04-27 07:35:53.380544 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc
--rw-r--r--   0        0        0     2200 2023-04-25 08:58:10.182432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
--rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0      481 2023-04-25 08:58:10.183432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3911 2023-04-25 08:58:10.184432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
--rw-r--r--   0        0        0     3056 2023-04-26 08:48:05.030700 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
--rw-r--r--   0        0        0     7795 2023-04-25 08:58:10.186432 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
--rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      885 2023-04-25 08:58:19.202438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0      173 2023-04-25 08:58:19.202438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3093 2023-04-25 08:58:19.203438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1820 2023-04-25 08:58:19.205438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     3022 2023-04-25 03:00:27.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1356 2023-04-25 03:00:42.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0    13396 2023-04-25 03:01:05.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0    11209 2023-04-25 08:58:19.207438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3005 2023-04-25 08:58:19.211438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
--rw-r--r--   0        0        0      717 2023-04-25 08:58:19.219438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1998 2023-04-25 08:58:19.220438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-04-25 08:58:19.223438 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     2824 2023-04-25 03:01:16.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2840 2023-04-25 03:01:31.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3794 2023-04-25 03:02:20.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     6737 2023-04-25 03:02:38.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0     4569 2023-04-25 08:54:13.141266 ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      760 2023-04-25 08:54:14.345267 ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-2.0.1/ayugespidertools/spiders.py
--rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/.gitignore
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      613 2023-04-25 05:46:03.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     4093 2023-04-25 04:01:51.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-2.0.1/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6409 2023-04-25 08:46:25.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1941 2023-04-25 08:47:57.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-2.0.1/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.1/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0      155 2023-04-25 08:55:31.774321 ayugespidertools-2.0.1/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5327 2023-04-27 08:04:47.882360 ayugespidertools-2.0.1/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
--rw-r--r--   0        0        0     5920 2023-04-27 07:40:39.000000 ayugespidertools-2.0.1/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-2.0.1/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     3004 2023-04-26 09:50:14.000000 ayugespidertools-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    15467 1970-01-01 00:00:00.000000 ayugespidertools-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/LICENSE
+-rw-r--r--   0        0        0    13798 2023-04-27 03:19:49.000000 ayugespidertools-2.0.2/README.md
+-rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-2.0.2/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-2.0.2/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-25 08:54:15.594268 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      536 2023-04-25 08:55:28.881319 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0      685 2023-04-25 08:54:15.595268 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
+-rw-r--r--   0        0        0     2871 2023-04-27 08:04:48.083361 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
+-rw-r--r--   0        0        0     1086 2023-04-25 08:54:15.618268 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-2.0.2/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     4050 2023-04-27 07:39:48.000000 ayugespidertools-2.0.2/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-2.0.2/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-2.0.2/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-2.0.2/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     6885 2023-05-05 06:09:23.000000 ayugespidertools-2.0.2/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    11765 2023-04-27 08:36:37.000000 ayugespidertools-2.0.2/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    13474 2023-04-25 02:55:56.000000 ayugespidertools-2.0.2/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-2.0.2/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-2.0.2/ayugespidertools/common/spiderdbconf.py
+-rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-2.0.2/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-2.0.2/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    11325 2023-04-26 08:38:41.000000 ayugespidertools-2.0.2/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-2.0.2/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-2.0.2/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-2.0.2/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-2.0.2/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-2.0.2/ayugespidertools/items.py
+-rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-2.0.2/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-2.0.2/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-2.0.2/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-2.0.2/ayugespidertools/oss.py
+-rw-r--r--   0        0        0      802 2023-05-04 09:14:56.000000 ayugespidertools-2.0.2/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/processmanager.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-2.0.2/ayugespidertools/request.py
+-rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-2.0.2/ayugespidertools/rpa.py
+-rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/runjs.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0      356 2023-04-26 08:48:02.859698 ayugespidertools-2.0.2/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1442 2023-04-25 08:54:13.045266 ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1068 2023-04-27 08:45:17.819120 ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-25 08:58:10.179432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-04-25 08:58:10.180432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
+-rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-25 08:58:10.180432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7677 2023-04-27 07:35:53.380544 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc
+-rw-r--r--   0        0        0     2200 2023-04-25 08:58:10.182432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
+-rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/requestslib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0      481 2023-04-25 08:58:10.183432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3911 2023-04-25 08:58:10.184432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
+-rw-r--r--   0        0        0     3056 2023-04-26 08:48:05.030700 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
+-rw-r--r--   0        0        0     7795 2023-04-25 08:58:10.186432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
+-rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-25 08:58:19.202438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-25 08:58:19.202438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2624 2023-05-05 08:55:33.703084 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc
+-rw-r--r--   0        0        0     2971 2023-05-05 08:55:33.673084 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1820 2023-04-25 08:58:19.205438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     2114 2023-05-05 07:48:47.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2872 2023-05-04 09:09:37.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1356 2023-04-25 03:00:42.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0    13396 2023-04-25 03:01:05.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0    11209 2023-04-25 08:58:19.207438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4019 2023-05-05 08:55:33.680084 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
+-rw-r--r--   0        0        0      717 2023-04-25 08:58:19.219438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1998 2023-05-04 07:33:52.883359 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-04-25 08:58:19.223438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     4379 2023-05-05 08:25:40.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3794 2023-04-25 03:02:20.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     6737 2023-04-25 03:02:38.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     4569 2023-04-25 08:54:13.141266 ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      760 2023-04-25 08:54:14.345267 ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-2.0.2/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/.gitignore
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      613 2023-04-25 05:46:03.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     4093 2023-04-25 04:01:51.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     6409 2023-04-25 08:46:25.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1941 2023-04-25 08:47:57.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-25 08:55:31.774321 ayugespidertools-2.0.2/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5327 2023-04-27 08:04:47.882360 ayugespidertools-2.0.2/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
+-rw-r--r--   0        0        0     5920 2023-04-27 07:40:39.000000 ayugespidertools-2.0.2/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-2.0.2/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     3021 2023-05-05 09:31:16.000000 ayugespidertools-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    15498 1970-01-01 00:00:00.000000 ayugespidertools-2.0.2/PKG-INFO
```

### Comparing `ayugespidertools-2.0.1/LICENSE` & `ayugespidertools-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/README.md` & `ayugespidertools-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/commands/__pycache__/version.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/version.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/commands/startproject.py` & `ayugespidertools-2.0.2/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/commands/version.py` & `ayugespidertools-2.0.2/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/encryption.py` & `ayugespidertools-2.0.2/ayugespidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/expend.py` & `ayugespidertools-2.0.2/ayugespidertools/common/expend.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/multiplexing.py` & `ayugespidertools-2.0.2/ayugespidertools/common/multiplexing.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-2.0.2/ayugespidertools/common/mysqlerrhandle.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/params.py` & `ayugespidertools-2.0.2/ayugespidertools/common/params.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/spiderdbconf.py` & `ayugespidertools-2.0.2/ayugespidertools/common/spiderdbconf.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/sqlformat.py` & `ayugespidertools-2.0.2/ayugespidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/typevars.py` & `ayugespidertools-2.0.2/ayugespidertools/common/typevars.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/utils.py` & `ayugespidertools-2.0.2/ayugespidertools/common/utils.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/common/yidungap.py` & `ayugespidertools-2.0.2/ayugespidertools/common/yidungap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/formatdata.py` & `ayugespidertools-2.0.2/ayugespidertools/formatdata.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/imgoperation.py` & `ayugespidertools-2.0.2/ayugespidertools/imgoperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/items.py` & `ayugespidertools-2.0.2/ayugespidertools/items.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/middlewares.py` & `ayugespidertools-2.0.2/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/mongoclient.py` & `ayugespidertools-2.0.2/ayugespidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/mysqlclient.py` & `ayugespidertools-2.0.2/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/oss.py` & `ayugespidertools-2.0.2/ayugespidertools/oss.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/pipelines.py` & `ayugespidertools-2.0.2/ayugespidertools/pipelines.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from ayugespidertools.scraper.pipelines.mongo.asynced import AsyncMongoPipeline
 from ayugespidertools.scraper.pipelines.mongo.fantasy import AyuFtyMongoPipeline
 from ayugespidertools.scraper.pipelines.mongo.twisted import AyuTwistedMongoPipeline
 from ayugespidertools.scraper.pipelines.mysql.asynced import AsyncMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.fantasy import AyuFtyMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.turbo import AyuTurboMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.twisted import AyuTwistedMysqlPipeline
 
 __all__ = [
     "AyuFtyMysqlPipeline",
     "AyuTurboMysqlPipeline",
     "AyuTwistedMysqlPipeline",
+    "AsyncMongoPipeline",
     "AsyncMysqlPipeline",
     "AyuFtyMongoPipeline",
     "AyuTwistedMongoPipeline",
 ]
```

### Comparing `ayugespidertools-2.0.1/ayugespidertools/rpa.py` & `ayugespidertools-2.0.2/ayugespidertools/rpa.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/runjs.py` & `ayugespidertools-2.0.2/ayugespidertools/runjs.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/netlib/requestslib.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/requestslib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 25 03:00:27 2023 UTC, .py size: 3022 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,194 +1,186 @@
-00000000: 550d 0d0a 0000 0000 4b42 4764 ce0b 0000  U.......KBGd....
+00000000: 550d 0d0a 0000 0000 5176 5364 380b 0000  U.......QvSd8...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
-00000070: 6701 5a0b 4700 6407 6406 8400 6406 650a  g.Z.G.d.d...d.e.
-00000080: 8303 5a0c 6408 5300 2909 e900 0000 0029  ..Z.d.S.)......)
-00000090: 01da 084f 7074 696f 6e61 6c29 02da 0b53  ...Optional)...S
-000000a0: 796e 6368 726f 6e69 7a65 da0c 6d6f 6e67  ynchronize..mong
-000000b0: 6f64 625f 7069 7065 2901 da0d 4d6f 6e67  odb_pipe)...Mong
-000000c0: 6f44 4243 6f6e 6669 6729 01da 0b54 6f6f  oDBConfig)...Too
-000000d0: 6c73 466f 7241 7975 2901 da0b 4d6f 6e67  lsForAyu)...Mong
-000000e0: 6f44 6242 6173 65da 1341 7975 4674 794d  oDbBase..AyuFtyM
-000000f0: 6f6e 676f 5069 7065 6c69 6e65 6300 0000  ongoPipelinec...
-00000100: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00000110: 0000 0000 0073 4e00 0000 6500 5a01 6400  .....sN...e.Z.d.
-00000120: 5a02 6401 5a03 640f 6504 6403 6404 9c02  Z.d.Z.d.e.d.d...
-00000130: 6405 6406 8405 5a05 6506 6407 6408 8400  d.d...Z.e.d.d...
-00000140: 8301 5a07 8700 6601 6409 640a 8408 5a08  ..Z...f.d.d...Z.
-00000150: 640b 640c 8400 5a09 640d 640e 8400 5a0a  d.d...Z.d.d...Z.
-00000160: 8700 0400 5a0b 5300 2910 7208 0000 0075  ....Z.S.).r....u
-00000170: 3800 0000 0a20 2020 204d 6f6e 676f 4442  8....    MongoDB
-00000180: 20e5 ad98 e582 a8e5 9cba e699 afe7 9a84   ...............
-00000190: 2073 6372 6170 7920 7069 7065 6c69 6e65   scrapy pipeline
-000001a0: 20e6 89a9 e5b1 950a 2020 2020 da00 4e29   .......    ..N)
-000001b0: 02da 1163 6f6c 6c65 6374 696f 6e5f 7072  ...collection_pr
-000001c0: 6566 6978 da06 7265 7475 726e 6302 0000  efix..returnc...
-000001d0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-000001e0: 0043 0000 0073 3200 0000 7400 7c01 7401  .C...s2...t.|.t.
-000001f0: 8302 7312 7402 6401 8301 8201 7c01 7018  ..s.t.d.....|.p.
-00000200: 6402 7c00 5f03 6403 7c00 5f04 6403 7c00  d.|._.d.|._.d.|.
-00000210: 5f05 6403 7c00 5f06 6403 5300 2904 75ab  _.d.|._.d.S.).u.
-00000220: 0000 000a 2020 2020 2020 2020 e588 9de5  ....        ....
-00000230: a78b e58c 960a 2020 2020 2020 2020 4172  ......        Ar
-00000240: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00000250: 6d6f 6e67 6f64 625f 636f 6e66 3a20 6d6f  mongodb_conf: mo
-00000260: 6e67 4442 20e7 9a84 e8bf 9ee6 8ea5 e985  ngDB ...........
-00000270: 8de7 bdae 0a20 2020 2020 2020 2020 2020  .....           
-00000280: 2063 6f6c 6c65 6374 696f 6e5f 7072 6566   collection_pref
-00000290: 6978 3a20 6d6f 6e67 4442 20e5 ad98 e582  ix: mongDB .....
-000002a0: a8e9 9b86 e590 88e7 9a84 e589 8de7 bc80  ................
-000002b0: efbc 8ce9 bb98 e8ae a4e4 b8ba e7a9 bae5  ................
-000002c0: ad97 e7ac a60a 2020 2020 2020 2020 7540  ......        u@
-000002d0: 0000 006d 6f6e 676f 4442 20e6 8980 e8a6  ...mongoDB .....
-000002e0: 81e5 ad98 e582 a8e7 9a84 e99b 86e5 9088  ................
-000002f0: e589 8de7 bc80 e590 8de7 a7b0 e99c 80e8  ................
-00000300: a681 e698 af20 7374 7220 e6a0 bce5 bc8f  ..... str ......
-00000310: efbc 8172 0900 0000 4e29 07da 0a69 7369  ...r....N)...isi
-00000320: 6e73 7461 6e63 65da 0373 7472 da0e 4173  nstance..str..As
-00000330: 7365 7274 696f 6e45 7272 6f72 720a 0000  sertionErrorr...
-00000340: 00da 0c6d 6f6e 676f 6462 5f63 6f6e 66da  ...mongodb_conf.
-00000350: 0463 6f6e 6eda 0264 6229 02da 0473 656c  .conn..db)...sel
-00000360: 6672 0a00 0000 a900 7213 0000 00fa 512f  fr......r.....Q/
-00000370: 726f 6f74 2f6d 7970 726f 6a2f 4179 7567  root/myproj/Ayug
-00000380: 6553 7069 6465 7254 6f6f 6c73 2f61 7975  eSpiderTools/ayu
-00000390: 6765 7370 6964 6572 746f 6f6c 732f 7363  gespidertools/sc
-000003a0: 7261 7065 722f 7069 7065 6c69 6e65 732f  raper/pipelines/
-000003b0: 6d6f 6e67 6f2f 6661 6e74 6173 792e 7079  mongo/fantasy.py
-000003c0: da08 5f5f 696e 6974 5f5f 1200 0000 730a  ..__init__....s.
-000003d0: 0000 0000 0a12 020a 0106 0206 017a 1c41  .............z.A
-000003e0: 7975 4674 794d 6f6e 676f 5069 7065 6c69  yuFtyMongoPipeli
-000003f0: 6e65 2e5f 5f69 6e69 745f 5f63 0200 0000  ne.__init__c....
-00000400: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000410: 4300 0000 7314 0000 007c 007c 016a 00a0  C...s....|.|.j..
-00000420: 0164 0164 02a1 0264 038d 0153 0029 044e  .d.d...d...S.).N
-00000430: 5a19 4d4f 4e47 4f44 425f 434f 4c4c 4543  Z.MONGODB_COLLEC
-00000440: 5449 4f4e 5f50 5245 4649 5872 0900 0000  TION_PREFIXr....
-00000450: 2901 720a 0000 0029 02da 0873 6574 7469  ).r....)...setti
-00000460: 6e67 73da 0367 6574 2902 da03 636c 73da  ngs..get)...cls.
-00000470: 0763 7261 776c 6572 7213 0000 0072 1300  .crawlerr....r..
-00000480: 0000 7214 0000 00da 0c66 726f 6d5f 6372  ..r......from_cr
-00000490: 6177 6c65 7224 0000 0073 0600 0000 0002  awler$...s......
-000004a0: 0201 0cff 7a20 4179 7546 7479 4d6f 6e67  ....z AyuFtyMong
-000004b0: 6f50 6970 656c 696e 652e 6672 6f6d 5f63  oPipeline.from_c
-000004c0: 7261 776c 6572 6302 0000 0000 0000 0000  rawlerc.........
-000004d0: 0000 0002 0000 0008 0000 0003 0000 0073  ...............s
-000004e0: 7c00 0000 7400 7c01 6401 8302 7312 7401  |...t.|.d...s.t.
-000004f0: 6402 8301 8201 7402 7403 7c00 8302 6a04  d.....t.t.|...j.
-00000500: 7c01 6a05 6a06 7c01 6a05 6a07 7c01 6a05  |.j.j.|.j.j.|.j.
-00000510: 6a08 7c01 6a05 6a09 7c01 6a05 6a0a 7c01  j.|.j.j.|.j.j.|.
-00000520: 6a05 6a0b 6403 8d06 0100 740c 7c00 6a0d  j.j.d.....t.|.j.
-00000530: 7c00 6a0e 6702 8301 7278 7c01 6a0f a010  |.j.g...rx|.j...
-00000540: 6404 7c01 6a05 6a08 9b00 6405 7c01 6a05  d.|.j.j...d.|.j.
-00000550: 6a0a 9b00 6406 9d05 a101 0100 6400 5300  j...d.......d.S.
-00000560: 2907 4e72 0f00 0000 7554 0000 00e6 9caa  ).Nr....uT......
-00000570: e985 8de7 bdae 204d 6f6e 676f 4442 20e8  ...... MongoDB .
-00000580: bf9e e68e a5e4 bfa1 e681 afef bc8c e8af  ................
-00000590: b7e6 9fa5 e79c 8b20 2e63 6f6e 6620 e688  ....... .conf ..
-000005a0: 9620 636f 6e73 756c 20e4 b88a e5af b9e5  . consul .......
-000005b0: ba94 e985 8de7 bdae e4bf a1e6 81af efbc  ................
-000005c0: 8129 06da 0475 7365 72da 0870 6173 7377  .)...user..passw
-000005d0: 6f72 64da 0468 6f73 74da 0470 6f72 74da  ord..host..port.
-000005e0: 0864 6174 6162 6173 65da 0a61 7574 6873  .database..auths
-000005f0: 6f75 7263 6575 1300 0000 e5b7 b2e8 bf9e  ourceu..........
-00000600: e68e a5e8 87b3 2068 6f73 743a 207a 0c2c  ...... host: z.,
-00000610: 2064 6174 6162 6173 653a 2075 1c00 0000   database: u....
-00000620: 20e7 9a84 204d 6f6e 676f 4442 20e7 9bae   ... MongoDB ...
-00000630: e6a0 87e6 95b0 e68d aee5 ba93 2911 da07  ............)...
-00000640: 6861 7361 7474 7272 0e00 0000 da05 7375  hasattrr......su
-00000650: 7065 7272 0800 0000 7215 0000 0072 0f00  perr....r....r..
-00000660: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000670: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00000680: da03 616c 6c72 1000 0000 7211 0000 00da  ..allr....r.....
-00000690: 0473 6c6f 67da 0469 6e66 6fa9 0272 1200  .slog..info..r..
-000006a0: 0000 da06 7370 6964 6572 a901 da09 5f5f  ....spider....__
-000006b0: 636c 6173 735f 5f72 1300 0000 7214 0000  class__r....r...
-000006c0: 00da 0b6f 7065 6e5f 7370 6964 6572 2a00  ...open_spider*.
-000006d0: 0000 7324 0000 0000 0102 0102 0002 ff06  ..s$............
-000006e0: 0202 fe04 030a 0106 0106 0106 0106 0106  ................
-000006f0: 0106 fa06 0a10 0106 0118 ff7a 1f41 7975  ...........z.Ayu
-00000700: 4674 794d 6f6e 676f 5069 7065 6c69 6e65  FtyMongoPipeline
-00000710: 2e6f 7065 6e5f 7370 6964 6572 6302 0000  .open_spiderc...
-00000720: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00000730: 0043 0000 0073 1400 0000 7c00 6a00 7210  .C...s....|.j.r.
-00000740: 7c00 6a00 a001 a100 0100 6400 5300 2901  |.j.......d.S.).
-00000750: 4e29 0272 1000 0000 da05 636c 6f73 6572  N).r......closer
-00000760: 2600 0000 7213 0000 0072 1300 0000 7214  &...r....r....r.
-00000770: 0000 00da 0c63 6c6f 7365 5f73 7069 6465  .....close_spide
-00000780: 723d 0000 0073 0400 0000 0001 0601 7a20  r=...s........z 
-00000790: 4179 7546 7479 4d6f 6e67 6f50 6970 656c  AyuFtyMongoPipel
-000007a0: 696e 652e 636c 6f73 655f 7370 6964 6572  ine.close_spider
-000007b0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-000007c0: 0006 0000 0043 0000 0073 3000 0000 7400  .....C...s0...t.
-000007d0: a001 7c01 a101 7d03 7c03 6401 1900 6402  ..|...}.|.d...d.
-000007e0: 6b02 722c 7402 7403 8300 7c03 7c00 6a04  k.r,t.t...|.|.j.
-000007f0: 7c00 6a05 6403 8d04 0100 7c01 5300 2904  |.j.d.....|.S.).
-00000800: 75aa 0100 000a 2020 2020 2020 2020 6d6f  u.....        mo
-00000810: 6e67 6f44 4220 e5ad 98e5 82a8 e79a 84e6  ngoDB ..........
-00000820: 96b9 e6b3 95ef bc8c 6974 656d 5b22 6d6f  ........item["mo
-00000830: 6e67 6f5f 7570 6461 7465 5f72 756c 6522  ngo_update_rule"
-00000840: 5d20 e794 a8e4 ba8e e5ad 98e5 82a8 e69f  ] ..............
-00000850: a5e8 afa2 e69d a1e4 bbb6 efbc 8ce5 a682  ................
-00000860: e69e 9ce6 9fa5 e8af a2e6 95b0 e68d aee5  ................
-00000870: ad98 e59c a8e7 9a84 e8af 9de5 b0b1 e69b  ................
-00000880: b4e6 96b0 efbc 8ce4 b88d e5ad 98e5 9ca8  ................
-00000890: e79a 84e8 af9d e5b0 b1e6 8f92 e585 a5ef  ................
-000008a0: bc9b 0a20 2020 2020 2020 20e5 a682 e69e  ...        .....
-000008b0: 9ce6 b2a1 e69c 8920 6d6f 6e67 6f5f 7570  ....... mongo_up
-000008c0: 6461 7465 5f72 756c 6520 e588 99e6 af8f  date_rule ......
-000008d0: e6ac a1e9 83bd e696 b0e5 a29e 0a20 2020  .............   
-000008e0: 2020 2020 20e6 ada4 e59c bae6 99af e4b8       ...........
-000008f0: 8de9 9c80 e8a6 81e5 838f 204d 7973 716c  .......... Mysql
-00000900: 20e4 b880 e6a0 b7e4 be9d e8b5 96e5 a487   ...............
-00000910: e6b3 a8e6 9da5 e794 9fe6 8890 e5ad 97e6  ................
-00000920: aeb5 e6b3 a8e9 878a 0a20 2020 2020 2020  .........       
-00000930: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00000940: 2020 2069 7465 6d3a 2073 6372 6170 7920     item: scrapy 
-00000950: 6974 656d 0a20 2020 2020 2020 2020 2020  item.           
-00000960: 2073 7069 6465 723a 2073 6372 6170 7920   spider: scrapy 
-00000970: 7370 6964 6572 0a0a 2020 2020 2020 2020  spider..        
-00000980: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00000990: 2020 2020 2069 7465 6d3a 2073 6372 6170       item: scrap
-000009a0: 7920 6974 656d 0a20 2020 2020 2020 20da  y item.        .
-000009b0: 0969 7465 6d5f 6d6f 6465 da07 4d6f 6e67  .item_mode..Mong
-000009c0: 6f44 4229 03da 0969 7465 6d5f 6469 6374  oDB)...item_dict
-000009d0: 7211 0000 0072 0a00 0000 2906 7206 0000  r....r....).r...
-000009e0: 00da 1563 6f6e 7665 7274 5f69 7465 6d73  ...convert_items
-000009f0: 5f74 6f5f 6469 6374 7204 0000 0072 0300  _to_dictr....r..
-00000a00: 0000 7211 0000 0072 0a00 0000 2904 7212  ..r....r....).r.
-00000a10: 0000 00da 0469 7465 6d72 2700 0000 722f  .....itemr'...r/
-00000a20: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000a30: 0000 da0c 7072 6f63 6573 735f 6974 656d  ....process_item
-00000a40: 4100 0000 7312 0000 0000 0c0a 020c 0102  A...s...........
-00000a50: 0104 0102 0104 0104 fc06 067a 2041 7975  ...........z Ayu
-00000a60: 4674 794d 6f6e 676f 5069 7065 6c69 6e65  FtyMongoPipeline
-00000a70: 2e70 726f 6365 7373 5f69 7465 6d29 0172  .process_item).r
-00000a80: 0900 0000 290c da08 5f5f 6e61 6d65 5f5f  ....)...__name__
-00000a90: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000aa0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000ab0: 635f 5f72 0d00 0000 7215 0000 00da 0b63  c__r....r......c
-00000ac0: 6c61 7373 6d65 7468 6f64 721a 0000 0072  lassmethodr....r
-00000ad0: 2a00 0000 722c 0000 0072 3200 0000 da0d  *...r,...r2.....
-00000ae0: 5f5f 636c 6173 7363 656c 6c5f 5f72 1300  __classcell__r..
-00000af0: 0000 7213 0000 0072 2800 0000 7214 0000  ..r....r(...r...
-00000b00: 0072 0800 0000 0d00 0000 7316 0000 0008  .r........s.....
-00000b10: 0104 0600 fe02 0202 0102 fd0c 1202 010a  ................
-00000b20: 050c 1308 044e 290d da06 7479 7069 6e67  .....N)...typing
-00000b30: 7202 0000 005a 2361 7975 6765 7370 6964  r....Z#ayugespid
-00000b40: 6572 746f 6f6c 732e 636f 6d6d 6f6e 2e6d  ertools.common.m
-00000b50: 6f6e 676f 6462 7069 7065 7203 0000 0072  ongodbpiper....r
-00000b60: 0400 0000 da20 6179 7567 6573 7069 6465  ..... ayugespide
-00000b70: 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e 7479  rtools.common.ty
-00000b80: 7065 7661 7273 7205 0000 00da 1d61 7975  pevarsr......ayu
-00000b90: 6765 7370 6964 6572 746f 6f6c 732e 636f  gespidertools.co
-00000ba0: 6d6d 6f6e 2e75 7469 6c73 7206 0000 005a  mmon.utilsr....Z
-00000bb0: 1c61 7975 6765 7370 6964 6572 746f 6f6c  .ayugespidertool
-00000bc0: 732e 6d6f 6e67 6f63 6c69 656e 7472 0700  s.mongoclientr..
-00000bd0: 0000 da07 5f5f 616c 6c5f 5f72 0800 0000  ....__all__r....
-00000be0: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-00000bf0: 1400 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000c00: 0000 730e 0000 000c 0210 010c 010c 010c  ..s.............
-00000c10: 0302 ff04 05                             .....
+00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6404 6701 5a07 4700 6405  m.Z...d.g.Z.G.d.
+00000060: 6404 8400 6404 6506 8303 5a08 6406 5300  d...d.e...Z.d.S.
+00000070: 2907 e900 0000 0029 02da 0b53 796e 6368  )......)...Synch
+00000080: 726f 6e69 7a65 da0c 6d6f 6e67 6f64 625f  ronize..mongodb_
+00000090: 7069 7065 2901 da0b 546f 6f6c 7346 6f72  pipe)...ToolsFor
+000000a0: 4179 7529 01da 0b4d 6f6e 676f 4462 4261  Ayu)...MongoDbBa
+000000b0: 7365 da13 4179 7546 7479 4d6f 6e67 6f50  se..AyuFtyMongoP
+000000c0: 6970 656c 696e 6563 0000 0000 0000 0000  ipelinec........
+000000d0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+000000e0: 734e 0000 0065 005a 0164 005a 0264 015a  sN...e.Z.d.Z.d.Z
+000000f0: 0364 0f65 0464 0364 049c 0264 0564 0684  .d.e.d.d...d.d..
+00000100: 055a 0565 0664 0764 0884 0083 015a 0787  .Z.e.d.d.....Z..
+00000110: 0066 0164 0964 0a84 085a 0864 0b64 0c84  .f.d.d...Z.d.d..
+00000120: 005a 0964 0d64 0e84 005a 0a87 0004 005a  .Z.d.d...Z.....Z
+00000130: 0b53 0029 1072 0600 0000 7538 0000 000a  .S.).r....u8....
+00000140: 2020 2020 4d6f 6e67 6f44 4220 e5ad 98e5      MongoDB ....
+00000150: 82a8 e59c bae6 99af e79a 8420 7363 7261  ........... scra
+00000160: 7079 2070 6970 656c 696e 6520 e689 a9e5  py pipeline ....
+00000170: b195 0a20 2020 20da 004e 2902 da11 636f  ...    ..N)...co
+00000180: 6c6c 6563 7469 6f6e 5f70 7265 6669 78da  llection_prefix.
+00000190: 0672 6574 7572 6e63 0200 0000 0000 0000  .returnc........
+000001a0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+000001b0: 732c 0000 0074 007c 0174 0183 0273 1274  s,...t.|.t...s.t
+000001c0: 0264 0183 0182 017c 0170 1864 027c 005f  .d.....|.p.d.|._
+000001d0: 0364 037c 005f 0464 037c 005f 0564 0353  .d.|._.d.|._.d.S
+000001e0: 0029 0475 ab00 0000 0a20 2020 2020 2020  .).u.....       
+000001f0: 20e5 889d e5a7 8be5 8c96 0a20 2020 2020   ..........     
+00000200: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00000210: 2020 2020 206d 6f6e 676f 6462 5f63 6f6e       mongodb_con
+00000220: 663a 206d 6f6e 6744 4220 e79a 84e8 bf9e  f: mongDB ......
+00000230: e68e a5e9 858d e7bd ae0a 2020 2020 2020  ..........      
+00000240: 2020 2020 2020 636f 6c6c 6563 7469 6f6e        collection
+00000250: 5f70 7265 6669 783a 206d 6f6e 6744 4220  _prefix: mongDB 
+00000260: e5ad 98e5 82a8 e99b 86e5 9088 e79a 84e5  ................
+00000270: 898d e7bc 80ef bc8c e9bb 98e8 aea4 e4b8  ................
+00000280: bae7 a9ba e5ad 97e7 aca6 0a20 2020 2020  ...........     
+00000290: 2020 2075 4000 0000 6d6f 6e67 6f44 4220     u@...mongoDB 
+000002a0: e689 80e8 a681 e5ad 98e5 82a8 e79a 84e9  ................
+000002b0: 9b86 e590 88e5 898d e7bc 80e5 908d e7a7  ................
+000002c0: b0e9 9c80 e8a6 81e6 98af 2073 7472 20e6  .......... str .
+000002d0: a0bc e5bc 8fef bc81 7207 0000 004e 2906  ........r....N).
+000002e0: da0a 6973 696e 7374 616e 6365 da03 7374  ..isinstance..st
+000002f0: 72da 0e41 7373 6572 7469 6f6e 4572 726f  r..AssertionErro
+00000300: 7272 0800 0000 da04 636f 6e6e da02 6462  rr......conn..db
+00000310: 2902 da04 7365 6c66 7208 0000 00a9 0072  )...selfr......r
+00000320: 1000 0000 fa51 2f72 6f6f 742f 6d79 7072  .....Q/root/mypr
+00000330: 6f6a 2f41 7975 6765 5370 6964 6572 546f  oj/AyugeSpiderTo
+00000340: 6f6c 732f 6179 7567 6573 7069 6465 7274  ols/ayugespidert
+00000350: 6f6f 6c73 2f73 6372 6170 6572 2f70 6970  ools/scraper/pip
+00000360: 656c 696e 6573 2f6d 6f6e 676f 2f66 616e  elines/mongo/fan
+00000370: 7461 7379 2e70 79da 085f 5f69 6e69 745f  tasy.py..__init_
+00000380: 5f0f 0000 0073 0800 0000 000a 1202 0a02  _....s..........
+00000390: 0601 7a1c 4179 7546 7479 4d6f 6e67 6f50  ..z.AyuFtyMongoP
+000003a0: 6970 656c 696e 652e 5f5f 696e 6974 5f5f  ipeline.__init__
+000003b0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000003c0: 0005 0000 0043 0000 0073 1400 0000 7c00  .....C...s....|.
+000003d0: 7c01 6a00 a001 6401 6402 a102 6403 8d01  |.j...d.d...d...
+000003e0: 5300 2904 4e5a 194d 4f4e 474f 4442 5f43  S.).NZ.MONGODB_C
+000003f0: 4f4c 4c45 4354 494f 4e5f 5052 4546 4958  OLLECTION_PREFIX
+00000400: 7207 0000 0029 0172 0800 0000 2902 da08  r....).r....)...
+00000410: 7365 7474 696e 6773 da03 6765 7429 02da  settings..get)..
+00000420: 0363 6c73 da07 6372 6177 6c65 7272 1000  .cls..crawlerr..
+00000430: 0000 7210 0000 0072 1100 0000 da0c 6672  ..r....r......fr
+00000440: 6f6d 5f63 7261 776c 6572 2000 0000 7306  om_crawler ...s.
+00000450: 0000 0000 0202 010c ff7a 2041 7975 4674  .........z AyuFt
+00000460: 794d 6f6e 676f 5069 7065 6c69 6e65 2e66  yMongoPipeline.f
+00000470: 726f 6d5f 6372 6177 6c65 7263 0200 0000  rom_crawlerc....
+00000480: 0000 0000 0000 0000 0200 0000 0800 0000  ................
+00000490: 0300 0000 737c 0000 0074 007c 0164 0183  ....s|...t.|.d..
+000004a0: 0273 1274 0164 0283 0182 0174 0274 037c  .s.t.d.....t.t.|
+000004b0: 0083 026a 047c 016a 056a 067c 016a 056a  ...j.|.j.j.|.j.j
+000004c0: 077c 016a 056a 087c 016a 056a 097c 016a  .|.j.j.|.j.j.|.j
+000004d0: 056a 0a7c 016a 056a 0b64 038d 0601 0074  .j.|.j.j.d.....t
+000004e0: 0c7c 006a 0d7c 006a 0e67 0283 0172 787c  .|.j.|.j.g...rx|
+000004f0: 016a 0fa0 1064 047c 016a 056a 089b 0064  .j...d.|.j.j...d
+00000500: 057c 016a 056a 0a9b 0064 069d 05a1 0101  .|.j.j...d......
+00000510: 0064 0053 0029 074e da0c 6d6f 6e67 6f64  .d.S.).N..mongod
+00000520: 625f 636f 6e66 7554 0000 00e6 9caa e985  b_confuT........
+00000530: 8de7 bdae 204d 6f6e 676f 4442 20e8 bf9e  .... MongoDB ...
+00000540: e68e a5e4 bfa1 e681 afef bc8c e8af b7e6  ................
+00000550: 9fa5 e79c 8b20 2e63 6f6e 6620 e688 9620  ..... .conf ... 
+00000560: 636f 6e73 756c 20e4 b88a e5af b9e5 ba94  consul .........
+00000570: e985 8de7 bdae e4bf a1e6 81af efbc 8129  ...............)
+00000580: 06da 0475 7365 72da 0870 6173 7377 6f72  ...user..passwor
+00000590: 64da 0468 6f73 74da 0470 6f72 74da 0864  d..host..port..d
+000005a0: 6174 6162 6173 65da 0a61 7574 6873 6f75  atabase..authsou
+000005b0: 7263 6575 1300 0000 e5b7 b2e8 bf9e e68e  rceu............
+000005c0: a5e8 87b3 2068 6f73 743a 207a 0c2c 2064  .... host: z., d
+000005d0: 6174 6162 6173 653a 2075 1c00 0000 20e7  atabase: u.... .
+000005e0: 9a84 204d 6f6e 676f 4442 20e7 9bae e6a0  .. MongoDB .....
+000005f0: 87e6 95b0 e68d aee5 ba93 2911 da07 6861  ..........)...ha
+00000600: 7361 7474 7272 0c00 0000 da05 7375 7065  sattrr......supe
+00000610: 7272 0600 0000 7212 0000 0072 1800 0000  rr....r....r....
+00000620: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00000630: 1c00 0000 721d 0000 0072 1e00 0000 da03  ....r....r......
+00000640: 616c 6c72 0d00 0000 720e 0000 00da 0473  allr....r......s
+00000650: 6c6f 67da 0469 6e66 6fa9 0272 0f00 0000  log..info..r....
+00000660: da06 7370 6964 6572 a901 da09 5f5f 636c  ..spider....__cl
+00000670: 6173 735f 5f72 1000 0000 7211 0000 00da  ass__r....r.....
+00000680: 0b6f 7065 6e5f 7370 6964 6572 2600 0000  .open_spider&...
+00000690: 7324 0000 0000 0102 0102 0002 ff06 0202  s$..............
+000006a0: fe04 030a 0106 0106 0106 0106 0106 0106  ................
+000006b0: fa06 0a10 0106 0118 ff7a 1f41 7975 4674  .........z.AyuFt
+000006c0: 794d 6f6e 676f 5069 7065 6c69 6e65 2e6f  yMongoPipeline.o
+000006d0: 7065 6e5f 7370 6964 6572 6302 0000 0000  pen_spiderc.....
+000006e0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+000006f0: 0000 0073 1400 0000 7c00 6a00 7210 7c00  ...s....|.j.r.|.
+00000700: 6a00 a001 a100 0100 6400 5300 2901 4e29  j.......d.S.).N)
+00000710: 0272 0d00 0000 da05 636c 6f73 6572 2400  .r......closer$.
+00000720: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00000730: 00da 0c63 6c6f 7365 5f73 7069 6465 7239  ...close_spider9
+00000740: 0000 0073 0400 0000 0001 0601 7a20 4179  ...s........z Ay
+00000750: 7546 7479 4d6f 6e67 6f50 6970 656c 696e  uFtyMongoPipelin
+00000760: 652e 636c 6f73 655f 7370 6964 6572 6303  e.close_spiderc.
+00000770: 0000 0000 0000 0000 0000 0004 0000 0006  ................
+00000780: 0000 0043 0000 0073 3000 0000 7400 a001  ...C...s0...t...
+00000790: 7c01 a101 7d03 7c03 6401 1900 6402 6b02  |...}.|.d...d.k.
+000007a0: 722c 7402 7403 8300 7c03 7c00 6a04 7c00  r,t.t...|.|.j.|.
+000007b0: 6a05 6403 8d04 0100 7c01 5300 2904 75aa  j.d.....|.S.).u.
+000007c0: 0100 000a 2020 2020 2020 2020 6d6f 6e67  ....        mong
+000007d0: 6f44 4220 e5ad 98e5 82a8 e79a 84e6 96b9  oDB ............
+000007e0: e6b3 95ef bc8c 6974 656d 5b22 6d6f 6e67  ......item["mong
+000007f0: 6f5f 7570 6461 7465 5f72 756c 6522 5d20  o_update_rule"] 
+00000800: e794 a8e4 ba8e e5ad 98e5 82a8 e69f a5e8  ................
+00000810: afa2 e69d a1e4 bbb6 efbc 8ce5 a682 e69e  ................
+00000820: 9ce6 9fa5 e8af a2e6 95b0 e68d aee5 ad98  ................
+00000830: e59c a8e7 9a84 e8af 9de5 b0b1 e69b b4e6  ................
+00000840: 96b0 efbc 8ce4 b88d e5ad 98e5 9ca8 e79a  ................
+00000850: 84e8 af9d e5b0 b1e6 8f92 e585 a5ef bc9b  ................
+00000860: 0a20 2020 2020 2020 20e5 a682 e69e 9ce6  .        .......
+00000870: b2a1 e69c 8920 6d6f 6e67 6f5f 7570 6461  ..... mongo_upda
+00000880: 7465 5f72 756c 6520 e588 99e6 af8f e6ac  te_rule ........
+00000890: a1e9 83bd e696 b0e5 a29e 0a20 2020 2020  ...........     
+000008a0: 2020 20e6 ada4 e59c bae6 99af e4b8 8de9     .............
+000008b0: 9c80 e8a6 81e5 838f 204d 7973 716c 20e4  ........ Mysql .
+000008c0: b880 e6a0 b7e4 be9d e8b5 96e5 a487 e6b3  ................
+000008d0: a8e6 9da5 e794 9fe6 8890 e5ad 97e6 aeb5  ................
+000008e0: e6b3 a8e9 878a 0a20 2020 2020 2020 2041  .......        A
+000008f0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00000900: 2069 7465 6d3a 2073 6372 6170 7920 6974   item: scrapy it
+00000910: 656d 0a20 2020 2020 2020 2020 2020 2073  em.            s
+00000920: 7069 6465 723a 2073 6372 6170 7920 7370  pider: scrapy sp
+00000930: 6964 6572 0a0a 2020 2020 2020 2020 5265  ider..        Re
+00000940: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00000950: 2020 2069 7465 6d3a 2073 6372 6170 7920     item: scrapy 
+00000960: 6974 656d 0a20 2020 2020 2020 20da 0969  item.        ..i
+00000970: 7465 6d5f 6d6f 6465 da07 4d6f 6e67 6f44  tem_mode..MongoD
+00000980: 4229 03da 0969 7465 6d5f 6469 6374 720e  B)...item_dictr.
+00000990: 0000 0072 0800 0000 2906 7204 0000 00da  ...r....).r.....
+000009a0: 1563 6f6e 7665 7274 5f69 7465 6d73 5f74  .convert_items_t
+000009b0: 6f5f 6469 6374 7203 0000 0072 0200 0000  o_dictr....r....
+000009c0: 720e 0000 0072 0800 0000 2904 720f 0000  r....r....).r...
+000009d0: 00da 0469 7465 6d72 2500 0000 722d 0000  ...itemr%...r-..
+000009e0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+000009f0: da0c 7072 6f63 6573 735f 6974 656d 3d00  ..process_item=.
+00000a00: 0000 7312 0000 0000 0c0a 020c 0102 0104  ..s.............
+00000a10: 0102 0104 0104 fc06 067a 2041 7975 4674  .........z AyuFt
+00000a20: 794d 6f6e 676f 5069 7065 6c69 6e65 2e70  yMongoPipeline.p
+00000a30: 726f 6365 7373 5f69 7465 6d29 0172 0700  rocess_item).r..
+00000a40: 0000 290c da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00000a50: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000a60: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00000a70: 5f72 0b00 0000 7212 0000 00da 0b63 6c61  _r....r......cla
+00000a80: 7373 6d65 7468 6f64 7217 0000 0072 2800  ssmethodr....r(.
+00000a90: 0000 722a 0000 0072 3000 0000 da0d 5f5f  ..r*...r0.....__
+00000aa0: 636c 6173 7363 656c 6c5f 5f72 1000 0000  classcell__r....
+00000ab0: 7210 0000 0072 2600 0000 7211 0000 0072  r....r&...r....r
+00000ac0: 0600 0000 0a00 0000 7316 0000 0008 0104  ........s.......
+00000ad0: 0600 fe02 0202 0102 fd0c 1102 010a 050c  ................
+00000ae0: 1308 044e 2909 da23 6179 7567 6573 7069  ...N)..#ayugespi
+00000af0: 6465 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e  dertools.common.
+00000b00: 6d6f 6e67 6f64 6270 6970 6572 0200 0000  mongodbpiper....
+00000b10: 7203 0000 00da 1d61 7975 6765 7370 6964  r......ayugespid
+00000b20: 6572 746f 6f6c 732e 636f 6d6d 6f6e 2e75  ertools.common.u
+00000b30: 7469 6c73 7204 0000 00da 1c61 7975 6765  tilsr......ayuge
+00000b40: 7370 6964 6572 746f 6f6c 732e 6d6f 6e67  spidertools.mong
+00000b50: 6f63 6c69 656e 7472 0500 0000 da07 5f5f  oclientr......__
+00000b60: 616c 6c5f 5f72 0600 0000 7210 0000 0072  all__r....r....r
+00000b70: 1000 0000 7210 0000 0072 1100 0000 da08  ....r....r......
+00000b80: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+00000b90: 0010 010c 010c 0302 ff04 05              ...........
```

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from typing import Optional
-
 from ayugespidertools.common.mongodbpipe import Synchronize, mongodb_pipe
-from ayugespidertools.common.typevars import MongoDBConfig
 from ayugespidertools.common.utils import ToolsForAyu
 from ayugespidertools.mongoclient import MongoDbBase
 
 __all__ = [
     "AyuFtyMongoPipeline",
 ]
 
@@ -24,15 +21,14 @@
         Args:
             mongodb_conf: mongDB 的连接配置
             collection_prefix: mongDB 存储集合的前缀，默认为空字符
         """
         assert isinstance(collection_prefix, str), "mongoDB 所要存储的集合前缀名称需要是 str 格式！"
 
         self.collection_prefix = collection_prefix or ""
-        self.mongodb_conf: Optional[MongoDBConfig] = None
         # conn 和 db 为父类的属性，用于存储连接信息
         self.conn = None
         self.db = None
 
     @classmethod
     def from_crawler(cls, crawler):
         return cls(
```

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 25 03:01:31 2023 UTC, .py size: 2840 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 8b42 4764 180b 0000  U........BGd....
+00000000: 550d 0d0a 0000 0000 7813 5364 1a0b 0000  U.......x.Sd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6701 5a07  d.l.m.Z...d.g.Z.
 00000060: 4700 6406 6405 8400 6405 6506 8303 5a08  G.d.d...d.e...Z.
 00000070: 6401 5300 2907 e900 0000 004e 2901 da08  d.S.)......N)...
```

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     def open_spider(self, spider):
         self.slog = spider.slog
         if not self.pool_db_conf:
             spider.slog.warning("未配置 POOL_DB_CONFIG 参数，将使用其默认参数")
             self.pool_db_conf = {
                 # 连接池允许的最大连接数
                 "maxconnections": 5,
-                # 连接池中空闲连接的最大数量。默认0，即无最大数量限制
+                # 连接池中空闲连接的最大数量。默认 0，即无最大数量限制
                 "maxcached": 0,
-                # 连接的最大使用次数。默认0，即无使用次数限制
+                # 连接的最大使用次数。默认 0，即无使用次数限制
                 "maxusage": 0,
                 # 连接数达到最大时，新连接是否可阻塞。默认False，即达到最大连接数时，再取新连接将会报错
                 "blocking": True,
             }
         self.mysql_conf = spider.mysql_conf
         self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
```

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/project/.gitignore` & `ayugespidertools-2.0.2/ayugespidertools/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-2.0.2/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-2.0.2/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-2.0.2/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-2.0.2/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc` & `ayugespidertools-2.0.2/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/utils/cmdline.py` & `ayugespidertools-2.0.2/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/ayugespidertools/verificationcode.py` & `ayugespidertools-2.0.2/ayugespidertools/verificationcode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.1/pyproject.toml` & `ayugespidertools-2.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "2.0.1"
+version = "2.0.2"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -35,14 +35,15 @@
 mmh3 = "^3.0.0"
 pycryptodome = "^3.15.0"
 oss2 = "^2.16.0"
 aiomysql = "^0.1.1"
 attrs = "^22.2.0"
 toml = "^0.10.2"
 python-hcl2 = "^4.3.0"
+motor = "2.5.1"
 
 [tool.poetry.scripts]
 ayuge = "ayugespidertools.utils.cmdline:execute"
 ayugespidertools = "ayugespidertools.utils.cmdline:execute"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
```

### Comparing `ayugespidertools-2.0.1/PKG-INFO` & `ayugespidertools-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 2.0.1
+Version: 2.0.2
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -24,14 +24,15 @@
 Requires-Dist: aiomysql (>=0.1.1,<0.2.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: environs (>=9.5.0,<10.0.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: itemadapter (>=0.7.0,<0.8.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
+Requires-Dist: motor (==2.5.1)
 Requires-Dist: numpy (==1.24.2)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
 Requires-Dist: oss2 (>=2.16.0,<3.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
 Requires-Dist: pymongo (>=3.12.3,<4.0.0)
 Requires-Dist: python-hcl2 (>=4.3.0,<5.0.0)
```

