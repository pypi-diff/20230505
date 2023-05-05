# Comparing `tmp/twitter_loctagger_it-0.0.1.tar.gz` & `tmp/twitter_loctagger_it-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_loctagger_it-0.0.1.tar", last modified: Sat Jan 21 14:37:30 2023, max compression
+gzip compressed data, was "twitter_loctagger_it-0.0.2.tar", last modified: Fri May  5 17:33:48 2023, max compression
```

## Comparing `twitter_loctagger_it-0.0.1.tar` & `twitter_loctagger_it-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-21 14:37:30.615877 twitter_loctagger_it-0.0.1/
--rw-rw-rw-   0        0        0      193 2023-01-21 14:37:30.615877 twitter_loctagger_it-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-01-21 14:37:30.615877 twitter_loctagger_it-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      309 2023-01-21 14:24:58.000000 twitter_loctagger_it-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-21 14:37:30.615877 twitter_loctagger_it-0.0.1/twitter_loctagger_it.egg-info/
--rw-rw-rw-   0        0        0      193 2023-01-21 14:37:30.000000 twitter_loctagger_it-0.0.1/twitter_loctagger_it.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-01-21 14:37:30.000000 twitter_loctagger_it-0.0.1/twitter_loctagger_it.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-21 14:37:30.000000 twitter_loctagger_it-0.0.1/twitter_loctagger_it.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-01-21 14:37:30.000000 twitter_loctagger_it-0.0.1/twitter_loctagger_it.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:48.298656 twitter_loctagger_it-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-01-21 12:32:12.000000 twitter_loctagger_it-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       35 2023-05-05 17:25:28.000000 twitter_loctagger_it-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4443 2023-05-05 17:33:48.299657 twitter_loctagger_it-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3926 2023-04-15 16:06:04.000000 twitter_loctagger_it-0.0.2/README.md
+-rw-rw-rw-   0        0        0      103 2023-05-05 17:20:12.000000 twitter_loctagger_it-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      615 2023-05-05 17:33:48.304655 twitter_loctagger_it-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:48.280743 twitter_loctagger_it-0.0.2/twitter_loctagger_it/
+-rw-rw-rw-   0        0        0        0 2023-01-21 15:36:47.000000 twitter_loctagger_it-0.0.2/twitter_loctagger_it/__init__.py
+-rw-rw-rw-   0        0        0    10984 2023-04-18 14:55:44.000000 twitter_loctagger_it-0.0.2/twitter_loctagger_it/geocoder.py
+-rw-rw-rw-   0        0        0   321291 2023-04-19 17:47:55.000000 twitter_loctagger_it-0.0.2/twitter_loctagger_it/istat.xlsx
+-rw-rw-rw-   0        0        0    20212 2023-01-23 14:58:45.000000 twitter_loctagger_it-0.0.2/twitter_loctagger_it/regions.xlsx
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:48.297648 twitter_loctagger_it-0.0.2/twitter_loctagger_it.egg-info/
+-rw-rw-rw-   0        0        0     4443 2023-05-05 17:33:48.000000 twitter_loctagger_it-0.0.2/twitter_loctagger_it.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-05-05 17:33:48.000000 twitter_loctagger_it-0.0.2/twitter_loctagger_it.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 17:33:48.000000 twitter_loctagger_it-0.0.2/twitter_loctagger_it.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-05 17:33:48.000000 twitter_loctagger_it-0.0.2/twitter_loctagger_it.egg-info/top_level.txt
```

