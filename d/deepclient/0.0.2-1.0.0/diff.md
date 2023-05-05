# Comparing `tmp/deepclient-0.0.2.tar.gz` & `tmp/deepclient-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepclient-0.0.2.tar", last modified: Thu May  4 15:15:29 2023, max compression
+gzip compressed data, was "deepclient-1.0.0.tar", last modified: Mon Apr 18 14:48:59 2022, max compression
```

## Comparing `deepclient-0.0.2.tar` & `deepclient-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:15:29.789080 deepclient-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 15:15:29.789080 deepclient-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:15:29.789080 deepclient-0.0.2/deepclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 15:15:29.000000 deepclient-0.0.2/deepclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-04 15:15:29.000000 deepclient-0.0.2/deepclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:15:29.000000 deepclient-0.0.2/deepclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:15:29.000000 deepclient-0.0.2/deepclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:15:29.789080 deepclient-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-04 15:15:19.000000 deepclient-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2022-04-18 14:48:59.169434 deepclient-1.0.0/
+-rw-rw-rw-   0        0        0      998 2022-04-18 14:48:59.169434 deepclient-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2022-01-27 09:13:39.000000 deepclient-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2022-04-18 14:48:59.148453 deepclient-1.0.0/deepclient/
+-rw-rw-rw-   0        0        0      148 2022-04-17 05:33:45.000000 deepclient-1.0.0/deepclient/__init__.py
+-rw-rw-rw-   0        0        0     7406 2022-04-18 14:47:20.000000 deepclient-1.0.0/deepclient/client.py
+-rw-rw-rw-   0        0        0      258 2022-04-17 05:25:40.000000 deepclient-1.0.0/deepclient/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-04-18 14:48:59.165432 deepclient-1.0.0/deepclient.egg-info/
+-rw-rw-rw-   0        0        0      998 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-04-18 14:48:59.169434 deepclient-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2022-04-18 14:48:37.000000 deepclient-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-04-18 14:48:59.168433 deepclient-1.0.0/tests/
+-rw-rw-rw-   0        0        0      103 2022-03-13 07:21:35.000000 deepclient-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      371 2022-04-17 05:12:27.000000 deepclient-1.0.0/tests/config.py
+-rw-rw-rw-   0        0        0     4332 2022-04-17 09:37:26.000000 deepclient-1.0.0/tests/test_client.py
```

