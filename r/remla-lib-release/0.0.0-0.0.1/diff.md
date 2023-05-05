# Comparing `tmp/remla-lib-release-0.0.0.tar.gz` & `tmp/remla-lib-release-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla-lib-release-0.0.0.tar", last modified: Fri May  5 10:22:08 2023, max compression
+gzip compressed data, was "remla-lib-release-0.0.1.tar", last modified: Fri May  5 10:40:04 2023, max compression
```

## Comparing `remla-lib-release-0.0.0.tar` & `remla-lib-release-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:22:08.372067 remla-lib-release-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-05 10:22:08.372067 remla-lib-release-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-05 10:21:58.000000 remla-lib-release-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:22:08.368067 remla-lib-release-0.0.0/remla_lib_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-05 10:22:08.000000 remla-lib-release-0.0.0/remla_lib_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-05 10:22:08.000000 remla-lib-release-0.0.0/remla_lib_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:22:08.000000 remla-lib-release-0.0.0/remla_lib_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:22:08.000000 remla-lib-release-0.0.0/remla_lib_release.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:22:08.372067 remla-lib-release-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-05 10:21:58.000000 remla-lib-release-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:40:04.896013 remla-lib-release-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-05 10:40:04.896013 remla-lib-release-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-05 10:39:53.000000 remla-lib-release-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:40:04.896013 remla-lib-release-0.0.1/remla_lib_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-05 10:40:04.000000 remla-lib-release-0.0.1/remla_lib_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-05 10:40:04.000000 remla-lib-release-0.0.1/remla_lib_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:40:04.000000 remla-lib-release-0.0.1/remla_lib_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:40:04.000000 remla-lib-release-0.0.1/remla_lib_release.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:40:04.896013 remla-lib-release-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-05 10:39:53.000000 remla-lib-release-0.0.1/setup.py
```

