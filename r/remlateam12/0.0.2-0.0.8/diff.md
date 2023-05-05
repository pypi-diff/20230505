# Comparing `tmp/remlateam12-0.0.2.tar.gz` & `tmp/remlateam12-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remlateam12-0.0.2.tar", last modified: Thu May  4 23:39:14 2023, max compression
+gzip compressed data, was "remlateam12-0.0.8.tar", last modified: Fri May  5 00:12:01 2023, max compression
```

## Comparing `remlateam12-0.0.2.tar` & `remlateam12-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:39:14.860978 remlateam12-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 23:39:14.860978 remlateam12-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 23:39:00.000000 remlateam12-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:39:14.860978 remlateam12-0.0.2/remlateam12.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 23:39:14.000000 remlateam12-0.0.2/remlateam12.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 23:39:14.000000 remlateam12-0.0.2/remlateam12.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:39:14.000000 remlateam12-0.0.2/remlateam12.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:39:14.000000 remlateam12-0.0.2/remlateam12.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 23:39:14.860978 remlateam12-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-04 23:39:00.000000 remlateam12-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:12:01.695651 remlateam12-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-05 00:12:01.695651 remlateam12-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 00:11:50.000000 remlateam12-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:12:01.695651 remlateam12-0.0.8/remlateam12.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-05 00:12:01.000000 remlateam12-0.0.8/remlateam12.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 00:12:01.000000 remlateam12-0.0.8/remlateam12.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:12:01.000000 remlateam12-0.0.8/remlateam12.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:12:01.000000 remlateam12-0.0.8/remlateam12.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 00:12:01.695651 remlateam12-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 00:11:50.000000 remlateam12-0.0.8/setup.py
```

