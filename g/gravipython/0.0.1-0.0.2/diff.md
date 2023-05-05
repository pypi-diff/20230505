# Comparing `tmp/gravipython-0.0.1.tar.gz` & `tmp/gravipython-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravipython-0.0.1.tar", last modified: Thu May  4 11:32:41 2023, max compression
+gzip compressed data, was "gravipython-0.0.2.tar", last modified: Fri May  5 13:29:20 2023, max compression
```

## Comparing `gravipython-0.0.1.tar` & `gravipython-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 11:32:41.697673 gravipython-0.0.1/
--rw-rw-rw-   0        0        0      147 2023-05-04 11:32:41.695894 gravipython-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-04 11:32:41.690766 gravipython-0.0.1/gravipython.egg-info/
--rw-rw-rw-   0        0        0      147 2023-05-04 11:32:41.000000 gravipython-0.0.1/gravipython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-04 11:32:41.000000 gravipython-0.0.1/gravipython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 11:32:41.000000 gravipython-0.0.1/gravipython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 11:32:41.000000 gravipython-0.0.1/gravipython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       40 2023-05-04 11:32:41.000000 gravipython-0.0.1/gravipython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 11:32:41.697673 gravipython-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 13:29:22.000000 gravipython-0.0.2/
+-rw-rw-rw-   0        0        0      174 2023-05-05 13:29:22.000000 gravipython-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1424 2023-05-03 09:36:18.000000 gravipython-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 13:29:22.000000 gravipython-0.0.2/gravipython.egg-info/
+-rw-rw-rw-   0        0        0      174 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       40 2023-05-05 13:29:20.000000 gravipython-0.0.2/gravipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1060 2023-05-02 13:51:28.000000 gravipython-0.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 13:29:22.000000 gravipython-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-05-05 13:29:14.000000 gravipython-0.0.2/setup.py
```

