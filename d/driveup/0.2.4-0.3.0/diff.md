# Comparing `tmp/driveup-0.2.4.tar.gz` & `tmp/driveup-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driveup-0.2.4.tar", last modified: Fri Apr 21 08:01:38 2023, max compression
+gzip compressed data, was "driveup-0.3.0.tar", last modified: Fri May  5 14:12:31 2023, max compression
```

## Comparing `driveup-0.2.4.tar` & `driveup-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:38.498036 driveup-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:38.498036 driveup-0.2.4/Driveup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:27.000000 driveup-0.2.4/Driveup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-21 08:01:27.000000 driveup-0.2.4/Driveup/drive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:38.498036 driveup-0.2.4/Driveup/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:27.000000 driveup-0.2.4/Driveup/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-21 08:01:27.000000 driveup-0.2.4/Driveup/features/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 08:01:27.000000 driveup-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 08:01:38.498036 driveup-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 08:01:27.000000 driveup-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:38.498036 driveup-0.2.4/driveup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 08:01:38.000000 driveup-0.2.4/driveup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-21 08:01:38.000000 driveup-0.2.4/driveup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:01:38.000000 driveup-0.2.4/driveup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 08:01:38.000000 driveup-0.2.4/driveup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 08:01:38.000000 driveup-0.2.4/driveup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:01:38.498036 driveup-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 08:01:27.000000 driveup-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:31.782610 driveup-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:31.778610 driveup-0.3.0/Driveup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:20.000000 driveup-0.3.0/Driveup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-05 14:12:20.000000 driveup-0.3.0/Driveup/drive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:31.778610 driveup-0.3.0/Driveup/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:20.000000 driveup-0.3.0/Driveup/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 14:12:20.000000 driveup-0.3.0/Driveup/features/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 14:12:20.000000 driveup-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 14:12:31.782610 driveup-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 14:12:20.000000 driveup-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:31.782610 driveup-0.3.0/driveup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:12:31.782610 driveup-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-05 14:12:20.000000 driveup-0.3.0/setup.py
```

### Comparing `driveup-0.2.4/LICENSE` & `driveup-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `driveup-0.2.4/setup.py` & `driveup-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # ...
 
 setup(
     long_description=README_DESCRIPTION,
     long_description_content_type="text/markdown",
     name='driveup',
-    version='0.2.4',
+    version='0.3.0',
     author='Raúl M.R.',
     author_email="raul.martin4bc@gmail.com",
     license="MIT",
     description='Python package for uploading files and folders to Google Drive',
     packages=find_packages(include=["Driveup","Driveup.features"]),
     install_requires=[
         'pandas',
```

