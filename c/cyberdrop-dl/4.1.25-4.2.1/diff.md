# Comparing `tmp/cyberdrop-dl-4.1.25.tar.gz` & `tmp/cyberdrop-dl-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.25.tar", last modified: Wed May  3 02:16:31 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.1.tar", last modified: Fri May  5 05:55:14 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.25.tar` & `cyberdrop-dl-4.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.749760 cyberdrop-dl-4.1.25/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-03 02:16:31.749760 cyberdrop-dl-4.1.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.741760 cyberdrop-dl-4.1.25/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.741760 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.741760 cyberdrop-dl-4.1.25/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.745760 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.745760 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13984 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.745760 cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.741760 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 02:16:31.749760 cyberdrop-dl-4.1.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:14.793122 cyberdrop-dl-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-05-05 05:55:14.793122 cyberdrop-dl-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:14.785122 cyberdrop-dl-4.2.1/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:14.789122 cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:14.789122 cyberdrop-dl-4.2.1/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:14.793122 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:14.793122 cyberdrop-dl-4.2.1/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:14.793122 cyberdrop-dl-4.2.1/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:14.785122 cyberdrop-dl-4.2.1/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-05-05 05:55:14.000000 cyberdrop-dl-4.2.1/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-05 05:55:14.000000 cyberdrop-dl-4.2.1/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:55:14.000000 cyberdrop-dl-4.2.1/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 05:55:14.000000 cyberdrop-dl-4.2.1/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 05:55:14.000000 cyberdrop-dl-4.2.1/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 05:55:14.000000 cyberdrop-dl-4.2.1/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-05 05:55:14.793122 cyberdrop-dl-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:54:58.000000 cyberdrop-dl-4.2.1/setup.py
```

### Comparing `cyberdrop-dl-4.1.25/LICENSE` & `cyberdrop-dl-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/PKG-INFO` & `cyberdrop-dl-4.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.25
+Version: 4.2.1
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -39,43 +39,43 @@
 
 ## More Information
 
 Read the [Wiki](https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/)!
 
 ## Supported Sites
 
-| Website                 | Supported Link Types                                                                                                                                                                                                                   |
-|-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Anonfiles               | Download page: Anonfiles.com/...                                                                                                                                                                                                       |
-| Bayfiles                | Download page: Bayfiles.com/...                                                                                                                                                                                                        |
-| Bunkr (ru/su/la)        | Albums: bunkr.ru/a/... <br> Direct Videos: stream.bunkr.ru/v/... <br> Direct links: cdn.bunkr.ru/... <br> Direct links: i.bunkr.ru/... <br> Direct links: files.bunkr.ru/... <br> Direct links: media-files.bunkr.ru/...               |
-| Coomer.party            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      |
-| Cyberdrop               | Albums: cyberdrop.me/a/... <br> Direct Videos: fs-0#.cyberdrop.me/... <br> Direct Videos: f.cyberdrop.me/... <br> Direct Images: img-0#.cyberdrop.me/... <br> Direct Images: f.cyberdrop.me/... <br> Also works with .cc, .to, and .nl |
-| Cyberfile               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    |
-| E-Hentai                | Albums: e-hentai.org/g/... <br> Posts: e-hentai.org/s/...                                                                                                                                                                              |
-| Erome                   | Albums: erome.com/a/...                                                                                                                                                                                                                |
-| Fapello                 | Models: fapello.com/...                                                                                                                                                                                                                |
-| Gallery.DeltaPorno.com  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
-| GoFile                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
-| Gfycat                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
-| HGameCG                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
-| ImgBox                  | Albums: imgbox.com/g/... <br> Direct Images: images#.imgbox.com/... <br> Single Files: imgbox.com/...                                                                                                                                  |
-| IMG.Kiwi                | Albums: img.kiwi/album/... <br> Direct Images: img.kiwi/image/... <br> User Profile: img.kiwi/#USER# <br> All User Albums: img.kiwi/#USER#/albums                                                                                      |
-| jpg.church<br/>jpg.fish | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
-| LoveFap                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
-| NSFW.XXX                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
-| PimpAndHost             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
-| PixelDrain              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
-| Pixl                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
-| Postimg.cc              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
-| NudoStar                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
-| SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
-| SocialMediaGirls        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
-| XBunker                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
-| XBunkr                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
+| Website                                 | Supported Link Types                                                                                                                                                                                                                   |
+|-----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Anonfiles                               | Download page: Anonfiles.com/...                                                                                                                                                                                                       |
+| Bayfiles                                | Download page: Bayfiles.com/...                                                                                                                                                                                                        |
+| Bunkr (ru/su/la)                        | Albums: bunkr.ru/a/... <br> Direct Videos: stream.bunkr.ru/v/... <br> Direct links: cdn.bunkr.ru/... <br> Direct links: i.bunkr.ru/... <br> Direct links: files.bunkr.ru/... <br> Direct links: media-files.bunkr.ru/...               |
+| Coomer.party                            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      |
+| Cyberdrop                               | Albums: cyberdrop.me/a/... <br> Direct Videos: fs-0#.cyberdrop.me/... <br> Direct Videos: f.cyberdrop.me/... <br> Direct Images: img-0#.cyberdrop.me/... <br> Direct Images: f.cyberdrop.me/... <br> Also works with .cc, .to, and .nl |
+| Cyberfile                               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    |
+| E-Hentai                                | Albums: e-hentai.org/g/... <br> Posts: e-hentai.org/s/...                                                                                                                                                                              |
+| Erome                                   | Albums: erome.com/a/...                                                                                                                                                                                                                |
+| Fapello                                 | Models: fapello.com/...                                                                                                                                                                                                                |
+| Gallery.DeltaPorno.com                  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
+| GoFile                                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
+| Gfycat                                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
+| HGameCG                                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
+| ImgBox                                  | Albums: imgbox.com/g/... <br> Direct Images: images#.imgbox.com/... <br> Single Files: imgbox.com/...                                                                                                                                  |
+| IMG.Kiwi                                | Albums: img.kiwi/album/... <br> Direct Images: img.kiwi/image/... <br> User Profile: img.kiwi/#USER# <br> All User Albums: img.kiwi/#USER#/albums                                                                                      |
+| jpg.church<br/>jpg.fish<br/>jpg.fishing | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
+| LoveFap                                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
+| NSFW.XXX                                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
+| PimpAndHost                             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
+| PixelDrain                              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
+| Pixl                                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
+| Postimg.cc                              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
+| NudoStar                                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
+| SimpCity                                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
+| SocialMediaGirls                        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
+| XBunker                                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
+| XBunkr                                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
 
 Reminder to leave the link full (include the https://)
 
 ## Information
 
 **Requires Python 3.7 or higher (3.10 recommended)**
 
@@ -191,10 +191,14 @@
 --hide-overall-progress         removes overall progress section while downloading
 --hide-forum-progress           removes forum progress section while downloading
 --hide-thread-progress          removes thread progress section while downloading
 --hide-domain-progress          removes domain progress section while downloading
 --hide-album-progress           removes album progress section while downloading
 --hide-file-progress            removes file progress section while downloading
 --refresh-rate                  changes the refresh rate of the progress table
+--visible-rows-threads          number of visible rows to use for the threads table
+--visible-rows-domains          number of visible rows to use for the domains table
+--visible-rows-albums           number of visible rows to use for the albums table
+--visible-rows-files            number of visible rows to use for the files table
 ```
 
 `--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.25 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.1 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -19,20 +19,20 @@
 Development [Buy_Me_A_Coffee] If you want to support me and my effort you can
 buy me a coffee or send me some crypto: BTC:
 bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B XMR:
 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
 ## More Information Read the [Wiki](https://github.com/Jules-WinnfieldX/
 CyberDropDownloader/wiki/)! ## Supported Sites | Website | Supported Link Types
-| |-------------------------|--------------------------------------------------
+| |-----------------------------------------|----------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------------------------| | Anonfiles | Download page: Anonfiles.com/... | |
-Bayfiles | Download page: Bayfiles.com/... | | Bunkr (ru/su/la) | Albums:
-bunkr.ru/a/...
+----------------------------------------| | Anonfiles | Download page:
+Anonfiles.com/... | | Bayfiles | Download page: Bayfiles.com/... | | Bunkr (ru/
+su/la) | Albums: bunkr.ru/a/...
 Direct Videos: stream.bunkr.ru/v/...
 Direct links: cdn.bunkr.ru/...
 Direct links: i.bunkr.ru/...
 Direct links: files.bunkr.ru/...
 Direct links: media-files.bunkr.ru/... | | Coomer.party | Profiles:
 coomer.party/...
 Thumbnail Links: coomer.party/thumbnail/...
@@ -55,15 +55,16 @@
 gofile.io/d/... | | Gfycat | Gif: gfycat.com/... | | HGameCG | Albums:
 hgamecg.com/.../index.html | | ImgBox | Albums: imgbox.com/g/...
 Direct Images: images#.imgbox.com/...
 Single Files: imgbox.com/... | | IMG.Kiwi | Albums: img.kiwi/album/...
 Direct Images: img.kiwi/image/...
 User Profile: img.kiwi/#USER#
 All User Albums: img.kiwi/#USER#/albums | | jpg.church
-jpg.fish | Albums: jpg.church/album/...
+jpg.fish
+jpg.fishing | Albums: jpg.church/album/...
 Direct Images: jpg.church/image/...
 User Profile: jpg.church/#USER#
 All User Albums: jpg.church/#USER#/albums | | LoveFap | Albums: lovefap.com/
 a/...
 Direct Images: s*.lovefap.com/content/photos/...
 Videos: lovefap.com/video/... | | NSFW.XXX | Profile: nsfw.xxx/user/...
 Post: nsfw.xxx/post/... | | PimpAndHost | Albums: pimpandhost.com/album/...
@@ -161,14 +162,17 @@
 disables the new rich progress entirely and uses older methods --hide-overall-
 progress removes overall progress section while downloading --hide-forum-
 progress removes forum progress section while downloading --hide-thread-
 progress removes thread progress section while downloading --hide-domain-
 progress removes domain progress section while downloading --hide-album-
 progress removes album progress section while downloading --hide-file-progress
 removes file progress section while downloading --refresh-rate changes the
-refresh rate of the progress table ``` `--only-hosts` and `--skip-hosts` can
-use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
-"cyberfile", "e-hentai", "erome", "fapello", "gfycat",
-"gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
-"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
-"socialmediagirls", "xbunker", "xbunkr"`
+refresh rate of the progress table --visible-rows-threads number of visible
+rows to use for the threads table --visible-rows-domains number of visible rows
+to use for the domains table --visible-rows-albums number of visible rows to
+use for the albums table --visible-rows-files number of visible rows to use for
+the files table ``` `--only-hosts` and `--skip-hosts` can use: `"anonfiles",
+"bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai",
+"erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg",
+"img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap",
+"nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
+"saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.1.25/README.md` & `cyberdrop-dl-4.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,43 +27,43 @@
 
 ## More Information
 
 Read the [Wiki](https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/)!
 
 ## Supported Sites
 
-| Website                 | Supported Link Types                                                                                                                                                                                                                   |
-|-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Anonfiles               | Download page: Anonfiles.com/...                                                                                                                                                                                                       |
-| Bayfiles                | Download page: Bayfiles.com/...                                                                                                                                                                                                        |
-| Bunkr (ru/su/la)        | Albums: bunkr.ru/a/... <br> Direct Videos: stream.bunkr.ru/v/... <br> Direct links: cdn.bunkr.ru/... <br> Direct links: i.bunkr.ru/... <br> Direct links: files.bunkr.ru/... <br> Direct links: media-files.bunkr.ru/...               |
-| Coomer.party            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      |
-| Cyberdrop               | Albums: cyberdrop.me/a/... <br> Direct Videos: fs-0#.cyberdrop.me/... <br> Direct Videos: f.cyberdrop.me/... <br> Direct Images: img-0#.cyberdrop.me/... <br> Direct Images: f.cyberdrop.me/... <br> Also works with .cc, .to, and .nl |
-| Cyberfile               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    |
-| E-Hentai                | Albums: e-hentai.org/g/... <br> Posts: e-hentai.org/s/...                                                                                                                                                                              |
-| Erome                   | Albums: erome.com/a/...                                                                                                                                                                                                                |
-| Fapello                 | Models: fapello.com/...                                                                                                                                                                                                                |
-| Gallery.DeltaPorno.com  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
-| GoFile                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
-| Gfycat                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
-| HGameCG                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
-| ImgBox                  | Albums: imgbox.com/g/... <br> Direct Images: images#.imgbox.com/... <br> Single Files: imgbox.com/...                                                                                                                                  |
-| IMG.Kiwi                | Albums: img.kiwi/album/... <br> Direct Images: img.kiwi/image/... <br> User Profile: img.kiwi/#USER# <br> All User Albums: img.kiwi/#USER#/albums                                                                                      |
-| jpg.church<br/>jpg.fish | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
-| LoveFap                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
-| NSFW.XXX                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
-| PimpAndHost             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
-| PixelDrain              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
-| Pixl                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
-| Postimg.cc              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
-| NudoStar                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
-| SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
-| SocialMediaGirls        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
-| XBunker                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
-| XBunkr                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
+| Website                                 | Supported Link Types                                                                                                                                                                                                                   |
+|-----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Anonfiles                               | Download page: Anonfiles.com/...                                                                                                                                                                                                       |
+| Bayfiles                                | Download page: Bayfiles.com/...                                                                                                                                                                                                        |
+| Bunkr (ru/su/la)                        | Albums: bunkr.ru/a/... <br> Direct Videos: stream.bunkr.ru/v/... <br> Direct links: cdn.bunkr.ru/... <br> Direct links: i.bunkr.ru/... <br> Direct links: files.bunkr.ru/... <br> Direct links: media-files.bunkr.ru/...               |
+| Coomer.party                            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      |
+| Cyberdrop                               | Albums: cyberdrop.me/a/... <br> Direct Videos: fs-0#.cyberdrop.me/... <br> Direct Videos: f.cyberdrop.me/... <br> Direct Images: img-0#.cyberdrop.me/... <br> Direct Images: f.cyberdrop.me/... <br> Also works with .cc, .to, and .nl |
+| Cyberfile                               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    |
+| E-Hentai                                | Albums: e-hentai.org/g/... <br> Posts: e-hentai.org/s/...                                                                                                                                                                              |
+| Erome                                   | Albums: erome.com/a/...                                                                                                                                                                                                                |
+| Fapello                                 | Models: fapello.com/...                                                                                                                                                                                                                |
+| Gallery.DeltaPorno.com                  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
+| GoFile                                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
+| Gfycat                                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
+| HGameCG                                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
+| ImgBox                                  | Albums: imgbox.com/g/... <br> Direct Images: images#.imgbox.com/... <br> Single Files: imgbox.com/...                                                                                                                                  |
+| IMG.Kiwi                                | Albums: img.kiwi/album/... <br> Direct Images: img.kiwi/image/... <br> User Profile: img.kiwi/#USER# <br> All User Albums: img.kiwi/#USER#/albums                                                                                      |
+| jpg.church<br/>jpg.fish<br/>jpg.fishing | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
+| LoveFap                                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
+| NSFW.XXX                                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
+| PimpAndHost                             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
+| PixelDrain                              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
+| Pixl                                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
+| Postimg.cc                              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
+| NudoStar                                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
+| SimpCity                                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
+| SocialMediaGirls                        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
+| XBunker                                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
+| XBunkr                                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
 
 Reminder to leave the link full (include the https://)
 
 ## Information
 
 **Requires Python 3.7 or higher (3.10 recommended)**
 
@@ -179,10 +179,14 @@
 --hide-overall-progress         removes overall progress section while downloading
 --hide-forum-progress           removes forum progress section while downloading
 --hide-thread-progress          removes thread progress section while downloading
 --hide-domain-progress          removes domain progress section while downloading
 --hide-album-progress           removes album progress section while downloading
 --hide-file-progress            removes file progress section while downloading
 --refresh-rate                  changes the refresh rate of the progress table
+--visible-rows-threads          number of visible rows to use for the threads table
+--visible-rows-domains          number of visible rows to use for the domains table
+--visible-rows-albums           number of visible rows to use for the albums table
+--visible-rows-files            number of visible rows to use for the files table
 ```
 
 `--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

#### html2text {}

```diff
@@ -13,20 +13,20 @@
 0d0b3680e83f.png) ## Support Cyberdrop-DL Development [Buy_Me_A_Coffee] If you
 want to support me and my effort you can buy me a coffee or send me some
 crypto: BTC: bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B XMR:
 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
 ## More Information Read the [Wiki](https://github.com/Jules-WinnfieldX/
 CyberDropDownloader/wiki/)! ## Supported Sites | Website | Supported Link Types
-| |-------------------------|--------------------------------------------------
+| |-----------------------------------------|----------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------------------------| | Anonfiles | Download page: Anonfiles.com/... | |
-Bayfiles | Download page: Bayfiles.com/... | | Bunkr (ru/su/la) | Albums:
-bunkr.ru/a/...
+----------------------------------------| | Anonfiles | Download page:
+Anonfiles.com/... | | Bayfiles | Download page: Bayfiles.com/... | | Bunkr (ru/
+su/la) | Albums: bunkr.ru/a/...
 Direct Videos: stream.bunkr.ru/v/...
 Direct links: cdn.bunkr.ru/...
 Direct links: i.bunkr.ru/...
 Direct links: files.bunkr.ru/...
 Direct links: media-files.bunkr.ru/... | | Coomer.party | Profiles:
 coomer.party/...
 Thumbnail Links: coomer.party/thumbnail/...
@@ -49,15 +49,16 @@
 gofile.io/d/... | | Gfycat | Gif: gfycat.com/... | | HGameCG | Albums:
 hgamecg.com/.../index.html | | ImgBox | Albums: imgbox.com/g/...
 Direct Images: images#.imgbox.com/...
 Single Files: imgbox.com/... | | IMG.Kiwi | Albums: img.kiwi/album/...
 Direct Images: img.kiwi/image/...
 User Profile: img.kiwi/#USER#
 All User Albums: img.kiwi/#USER#/albums | | jpg.church
-jpg.fish | Albums: jpg.church/album/...
+jpg.fish
+jpg.fishing | Albums: jpg.church/album/...
 Direct Images: jpg.church/image/...
 User Profile: jpg.church/#USER#
 All User Albums: jpg.church/#USER#/albums | | LoveFap | Albums: lovefap.com/
 a/...
 Direct Images: s*.lovefap.com/content/photos/...
 Videos: lovefap.com/video/... | | NSFW.XXX | Profile: nsfw.xxx/user/...
 Post: nsfw.xxx/post/... | | PimpAndHost | Albums: pimpandhost.com/album/...
@@ -155,14 +156,17 @@
 disables the new rich progress entirely and uses older methods --hide-overall-
 progress removes overall progress section while downloading --hide-forum-
 progress removes forum progress section while downloading --hide-thread-
 progress removes thread progress section while downloading --hide-domain-
 progress removes domain progress section while downloading --hide-album-
 progress removes album progress section while downloading --hide-file-progress
 removes file progress section while downloading --refresh-rate changes the
-refresh rate of the progress table ``` `--only-hosts` and `--skip-hosts` can
-use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
-"cyberfile", "e-hentai", "erome", "fapello", "gfycat",
-"gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
-"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
-"socialmediagirls", "xbunker", "xbunkr"`
+refresh rate of the progress table --visible-rows-threads number of visible
+rows to use for the threads table --visible-rows-domains number of visible rows
+to use for the domains table --visible-rows-albums number of visible rows to
+use for the albums table --visible-rows-files number of visible rows to use for
+the files table ``` `--only-hosts` and `--skip-hosts` can use: `"anonfiles",
+"bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai",
+"erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg",
+"img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap",
+"nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
+"saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,19 +37,14 @@
     }
 }
 
 logger = logging.getLogger(__name__)
 MAX_FILENAME_LENGTH = 95
 
 
-async def adjust(s: str, length: int = 40, placeholder: str = "...") -> str:
-    """Collapse and truncate or pad the given string to fit in the given length"""
-    return f"{s[:length - len(placeholder)]}{placeholder}" if len(s) >= length else s.ljust(length)
-
-
 async def clear() -> None:
     """Clears the terminal screen"""
     os.system('cls' if os.name == 'nt' else 'clear')
 
 
 def log(text: str, quiet: bool = False, style: str = "") -> None:
     """Logs to the output log file and optionally (by default) prints to the terminal with given style"""
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,18 @@
             "hide_overall_progress": False,
             "hide_forum_progress": False,
             "hide_thread_progress": False,
             "hide_domain_progress": False,
             "hide_album_progress": False,
             "hide_file_progress": False,
             "refresh_rate": 10,
+            "visible_rows_threads": 2,
+            "visible_rows_domains": 2,
+            "visible_rows_albums": 2,
+            "visible_rows_files": 10,
         },
         "Ratelimiting": {
             "connection_timeout": 15,
             "ratelimit": 50,
             "throttle": 0.5,
         },
         "Runtime": {
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,12 +232,12 @@
 
 @dataclass
 class SkipData:
     """The allows optoins for domains to skip when scraping"""
     supported_hosts: ClassVar[Tuple[str, ...]] = ("anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
                                                   "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gofile",
                                                   "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish",
-                                                  "gallery.deltaporno.com", "kemono.party",
+                                                  "jpg.fishing", "gallery.deltaporno.com", "kemono.party",
                                                   "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li",
                                                   "postimg", "saint", "nudostar", "simpcity", "socialmediagirls",
                                                   "xbunker", "xbunkr")
     sites: List[str]
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 import aiofiles
 import aiohttp
 import certifi
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 from yarl import URL
 
-from ..base_functions.base_functions import adjust, logger
+from ..base_functions.base_functions import logger
 from ..base_functions.error_classes import DownloadFailure, InvalidContentTypeFailure
 from ..downloader.downloader_utils import CustomHTTPStatus
-from ..downloader.progress_definitions import file_progress
+from ..downloader.progress_definitions import ProgressMaster, adjust_title
 from .rate_limiting import AsyncRateLimiter
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from rich.progress import TaskID
 
@@ -169,29 +169,30 @@
             if elapsed >= delay:
                 self.throttle_times[key] = now
                 return
 
             remaining = delay - elapsed + 0.1
             await asyncio.sleep(remaining)
 
-    async def download_file(self, media: MediaItem, file: Path, current_throttle: float, resume_point: int,
-                            proxy: str, headers: Dict, file_task: TaskID) -> None:
+    async def download_file(self, Progress_Master: ProgressMaster, media: MediaItem, file: Path,
+                            current_throttle: float, resume_point: int, proxy: str, headers: Dict,
+                            file_task: TaskID) -> None:
 
         async def save_content(content: aiohttp.StreamReader, size: int) -> None:
-            file_progress.update(file_task, total=size + resume_point)
-            file_progress.advance(file_task, resume_point)
-            await self._append_content(file, content, lambda chunk_len: file_progress.advance(file_task, chunk_len))
+            Progress_Master.FileProgress.update_file_length(file_task, size + resume_point)
+            Progress_Master.FileProgress.advance_file(file_task, resume_point)
+            await self._append_content(file, content, lambda chunk_len: Progress_Master.FileProgress.advance_file(file_task, chunk_len))
 
         await self._download(media, current_throttle, proxy, headers, save_content)
 
     async def old_download_file(self, media: MediaItem, file: Path, current_throttle: float, resume_point: int,
                                 proxy: str, headers: Dict):
 
         async def save_content(content: aiohttp.StreamReader, size: int) -> None:
-            task_description = await adjust(f"{media.url.host}: {media.filename}")
+            task_description = adjust_title(f"{media.url.host}: {media.filename}")
             with tqdm(total=size + resume_point, unit_scale=True, unit='B', leave=False,
                       initial=resume_point, desc=task_description) as progress:
                 await self._append_content(file, content, lambda chunk_len: progress.update(chunk_len))
 
         await self._download(media, current_throttle, proxy, headers, save_content)
 
     async def get_filesize(self, url: URL, referer: str, current_throttle: float) -> int:
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,22 +130,25 @@
             if not text:
                 text = await session.get_text(url)
                 assert text is not None
                 await self.SQL_Helper.insert_blob(text, url)
             soup = BeautifulSoup(text, 'html.parser')
 
             if self.separate_posts:
+                time_tag = soup.select_one("time[class*=timestamp]")
                 post_tag = soup.select_one("h1[class=post__title]")
                 assert post_tag is not None
+                assert time_tag is not None
                 post_title = post_tag.text.replace('\n', '').replace("..", "")
+                time = time_tag.text + " - "
                 prefix = f"{url.parts[-1]} - " if self.include_id else ""
                 if title:
-                    title = title + '/' + await make_title_safe(prefix + post_title)
+                    title = title + '/' + await make_title_safe(prefix + time + post_title)
                 else:
-                    title = await make_title_safe(prefix + post_title)
+                    title = await make_title_safe(prefix + time + post_title)
             elif not title:
                 post_tag = soup.select_one("h1[class=post__title]")
                 assert post_tag is not None
                 post_title = post_tag.text.replace('\n', '').replace("..", "")
                 title = await make_title_safe(post_title)
 
             images = soup.select('a[class="fileThumb"]')
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,16 @@
             await self.parse_profile(session, url, domain_obj)
 
         await self.SQL_Helper.insert_domain("sharex", url, domain_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return domain_obj
 
     async def jpg_fish_from_church(self, url: URL) -> URL:
-        pattern1 = r"simp([1-5])\.jpg\.fish/"
-        url = URL(re.sub(pattern1, r'simp\1.jpg.fishing/', str(url)))
         pattern2 = r"simp([1-5])\.jpg\.church/"
-        return URL(re.sub(pattern2, r'simp\1.jpg.fishing/', str(url)))
+        return URL(re.sub(pattern2, r'simp\1.jpg.fish/', str(url)))
 
     async def get_albums(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for Albums"""
         try:
             soup = await session.get_BS4(url)
             albums = soup.select("a[class='image-container --media']")
             for album in albums:
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,15 @@
             attachments_block = post.select_one(spec.attachment_block_tag)
             links.extend(await self.get_links(attachments_block, spec.attachment_tag, spec.attachment_attribute, domain))
 
             content_links.extend([(URL(link), temp_title) for link in links])
 
         # Handle links
         def is_direct_link(host: str) -> bool:
+            assert url.host is not None
             host_su = host.replace(".st", ".su")
             return host_su in url.host or url.host in host_su or "smgmedia" in host
 
         direct_links = [x for x in content_links if is_direct_link(x[0].host)]
         external_links = [x for x in content_links if x not in direct_links]
         await self.handle_direct_links(cascade, direct_links, url, spec.domain)
         await self.handle_external_links(external_links, url)
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,14 @@
                 return await f(self, *args, **kwargs)
             except DownloadFailure as e:
                 media = args[1]
                 url_path = args[2]
                 if not self.disable_attempt_limit and self.current_attempt[url_path] >= self.allowed_attempts - 1:
                     await self.output_failed(media, e)
                     logger.debug('Skipping %s...', media.url, exc_info=True)
-                    await self.files.add_failed()
+                    self.files.add_failed()
                     return None
                 logger.debug(e.message)
                 logger.debug(f'Retrying ({self.current_attempt[url_path]}) {media.url}...')
                 self.current_attempt[url_path] += 1
 
     return wrapper
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/downloader/downloaders.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import asyncio
 import contextlib
 import itertools
 import logging
 from http import HTTPStatus
 from pathlib import Path
 from random import gauss
-from typing import TYPE_CHECKING, Dict, Any, Tuple, Optional
+from typing import TYPE_CHECKING, Dict, Any, Tuple, Optional, Union
 
 import aiofiles
 import aiohttp.client_exceptions
 from rich.live import Live
 
 from cyberdrop_dl.base_functions.base_functions import (
-    adjust,
     clear,
     log,
     logger,
 )
 from cyberdrop_dl.base_functions.data_classes import (
     AlbumItem,
     CascadeItem,
@@ -37,261 +36,211 @@
     basic_auth,
     check_free_space,
     get_threads_number,
     is_4xx_client_error,
     retry,
 )
 from .progress_definitions import (
-    album_progress,
-    cascade_progress,
-    domain_progress,
-    file_progress,
-    forum_progress,
-    get_cascade_table,
-    get_forum_table,
-    overall_file_progress,
+    ProgressMaster, OverallFileProgress
 )
 
 if TYPE_CHECKING:
     from rich.progress import TaskID
 
 
-class Files:
-    """Class that keeps track of completed, skipped and failed files"""
+class CDLHelper:
+    def __init__(self, args: Dict, client: Client, files: OverallFileProgress, SQL_Helper: SQLHelper):
+        self.args = args
 
-    def __init__(self, total_files: int):
-        self.completed_files_task_id = overall_file_progress.add_task("[green]Completed", total=total_files)
-        self.completed_files = 0
-        self.skipped_files_task_id = overall_file_progress.add_task("[yellow]Skipped", total=total_files)
-        self.skipped_files = 0
-        self.failed_files_task_id = overall_file_progress.add_task("[red]Failed", total=total_files)
-        self.failed_files = 0
-
-    async def add_completed(self):
-        overall_file_progress.advance(self.completed_files_task_id, 1)
-        self.completed_files += 1
-
-    async def add_skipped(self):
-        overall_file_progress.advance(self.skipped_files_task_id, 1)
-        self.skipped_files += 1
-
-    async def add_failed(self):
-        overall_file_progress.advance(self.failed_files_task_id, 1)
-        self.failed_files += 1
-
-    async def hide(self):
-        overall_file_progress.update(self.completed_files_task_id, visible=False)
-        overall_file_progress.update(self.skipped_files_task_id, visible=False)
-        overall_file_progress.update(self.failed_files_task_id, visible=False)
-
-
-class Downloader:
-    """Downloader class, directs downloading for domain objects"""
-
-    def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper,
-                 domain: str, domain_obj: DomainItem, files: Files):
+        # CDL Objects
         self.client = client
-        self.download_session = DownloadSession(client)
-        self.File_Lock = FileLock()
-        self.SQL_Helper = SQL_Helper
-
-        self.domain = domain
-        self.domain_obj = domain_obj
-
-        self.errored_output = args['Runtime']['output_errored_urls']
-        self.errored_file = args['Files']['errored_urls_file']
-
         self.files = files
+        self.SQL_Helper = SQL_Helper
+        self.File_Lock = FileLock()
 
-        self.current_attempt: Dict[str, int] = {}
-        max_workers = get_threads_number(args, domain)
-        self._semaphore = asyncio.Semaphore(max_workers)
+        # Limits
         self.delay = {'cyberfile': 1.0, 'anonfiles': 1.0, "coomer": 0.2, "kemono": 0.2}
 
-        self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
-
+        # Exclude Args
         self.exclude_audio = args["Ignore"]["exclude_audio"]
         self.exclude_images = args["Ignore"]["exclude_images"]
         self.exclude_videos = args["Ignore"]["exclude_videos"]
         self.exclude_other = args["Ignore"]["exclude_other"]
 
+        # Runtime Args
         self.block_sub_folders = args['Runtime']['block_sub_folders']
         self.allowed_attempts = args["Runtime"]["attempts"]
         self.disable_attempt_limit = args["Runtime"]["disable_attempt_limit"]
         self.download_dir = args["Files"]["output_folder"]
         self.mark_downloaded = args["Runtime"]["skip_download_mark_completed"]
         self.proxy = args["Runtime"]["proxy"]
         self.required_free_space = args["Runtime"]["required_free_space"]
 
-    async def start_domain(self, cascade_task: TaskID) -> None:
-        """Handler for domains and the progress bars for it"""
-        domain_task = domain_progress.add_task("[light_pink3]" + self.domain.upper(), total=len(self.domain_obj.albums))
-        for album, album_obj in self.domain_obj.albums.items():
-            await self.start_album(domain_task, album, album_obj)
-        cascade_progress.advance(cascade_task, 1)
-        domain_progress.update(domain_task, visible=False)
-        await self.download_session.exit_handler()
+        # Output Args
+        self.errored_output = args['Runtime']['output_errored_urls']
+        self.errored_file = args['Files']['errored_urls_file']
 
-    async def start_album(self, domain_task: TaskID, album: str, album_obj: AlbumItem) -> None:
-        """Handler for albums and the progress bars for it"""
-        if await album_obj.is_empty():
-            return
-        task_description = album.split('/')[-1]
-        task_description = task_description.encode("ascii", "ignore").decode().strip()
-        task_description = await adjust(task_description)
-        album_task = album_progress.add_task("[pink3]" + task_description.upper(), total=len(album_obj.media))
-        download_tasks = []
-        for media in album_obj.media:
-            download_tasks.append(self.start_file(album_task, album, media))
-        await asyncio.gather(*download_tasks)
-        album_progress.update(album_task, visible=False)
-        domain_progress.advance(domain_task, 1)
+        # API Keys
+        self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
-    async def start_file(self, album_task: TaskID, album: str, media: MediaItem) -> None:
-        """Handler for files and the progress bars for it"""
-        if media.complete or await self.SQL_Helper.check_complete_singular(self.domain, media.url):
-            log(f"Previously Downloaded: {media.filename}", quiet=True)
-            await self.files.add_skipped()
-            album_progress.advance(album_task, 1)
-            return
+    def get_throttle(self, domain: str) -> float:
+        """Get the throttle for a domain"""
+        if domain in self.delay:
+            return self.delay[domain]
+        else:
+            return self.client.throttle
+
+
+class Downloader:
+    """Downloader class, directs downloading for domain objects"""
+
+    def __init__(self, domain: str, CDL_Helper: CDLHelper, Progress_Master: ProgressMaster):
+        self.domain = domain
+        self.throttle = CDL_Helper.get_throttle(domain)
+
+        max_workers = get_threads_number(CDL_Helper.args, domain)
+        self._semaphore = asyncio.Semaphore(max_workers)
+        self.current_attempt: Dict[str, int] = {}
+
+        self.download_session = DownloadSession(CDL_Helper.client)
+
+        self.CDL_Helper = CDL_Helper
+        self.files = CDL_Helper.files
+        self.Progress_Master = Progress_Master
+        self.disable_attempt_limit = CDL_Helper.disable_attempt_limit
+        self.allowed_attempts = CDL_Helper.allowed_attempts
+
+    async def download(self, album: str, media: MediaItem, url_path: str, album_task: TaskID) -> None:
         async with self._semaphore:
-            url_path = await get_db_path(media.url, self.domain)
             await self.download_file(album, media, url_path, album_task)
 
     @retry
     async def download_file(self, album: str, media: MediaItem, url_path: str, album_task: TaskID) -> None:
         """File downloader"""
-        if not await check_free_space(self.required_free_space, self.download_dir):
+        if not await check_free_space(self.CDL_Helper.required_free_space, self.CDL_Helper.download_dir):
             log("We've run out of free space.", quiet=True)
-            await self.files.add_skipped()
-            album_progress.advance(album_task, 1)
+            self.CDL_Helper.files.add_skipped()
+            self.Progress_Master.AlbumProgress.advance_album(album_task)
             return
 
-        if not await allowed_filetype(media, self.exclude_images, self.exclude_videos, self.exclude_audio,
-                                      self.exclude_other):
+        if not await allowed_filetype(media, self.CDL_Helper.exclude_images, self.CDL_Helper.exclude_videos,
+                                      self.CDL_Helper.exclude_audio, self.CDL_Helper.exclude_other):
             log(f"Blocked by file extension: {media.filename}", quiet=True)
-            await self.files.add_skipped()
-            album_progress.advance(album_task, 1)
+            self.CDL_Helper.files.add_skipped()
+            self.Progress_Master.AlbumProgress.advance_album(album_task)
             return
 
-        if self.block_sub_folders:
+        if self.CDL_Helper.block_sub_folders:
             album = album.split('/')[0]
 
         original_filename = media.original_filename
         filename = media.filename
 
         try:
-            while await self.File_Lock.check_lock(filename):
+            while await self.CDL_Helper.File_Lock.check_lock(filename):
                 await asyncio.sleep(gauss(1, 1.5))
-            await self.File_Lock.add_lock(filename)
+            await self.CDL_Helper.File_Lock.add_lock(filename)
 
             if url_path not in self.current_attempt:
                 self.current_attempt[url_path] = 0
 
-            current_throttle = self.client.throttle
-
-            complete_file = (self.download_dir / album / media.filename)
+            complete_file = (self.CDL_Helper.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
             fake_download = False
-            if self.mark_downloaded:
+            if self.CDL_Helper.mark_downloaded:
                 fake_download = True
 
             complete_file, partial_file, proceed = await self.check_file_exists(complete_file, partial_file, media,
                                                                                 album, url_path, original_filename,
-                                                                                current_throttle)
+                                                                                self.throttle)
             if not proceed:
                 fake_download = True
 
-            await self.SQL_Helper.update_pre_download(complete_file, media.filename, url_path, original_filename)
+            await self.CDL_Helper.SQL_Helper.update_pre_download(complete_file, media.filename, url_path,
+                                                                 original_filename)
 
             resume_point = 0
-            await self.SQL_Helper.sql_insert_temp(str(partial_file))
+            await self.CDL_Helper.SQL_Helper.sql_insert_temp(str(partial_file))
             range_num = None
             if partial_file.exists():
                 resume_point = partial_file.stat().st_size
                 range_num = f'bytes={resume_point}-'
 
             assert media.url.host is not None
-            for key, value in self.delay.items():
-                if key in media.url.host:
-                    current_throttle = value
-
-            headers = {"Authorization": await basic_auth("Cyberdrop-DL", self.pixeldrain_api_key)} \
-                if (self.pixeldrain_api_key and "pixeldrain" in media.url.host) else {}
+            headers = {"Authorization": await basic_auth("Cyberdrop-DL", self.CDL_Helper.pixeldrain_api_key)} \
+                if (self.CDL_Helper.pixeldrain_api_key and "pixeldrain" in media.url.host) else {}
             if range_num:
                 headers['Range'] = range_num
 
-            task_description = media.filename.encode("ascii", "ignore").decode().strip()
-            task_description = await adjust(task_description)
-            file_task = file_progress.add_task("[plum3]" + task_description, progress_type="file")
-
-            if not await self.SQL_Helper.sql_check_old_existing(url_path) and not fake_download:
-                await self.download_session.download_file(media, partial_file, current_throttle, resume_point,
-                                                          self.proxy, headers, file_task)
+            file_task = self.Progress_Master.FileProgress.add_file(media.filename)
+
+            if not await self.CDL_Helper.SQL_Helper.sql_check_old_existing(url_path) and not fake_download:
+                await self.download_session.download_file(self.Progress_Master, media, partial_file, self.throttle,
+                                                          resume_point, self.CDL_Helper.proxy, headers, file_task)
                 partial_file.rename(complete_file)
 
-            await self.SQL_Helper.mark_complete(url_path, original_filename)
+            await self.CDL_Helper.SQL_Helper.mark_complete(url_path, original_filename)
             if media.url.parts[-1] in self.current_attempt:
                 self.current_attempt.pop(media.url.parts[-1])
 
             if fake_download:
                 log(f"Already Downloaded: {media.filename} from {media.referer}", quiet=True)
-                await self.files.add_skipped()
+                self.CDL_Helper.files.add_skipped()
             else:
-                await self.files.add_completed()
-            album_progress.advance(album_task, 1)
-            file_progress.update(file_task, visible=False)
+                self.CDL_Helper.files.add_completed()
+            self.Progress_Master.FileProgress.mark_file_completed(file_task)
 
             log(f"Completed Download: {media.filename} from {media.referer}", quiet=True)
-            await self.File_Lock.remove_lock(filename)
+            await self.CDL_Helper.File_Lock.remove_lock(filename)
             return
 
         except (aiohttp.client_exceptions.ClientPayloadError, aiohttp.client_exceptions.ClientOSError,
                 aiohttp.client_exceptions.ServerDisconnectedError, asyncio.TimeoutError,
                 aiohttp.client_exceptions.ClientResponseError, aiohttp.client_exceptions.ServerTimeoutError,
                 DownloadFailure, FileNotFoundError, PermissionError) as e:
-            if await self.File_Lock.check_lock(filename):
-                await self.File_Lock.remove_lock(filename)
+            if await self.CDL_Helper.File_Lock.check_lock(filename):
+                await self.CDL_Helper.File_Lock.remove_lock(filename)
 
             with contextlib.suppress(Exception):
-                file_progress.update(file_task, visible=False)
+                self.Progress_Master.FileProgress.remove_file(file_task)
 
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
                     logger.debug("We ran into a 400 level error: %s", e.code)
                     log(f"Failed Download: {media.filename}", quiet=True)
-                    await self.files.add_failed()
+                    self.CDL_Helper.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
+
                 if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == HTTPStatus.BAD_GATEWAY \
                         or e.code == CustomHTTPStatus.WEB_SERVER_IS_DOWN:
                     if hasattr(e, "message"):
                         if not e.message:
                             e.message = "Web server is down"
                         logging.debug(f"\n{media.url} ({e.message})")
                     log(f"Failed Download: {media.filename}", quiet=True)
-                    await self.files.add_failed()
+                    self.CDL_Helper.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
 
                 logger.debug("Error status code: %s", e.code)
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
     async def output_failed(self, media: MediaItem, e: Any) -> None:
-        if self.errored_output:
-            async with aiofiles.open(self.errored_file, mode='a') as file:
+        if self.CDL_Helper.errored_output:
+            async with aiofiles.open(self.CDL_Helper.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
 
     async def check_file_exists(self, complete_file: Path, partial_file: Path, media: MediaItem, album: str,
                                 url_path: str, original_filename: str, current_throttle: float):
         """Complicated checker for if a file already exists, and was already downloaded"""
         expected_size = None
         proceed = True
@@ -302,15 +251,15 @@
             if not expected_size:
                 expected_size = await self.download_session.get_filesize(media.url, str(media.referer),
                                                                          current_throttle)
             if complete_file.exists() and complete_file.stat().st_size == expected_size:
                 proceed = False
                 break
 
-            downloaded_filename = await self.SQL_Helper.get_downloaded_filename(url_path, original_filename)
+            downloaded_filename = await self.CDL_Helper.SQL_Helper.get_downloaded_filename(url_path, original_filename)
             if not downloaded_filename:
                 complete_file, partial_file = await self.iterate_filename(complete_file, media, album)
                 break
 
             if media.filename == downloaded_filename:
                 if partial_file.exists():
                     if partial_file.stat().st_size == expected_size:
@@ -320,70 +269,117 @@
                     if complete_file.stat().st_size == expected_size:
                         proceed = False
                     else:
                         complete_file, partial_file = await self.iterate_filename(complete_file, media, album)
                 break
 
             media.filename = downloaded_filename
-            complete_file = (self.download_dir / album / media.filename)
+            complete_file = (self.CDL_Helper.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
         return complete_file, partial_file, proceed
 
     async def iterate_filename(self, complete_file: Path, media: MediaItem, album: str) -> Tuple[Path, Path]:
         for iterations in itertools.count(1):
             filename = f"{complete_file.stem} ({iterations}){media.ext}"
-            temp_complete_file = (self.download_dir / album / filename)
-            if not temp_complete_file.exists() and not await self.SQL_Helper.check_filename(filename):
+            temp_complete_file = (self.CDL_Helper.download_dir / album / filename)
+            if not temp_complete_file.exists() and not await self.CDL_Helper.SQL_Helper.check_filename(filename):
                 media.filename = filename
-                complete_file = (self.download_dir / album / media.filename)
+                complete_file = (self.CDL_Helper.download_dir / album / media.filename)
                 partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
                 break
         return complete_file, partial_file
 
 
-async def download_cascade(args: Dict, Cascade: CascadeItem, SQL_Helper: SQLHelper, client: Client) -> None:
-    """Handler for cascades and the progress bars for it"""
-    progress_table = await get_cascade_table(args["Progress_Options"])
-    total_files = await Cascade.get_total()
-    files = Files(total_files)
-    with Live(progress_table, refresh_per_second=args["Progress_Options"]["refresh_rate"]):
-        cascade_task = cascade_progress.add_task("[light_salmon3]Domains", progress_type="cascade",
-                                                 total=len(Cascade.domains))
-
-        tasks = []
+class DownloadManager:
+    def __init__(self, CDL_Helper: CDLHelper, Progress_Master: ProgressMaster):
+        self.downloaders: Dict[str, Downloader] = {}
+        self.CDL_Helper = CDL_Helper
+        self.Progress_Master = Progress_Master
+
+    async def create_downloader(self, domain: str):
+        if domain in self.downloaders:
+            return self.downloaders[domain]
+        else:
+            new_downloader = Downloader(domain, self.CDL_Helper, self.Progress_Master)
+            self.downloaders[domain] = new_downloader
+            return new_downloader
+
+    async def get_downloader(self, domain: str):
+        if domain not in self.downloaders:
+            return await self.create_downloader(domain)
+        return self.downloaders[domain]
+
+
+class DownloadDirector:
+    def __init__(self, args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client):
+        self.Progress_Master = ProgressMaster(args["Progress_Options"])
+        self.CDL_Helper = CDLHelper(args, client, self.Progress_Master.OverallFileProgress, SQL_Helper)
+
+        self.Download_Manager = DownloadManager(self.CDL_Helper, self.Progress_Master)
+
+        self.Forums = Forums
+
+    async def start(self):
+        self.CDL_Helper.files.update_total(await self.Forums.get_total())
+
+        progress_table = await self.Progress_Master.get_table()
+        with Live(progress_table, refresh_per_second=self.Progress_Master.refresh_rate):
+            forum_task = self.Progress_Master.ForumProgress.add_forum(len(self.Forums.threads))
+            cascade_tasks = []
+            for title, Cascade in self.Forums.threads.items():
+                cascade_tasks.append(self.start_cascade(forum_task, title, Cascade))
+            await asyncio.gather(*cascade_tasks)
+
+        await clear()
+        completed_files, skipped_files, failed_files = self.Progress_Master.OverallFileProgress.return_totals()
+        log(f"| [green]Files Complete: {completed_files}[/green] - [yellow]Files Skipped:  {skipped_files}[/yellow] - [red]Files Failed: {failed_files}[/red] |")
+
+        for downloader in self.Download_Manager.downloaders.values():
+            await downloader.close()
+
+    async def start_cascade(self, forum_task: TaskID, title: str, Cascade: CascadeItem) -> None:
+        cascade_task = self.Progress_Master.CascadeProgress.add_cascade(title, len(Cascade.domains))
+        domain_tasks = []
         for domain, domain_obj in Cascade.domains.items():
-            downloader = Downloader(args, client, SQL_Helper, domain, domain_obj, files)
-            tasks.append(downloader.start_domain(cascade_task))
-        await asyncio.gather(*tasks)
-
-        cascade_progress.update(cascade_task, visible=False)
-
-    await files.hide()
-
-    await clear()
-    log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
-              f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
-
-
-async def download_forums(args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client) -> None:
-    """Handler for forum threads and the progress bars for it"""
-    progress_table = await get_forum_table(args["Progress_Options"])
-    total_files = await Forums.get_total()
-    files = Files(total_files)
-    with Live(progress_table, refresh_per_second=args["Progress_Options"]["refresh_rate"]):
-        forum_task = forum_progress.add_task("[orange3]FORUM THREADS", total=len(Forums.threads))
-        for title, Cascade in Forums.threads.items():
-            cascade_task = cascade_progress.add_task("[light_salmon3]" + title.upper(), total=len(Cascade.domains))
-
-            tasks = []
-            for domain, domain_obj in Cascade.domains.items():
-                downloader = Downloader(args, client, SQL_Helper, domain, domain_obj, files)
-                tasks.append(downloader.start_domain(cascade_task))
-            await asyncio.gather(*tasks)
-
-            cascade_progress.update(cascade_task, visible=False)
-            forum_progress.advance(forum_task, 1)
-
-    await clear()
-    log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
-              f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
+            domain_tasks.append(self.start_domain(cascade_task, title, domain, domain_obj))
+        await asyncio.gather(*domain_tasks)
+        self.Progress_Master.CascadeProgress.mark_cascade_completed(cascade_task)
+        self.Progress_Master.ForumProgress.advance_forum(forum_task)
+
+    async def start_domain(self, cascade_task: TaskID, title: str, domain: str, domain_obj: DomainItem) -> None:
+        """Handler for domains and the progress bars for it"""
+        downloader = await self.Download_Manager.get_downloader(domain)
+
+        domain_task = self.Progress_Master.DomainProgress.add_domain(domain, len(domain_obj.albums))
+        album_tasks = []
+        for album, album_obj in domain_obj.albums.items():
+            album_tasks.append(self.start_album(downloader, domain_task, domain, album, album_obj))
+        await asyncio.gather(*album_tasks)
+        self.Progress_Master.CascadeProgress.advance_cascade(cascade_task)
+        self.Progress_Master.DomainProgress.mark_domain_completed(domain, domain_task)
+
+    async def start_album(self, downloader: Downloader, domain_task: TaskID, domain: str, album: str,
+                          album_obj: AlbumItem) -> None:
+        """Handler for albums and the progress bars for it"""
+        if await album_obj.is_empty():
+            return
+
+        album_task = self.Progress_Master.AlbumProgress.add_album(album, len(album_obj.media))
+        download_tasks = []
+        for media in album_obj.media:
+            download_tasks.append(self.start_file(downloader, album_task, domain, album, media))
+        await asyncio.gather(*download_tasks)
+        self.Progress_Master.DomainProgress.advance_domain(domain_task)
+        self.Progress_Master.AlbumProgress.mark_album_completed(album_task)
+
+    async def start_file(self, downloader: Downloader, album_task: TaskID, domain: str, album: str, media: MediaItem) -> None:
+        """Handler for files and the progress bars for it"""
+        if media.complete or await self.CDL_Helper.SQL_Helper.check_complete_singular(domain, media.url):
+            log(f"Previously Downloaded: {media.filename}", quiet=True)
+            self.CDL_Helper.files.add_skipped()
+            self.Progress_Master.AlbumProgress.advance_album(album_task)
+            return
+
+        url_path = await get_db_path(media.url, domain)
+        await downloader.download(album, media, url_path, album_task)
+        self.Progress_Master.AlbumProgress.advance_album(album_task)
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from tqdm import tqdm
 
 from cyberdrop_dl.base_functions.base_functions import (
     clear,
     log,
     logger,
 )
-from cyberdrop_dl.base_functions.data_classes import AlbumItem, CascadeItem, DomainItem, FileLock, ForumItem, MediaItem
+from cyberdrop_dl.base_functions.data_classes import AlbumItem, DomainItem, FileLock, ForumItem, MediaItem
 from cyberdrop_dl.base_functions.error_classes import DownloadFailure
 from cyberdrop_dl.base_functions.sql_helper import SQLHelper, get_db_path
 from cyberdrop_dl.client.client import Client, DownloadSession
 
 from .downloader_utils import (
     CustomHTTPStatus,
     allowed_filetype,
@@ -38,23 +38,23 @@
 
     def __init__(self, progress: tqdm):
         self.progress = progress
         self.completed_files = 0
         self.skipped_files = 0
         self.failed_files = 0
 
-    async def add_completed(self) -> None:
+    def add_completed(self) -> None:
         self.completed_files += 1
         self.progress.update(1)
 
-    async def add_skipped(self) -> None:
+    def add_skipped(self) -> None:
         self.skipped_files += 1
         self.progress.update(1)
 
-    async def add_failed(self) -> None:
+    def add_failed(self) -> None:
         self.failed_files += 1
         self.progress.update(1)
 
 
 class Old_Downloader:
     """Downloader class, directs downloading for domain objects"""
 
@@ -108,32 +108,32 @@
             download_tasks.append(self.start_file(album, media))
         await asyncio.gather(*download_tasks)
 
     async def start_file(self, album: str, media: MediaItem) -> None:
         """Handler for files and the progress bars for it"""
         if media.complete or await self.SQL_Helper.check_complete_singular(self.domain, media.url):
             log(f"Previously Downloaded: {media.filename}", quiet=True)
-            await self.files.add_skipped()
+            self.files.add_skipped()
             return
         async with self._semaphore:
             url_path = await get_db_path(media.url, self.domain)
             await self.download_file(album, media, url_path)
 
     @retry
     async def download_file(self, album: str, media: MediaItem, url_path: str) -> None:
         """File downloader"""
         if not await check_free_space(self.required_free_space, self.download_dir):
             log("We've run out of free space.", quiet=True)
-            await self.files.add_skipped()
+            self.files.add_skipped()
             return
 
         if not await allowed_filetype(media, self.exclude_images, self.exclude_videos, self.exclude_audio,
                                       self.exclude_other):
             log(f"Blocked by file extension: {media.filename}", quiet=True)
-            await self.files.add_skipped()
+            self.files.add_skipped()
             return
 
         if self.block_sub_folders:
             album = album.split('/')[0]
 
         try:
             while await self.File_Lock.check_lock(media.filename):
@@ -184,17 +184,17 @@
                 partial_file.rename(complete_file)
 
             await self.SQL_Helper.mark_complete(url_path, original_filename)
             if media.url.parts[-1] in self.current_attempt:
                 self.current_attempt.pop(media.url.parts[-1])
 
             if fake_download:
-                await self.files.add_skipped()
+                self.files.add_skipped()
             else:
-                await self.files.add_completed()
+                self.files.add_completed()
 
             log(f"Completed Download: {media.filename} from {media.referer}", quiet=True)
             await self.File_Lock.remove_lock(original_filename)
             return
 
         except (aiohttp.client_exceptions.ClientPayloadError, aiohttp.client_exceptions.ClientOSError,
                 aiohttp.client_exceptions.ServerDisconnectedError, asyncio.TimeoutError,
@@ -206,26 +206,26 @@
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
                     logger.debug("We ran into a 400 level error: %s", e.code)
                     log(f"Failed Download: {media.filename}", quiet=True)
-                    await self.files.add_failed()
+                    self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
                 if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == CustomHTTPStatus.WEB_SERVER_IS_DOWN:
                     if hasattr(e, "message"):
                         if not e.message:
                             e.message = "Web server is down"
                         logging.debug(f"\n{media.url} ({e.message})")
                     log(f"Failed Download: {media.filename}", quiet=True)
-                    await self.files.add_failed()
+                    self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
                 logger.debug("Error status code: %s", e.code)
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
@@ -275,31 +275,14 @@
             media.filename = downloaded_filename
             complete_file = (self.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
         return complete_file, partial_file, proceed
 
 
-async def old_download_cascade(args: dict, Cascade: CascadeItem, SQL_Helper: SQLHelper, client: Client) -> None:
-    """Handler for cascades and the progress bars for it"""
-    total_files = await Cascade.get_total()
-    with tqdm(total=total_files, unit_scale=True, unit='Files', leave=True, initial=0,
-              desc="Files Downloaded") as progress:
-        files = Files(progress)
-        tasks = []
-        for domain, domain_obj in Cascade.domains.items():
-            downloader = Old_Downloader(args, client, SQL_Helper, domain, domain_obj, files)
-            tasks.append(downloader.start_domain())
-        await asyncio.gather(*tasks)
-
-    await clear()
-    log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
-              f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
-
-
 async def old_download_forums(args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client) -> None:
     """Handler for forum threads and the progress bars for it"""
     total_files = await Forums.get_total()
     with tqdm(total=total_files, unit_scale=True, unit='Files', leave=True, initial=0,
               desc="Files Downloaded") as progress:
         files = Files(progress)
         for title, Cascade in Forums.threads.items():
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from cyberdrop_dl.base_functions.base_functions import clear, log, purge_dir
 from cyberdrop_dl.base_functions.config_manager import document_args, run_args
 from cyberdrop_dl.base_functions.config_schema import config_default
 from cyberdrop_dl.base_functions.sorting_functions import Sorter
 from cyberdrop_dl.base_functions.sql_helper import SQLHelper
 from cyberdrop_dl.client.client import Client
 from cyberdrop_dl.downloader.downloader_utils import check_free_space
-from cyberdrop_dl.downloader.downloaders import download_cascade, download_forums
-from cyberdrop_dl.downloader.old_downloaders import old_download_cascade, old_download_forums
+from cyberdrop_dl.downloader.downloaders import DownloadDirector
+from cyberdrop_dl.downloader.old_downloaders import old_download_forums
 from cyberdrop_dl.scraper.Scraper import ScrapeMapper
 
 from . import __version__ as VERSION
 from .base_functions.data_classes import CascadeItem, ForumItem, SkipData
 
 
 def parse_args() -> argparse.Namespace:
@@ -133,14 +133,18 @@
     progress_opts.add_argument("--hide-overall-progress", help="removes overall progress section while downloading", action="store_true")
     progress_opts.add_argument("--hide-forum-progress", help="removes forum progress section while downloading", action="store_true")
     progress_opts.add_argument("--hide-thread-progress", help="removes thread progress section while downloading", action="store_true")
     progress_opts.add_argument("--hide-domain-progress", help="removes domain progress section while downloading", action="store_true")
     progress_opts.add_argument("--hide-album-progress", help="removes album progress section while downloading", action="store_true")
     progress_opts.add_argument("--hide-file-progress", help="removes file progress section while downloading", action="store_true")
     progress_opts.add_argument("--refresh-rate", type=int, help="refresh rate for the progress table (default: %(default)s)", default=config_group["refresh_rate"])
+    progress_opts.add_argument("--visible-rows-threads", type=int, help="number of visible rows to use for the threads table (default: %(default)s)", default=config_group["visible_rows_threads"])
+    progress_opts.add_argument("--visible-rows-domains", type=int, help="number of visible rows to use for the domains table (default: %(default)s)", default=config_group["visible_rows_domains"])
+    progress_opts.add_argument("--visible-rows-albums", type=int, help="number of visible rows to use for the albums table (default: %(default)s)", default=config_group["visible_rows_albums"])
+    progress_opts.add_argument("--visible-rows-files", type=int, help="number of visiblerows to use for the files table (default: %(default)s)", default=config_group["visible_rows_files"])
 
     # Links
     parser.add_argument("links", metavar="link", nargs="*", help="link to content to download (passing multiple links is supported)", default=[])
     return parser.parse_args()
 
 
 async def file_management(args: Dict, links: List) -> None:
@@ -198,31 +202,34 @@
     links = list(filter(None, links))
 
     if not links:
         log("No valid links found.", style="red")
     return links
 
 
-async def scrape_links(scraper: ScrapeMapper, links: List, quiet=False) -> Tuple[CascadeItem, ForumItem]:
+async def scrape_links(scraper: ScrapeMapper, links: List, quiet=False) -> ForumItem:
     """Maps links from URLs.txt or command to the scraper class"""
     log("Starting Scrape", quiet=quiet, style="green")
     tasks = []
 
     for link in links:
         tasks.append(asyncio.create_task(scraper.map_url(link)))
     await asyncio.wait(tasks)
 
     Cascade = scraper.Cascade
     await Cascade.dedupe()
     Forums = scraper.Forums
     await Forums.dedupe()
 
+    if not await Cascade.is_empty():
+        await Forums.add_thread("Loose Files/Albums", Cascade)
+
     log("", quiet=quiet)
     log("Finished Scrape", quiet=quiet, style="green")
-    return Cascade, Forums
+    return Forums
 
 
 async def director(args: Dict, links: List) -> None:
     """This is the overarching director coordinator for CDL."""
     await clear()
     await document_args(args)
     await file_management(args, links)
@@ -238,28 +245,25 @@
                     args['Runtime']['user_agent'])
     SQL_Helper = SQLHelper(args['Ignore']['ignore_history'], args['Ignore']['ignore_cache'], args['Files']['db_file'])
     Scraper = ScrapeMapper(args, client, SQL_Helper, False)
 
     await SQL_Helper.sql_initialize()
 
     if links:
-        Cascade, Forums = await scrape_links(Scraper, links)
+        Forums = await scrape_links(Scraper, links)
         await asyncio.sleep(5)
         await clear()
 
         if args['Progress_Options']['hide_new_progress']:
-            if not await Cascade.is_empty():
-                await old_download_cascade(args, Cascade, SQL_Helper, client)
             if not await Forums.is_empty():
                 await old_download_forums(args, Forums, SQL_Helper, client)
         else:
-            if not await Cascade.is_empty():
-                await download_cascade(args, Cascade, SQL_Helper, client)
             if not await Forums.is_empty():
-                await download_forums(args, Forums, SQL_Helper, client)
+                download_director = DownloadDirector(args, Forums, SQL_Helper, client)
+                await download_director.start()
 
     if args['Files']['output_folder'].is_dir():
         if args['Sorting']['sort_downloads']:
             log("")
             log("Sorting Downloads")
             sorter = Sorter(args['Files']['output_folder'], args['Sorting']['sort_directory'],
                             args['Sorting']['sorted_audio'], args['Sorting']['sorted_images'],
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.1/cyberdrop_dl/scraper/Scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.include_id = args['Runtime']['include_id']
         self.remove_bunkr_id = args['Runtime']['remove_bunkr_identifier']
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.quiet = quiet
         self.jdownloader = JDownloader(args['JDownloader'], quiet)
 
-        self.bunkr_limiter = AsyncRateLimiter(10)
+        self.bunkr_limiter = AsyncRateLimiter(4)
         self.coomer_limiter = AsyncRateLimiter(8)
         self.gofile_limiter = AsyncRateLimiter(max_calls=1, period=3)
         self.jpgfish_limiter = AsyncRateLimiter(10)
         self.kemono_limiter = AsyncRateLimiter(8)
 
         self.coomer_semaphore = asyncio.Semaphore(1)
         self.cyberfile_semaphore = asyncio.Semaphore(2)
@@ -358,15 +358,15 @@
     """URL to Function Mapper"""
 
     async def is_skip_host(self, host: str) -> bool:
         if self.only_data.sites:
             return not any(site in host for site in self.only_data.sites)
         return any(site in host for site in self.skip_data.sites)
 
-    async def map_url(self, url_to_map: URL, title=None, referer: URL = None):
+    async def map_url(self, url_to_map: URL, title=None, referer: Optional[URL] = None):
         if not url_to_map:
             return
         if not url_to_map.host:
             log(f"Not Supported: {url_to_map}", quiet=self.quiet, style="yellow")
             return
 
         key = next((key for key in self.mapping if key in url_to_map.host), None)
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.1/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.25
+Version: 4.2.1
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -39,43 +39,43 @@
 
 ## More Information
 
 Read the [Wiki](https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/)!
 
 ## Supported Sites
 
-| Website                 | Supported Link Types                                                                                                                                                                                                                   |
-|-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Anonfiles               | Download page: Anonfiles.com/...                                                                                                                                                                                                       |
-| Bayfiles                | Download page: Bayfiles.com/...                                                                                                                                                                                                        |
-| Bunkr (ru/su/la)        | Albums: bunkr.ru/a/... <br> Direct Videos: stream.bunkr.ru/v/... <br> Direct links: cdn.bunkr.ru/... <br> Direct links: i.bunkr.ru/... <br> Direct links: files.bunkr.ru/... <br> Direct links: media-files.bunkr.ru/...               |
-| Coomer.party            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      |
-| Cyberdrop               | Albums: cyberdrop.me/a/... <br> Direct Videos: fs-0#.cyberdrop.me/... <br> Direct Videos: f.cyberdrop.me/... <br> Direct Images: img-0#.cyberdrop.me/... <br> Direct Images: f.cyberdrop.me/... <br> Also works with .cc, .to, and .nl |
-| Cyberfile               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    |
-| E-Hentai                | Albums: e-hentai.org/g/... <br> Posts: e-hentai.org/s/...                                                                                                                                                                              |
-| Erome                   | Albums: erome.com/a/...                                                                                                                                                                                                                |
-| Fapello                 | Models: fapello.com/...                                                                                                                                                                                                                |
-| Gallery.DeltaPorno.com  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
-| GoFile                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
-| Gfycat                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
-| HGameCG                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
-| ImgBox                  | Albums: imgbox.com/g/... <br> Direct Images: images#.imgbox.com/... <br> Single Files: imgbox.com/...                                                                                                                                  |
-| IMG.Kiwi                | Albums: img.kiwi/album/... <br> Direct Images: img.kiwi/image/... <br> User Profile: img.kiwi/#USER# <br> All User Albums: img.kiwi/#USER#/albums                                                                                      |
-| jpg.church<br/>jpg.fish | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
-| LoveFap                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
-| NSFW.XXX                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
-| PimpAndHost             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
-| PixelDrain              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
-| Pixl                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
-| Postimg.cc              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
-| NudoStar                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
-| SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
-| SocialMediaGirls        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
-| XBunker                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
-| XBunkr                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
+| Website                                 | Supported Link Types                                                                                                                                                                                                                   |
+|-----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Anonfiles                               | Download page: Anonfiles.com/...                                                                                                                                                                                                       |
+| Bayfiles                                | Download page: Bayfiles.com/...                                                                                                                                                                                                        |
+| Bunkr (ru/su/la)                        | Albums: bunkr.ru/a/... <br> Direct Videos: stream.bunkr.ru/v/... <br> Direct links: cdn.bunkr.ru/... <br> Direct links: i.bunkr.ru/... <br> Direct links: files.bunkr.ru/... <br> Direct links: media-files.bunkr.ru/...               |
+| Coomer.party                            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      |
+| Cyberdrop                               | Albums: cyberdrop.me/a/... <br> Direct Videos: fs-0#.cyberdrop.me/... <br> Direct Videos: f.cyberdrop.me/... <br> Direct Images: img-0#.cyberdrop.me/... <br> Direct Images: f.cyberdrop.me/... <br> Also works with .cc, .to, and .nl |
+| Cyberfile                               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    |
+| E-Hentai                                | Albums: e-hentai.org/g/... <br> Posts: e-hentai.org/s/...                                                                                                                                                                              |
+| Erome                                   | Albums: erome.com/a/...                                                                                                                                                                                                                |
+| Fapello                                 | Models: fapello.com/...                                                                                                                                                                                                                |
+| Gallery.DeltaPorno.com                  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
+| GoFile                                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
+| Gfycat                                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
+| HGameCG                                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
+| ImgBox                                  | Albums: imgbox.com/g/... <br> Direct Images: images#.imgbox.com/... <br> Single Files: imgbox.com/...                                                                                                                                  |
+| IMG.Kiwi                                | Albums: img.kiwi/album/... <br> Direct Images: img.kiwi/image/... <br> User Profile: img.kiwi/#USER# <br> All User Albums: img.kiwi/#USER#/albums                                                                                      |
+| jpg.church<br/>jpg.fish<br/>jpg.fishing | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
+| LoveFap                                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
+| NSFW.XXX                                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
+| PimpAndHost                             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
+| PixelDrain                              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
+| Pixl                                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
+| Postimg.cc                              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
+| NudoStar                                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
+| SimpCity                                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
+| SocialMediaGirls                        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
+| XBunker                                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
+| XBunkr                                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
 
 Reminder to leave the link full (include the https://)
 
 ## Information
 
 **Requires Python 3.7 or higher (3.10 recommended)**
 
@@ -191,10 +191,14 @@
 --hide-overall-progress         removes overall progress section while downloading
 --hide-forum-progress           removes forum progress section while downloading
 --hide-thread-progress          removes thread progress section while downloading
 --hide-domain-progress          removes domain progress section while downloading
 --hide-album-progress           removes album progress section while downloading
 --hide-file-progress            removes file progress section while downloading
 --refresh-rate                  changes the refresh rate of the progress table
+--visible-rows-threads          number of visible rows to use for the threads table
+--visible-rows-domains          number of visible rows to use for the domains table
+--visible-rows-albums           number of visible rows to use for the albums table
+--visible-rows-files            number of visible rows to use for the files table
 ```
 
 `--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.25 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.1 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -19,20 +19,20 @@
 Development [Buy_Me_A_Coffee] If you want to support me and my effort you can
 buy me a coffee or send me some crypto: BTC:
 bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B XMR:
 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
 ## More Information Read the [Wiki](https://github.com/Jules-WinnfieldX/
 CyberDropDownloader/wiki/)! ## Supported Sites | Website | Supported Link Types
-| |-------------------------|--------------------------------------------------
+| |-----------------------------------------|----------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------------------------| | Anonfiles | Download page: Anonfiles.com/... | |
-Bayfiles | Download page: Bayfiles.com/... | | Bunkr (ru/su/la) | Albums:
-bunkr.ru/a/...
+----------------------------------------| | Anonfiles | Download page:
+Anonfiles.com/... | | Bayfiles | Download page: Bayfiles.com/... | | Bunkr (ru/
+su/la) | Albums: bunkr.ru/a/...
 Direct Videos: stream.bunkr.ru/v/...
 Direct links: cdn.bunkr.ru/...
 Direct links: i.bunkr.ru/...
 Direct links: files.bunkr.ru/...
 Direct links: media-files.bunkr.ru/... | | Coomer.party | Profiles:
 coomer.party/...
 Thumbnail Links: coomer.party/thumbnail/...
@@ -55,15 +55,16 @@
 gofile.io/d/... | | Gfycat | Gif: gfycat.com/... | | HGameCG | Albums:
 hgamecg.com/.../index.html | | ImgBox | Albums: imgbox.com/g/...
 Direct Images: images#.imgbox.com/...
 Single Files: imgbox.com/... | | IMG.Kiwi | Albums: img.kiwi/album/...
 Direct Images: img.kiwi/image/...
 User Profile: img.kiwi/#USER#
 All User Albums: img.kiwi/#USER#/albums | | jpg.church
-jpg.fish | Albums: jpg.church/album/...
+jpg.fish
+jpg.fishing | Albums: jpg.church/album/...
 Direct Images: jpg.church/image/...
 User Profile: jpg.church/#USER#
 All User Albums: jpg.church/#USER#/albums | | LoveFap | Albums: lovefap.com/
 a/...
 Direct Images: s*.lovefap.com/content/photos/...
 Videos: lovefap.com/video/... | | NSFW.XXX | Profile: nsfw.xxx/user/...
 Post: nsfw.xxx/post/... | | PimpAndHost | Albums: pimpandhost.com/album/...
@@ -161,14 +162,17 @@
 disables the new rich progress entirely and uses older methods --hide-overall-
 progress removes overall progress section while downloading --hide-forum-
 progress removes forum progress section while downloading --hide-thread-
 progress removes thread progress section while downloading --hide-domain-
 progress removes domain progress section while downloading --hide-album-
 progress removes album progress section while downloading --hide-file-progress
 removes file progress section while downloading --refresh-rate changes the
-refresh rate of the progress table ``` `--only-hosts` and `--skip-hosts` can
-use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
-"cyberfile", "e-hentai", "erome", "fapello", "gfycat",
-"gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
-"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
-"socialmediagirls", "xbunker", "xbunkr"`
+refresh rate of the progress table --visible-rows-threads number of visible
+rows to use for the threads table --visible-rows-domains number of visible rows
+to use for the domains table --visible-rows-albums number of visible rows to
+use for the albums table --visible-rows-files number of visible rows to use for
+the files table ``` `--only-hosts` and `--skip-hosts` can use: `"anonfiles",
+"bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai",
+"erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg",
+"img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap",
+"nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
+"saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.1/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.25/setup.cfg` & `cyberdrop-dl-4.2.1/setup.cfg`

 * *Files identical despite different names*

