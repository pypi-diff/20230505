# Comparing `tmp/alirpa_pack-3.0.2.tar.gz` & `tmp/alirpa_pack-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\alirpa_pack-3.0.2.tar", last modified: Fri May  5 06:32:54 2023, max compression
+gzip compressed data, was "dist\alirpa_pack-3.0.3.tar", last modified: Fri May  5 06:38:57 2023, max compression
```

## Comparing `alirpa_pack-3.0.2.tar` & `alirpa_pack-3.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:32:54.000000 alirpa_pack-3.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-05 06:32:54.000000 alirpa_pack-3.0.2/alirpa_pack.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-05 06:32:53.000000 alirpa_pack-3.0.2/alirpa_pack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2023-05-05 06:32:53.000000 alirpa_pack-3.0.2/alirpa_pack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-05-05 06:32:53.000000 alirpa_pack-3.0.2/alirpa_pack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 06:32:53.000000 alirpa_pack-3.0.2/alirpa_pack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3608 2023-04-19 11:29:31.000000 alirpa_pack-3.0.2/alirpa_pack.py
--rw-rw-rw-   0        0        0      274 2023-05-05 06:32:54.000000 alirpa_pack-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-05 06:32:54.000000 alirpa_pack-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-05-05 06:31:57.000000 alirpa_pack-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:38:56.000000 alirpa_pack-3.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:38:56.000000 alirpa_pack-3.0.3/alirpa_pack.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:38:56.000000 alirpa_pack-3.0.3/alirpa_pack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2023-05-05 06:38:56.000000 alirpa_pack-3.0.3/alirpa_pack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-05 06:38:56.000000 alirpa_pack-3.0.3/alirpa_pack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 06:38:56.000000 alirpa_pack-3.0.3/alirpa_pack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3998 2023-05-05 06:37:14.000000 alirpa_pack-3.0.3/alirpa_pack.py
+-rw-rw-rw-   0        0        0      274 2023-05-05 06:38:56.000000 alirpa_pack-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-05 06:38:56.000000 alirpa_pack-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      396 2023-05-05 06:38:47.000000 alirpa_pack-3.0.3/setup.py
```

