# Comparing `tmp/freeplay_sdk-0.1.8.tar.gz` & `tmp/freeplay_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay_sdk-0.1.8.tar", max compression
+gzip compressed data, was "freeplay_sdk-0.1.9.tar", max compression
```

## Comparing `freeplay_sdk-0.1.8.tar` & `freeplay_sdk-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-21 22:52:48.038840 freeplay_sdk-0.1.8/README.md
--rw-r--r--   0        0        0       62 2023-04-24 20:37:56.560899 freeplay_sdk-0.1.8/freeplay_sdk/__init__.py
--rw-r--r--   0        0        0     1841 2023-04-24 20:37:56.561069 freeplay_sdk-0.1.8/freeplay_sdk/freeplay.py
--rw-r--r--   0        0        0      516 2023-04-21 22:46:23.482809 freeplay_sdk-0.1.8/freeplay_sdk/json_support.py
--rw-r--r--   0        0        0      350 2023-04-24 20:52:39.875656 freeplay_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 freeplay_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-21 22:52:48.038840 freeplay_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0       62 2023-04-24 20:37:56.560899 freeplay_sdk-0.1.9/freeplay_sdk/__init__.py
+-rw-r--r--   0        0        0     1841 2023-04-24 20:37:56.561069 freeplay_sdk-0.1.9/freeplay_sdk/freeplay.py
+-rw-r--r--   0        0        0      516 2023-04-21 22:46:23.482809 freeplay_sdk-0.1.9/freeplay_sdk/json_support.py
+-rw-r--r--   0        0        0      354 2023-04-24 20:58:06.641125 freeplay_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 freeplay_sdk-0.1.9/PKG-INFO
```

### Comparing `freeplay_sdk-0.1.8/freeplay_sdk/freeplay.py` & `freeplay_sdk-0.1.9/freeplay_sdk/freeplay.py`

 * *Files identical despite different names*

### Comparing `freeplay_sdk-0.1.8/freeplay_sdk/json_support.py` & `freeplay_sdk-0.1.9/freeplay_sdk/json_support.py`

 * *Files identical despite different names*

