# Comparing `tmp/bdfrx-1.0.4.tar.gz` & `tmp/bdfrx-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdfrx-1.0.4.tar", last modified: Fri Mar 31 20:51:55 2023, max compression
+gzip compressed data, was "bdfrx-1.0.5.tar", last modified: Fri May  5 03:29:52 2023, max compression
```

## Comparing `bdfrx-1.0.4.tar` & `bdfrx-1.0.5.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:51:55.066632 bdfrx-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-03-31 20:51:35.000000 bdfrx-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    68622 2023-03-31 20:51:55.066632 bdfrx-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-03-31 20:51:35.000000 bdfrx-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:51:55.058632 bdfrx-1.0.4/bdfrx/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6819 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/bdfrx.db
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/default_config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_authenticator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:51:55.062632 bdfrx-1.0.4/bdfrx/site_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/delay_for_reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/download_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/erome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:51:55.062632 bdfrx-1.0.4/bdfrx/site_downloaders/fallback_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/fallback_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/gfycat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/imgur.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/pornhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/redgifs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/self_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/vidble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/vreddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-31 20:51:35.000000 bdfrx-1.0.4/bdfrx/site_downloaders/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:51:55.058632 bdfrx-1.0.4/bdfrx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    68622 2023-03-31 20:51:55.000000 bdfrx-1.0.4/bdfrx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-31 20:51:55.000000 bdfrx-1.0.4/bdfrx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 20:51:55.000000 bdfrx-1.0.4/bdfrx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 20:51:55.000000 bdfrx-1.0.4/bdfrx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-31 20:51:55.000000 bdfrx-1.0.4/bdfrx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 20:51:55.000000 bdfrx-1.0.4/bdfrx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-03-31 20:51:35.000000 bdfrx-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 20:51:55.066632 bdfrx-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:51:55.066632 bdfrx-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-31 20:51:35.000000 bdfrx-1.0.4/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-31 20:51:35.000000 bdfrx-1.0.4/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-03-31 20:51:35.000000 bdfrx-1.0.4/tests/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-31 20:51:35.000000 bdfrx-1.0.4/tests/test_download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-31 20:51:35.000000 bdfrx-1.0.4/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-03-31 20:51:35.000000 bdfrx-1.0.4/tests/test_file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-03-31 20:51:35.000000 bdfrx-1.0.4/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-31 20:51:35.000000 bdfrx-1.0.4/tests/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.204241 bdfrx-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-05-05 03:29:38.000000 bdfrx-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-05 03:29:52.204241 bdfrx-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-05-05 03:29:38.000000 bdfrx-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.200241 bdfrx-1.0.5/bdfrx/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6880 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/bdfrx.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23005 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/default_config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_authenticator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.204241 bdfrx-1.0.5/bdfrx/site_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/catbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/delay_for_reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/download_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/erome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.204241 bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/gfycat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/imgur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/pornhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/redgifs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/self_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/vidble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/vreddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-05 03:29:38.000000 bdfrx-1.0.5/bdfrx/site_downloaders/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.200241 bdfrx-1.0.5/bdfrx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 03:29:52.000000 bdfrx-1.0.5/bdfrx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-05 03:29:38.000000 bdfrx-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:29:52.208241 bdfrx-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:29:52.204241 bdfrx-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-05 03:29:38.000000 bdfrx-1.0.5/tests/test_resource.py
```

### Comparing `bdfrx-1.0.4/LICENSE` & `bdfrx-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/PKG-INFO` & `bdfrx-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.4
+Version: 1.0.5
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -821,14 +821,17 @@
     - Complements exclude-id options but does not require them
 - `--db-file`
     - Allows to specify a location of the sqlite3 db rather than storing in the config directory
 - `--disable-module`
     - Can be specified multiple times
     - Disables certain modules from being used
     - See [Disabling Modules](#disabling-modules) for more information and a list of module names
+- `--downvoted`
+    - This will use a user's downvoted posts as a source of posts to scrape
+    - This requires an authenticated Reddit instance, using the `--authenticate` flag, as well as `--user` set to `me`
 - `--exclude-id`
     - This will skip the download of any submission with the ID provided
     - Can be specified multiple times
 - `--exclude-id-file`
     - This will skip the download of any submission with any of the IDs in the files provided
     - Can be specified multiple times
     - Format is one ID per line
@@ -909,15 +912,15 @@
     - Domains must be supplied in the form `example.com` or `img.example.com`
 - `--skip-subreddit`
     - This skips all submissions from the specified subreddit
     - Can be specified multiple times
     - Also accepts CSV subreddit names
 - `-S, --sort`
     - This is the sort type for each applicable submission source supplied to BDFRx
-    - This option does not apply to upvoted or saved posts when scraping from these sources
+    - This option does not apply to upvoted, downvoted or saved posts when scraping from these sources
     - The following options are available:
         - `controversial`
         - `hot` (default)
         - `new`
         - `relevance` (only available when using `--search`)
         - `rising`
         - `top`
@@ -927,15 +930,15 @@
 - `-s, --subreddit`
     - This adds a subreddit as a source
     - Can be used mutliple times
         - This can be done by using `-s` multiple times
         - Subreddits can also be used to provide CSV subreddits e.g. `-m "all, python, mindustry"`
 - `-t, --time`
     - This is the time filter that will be applied to all applicable sources
-    - This option does not apply to upvoted or saved posts when scraping from these sources
+    - This option does not apply to upvoted, downvoted or saved posts when scraping from these sources
     - This option only applies if sorting by top or controversial.  See --sort for more detail.
     - The following options are available:
         - `all` (default)
         - `hour`
         - `day`
         - `week`
         - `month`
@@ -966,17 +969,17 @@
 cat users.txt | xargs -L 1 echo --user | xargs -L 50 bdfrx download <ARGS>
 ```
 
 The part `-L 50` is to make sure that the character limit for a single line isn't exceeded, but may not be necessary. This can also be used to load subreddits from a file, simply exchange `--user` with `--subreddit` and so on.
 
 ## Authentication and Security
 
-BDFRx uses OAuth2 authentication to connect to Reddit if authentication is required. This means that it is a secure, token-based system for making requests. This also means that BDFRx only has access to specific parts of the account authenticated, by default only saved posts, upvoted posts, and the identity of the authenticated account. Note that authentication is not required unless accessing private things like upvoted posts, saved posts, and private multireddits.
+BDFRx uses OAuth2 authentication to connect to Reddit if authentication is required. This means that it is a secure, token-based system for making requests. This also means that BDFRx only has access to specific parts of the account authenticated, by default only saved posts, upvoted posts, downvoted posts, and the identity of the authenticated account. Note that authentication is not required unless accessing private things like upvoted posts, downvoted posts, saved posts, and private multireddits.
 
-To authenticate, BDFRx will first look for a token in the configuration file that signals that there's been a previous authentication. If this is not there, then BDFRx will attempt to register itself with your account. This is normal, and if you run the program, it will pause and show a Reddit URL. Click on this URL and it will take you to Reddit, where the permissions being requested will be shown. Read this and **confirm that there are no more permissions than needed to run the program**. You should not grant unneeded permissions; by default, BDFRx only requests permission to read your saved or upvoted submissions and identify as you.
+To authenticate, BDFRx will first look for a token in the configuration file that signals that there's been a previous authentication. If this is not there, then BDFRx will attempt to register itself with your account. This is normal, and if you run the program, it will pause and show a Reddit URL. Click on this URL and it will take you to Reddit, where the permissions being requested will be shown. Read this and **confirm that there are no more permissions than needed to run the program**. You should not grant unneeded permissions; by default, BDFRx only requests permission to read your saved, upvoted, or downvoted submissions and identify as you.
 
 If the permissions look safe, confirm it, and BDFRx will save a token that will allow it to authenticate with Reddit from then on.
 
 ## Changing Permissions
 
 Most users will not need to do anything extra to use any of the current features. However, if additional features such as scraping messages, PMs, etc are added in the future, these will require additional scopes. Additionally, advanced users may wish to use BDFRx with their own API key and secret. There is normally no need to do this, but it *is* allowed by BDFRx.
```

### Comparing `bdfrx-1.0.4/README.md` & `bdfrx-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,17 @@
     - Complements exclude-id options but does not require them
 - `--db-file`
     - Allows to specify a location of the sqlite3 db rather than storing in the config directory
 - `--disable-module`
     - Can be specified multiple times
     - Disables certain modules from being used
     - See [Disabling Modules](#disabling-modules) for more information and a list of module names
+- `--downvoted`
+    - This will use a user's downvoted posts as a source of posts to scrape
+    - This requires an authenticated Reddit instance, using the `--authenticate` flag, as well as `--user` set to `me`
 - `--exclude-id`
     - This will skip the download of any submission with the ID provided
     - Can be specified multiple times
 - `--exclude-id-file`
     - This will skip the download of any submission with any of the IDs in the files provided
     - Can be specified multiple times
     - Format is one ID per line
@@ -212,15 +215,15 @@
     - Domains must be supplied in the form `example.com` or `img.example.com`
 - `--skip-subreddit`
     - This skips all submissions from the specified subreddit
     - Can be specified multiple times
     - Also accepts CSV subreddit names
 - `-S, --sort`
     - This is the sort type for each applicable submission source supplied to BDFRx
-    - This option does not apply to upvoted or saved posts when scraping from these sources
+    - This option does not apply to upvoted, downvoted or saved posts when scraping from these sources
     - The following options are available:
         - `controversial`
         - `hot` (default)
         - `new`
         - `relevance` (only available when using `--search`)
         - `rising`
         - `top`
@@ -230,15 +233,15 @@
 - `-s, --subreddit`
     - This adds a subreddit as a source
     - Can be used mutliple times
         - This can be done by using `-s` multiple times
         - Subreddits can also be used to provide CSV subreddits e.g. `-m "all, python, mindustry"`
 - `-t, --time`
     - This is the time filter that will be applied to all applicable sources
-    - This option does not apply to upvoted or saved posts when scraping from these sources
+    - This option does not apply to upvoted, downvoted or saved posts when scraping from these sources
     - This option only applies if sorting by top or controversial.  See --sort for more detail.
     - The following options are available:
         - `all` (default)
         - `hour`
         - `day`
         - `week`
         - `month`
@@ -269,17 +272,17 @@
 cat users.txt | xargs -L 1 echo --user | xargs -L 50 bdfrx download <ARGS>
 ```
 
 The part `-L 50` is to make sure that the character limit for a single line isn't exceeded, but may not be necessary. This can also be used to load subreddits from a file, simply exchange `--user` with `--subreddit` and so on.
 
 ## Authentication and Security
 
-BDFRx uses OAuth2 authentication to connect to Reddit if authentication is required. This means that it is a secure, token-based system for making requests. This also means that BDFRx only has access to specific parts of the account authenticated, by default only saved posts, upvoted posts, and the identity of the authenticated account. Note that authentication is not required unless accessing private things like upvoted posts, saved posts, and private multireddits.
+BDFRx uses OAuth2 authentication to connect to Reddit if authentication is required. This means that it is a secure, token-based system for making requests. This also means that BDFRx only has access to specific parts of the account authenticated, by default only saved posts, upvoted posts, downvoted posts, and the identity of the authenticated account. Note that authentication is not required unless accessing private things like upvoted posts, downvoted posts, saved posts, and private multireddits.
 
-To authenticate, BDFRx will first look for a token in the configuration file that signals that there's been a previous authentication. If this is not there, then BDFRx will attempt to register itself with your account. This is normal, and if you run the program, it will pause and show a Reddit URL. Click on this URL and it will take you to Reddit, where the permissions being requested will be shown. Read this and **confirm that there are no more permissions than needed to run the program**. You should not grant unneeded permissions; by default, BDFRx only requests permission to read your saved or upvoted submissions and identify as you.
+To authenticate, BDFRx will first look for a token in the configuration file that signals that there's been a previous authentication. If this is not there, then BDFRx will attempt to register itself with your account. This is normal, and if you run the program, it will pause and show a Reddit URL. Click on this URL and it will take you to Reddit, where the permissions being requested will be shown. Read this and **confirm that there are no more permissions than needed to run the program**. You should not grant unneeded permissions; by default, BDFRx only requests permission to read your saved, upvoted, or downvoted submissions and identify as you.
 
 If the permissions look safe, confirm it, and BDFRx will save a token that will allow it to authenticate with Reddit from then on.
 
 ## Changing Permissions
 
 Most users will not need to do anything extra to use any of the current features. However, if additional features such as scraping messages, PMs, etc are added in the future, these will require additional scopes. Additionally, advanced users may wish to use BDFRx with their own API key and secret. There is normally no need to do this, but it *is* allowed by BDFRx.
```

### Comparing `bdfrx-1.0.4/bdfrx/__main__.py` & `bdfrx-1.0.5/bdfrx/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 _common_options = [
     click.argument("directory", type=str),
     click.option("--authenticate", is_flag=True, default=None),
     click.option("--config", type=str, default=None),
     click.option("--db", is_flag=True, default=None),
     click.option("--db-file", type=str, default=None),
     click.option("--disable-module", type=str, multiple=True, default=None),
+    click.option("--downvoted", is_flag=True, default=None),
     click.option("--exclude-id", type=str, multiple=True, default=None),
     click.option("--exclude-id-file", type=str, multiple=True, default=None),
     click.option("--file-scheme", type=str, default=None),
     click.option("--filename-restriction-scheme", type=click.Choice(("linux", "windows")), default=None),
     click.option("--folder-scheme", type=str, default=None),
     click.option("--ignore-user", type=str, multiple=True, default=None),
     click.option("--include-id-file", type=str, multiple=True, default=None),
```

### Comparing `bdfrx-1.0.4/bdfrx/bdfrx.db` & `bdfrx-1.0.5/bdfrx/bdfrx.db`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/completion.py` & `bdfrx-1.0.5/bdfrx/completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,35 +17,41 @@
             comp_dir = self.share_dir + "/bash-completion/completions/"
             if not Path(comp_dir).exists():
                 print("Creating Bash completion directory.")
                 Path(comp_dir).mkdir(parents=True, exist_ok=True)
             for point in self.entry_points:
                 self.env[f"_{point.upper().replace('-', '_')}_COMPLETE"] = "bash_source"
                 with Path(comp_dir + point).open(mode="w") as file:
-                    file.write(subprocess.run([point], env=self.env, capture_output=True, text=True).stdout)
+                    file.write(
+                        subprocess.run([point], env=self.env, capture_output=True, text=True).stdout,  # noqa: S603
+                    )
                     print(f"Bash completion for {point} written to {comp_dir}{point}")
         if self.shell in ("all", "fish"):
             comp_dir = self.share_dir + "/fish/vendor_completions.d/"
             if not Path(comp_dir).exists():
                 print("Creating Fish completion directory.")
                 Path(comp_dir).mkdir(parents=True, exist_ok=True)
             for point in self.entry_points:
                 self.env[f"_{point.upper().replace('-', '_')}_COMPLETE"] = "fish_source"
                 with Path(comp_dir + point + ".fish").open(mode="w") as file:
-                    file.write(subprocess.run([point], env=self.env, capture_output=True, text=True).stdout)
+                    file.write(
+                        subprocess.run([point], env=self.env, capture_output=True, text=True).stdout,  # noqa: S603
+                    )
                     print(f"Fish completion for {point} written to {comp_dir}{point}.fish")
         if self.shell in ("all", "zsh"):
             comp_dir = self.share_dir + "/zsh/site-functions/"
             if not Path(comp_dir).exists():
                 print("Creating Zsh completion directory.")
                 Path(comp_dir).mkdir(parents=True, exist_ok=True)
             for point in self.entry_points:
                 self.env[f"_{point.upper().replace('-', '_')}_COMPLETE"] = "zsh_source"
                 with Path(comp_dir + "_" + point).open(mode="w") as file:
-                    file.write(subprocess.run([point], env=self.env, capture_output=True, text=True).stdout)
+                    file.write(
+                        subprocess.run([point], env=self.env, capture_output=True, text=True).stdout,  # noqa: S603
+                    )
                     print(f"Zsh completion for {point} written to {comp_dir}_{point}")
 
     def uninstall(self) -> None:
         if self.shell in ("all", "bash"):
             comp_dir = self.share_dir + "/bash-completion/completions/"
             for point in self.entry_points:
                 if Path(comp_dir + point).exists():
```

### Comparing `bdfrx-1.0.4/bdfrx/configuration.py` & `bdfrx-1.0.5/bdfrx/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         super().__init__()
         self.authenticate = False
         self.config = None
         self.db = False
         self.db_file: Optional[str] = None
         self.directory: str = "."
         self.disable_module: list[str] = []
+        self.downvoted: bool = False
         self.exclude_id = []
         self.exclude_id_file = []
         self.file_scheme: str = "{REDDITOR}_{TITLE}_{POSTID}"
         self.filename_restriction_scheme = None
         self.folder_scheme: str = "{SUBREDDIT}"
         self.ignore_user = []
         self.include_id_file = []
```

### Comparing `bdfrx-1.0.4/bdfrx/connector.py` & `bdfrx-1.0.5/bdfrx/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,25 +279,25 @@
         file_handler.setFormatter(formatter)
         file_handler.setLevel(0)
         return file_handler
 
     @staticmethod
     def sanitise_subreddit_name(subreddit: str) -> str:
         pattern = re.compile(r"^(?:https://www\.reddit\.com/)?(?:r/)?(.*?)/?$")
-        match = re.match(pattern, subreddit)
+        match = pattern.match(subreddit)
         if not match:
             raise errors.BulkDownloaderException(f"Could not find subreddit name in string {subreddit!r}")
         return match.group(1)
 
     @staticmethod
     def split_args_input(entries: list[str]) -> set[str]:
         all_entries = []
         split_pattern = re.compile(r"[,;]\s?")
         for entry in entries:
-            results = re.split(split_pattern, entry)
+            results = split_pattern.split(entry)
             all_entries.extend([RedditConnector.sanitise_subreddit_name(name) for name in results])
         return set(all_entries)
 
     def get_subreddits(self) -> list[praw.models.ListingGenerator]:  # noqa: PLR0912
         out = []
         subscribed_subreddits = set()
         if self.args.subscribed:
@@ -396,15 +396,15 @@
     ) -> Iterator:
         sort_function = self.determine_sort_function()
         if self.sort_filter in (RedditTypes.SortType.TOP, RedditTypes.SortType.CONTROVERSIAL):
             return sort_function(reddit_source, limit=self.args.limit, time_filter=self.time_filter.value)
         return sort_function(reddit_source, limit=self.args.limit)
 
     def get_user_data(self) -> list[Iterator]:
-        if any([self.args.submitted, self.args.upvoted, self.args.saved]):
+        if any([self.args.downvoted, self.args.saved, self.args.submitted, self.args.upvoted]):
             if not self.args.user:
                 logger.warning("At least one user must be supplied to download user data")
                 return []
             generators = []
             for user in self.args.user:
                 try:
                     try:
@@ -415,23 +415,26 @@
                     if self.args.submitted:
                         logger.debug(f"Retrieving submitted posts of user {user}")
                         generators.append(
                             self.create_filtered_listing_generator(
                                 self.reddit_instance.redditor(user).submissions,
                             ),
                         )
-                    if not self.authenticated and any((self.args.upvoted, self.args.saved)):
+                    if not self.authenticated and any((self.args.downvoted, self.args.saved, self.args.upvoted)):
                         logger.warning("Accessing user lists requires authentication")
                     else:
                         if self.args.upvoted:
                             logger.debug(f"Retrieving upvoted posts of user {user}")
                             generators.append(self.reddit_instance.redditor(user).upvoted(limit=self.args.limit))
                         if self.args.saved:
                             logger.debug(f"Retrieving saved posts of user {user}")
                             generators.append(self.reddit_instance.redditor(user).saved(limit=self.args.limit))
+                        if self.args.downvoted:
+                            logger.debug(f"Retrieving downvoted posts of user {user}")
+                            generators.append(self.reddit_instance.redditor(user).downvoted(limit=self.args.limit))
                 except prawcore.PrawcoreException as e:
                     logger.error(f"User {user} failed to be retrieved due to a PRAW exception: {e}")
                     logger.debug("Waiting 60 seconds to continue")
                     sleep(60)
             return generators
         return []
 
@@ -494,11 +497,11 @@
     def read_id_files(file_locations: list[str]) -> set[str]:
         out = []
         for location in file_locations:
             id_file = Path(location).resolve().expanduser()
             if not id_file.exists():
                 logger.warning(f"ID file at {id_file} does not exist")
                 continue
-            with id_file.open("r") as file:
+            with id_file.open() as file:
                 for line in file:
                     out.append(line.strip())
         return set(out)
```

### Comparing `bdfrx-1.0.4/bdfrx/download_filter.py` & `bdfrx-1.0.5/bdfrx/download_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,21 +23,21 @@
         return True
 
     def _check_extension(self, resource_extension: str) -> bool:
         if not self.excluded_extensions:
             return True
         combined_extensions = "|".join(self.excluded_extensions)
         pattern = re.compile(rf".*({combined_extensions})$")
-        if re.match(pattern, resource_extension):
+        if pattern.match(resource_extension):
             logger.log(9, f"Url extension {resource_extension!r} matched with {pattern!r}")
             return False
         return True
 
     def _check_domain(self, url: str) -> bool:
         if not self.excluded_domains:
             return True
         combined_domains = "|".join(self.excluded_domains)
         pattern = re.compile(rf"https?://.*({combined_domains}).*")
-        if re.match(pattern, url):
+        if pattern.match(url):
             logger.log(9, f"Url domain {url!r} matched with {pattern!r}")
             return False
         return True
```

### Comparing `bdfrx-1.0.4/bdfrx/downloader.py` & `bdfrx-1.0.5/bdfrx/downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/file_name_formatter.py` & `bdfrx-1.0.5/bdfrx/file_name_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             logger.debug("Forcing Windows-compatible filenames")
             result = FileNameFormatter._format_for_windows(result)
         return result
 
     @staticmethod
     def _convert_unicode_escapes(in_string: str) -> str:
         pattern = re.compile(r"(\\u\d{4})")
-        matches = re.search(pattern, in_string)
+        matches = pattern.search(in_string)
         if matches:
             for match in matches.groups():
                 converted_match = bytes(match, "utf-8").decode("unicode-escape")
                 in_string = in_string.replace(match, converted_match)
         return in_string
 
     def _generate_name_dict_from_submission(self, submission: Submission) -> dict:
@@ -162,15 +162,15 @@
             out = Path(root, filename + ending)
 
         return out
 
     @staticmethod
     def find_max_path_length() -> int:
         try:
-            return int(subprocess.check_output(["getconf", "PATH_MAX", "/"]))
+            return int(subprocess.check_output(["/usr/bin/getconf", "PATH_MAX", "/"]))  # noqa: S603
         except (ValueError, subprocess.CalledProcessError, OSError):
             if platform.system() == "Windows":
                 return FileNameFormatter.WINDOWS_MAX_PATH_LENGTH
             return FileNameFormatter.LINUX_MAX_PATH_LENGTH
 
     def format_resource_paths(
         self,
```

### Comparing `bdfrx-1.0.4/bdfrx/oauth2.py` & `bdfrx-1.0.5/bdfrx/oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/resource.py` & `bdfrx-1.0.5/bdfrx/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def create_hash(self) -> None:
         self.hash = hashlib.md5(self.content, usedforsecurity=False)
 
     def _determine_extension(self) -> Optional[str]:
         extension_pattern = re.compile(r".*(\..{3,5})$")
         stripped_url = urllib.parse.urlsplit(self.url).path
-        match = re.search(extension_pattern, stripped_url)
+        match = extension_pattern.search(stripped_url)
         if match:
             return match.group(1)
         return None
 
     @staticmethod
     def http_download(url: str, download_parameters: dict) -> Optional[bytes]:
         headers = download_parameters.get("headers")
```

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/base_downloader.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/delay_for_reddit.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/delay_for_reddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/direct.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/direct.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/download_factory.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/download_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import urllib.parse
 
 from bdfrx.exceptions import NotADownloadableLinkError
 from bdfrx.site_downloaders.base_downloader import BaseDownloader
+from bdfrx.site_downloaders.catbox import Catbox
 from bdfrx.site_downloaders.delay_for_reddit import DelayForReddit
 from bdfrx.site_downloaders.direct import Direct
 from bdfrx.site_downloaders.erome import Erome
 from bdfrx.site_downloaders.fallback_downloaders.ytdlp_fallback import YtdlpFallback
 from bdfrx.site_downloaders.gallery import Gallery
 from bdfrx.site_downloaders.gfycat import Gfycat
 from bdfrx.site_downloaders.imgur import Imgur
@@ -20,24 +21,26 @@
 
 class DownloadFactory:
     @staticmethod
     def pull_lever(url: str) -> type[BaseDownloader]:  # noqa: PLR0911,PLR0912
         sanitised_url = DownloadFactory.sanitise_url(url).lower()
         if re.match(r"(i\.|m\.|o\.)?imgur", sanitised_url):
             return Imgur
-        if re.match(r"(i\.|thumbs\d\.|v\d\.)?(redgifs|gifdeliverynetwork)", sanitised_url):
+        if re.match(r"(i\.|thumbs\d{1,2}\.|v\d\.)?(redgifs|gifdeliverynetwork)", sanitised_url):
             return Redgifs
         if re.match(r"(thumbs\.|giant\.)?gfycat\.", sanitised_url):
             return Gfycat
         if re.match(r".*/.*\.[a-zA-Z34]{3,4}(\?[\w;&=]*)?$", sanitised_url) and not DownloadFactory.is_web_resource(
             sanitised_url,
         ):
             return Direct
         if re.match(r"erome\.com.*", sanitised_url):
             return Erome
+        if re.match(r"catbox\.moe", sanitised_url):
+            return Catbox
         if re.match(r"delayforreddit\.com", sanitised_url):
             return DelayForReddit
         if re.match(r"reddit\.com/gallery/.*", sanitised_url) or re.match(r"patreon\.com.*", sanitised_url):
             return Gallery
         if re.match(r"reddit\.com/r/", sanitised_url):
             return SelfPost
         if re.match(r"(m\.)?youtu\.?be", sanitised_url):
@@ -55,15 +58,15 @@
         raise NotADownloadableLinkError(f"No downloader module exists for url {url}")
 
     @staticmethod
     def sanitise_url(url: str) -> str:
         beginning_regex = re.compile(r"\s*(www\.?)?")
         split_url = urllib.parse.urlsplit(url)
         split_url = split_url.netloc + split_url.path
-        split_url = re.sub(beginning_regex, "", split_url)
+        split_url = beginning_regex.sub("", split_url)
         return split_url
 
     @staticmethod
     def is_web_resource(url: str) -> bool:
         web_extensions = (
             "asp",
             "aspx",
```

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/erome.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/erome.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/gallery.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/gallery.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/gfycat.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/gfycat.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/imgur.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/imgur.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,26 +28,28 @@
         elif "mp4" in self.raw_data:
             out.append(Resource(self.post, self.raw_data["mp4"], Resource.retry_download(self.raw_data["mp4"])))
         else:
             out.append(Resource(self.post, self.raw_data["link"], Resource.retry_download(self.raw_data["link"])))
         return out
 
     @staticmethod
-    def _get_data(link: str) -> dict:
+    def _get_id(link: str) -> str:
         try:
-            if link.endswith("/"):
-                link = link.removesuffix("/")
-            if re.search(r".*/(.*?)(gallery/|a/)", link):
-                imgur_id = re.match(r".*/(?:gallery/|a/)(.*?)(?:/.*|\..{3,4})?$", link).group(1)
-                api = f"https://api.imgur.com/3/album/{imgur_id}"
-            else:
-                imgur_id = re.match(r".*/(.*?)(?:_d)?(?:\..{0,})?$", link).group(1)
-                api = f"https://api.imgur.com/3/image/{imgur_id}"
+            imgur_id = re.search(r"imgur\.com/(?:a/|gallery/)?([a-zA-Z0-9]+)", link).group(1)
         except AttributeError:
             raise SiteDownloaderError(f"Could not extract Imgur ID from {link}")
+        return imgur_id
+
+    @staticmethod
+    def _get_data(link: str) -> dict:
+        imgur_id = Imgur._get_id(link)
+        if re.search(r"/(gallery|a)/", link):
+            api = f"https://api.imgur.com/3/album/{imgur_id}"
+        else:
+            api = f"https://api.imgur.com/3/image/{imgur_id}"
 
         headers = {
             "referer": "https://imgur.com/",
             "origin": "https://imgur.com",
             "content-type": "application/json",
             "Authorization": "Client-ID 546c25a59c58ad7",
         }
```

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/pornhub.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/pornhub.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/redgifs.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/redgifs.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
     @staticmethod
     def _get_id(url: str) -> str:
         try:
             if url.endswith("/"):
                 url = url.removesuffix("/")
             redgif_id = re.match(r".*/(.*?)(?:#.*|\?.*|\..{0,})?$", url).group(1).lower()
-            if redgif_id.endswith("-mobile"):
-                redgif_id = redgif_id.removesuffix("-mobile")
+            redgif_id = re.sub(r"(-.*)$", "", redgif_id)
         except AttributeError:
             raise SiteDownloaderError(f"Could not extract Redgifs ID from {url}")
         return redgif_id
 
     @staticmethod
     def _get_link(url: str) -> set[str]:
         redgif_id = Redgifs._get_id(url)
```

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/self_post.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/self_post.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/vidble.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/vidble.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/vreddit.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/vreddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx/site_downloaders/youtube.py` & `bdfrx-1.0.5/bdfrx/site_downloaders/youtube.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/bdfrx.egg-info/PKG-INFO` & `bdfrx-1.0.5/bdfrx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.4
+Version: 1.0.5
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -821,14 +821,17 @@
     - Complements exclude-id options but does not require them
 - `--db-file`
     - Allows to specify a location of the sqlite3 db rather than storing in the config directory
 - `--disable-module`
     - Can be specified multiple times
     - Disables certain modules from being used
     - See [Disabling Modules](#disabling-modules) for more information and a list of module names
+- `--downvoted`
+    - This will use a user's downvoted posts as a source of posts to scrape
+    - This requires an authenticated Reddit instance, using the `--authenticate` flag, as well as `--user` set to `me`
 - `--exclude-id`
     - This will skip the download of any submission with the ID provided
     - Can be specified multiple times
 - `--exclude-id-file`
     - This will skip the download of any submission with any of the IDs in the files provided
     - Can be specified multiple times
     - Format is one ID per line
@@ -909,15 +912,15 @@
     - Domains must be supplied in the form `example.com` or `img.example.com`
 - `--skip-subreddit`
     - This skips all submissions from the specified subreddit
     - Can be specified multiple times
     - Also accepts CSV subreddit names
 - `-S, --sort`
     - This is the sort type for each applicable submission source supplied to BDFRx
-    - This option does not apply to upvoted or saved posts when scraping from these sources
+    - This option does not apply to upvoted, downvoted or saved posts when scraping from these sources
     - The following options are available:
         - `controversial`
         - `hot` (default)
         - `new`
         - `relevance` (only available when using `--search`)
         - `rising`
         - `top`
@@ -927,15 +930,15 @@
 - `-s, --subreddit`
     - This adds a subreddit as a source
     - Can be used mutliple times
         - This can be done by using `-s` multiple times
         - Subreddits can also be used to provide CSV subreddits e.g. `-m "all, python, mindustry"`
 - `-t, --time`
     - This is the time filter that will be applied to all applicable sources
-    - This option does not apply to upvoted or saved posts when scraping from these sources
+    - This option does not apply to upvoted, downvoted or saved posts when scraping from these sources
     - This option only applies if sorting by top or controversial.  See --sort for more detail.
     - The following options are available:
         - `all` (default)
         - `hour`
         - `day`
         - `week`
         - `month`
@@ -966,17 +969,17 @@
 cat users.txt | xargs -L 1 echo --user | xargs -L 50 bdfrx download <ARGS>
 ```
 
 The part `-L 50` is to make sure that the character limit for a single line isn't exceeded, but may not be necessary. This can also be used to load subreddits from a file, simply exchange `--user` with `--subreddit` and so on.
 
 ## Authentication and Security
 
-BDFRx uses OAuth2 authentication to connect to Reddit if authentication is required. This means that it is a secure, token-based system for making requests. This also means that BDFRx only has access to specific parts of the account authenticated, by default only saved posts, upvoted posts, and the identity of the authenticated account. Note that authentication is not required unless accessing private things like upvoted posts, saved posts, and private multireddits.
+BDFRx uses OAuth2 authentication to connect to Reddit if authentication is required. This means that it is a secure, token-based system for making requests. This also means that BDFRx only has access to specific parts of the account authenticated, by default only saved posts, upvoted posts, downvoted posts, and the identity of the authenticated account. Note that authentication is not required unless accessing private things like upvoted posts, downvoted posts, saved posts, and private multireddits.
 
-To authenticate, BDFRx will first look for a token in the configuration file that signals that there's been a previous authentication. If this is not there, then BDFRx will attempt to register itself with your account. This is normal, and if you run the program, it will pause and show a Reddit URL. Click on this URL and it will take you to Reddit, where the permissions being requested will be shown. Read this and **confirm that there are no more permissions than needed to run the program**. You should not grant unneeded permissions; by default, BDFRx only requests permission to read your saved or upvoted submissions and identify as you.
+To authenticate, BDFRx will first look for a token in the configuration file that signals that there's been a previous authentication. If this is not there, then BDFRx will attempt to register itself with your account. This is normal, and if you run the program, it will pause and show a Reddit URL. Click on this URL and it will take you to Reddit, where the permissions being requested will be shown. Read this and **confirm that there are no more permissions than needed to run the program**. You should not grant unneeded permissions; by default, BDFRx only requests permission to read your saved, upvoted, or downvoted submissions and identify as you.
 
 If the permissions look safe, confirm it, and BDFRx will save a token that will allow it to authenticate with Reddit from then on.
 
 ## Changing Permissions
 
 Most users will not need to do anything extra to use any of the current features. However, if additional features such as scraping messages, PMs, etc are added in the future, these will require additional scopes. Additionally, advanced users may wish to use BDFRx with their own API key and secret. There is normally no need to do this, but it *is* allowed by BDFRx.
```

### Comparing `bdfrx-1.0.4/bdfrx.egg-info/SOURCES.txt` & `bdfrx-1.0.5/bdfrx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 bdfrx.egg-info/SOURCES.txt
 bdfrx.egg-info/dependency_links.txt
 bdfrx.egg-info/entry_points.txt
 bdfrx.egg-info/requires.txt
 bdfrx.egg-info/top_level.txt
 bdfrx/site_downloaders/__init__.py
 bdfrx/site_downloaders/base_downloader.py
+bdfrx/site_downloaders/catbox.py
 bdfrx/site_downloaders/delay_for_reddit.py
 bdfrx/site_downloaders/direct.py
 bdfrx/site_downloaders/download_factory.py
 bdfrx/site_downloaders/erome.py
 bdfrx/site_downloaders/gallery.py
 bdfrx/site_downloaders/gfycat.py
 bdfrx/site_downloaders/imgur.py
```

### Comparing `bdfrx-1.0.4/pyproject.toml` & `bdfrx-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,31 @@
 dependencies = [
     "appdirs>=1.4.4",
     "beautifulsoup4>=4.10.0",
     "cachetools>=5.3.0",
     "click>=8.0.0",
     "praw>=7.2.0",
     "pyyaml>=5.4.1",
-    "requests>=2.28.2",
+    "requests>=2.30.0",
     "yt-dlp>=2023.3.4",
 ]
 dynamic = ["version"]
 
 [tool.setuptools]
 dynamic = {"version" = {attr = "bdfrx.__version__"}}
 packages = ["bdfrx", "bdfrx.site_downloaders", "bdfrx.site_downloaders.fallback_downloaders",]
 package-data = {"bdfrx" = ["default_config.cfg", "bdfrx.db",]}
 
 [project.optional-dependencies]
 dev = [
-    "black>=23.1.0",
-    "pre-commit>=3.0.4",
-    "pytest>=7.2.1",
-    "ruff>=0.0.258",
+    "black>=23.3.0",
+    "pre-commit>=3.3.1",
+    "pytest>=7.3.1",
+    "refurb>=1.16.0",
+    "ruff>=0.0.264",
 ]
 
 [project.urls]
 "Homepage" = "https://omegarazer.github.io/bulk-downloader-for-reddit-x"
 "Source" = "https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x"
 "Bug Reports" = "https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/issues"
```

### Comparing `bdfrx-1.0.4/tests/test_completion.py` & `bdfrx-1.0.5/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/tests/test_configuration.py` & `bdfrx-1.0.5/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/tests/test_connector.py` & `bdfrx-1.0.5/tests/test_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,14 +360,15 @@
 
 @pytest.mark.online
 @pytest.mark.reddit
 @pytest.mark.authenticated
 @pytest.mark.parametrize(
     "test_flag",
     (
+        "downvoted",
         "upvoted",
         "saved",
     ),
 )
 def test_get_user_authenticated_lists(
     test_flag: str,
     downloader_mock: MagicMock,
@@ -431,15 +432,15 @@
     ),
 )
 def test_split_subreddit_entries(test_subreddit_entries: list[str], expected: set[str]):
     results = RedditConnector.split_args_input(test_subreddit_entries)
     assert results == expected
 
 
-def test_read_submission_ids_from_file(downloader_mock: MagicMock, tmp_path: Path):
+def test_read_submission_ids_from_file(tmp_path: Path):
     test_file = tmp_path / "test.txt"
     test_file.write_text("aaaaaa\nbbbbbb")
     results = RedditConnector.read_id_files([str(test_file)])
     assert results == {"aaaaaa", "bbbbbb"}
 
 
 @pytest.mark.online
```

### Comparing `bdfrx-1.0.4/tests/test_download_filter.py` & `bdfrx-1.0.5/tests/test_download_filter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/tests/test_downloader.py` & `bdfrx-1.0.5/tests/test_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import re
+import sys
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 import praw.models
 import pytest
 
 from bdfrx.__main__ import make_console_logging_handler
@@ -152,14 +153,15 @@
     output = capsys.readouterr()
     assert not folder_contents
     assert re.search(r"Resource hash .*? downloaded elsewhere", output.out)
 
 
 @pytest.mark.online
 @pytest.mark.reddit
+@pytest.mark.skipif(sys.platform == "win32", reason="Hangs on Github Windows.")
 def test_download_submission_file_exists(
     downloader_mock: MagicMock,
     reddit_instance: praw.Reddit,
     tmp_path: Path,
     capsys: pytest.CaptureFixture,
 ):
     add_console_handler()
```

### Comparing `bdfrx-1.0.4/tests/test_file_name_formatter.py` & `bdfrx-1.0.5/tests/test_file_name_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,14 +399,15 @@
     test_comment = reddit_instance.comment(id=test_comment_id)
     test_formatter = FileNameFormatter(test_file_scheme, test_folder_scheme, "ISO")
     test_entry = Resource(test_comment, "", lambda: None, ".json")
     result = test_formatter.format_path(test_entry, tmp_path)
     assert do_test_string_equality(result, expected_name)
 
 
+@pytest.mark.skipif(sys.platform == "win32", reason="Hangs on Github Windows.")
 @pytest.mark.parametrize(
     ("test_folder_scheme", "expected"),
     (
         ("{REDDITOR}/{SUBREDDIT}", "person/randomreddit"),
         ("{POSTID}/{SUBREDDIT}/{REDDITOR}", "12345/randomreddit/person"),
     ),
 )
```

### Comparing `bdfrx-1.0.4/tests/test_oauth2.py` & `bdfrx-1.0.5/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.4/tests/test_resource.py` & `bdfrx-1.0.5/tests/test_resource.py`

 * *Files identical despite different names*

