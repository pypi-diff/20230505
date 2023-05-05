# Comparing `tmp/scrapetron-1.0.0.tar.gz` & `tmp/scrapetron-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapetron-1.0.0.tar", last modified: Fri May  5 06:24:17 2023, max compression
+gzip compressed data, was "scrapetron-1.0.1.tar", last modified: Fri May  5 08:36:00 2023, max compression
```

## Comparing `scrapetron-1.0.0.tar` & `scrapetron-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 rohansanjeev   (501) staff       (20)        0 2023-05-05 06:24:17.267677 scrapetron-1.0.0/
--rw-r--r--   0 rohansanjeev   (501) staff       (20)     1062 2023-05-05 06:20:23.000000 scrapetron-1.0.0/LICENSE
--rw-r--r--   0 rohansanjeev   (501) staff       (20)      265 2023-05-05 06:24:17.267512 scrapetron-1.0.0/PKG-INFO
-drwxr-xr-x   0 rohansanjeev   (501) staff       (20)        0 2023-05-05 06:24:17.267254 scrapetron-1.0.0/scrapetron.egg-info/
--rw-r--r--   0 rohansanjeev   (501) staff       (20)      265 2023-05-05 06:24:17.000000 scrapetron-1.0.0/scrapetron.egg-info/PKG-INFO
--rw-r--r--   0 rohansanjeev   (501) staff       (20)      185 2023-05-05 06:24:17.000000 scrapetron-1.0.0/scrapetron.egg-info/SOURCES.txt
--rw-r--r--   0 rohansanjeev   (501) staff       (20)        1 2023-05-05 06:24:17.000000 scrapetron-1.0.0/scrapetron.egg-info/dependency_links.txt
--rw-r--r--   0 rohansanjeev   (501) staff       (20)       35 2023-05-05 06:24:17.000000 scrapetron-1.0.0/scrapetron.egg-info/requires.txt
--rw-r--r--   0 rohansanjeev   (501) staff       (20)        1 2023-05-05 06:24:17.000000 scrapetron-1.0.0/scrapetron.egg-info/top_level.txt
--rw-r--r--   0 rohansanjeev   (501) staff       (20)       38 2023-05-05 06:24:17.267751 scrapetron-1.0.0/setup.cfg
--rw-r--r--   0 rohansanjeev   (501) staff       (20)      392 2023-05-05 06:23:45.000000 scrapetron-1.0.0/setup.py
+drwxr-xr-x   0 rohansanjeev   (501) staff       (20)        0 2023-05-05 08:36:00.309309 scrapetron-1.0.1/
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)     1062 2023-05-05 06:20:23.000000 scrapetron-1.0.1/LICENSE
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)      448 2023-05-05 08:36:00.309152 scrapetron-1.0.1/PKG-INFO
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)     1436 2023-05-05 08:31:47.000000 scrapetron-1.0.1/README.md
+drwxr-xr-x   0 rohansanjeev   (501) staff       (20)        0 2023-05-05 08:36:00.308916 scrapetron-1.0.1/scrapetron.egg-info/
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)      448 2023-05-05 08:36:00.000000 scrapetron-1.0.1/scrapetron.egg-info/PKG-INFO
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)      195 2023-05-05 08:36:00.000000 scrapetron-1.0.1/scrapetron.egg-info/SOURCES.txt
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)        1 2023-05-05 08:36:00.000000 scrapetron-1.0.1/scrapetron.egg-info/dependency_links.txt
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)       35 2023-05-05 08:36:00.000000 scrapetron-1.0.1/scrapetron.egg-info/requires.txt
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)        1 2023-05-05 08:36:00.000000 scrapetron-1.0.1/scrapetron.egg-info/top_level.txt
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)       38 2023-05-05 08:36:00.309367 scrapetron-1.0.1/setup.cfg
+-rw-r--r--   0 rohansanjeev   (501) staff       (20)      575 2023-05-05 08:32:15.000000 scrapetron-1.0.1/setup.py
```

### Comparing `scrapetron-1.0.0/LICENSE` & `scrapetron-1.0.1/LICENSE`

 * *Files identical despite different names*

