# Comparing `tmp/tybase-0.0.2.tar.gz` & `tmp/tybase-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.0.2.tar", last modified: Thu May  4 00:03:59 2023, max compression
+gzip compressed data, was "tybase-0.0.3.tar", last modified: Fri May  5 10:41:57 2023, max compression
```

## Comparing `tybase-0.0.2.tar` & `tybase-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-04 00:03:59.636821 tybase-0.0.2/
--rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.0.2/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      438 2023-05-04 00:03:59.636521 tybase-0.0.2/PKG-INFO
--rw-r--r--   0 zhangte    (501) staff       (20)       10 2023-05-03 23:47:36.000000 tybase-0.0.2/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-04 00:03:59.636929 tybase-0.0.2/setup.cfg
--rw-r--r--   0 zhangte    (501) staff       (20)      789 2023-05-04 00:03:27.000000 tybase-0.0.2/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-04 00:03:59.633835 tybase-0.0.2/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.0.2/tybase/__init__.py
--rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.0.2/tybase/datatest.txt
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.0.2/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-04 00:03:59.635906 tybase-0.0.2/tybase.egg-info/
--rw-r--r--   0 zhangte    (501) staff       (20)      438 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/PKG-INFO
--rw-r--r--   0 zhangte    (501) staff       (20)      235 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/dependency_links.txt
--rw-r--r--   0 zhangte    (501) staff       (20)       20 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-05 10:41:57.025047 tybase-0.0.3/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.0.3/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      612 2023-05-05 10:41:57.024679 tybase-0.0.3/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      100 2023-05-05 10:39:34.000000 tybase-0.0.3/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-05 10:41:57.025164 tybase-0.0.3/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      837 2023-05-05 10:41:53.000000 tybase-0.0.3/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-05 10:41:56.976924 tybase-0.0.3/tybase/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.0.3/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-05 10:41:56.980045 tybase-0.0.3/tybase/baidu/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.0.3/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4126 2023-05-05 10:37:20.000000 tybase-0.0.3/tybase/baidu/kw_tool.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.0.3/tybase/datatest.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.0.3/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-05 10:41:56.979438 tybase-0.0.3/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      612 2023-05-05 10:41:55.000000 tybase-0.0.3/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      284 2023-05-05 10:41:56.000000 tybase-0.0.3/tybase.egg-info/SOURCES.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-05-05 10:41:55.000000 tybase-0.0.3/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       20 2023-05-05 10:41:56.000000 tybase-0.0.3/tybase.egg-info/requires.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-05-05 10:41:56.000000 tybase-0.0.3/tybase.egg-info/top_level.txt
```

