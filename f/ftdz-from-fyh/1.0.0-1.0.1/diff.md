# Comparing `tmp/ftdz_from_fyh-1.0.0.tar.gz` & `tmp/ftdz_from_fyh-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ftdz_from_fyh-1.0.0.tar", last modified: Thu May  4 11:03:16 2023, max compression
+gzip compressed data, was "dist\ftdz_from_fyh-1.0.1.tar", last modified: Fri May  5 10:18:28 2023, max compression
```

## Comparing `ftdz_from_fyh-1.0.0.tar` & `ftdz_from_fyh-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 11:03:16.000000 ftdz_from_fyh-1.0.0/
--rw-rw-rw-   0        0        0      391 2023-05-04 11:03:16.000000 ftdz_from_fyh-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      346 2019-08-22 10:27:16.000000 ftdz_from_fyh-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 11:03:16.000000 ftdz_from_fyh-1.0.0/ftdz_from_fyh.egg-info/
--rw-rw-rw-   0        0        0      391 2023-05-04 11:03:16.000000 ftdz_from_fyh-1.0.0/ftdz_from_fyh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-05-04 11:03:16.000000 ftdz_from_fyh-1.0.0/ftdz_from_fyh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 11:03:16.000000 ftdz_from_fyh-1.0.0/ftdz_from_fyh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 11:03:16.000000 ftdz_from_fyh-1.0.0/ftdz_from_fyh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 11:03:16.000000 ftdz_from_fyh-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 10:18:28.000000 ftdz_from_fyh-1.0.1/
+-rw-rw-rw-   0        0        0      391 2023-05-05 10:18:28.000000 ftdz_from_fyh-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2019-08-22 10:27:16.000000 ftdz_from_fyh-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 10:18:28.000000 ftdz_from_fyh-1.0.1/ftdz_from_fyh.egg-info/
+-rw-rw-rw-   0        0        0      391 2023-05-05 10:18:28.000000 ftdz_from_fyh-1.0.1/ftdz_from_fyh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-05-05 10:18:28.000000 ftdz_from_fyh-1.0.1/ftdz_from_fyh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:18:28.000000 ftdz_from_fyh-1.0.1/ftdz_from_fyh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:18:28.000000 ftdz_from_fyh-1.0.1/ftdz_from_fyh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 10:18:28.000000 ftdz_from_fyh-1.0.1/setup.cfg
```

