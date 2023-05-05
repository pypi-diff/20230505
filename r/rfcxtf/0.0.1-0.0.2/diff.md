# Comparing `tmp/rfcxtf-0.0.1.tar.gz` & `tmp/rfcxtf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcxtf-0.0.1.tar", last modified: Fri May  5 09:41:04 2023, max compression
+gzip compressed data, was "rfcxtf-0.0.2.tar", last modified: Fri May  5 10:36:50 2023, max compression
```

## Comparing `rfcxtf-0.0.1.tar` & `rfcxtf-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:41:04.183484 rfcxtf-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 09:41:04.181973 rfcxtf-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2955 2023-05-05 09:40:52.000000 rfcxtf-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:41:04.177622 rfcxtf-0.0.1/rfcxtf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 09:41:04.000000 rfcxtf-0.0.1/rfcxtf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-05 09:41:04.000000 rfcxtf-0.0.1/rfcxtf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 09:41:04.000000 rfcxtf-0.0.1/rfcxtf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 09:41:04.000000 rfcxtf-0.0.1/rfcxtf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 09:41:04.000000 rfcxtf-0.0.1/rfcxtf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 09:41:04.184380 rfcxtf-0.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 10:36:50.231644 rfcxtf-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 10:36:50.229963 rfcxtf-0.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 10:36:50.197663 rfcxtf-0.0.2/rfcxtf/
+-rw-r--r--   0 root         (0) root         (0)      593 2023-05-04 09:58:45.000000 rfcxtf-0.0.2/rfcxtf/ClassifierBase.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-05-04 10:33:29.000000 rfcxtf-0.0.2/rfcxtf/ClassifierTF2.py
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-04 10:26:02.000000 rfcxtf-0.0.2/rfcxtf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 10:36:50.225754 rfcxtf-0.0.2/rfcxtf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 10:36:50.232666 rfcxtf-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-05 10:36:01.000000 rfcxtf-0.0.2/setup.py
```

