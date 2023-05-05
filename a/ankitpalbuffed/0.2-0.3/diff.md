# Comparing `tmp/ankitpalbuffed-0.2.tar.gz` & `tmp/ankitpalbuffed-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ankitpalbuffed-0.2.tar", last modified: Fri May  5 13:05:47 2023, max compression
+gzip compressed data, was "dist\ankitpalbuffed-0.3.tar", last modified: Fri May  5 13:14:11 2023, max compression
```

## Comparing `ankitpalbuffed-0.2.tar` & `ankitpalbuffed-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:05:47.000000 ankitpalbuffed-0.2/
--rw-rw-rw-   0        0        0      127 2023-05-05 13:05:47.000000 ankitpalbuffed-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 13:05:47.000000 ankitpalbuffed-0.2/ankitpal/
--rw-rw-rw-   0        0        0       24 2023-05-05 13:05:09.000000 ankitpalbuffed-0.2/ankitpal/__init__.py
--rw-rw-rw-   0        0        0       50 2023-05-05 12:54:39.000000 ankitpalbuffed-0.2/ankitpal/mod1.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:05:47.000000 ankitpalbuffed-0.2/ankitpalbuffed.egg-info/
--rw-rw-rw-   0        0        0      127 2023-05-05 13:05:46.000000 ankitpalbuffed-0.2/ankitpalbuffed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-05-05 13:05:47.000000 ankitpalbuffed-0.2/ankitpalbuffed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:05:46.000000 ankitpalbuffed-0.2/ankitpalbuffed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 13:05:46.000000 ankitpalbuffed-0.2/ankitpalbuffed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 13:05:47.000000 ankitpalbuffed-0.2/setup.cfg
--rw-rw-rw-   0        0        0      161 2023-05-05 13:05:37.000000 ankitpalbuffed-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:11.000000 ankitpalbuffed-0.3/
+-rw-rw-rw-   0        0        0      127 2023-05-05 13:14:11.000000 ankitpalbuffed-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:11.000000 ankitpalbuffed-0.3/ankitpal/
+-rw-rw-rw-   0        0        0       24 2023-05-05 13:05:09.000000 ankitpalbuffed-0.3/ankitpal/__init__.py
+-rw-rw-rw-   0        0        0    38397 2023-05-05 13:13:43.000000 ankitpalbuffed-0.3/ankitpal/mod1.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:11.000000 ankitpalbuffed-0.3/ankitpalbuffed.egg-info/
+-rw-rw-rw-   0        0        0      127 2023-05-05 13:14:10.000000 ankitpalbuffed-0.3/ankitpalbuffed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-05-05 13:14:11.000000 ankitpalbuffed-0.3/ankitpalbuffed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:14:10.000000 ankitpalbuffed-0.3/ankitpalbuffed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 13:14:11.000000 ankitpalbuffed-0.3/ankitpalbuffed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 13:14:11.000000 ankitpalbuffed-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      161 2023-05-05 13:14:07.000000 ankitpalbuffed-0.3/setup.py
```

