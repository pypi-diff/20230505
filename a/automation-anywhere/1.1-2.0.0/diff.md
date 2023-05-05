# Comparing `tmp/automation_anywhere-1.1.tar.gz` & `tmp/automation_anywhere-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/automation_anywhere-1.1.tar", last modified: Fri Mar 29 22:18:05 2019, max compression
+gzip compressed data, was "automation_anywhere-2.0.0.tar", last modified: Fri May  5 19:03:06 2023, max compression
```

## Comparing `automation_anywhere-1.1.tar` & `automation_anywhere-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 minterciso  (1000) minterciso  (1000)        0 2019-03-29 22:18:05.000000 automation_anywhere-1.1/
-drwxrwxr-x   0 minterciso  (1000) minterciso  (1000)        0 2019-03-29 22:18:05.000000 automation_anywhere-1.1/automation_anywhere.egg-info/
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)     5743 2019-03-29 22:18:05.000000 automation_anywhere-1.1/automation_anywhere.egg-info/PKG-INFO
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)      322 2019-03-29 22:18:05.000000 automation_anywhere-1.1/automation_anywhere.egg-info/SOURCES.txt
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)       50 2019-03-29 22:18:05.000000 automation_anywhere-1.1/automation_anywhere.egg-info/requires.txt
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)        1 2019-03-29 22:18:05.000000 automation_anywhere-1.1/automation_anywhere.egg-info/dependency_links.txt
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)       20 2019-03-29 22:18:05.000000 automation_anywhere-1.1/automation_anywhere.egg-info/top_level.txt
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)     5743 2019-03-29 22:18:05.000000 automation_anywhere-1.1/PKG-INFO
-drwxrwxr-x   0 minterciso  (1000) minterciso  (1000)        0 2019-03-29 22:18:05.000000 automation_anywhere-1.1/automation_anywhere/
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)    14799 2019-03-29 22:13:46.000000 automation_anywhere-1.1/automation_anywhere/base.py
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)       56 2019-03-29 22:13:56.000000 automation_anywhere-1.1/automation_anywhere/__init__.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      224 2019-03-29 18:41:49.000000 automation_anywhere-1.1/automation_anywhere/errors.py
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)     4422 2019-03-29 22:13:46.000000 automation_anywhere-1.1/README.md
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)       38 2019-03-29 22:18:05.000000 automation_anywhere-1.1/setup.cfg
--rw-rw-r--   0 minterciso  (1000) minterciso  (1000)      783 2019-03-29 22:14:16.000000 automation_anywhere-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:03:06.632693 automation_anywhere-2.0.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-03 18:24:17.000000 automation_anywhere-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2386 2023-05-05 19:03:06.629692 automation_anywhere-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1794 2023-05-05 18:54:19.000000 automation_anywhere-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 19:03:06.434035 automation_anywhere-2.0.0/automation_anywhere/
+-rw-rw-rw-   0        0        0       57 2023-05-03 18:24:17.000000 automation_anywhere-2.0.0/automation_anywhere/__init__.py
+-rw-rw-rw-   0        0        0     4171 2023-05-05 18:15:54.000000 automation_anywhere-2.0.0/automation_anywhere/base.py
+-rw-rw-rw-   0        0        0      190 2023-05-05 16:43:55.000000 automation_anywhere-2.0.0/automation_anywhere/errors.py
+-rw-rw-rw-   0        0        0     7724 2023-05-05 18:30:08.000000 automation_anywhere-2.0.0/automation_anywhere/executor.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:03:06.620635 automation_anywhere-2.0.0/automation_anywhere.egg-info/
+-rw-rw-rw-   0        0        0     2386 2023-05-05 19:03:06.000000 automation_anywhere-2.0.0/automation_anywhere.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-05-05 19:03:06.000000 automation_anywhere-2.0.0/automation_anywhere.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:03:06.000000 automation_anywhere-2.0.0/automation_anywhere.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-05 19:03:06.000000 automation_anywhere-2.0.0/automation_anywhere.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      661 2023-05-05 19:02:29.000000 automation_anywhere-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 19:03:06.633691 automation_anywhere-2.0.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

