# Comparing `tmp/toast_auth-0.1.0.tar.gz` & `tmp/toast_auth-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toast_auth-0.1.0.tar", last modified: Fri May  5 19:46:07 2023, max compression
+gzip compressed data, was "toast_auth-0.1.1.tar", last modified: Fri May  5 19:51:35 2023, max compression
```

## Comparing `toast_auth-0.1.0.tar` & `toast_auth-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:46:07.047375 toast_auth-0.1.0/
--rw-rw-r--   0 turner    (1000) turner    (1000)      164 2023-05-05 19:46:07.047375 toast_auth-0.1.0/PKG-INFO
--rw-rw-r--   0 turner    (1000) turner    (1000)     1093 2023-05-05 16:23:48.000000 toast_auth-0.1.0/README.md
--rw-rw-r--   0 turner    (1000) turner    (1000)      107 2023-05-05 19:46:07.047375 toast_auth-0.1.0/setup.cfg
--rw-rw-r--   0 turner    (1000) turner    (1000)      555 2023-05-05 19:41:50.000000 toast_auth-0.1.0/setup.py
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:46:07.047375 toast_auth-0.1.0/src/
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:46:07.047375 toast_auth-0.1.0/src/storage/
--rw-rw-r--   0 turner    (1000) turner    (1000)        0 2023-05-05 14:42:59.000000 toast_auth-0.1.0/src/storage/__init__.py
--rw-rw-r--   0 turner    (1000) turner    (1000)     1250 2023-05-05 16:21:15.000000 toast_auth-0.1.0/src/storage/get_token.py
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:46:07.047375 toast_auth-0.1.0/src/toast_auth/
--rw-rw-r--   0 turner    (1000) turner    (1000)       35 2023-05-05 16:10:31.000000 toast_auth-0.1.0/src/toast_auth/__init__.py
--rw-rw-r--   0 turner    (1000) turner    (1000)     3221 2023-05-05 16:29:33.000000 toast_auth-0.1.0/src/toast_auth/toast_token.py
-drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:46:07.047375 toast_auth-0.1.0/src/toast_auth.egg-info/
--rw-rw-r--   0 turner    (1000) turner    (1000)      164 2023-05-05 19:46:07.000000 toast_auth-0.1.0/src/toast_auth.egg-info/PKG-INFO
--rw-rw-r--   0 turner    (1000) turner    (1000)      323 2023-05-05 19:46:07.000000 toast_auth-0.1.0/src/toast_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 turner    (1000) turner    (1000)        1 2023-05-05 19:46:07.000000 toast_auth-0.1.0/src/toast_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 turner    (1000) turner    (1000)      104 2023-05-05 19:46:07.000000 toast_auth-0.1.0/src/toast_auth.egg-info/requires.txt
--rw-rw-r--   0 turner    (1000) turner    (1000)       19 2023-05-05 19:46:07.000000 toast_auth-0.1.0/src/toast_auth.egg-info/top_level.txt
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/
+-rw-rw-r--   0 turner    (1000) turner    (1000)      247 2023-05-05 19:51:35.107593 toast_auth-0.1.1/PKG-INFO
+-rw-rw-r--   0 turner    (1000) turner    (1000)     1093 2023-05-05 16:23:48.000000 toast_auth-0.1.1/README.md
+-rw-rw-r--   0 turner    (1000) turner    (1000)      107 2023-05-05 19:51:35.111593 toast_auth-0.1.1/setup.cfg
+-rw-rw-r--   0 turner    (1000) turner    (1000)      638 2023-05-05 19:51:27.000000 toast_auth-0.1.1/setup.py
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/src/
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/src/storage/
+-rw-rw-r--   0 turner    (1000) turner    (1000)        0 2023-05-05 14:42:59.000000 toast_auth-0.1.1/src/storage/__init__.py
+-rw-rw-r--   0 turner    (1000) turner    (1000)     1250 2023-05-05 16:21:15.000000 toast_auth-0.1.1/src/storage/get_token.py
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/src/toast_auth/
+-rw-rw-r--   0 turner    (1000) turner    (1000)       35 2023-05-05 16:10:31.000000 toast_auth-0.1.1/src/toast_auth/__init__.py
+-rw-rw-r--   0 turner    (1000) turner    (1000)     3221 2023-05-05 16:29:33.000000 toast_auth-0.1.1/src/toast_auth/toast_token.py
+drwxrwxr-x   0 turner    (1000) turner    (1000)        0 2023-05-05 19:51:35.107593 toast_auth-0.1.1/src/toast_auth.egg-info/
+-rw-rw-r--   0 turner    (1000) turner    (1000)      247 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 turner    (1000) turner    (1000)      323 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 turner    (1000) turner    (1000)        1 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 turner    (1000) turner    (1000)      104 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/requires.txt
+-rw-rw-r--   0 turner    (1000) turner    (1000)       19 2023-05-05 19:51:35.000000 toast_auth-0.1.1/src/toast_auth.egg-info/top_level.txt
```

### Comparing `toast_auth-0.1.0/README.md` & `toast_auth-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `toast_auth-0.1.0/src/storage/get_token.py` & `toast_auth-0.1.1/src/storage/get_token.py`

 * *Files identical despite different names*

### Comparing `toast_auth-0.1.0/src/toast_auth/toast_token.py` & `toast_auth-0.1.1/src/toast_auth/toast_token.py`

 * *Files identical despite different names*

