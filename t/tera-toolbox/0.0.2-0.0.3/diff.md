# Comparing `tmp/tera-toolbox-0.0.2.tar.gz` & `tmp/tera-toolbox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tera-toolbox-0.0.2.tar", last modified: Tue Feb 14 20:00:53 2023, max compression
+gzip compressed data, was "tera-toolbox-0.0.3.tar", last modified: Fri May  5 14:00:28 2023, max compression
```

## Comparing `tera-toolbox-0.0.2.tar` & `tera-toolbox-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 20:00:53.544331 tera-toolbox-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-02-14 20:00:53.544331 tera-toolbox-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-02-14 20:00:45.000000 tera-toolbox-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-14 20:00:53.544331 tera-toolbox-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-02-14 20:00:45.000000 tera-toolbox-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 20:00:53.544331 tera-toolbox-0.0.2/tera_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-02-14 20:00:53.000000 tera-toolbox-0.0.2/tera_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-02-14 20:00:53.000000 tera-toolbox-0.0.2/tera_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-14 20:00:53.000000 tera-toolbox-0.0.2/tera_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-02-14 20:00:53.000000 tera-toolbox-0.0.2/tera_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-02-14 20:00:53.000000 tera-toolbox-0.0.2/tera_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 20:00:53.544331 tera-toolbox-0.0.2/toolbox/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-02-14 20:00:45.000000 tera-toolbox-0.0.2/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-02-14 20:00:45.000000 tera-toolbox-0.0.2/toolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-02-14 20:00:45.000000 tera-toolbox-0.0.2/toolbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 14:00:28.911651 tera-toolbox-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-05 14:00:28.911651 tera-toolbox-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-05 14:00:15.000000 tera-toolbox-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 14:00:28.911651 tera-toolbox-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-05 14:00:15.000000 tera-toolbox-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 14:00:28.907650 tera-toolbox-0.0.3/tera_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-05 14:00:28.000000 tera-toolbox-0.0.3/tera_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-05 14:00:28.000000 tera-toolbox-0.0.3/tera_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 14:00:28.000000 tera-toolbox-0.0.3/tera_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-05 14:00:28.000000 tera-toolbox-0.0.3/tera_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-05 14:00:28.000000 tera-toolbox-0.0.3/tera_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 14:00:28.911651 tera-toolbox-0.0.3/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-05-05 14:00:15.000000 tera-toolbox-0.0.3/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-05 14:00:15.000000 tera-toolbox-0.0.3/toolbox/stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-05 14:00:15.000000 tera-toolbox-0.0.3/toolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-05 14:00:15.000000 tera-toolbox-0.0.3/toolbox/version.py
```

### Comparing `tera-toolbox-0.0.2/setup.py` & `tera-toolbox-0.0.3/setup.py`

 * *Files identical despite different names*

