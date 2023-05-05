# Comparing `tmp/fpyo2ipa-1.0.tar.gz` & `tmp/fpyo2ipa-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpyo2ipa-1.0.tar", last modified: Fri May  5 17:35:34 2023, max compression
+gzip compressed data, was "fpyo2ipa-1.0.3.tar", last modified: Fri May  5 17:57:18 2023, max compression
```

## Comparing `fpyo2ipa-1.0.tar` & `fpyo2ipa-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,30 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:35:34.697909 fpyo2ipa-1.0/
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-05-05 13:41:18.000000 fpyo2ipa-1.0/LICENSE
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       17 2023-05-05 13:41:33.000000 fpyo2ipa-1.0/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      352 2023-05-05 17:35:34.697771 fpyo2ipa-1.0/PKG-INFO
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:19:31.000000 fpyo2ipa-1.0/README.md
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:35:34.697524 fpyo2ipa-1.0/fpyo2ipa.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      352 2023-05-05 17:35:34.000000 fpyo2ipa-1.0/fpyo2ipa.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      212 2023-05-05 17:35:34.000000 fpyo2ipa-1.0/fpyo2ipa.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-05-05 17:35:34.000000 fpyo2ipa-1.0/fpyo2ipa.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       10 2023-05-05 17:35:34.000000 fpyo2ipa-1.0/fpyo2ipa.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-05-05 17:35:34.000000 fpyo2ipa-1.0/fpyo2ipa.egg-info/top_level.txt
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-05-05 13:41:18.000000 fpyo2ipa-1.0/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-05-05 17:35:34.697959 fpyo2ipa-1.0/setup.cfg
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      501 2023-05-05 17:19:20.000000 fpyo2ipa-1.0/setup.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:57:18.596519 fpyo2ipa-1.0.3/
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-05-05 13:41:18.000000 fpyo2ipa-1.0.3/LICENSE
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)       83 2023-05-05 17:56:02.000000 fpyo2ipa-1.0.3/MANIFEST.in
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      354 2023-05-05 17:57:18.596388 fpyo2ipa-1.0.3/PKG-INFO
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:19:31.000000 fpyo2ipa-1.0.3/README.md
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:57:18.594066 fpyo2ipa-1.0.3/fpyo2ipa/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:57:18.595200 fpyo2ipa-1.0.3/fpyo2ipa/Tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:29.000000 fpyo2ipa-1.0.3/fpyo2ipa/Tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      124 2023-05-05 13:35:04.000000 fpyo2ipa-1.0.3/fpyo2ipa/Tools/check_system.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      137 2023-05-05 13:33:33.000000 fpyo2ipa-1.0.3/fpyo2ipa/Tools/check_venv.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1140 2023-05-05 17:29:43.000000 fpyo2ipa-1.0.3/fpyo2ipa/Tools/unzip_assets.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:02.000000 fpyo2ipa-1.0.3/fpyo2ipa/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:57:18.595434 fpyo2ipa-1.0.3/fpyo2ipa/assets/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:13.000000 fpyo2ipa-1.0.3/fpyo2ipa/assets/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)   478420 2023-05-05 17:30:11.000000 fpyo2ipa-1.0.3/fpyo2ipa/assets/pyo2ipadist.zip
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:57:18.596189 fpyo2ipa-1.0.3/fpyo2ipa/beeware_tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:20.000000 fpyo2ipa-1.0.3/fpyo2ipa/beeware_tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1721 2023-05-05 17:32:24.000000 fpyo2ipa-1.0.3/fpyo2ipa/beeware_tools/edit_beeware_project.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1838 2023-05-05 17:16:53.000000 fpyo2ipa-1.0.3/fpyo2ipa/beeware_tools/the_app_py.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      977 2023-05-05 14:43:41.000000 fpyo2ipa-1.0.3/fpyo2ipa/beeware_tools/the_localhost_py.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      593 2023-05-05 17:19:11.000000 fpyo2ipa-1.0.3/fpyo2ipa/build.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:57:18.594719 fpyo2ipa-1.0.3/fpyo2ipa.egg-info/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      354 2023-05-05 17:57:18.000000 fpyo2ipa-1.0.3/fpyo2ipa.egg-info/PKG-INFO
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      591 2023-05-05 17:57:18.000000 fpyo2ipa-1.0.3/fpyo2ipa.egg-info/SOURCES.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-05-05 17:57:18.000000 fpyo2ipa-1.0.3/fpyo2ipa.egg-info/dependency_links.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       10 2023-05-05 17:57:18.000000 fpyo2ipa-1.0.3/fpyo2ipa.egg-info/requires.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        9 2023-05-05 17:57:18.000000 fpyo2ipa-1.0.3/fpyo2ipa.egg-info/top_level.txt
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-05-05 17:49:16.000000 fpyo2ipa-1.0.3/pyproject.toml
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-05-05 17:57:18.596566 fpyo2ipa-1.0.3/setup.cfg
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      613 2023-05-05 17:57:11.000000 fpyo2ipa-1.0.3/setup.py
```

### Comparing `fpyo2ipa-1.0/LICENSE` & `fpyo2ipa-1.0.3/LICENSE`

 * *Files identical despite different names*

