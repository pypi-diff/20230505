# Comparing `tmp/cyberdrop-dl-4.2.11.tar.gz` & `tmp/cyberdrop-dl-4.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.11.tar", last modified: Fri May  5 06:05:01 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.12.tar", last modified: Fri May  5 19:58:42 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.11.tar` & `cyberdrop-dl-4.2.12.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:05:01.762690 cyberdrop-dl-4.2.11/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-05 06:05:01.762690 cyberdrop-dl-4.2.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:05:01.754690 cyberdrop-dl-4.2.11/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:05:01.758690 cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:05:01.758690 cyberdrop-dl-4.2.11/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:05:01.762690 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:05:01.762690 cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:05:01.762690 cyberdrop-dl-4.2.11/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:05:01.758690 cyberdrop-dl-4.2.11/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-05 06:05:01.000000 cyberdrop-dl-4.2.11/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-05 06:05:01.000000 cyberdrop-dl-4.2.11/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:05:01.000000 cyberdrop-dl-4.2.11/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 06:05:01.000000 cyberdrop-dl-4.2.11/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 06:05:01.000000 cyberdrop-dl-4.2.11/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 06:05:01.000000 cyberdrop-dl-4.2.11/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-05 06:05:01.762690 cyberdrop-dl-4.2.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 06:04:39.000000 cyberdrop-dl-4.2.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.779605 cyberdrop-dl-4.2.12/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.783605 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.783605 cyberdrop-dl-4.2.12/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:58:42.779605 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 19:58:42.000000 cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-05 19:58:42.787606 cyberdrop-dl-4.2.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:58:33.000000 cyberdrop-dl-4.2.12/setup.py
```

### Comparing `cyberdrop-dl-4.2.11/LICENSE` & `cyberdrop-dl-4.2.12/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/PKG-INFO` & `cyberdrop-dl-4.2.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.11
+Version: 4.2.12
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.11 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.12 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.11/README.md` & `cyberdrop-dl-4.2.12/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/downloaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         # CDL Objects
         self.client = client
         self.files = files
         self.SQL_Helper = SQL_Helper
         self.File_Lock = FileLock()
 
         # Limits
-        self.delay = {'cyberfile': 1.0, 'anonfiles': 1.0, "coomer": 0.2, "kemono": 0.2}
+        self.delay = {'cyberdrop': 1.0, 'cyberfile': 1.0, 'anonfiles': 1.0, "coomer": 0.2, "kemono": 0.2}
 
         # Exclude Args
         self.exclude_audio = args["Ignore"]["exclude_audio"]
         self.exclude_images = args["Ignore"]["exclude_images"]
         self.exclude_videos = args["Ignore"]["exclude_videos"]
         self.exclude_other = args["Ignore"]["exclude_other"]
```

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,38 +70,33 @@
     runtime_opts.add_argument("--disable-attempt-limit", help="disables the attempt limitation", action="store_true")
     runtime_opts.add_argument("--include-id", help="include the ID in the download folder name", action="store_true")
     runtime_opts.add_argument("--skip-download-mark-completed", help="sets the scraped files as downloaded without downloading", action="store_true")
     runtime_opts.add_argument("--output-errored-urls", help="sets the failed urls to be output to the errored urls file", action="store_true")
     runtime_opts.add_argument("--output-unsupported-urls", help="sets the unsupported urls to be output to the unsupported urls file", action="store_true")
     runtime_opts.add_argument("--proxy", help="HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]", default=config_group["proxy"])
     runtime_opts.add_argument("--remove-bunkr-identifier", help="removes the bunkr added identifier from output filenames", action="store_true")
-    runtime_opts.add_argument("--required-free-space", type=int, default=config_group["required_free_space"],
-                              help="required free space (in gigabytes) for the program to run (default: %(default)s)")
-    runtime_opts.add_argument("--simultaneous-downloads-per-domain", type=int, default=config_group["simultaneous_downloads_per_domain"],
-                              help="Number of simultaneous downloads to use per domain (default: %(default)s)")
+    runtime_opts.add_argument("--required-free-space", type=int, default=config_group["required_free_space"], help="required free space (in gigabytes) for the program to run (default: %(default)s)")
+    runtime_opts.add_argument("--simultaneous-downloads-per-domain", type=int, default=config_group["simultaneous_downloads_per_domain"], help="Number of simultaneous downloads to use per domain (default: %(default)s)")
 
     # Sorting
     config_group = config_data["Sorting"]
     sort_opts = parser.add_argument_group("Sorting options")
     sort_opts.add_argument("--sort-downloads", help="sorts downloaded files after downloads have finished", action="store_true")
     sort_opts.add_argument("--sort-directory", type=Path, help="folder to download files to (default: %(default)s)", default=config_group["sort_directory"])
     sort_opts.add_argument("--sorted-audio", help="schema to sort audio (default: %(default)s)", default=config_group["sorted_audio"])
     sort_opts.add_argument("--sorted-images", help="schema to sort images (default: %(default)s)", default=config_group["sorted_images"])
     sort_opts.add_argument("--sorted-others", help="schema to sort other (default: %(default)s)", default=config_group["sorted_others"])
     sort_opts.add_argument("--sorted-videos", help="schema to sort videos (default: %(default)s)", default=config_group["sorted_videos"])
 
     # Ratelimiting
     config_group = config_data["Ratelimiting"]
     ratelimit_opts = parser.add_argument_group("Ratelimiting options")
-    ratelimit_opts.add_argument("--connection-timeout", type=int, default=config_group["connection_timeout"],
-                                help="number of seconds to wait attempting to connect to a URL during the downloading phase (default: %(default)s)")
-    ratelimit_opts.add_argument("--ratelimit", type=int, default=config_group["ratelimit"],
-                                help="this applies to requests made in the program during scraping, the number you provide is in requests/seconds (default: %(default)s)")
-    ratelimit_opts.add_argument("--throttle", type=int, default=config_group["throttle"],
-                                help="this is a throttle between requests during the downloading phase, the number is in seconds (default: %(default)s)")
+    ratelimit_opts.add_argument("--connection-timeout", type=int, default=config_group["connection_timeout"], help="number of seconds to wait attempting to connect to a URL during the downloading phase (default: %(default)s)")
+    ratelimit_opts.add_argument("--ratelimit", type=int, default=config_group["ratelimit"], help="this applies to requests made in the program during scraping, the number you provide is in requests/seconds (default: %(default)s)")
+    ratelimit_opts.add_argument("--throttle", type=int, default=config_group["throttle"], help="this is a throttle between requests during the downloading phase, the number is in seconds (default: %(default)s)")
 
     # Forum Options
     forum_opts = parser.add_argument_group("Forum options")
     forum_opts.add_argument("--output-last-forum-post", help="outputs the last post of a forum scrape to use as a starting point for future runs", action="store_true")
     forum_opts.add_argument("--separate-posts", help="separates forum scraping into folders by post number", action="store_true")
 
     # Authentication details
```

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.12/cyberdrop_dl/scraper/Scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,20 +75,21 @@
 
         self.include_id = args['Runtime']['include_id']
         self.remove_bunkr_id = args['Runtime']['remove_bunkr_identifier']
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.quiet = quiet
         self.jdownloader = JDownloader(args['JDownloader'], quiet)
 
-        self.bunkr_limiter = AsyncRateLimiter(4)
+        self.bunkr_limiter = AsyncRateLimiter(max_calls=1, period=1)
         self.coomer_limiter = AsyncRateLimiter(8)
         self.gofile_limiter = AsyncRateLimiter(max_calls=1, period=3)
         self.jpgfish_limiter = AsyncRateLimiter(10)
         self.kemono_limiter = AsyncRateLimiter(8)
 
+        self.bunkr_semaphore = asyncio.Semaphore(2)
         self.coomer_semaphore = asyncio.Semaphore(1)
         self.cyberfile_semaphore = asyncio.Semaphore(2)
         self.gofile_semaphore = asyncio.Semaphore(1)
         self.jpgfish_semaphore = asyncio.Semaphore(5)
         self.kemono_semaphore = asyncio.Semaphore(1)
         self.nudostar_semaphore = asyncio.Semaphore(1)
         self.simpcity_semaphore = asyncio.Semaphore(1)
@@ -139,16 +140,17 @@
         await anonfiles_session.exit_handler()
 
     async def Bunkr(self, url: URL, title=None):
         bunkr_session = ScrapeSession(self.client)
         if not self.bunkr_crawler:
             self.bunkr_crawler = BunkrCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
                                               remove_bunkr_id=self.remove_bunkr_id)
-        async with self.bunkr_limiter:
-            album_obj = await self.bunkr_crawler.fetch(bunkr_session, url)
+        async with self.bunkr_semaphore:
+            async with self.bunkr_limiter:
+                album_obj = await self.bunkr_crawler.fetch(bunkr_session, url)
         if not await album_obj.is_empty():
             await self._handle_album_additions("bunkr", album_obj, title)
         await bunkr_session.exit_handler()
 
     async def Cyberdrop(self, url: URL, title=None):
         cyberdrop_session = ScrapeSession(self.client)
         if not self.cyberdrop_crawler:
```

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.11
+Version: 4.2.12
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.11 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.12 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.11/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.12/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.11/setup.cfg` & `cyberdrop-dl-4.2.12/setup.cfg`

 * *Files identical despite different names*

