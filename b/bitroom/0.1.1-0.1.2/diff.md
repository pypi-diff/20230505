# Comparing `tmp/bitroom-0.1.1.tar.gz` & `tmp/bitroom-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitroom-0.1.1.tar", last modified: Thu May  4 13:34:28 2023, max compression
+gzip compressed data, was "bitroom-0.1.2.tar", last modified: Fri May  5 00:09:08 2023, max compression
```

## Comparing `bitroom-0.1.1.tar` & `bitroom-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2444 2023-05-04 13:34:11.702201 bitroom-0.1.1/README.md
--rw-r--r--   0        0        0      782 2023-05-04 13:34:28.398402 bitroom-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-04 13:34:11.702201 bitroom-0.1.1/src/bitroom/__init__.py
--rw-r--r--   0        0        0       28 2023-05-04 13:34:11.702201 bitroom-0.1.1/src/bitroom/__main__.py
--rw-r--r--   0        0        0       43 2023-05-04 13:34:11.702201 bitroom-0.1.1/src/bitroom/auth/__init__.py
--rw-r--r--   0        0        0     2452 2023-05-04 13:34:11.702201 bitroom-0.1.1/src/bitroom/auth/auth.py
--rw-r--r--   0        0        0    18654 2023-05-04 13:34:11.702201 bitroom-0.1.1/src/bitroom/auth/encrypt_js.py
--rw-r--r--   0        0        0     2532 2023-05-04 13:34:11.706201 bitroom-0.1.1/src/bitroom/cli.py
--rw-r--r--   0        0        0     1642 2023-05-04 13:34:11.706201 bitroom-0.1.1/src/bitroom/config.py
--rw-r--r--   0        0        0     7312 2023-05-04 13:34:11.706201 bitroom-0.1.1/src/bitroom/room.py
--rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 bitroom-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3887 2023-05-05 00:08:46.647926 bitroom-0.1.2/README.md
+-rw-r--r--   0        0        0     1408 2023-05-05 00:09:08.928075 bitroom-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-05 00:08:46.647926 bitroom-0.1.2/src/bitroom/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-05 00:08:46.647926 bitroom-0.1.2/src/bitroom/__main__.py
+-rw-r--r--   0        0        0       43 2023-05-05 00:08:46.647926 bitroom-0.1.2/src/bitroom/auth/__init__.py
+-rw-r--r--   0        0        0     2452 2023-05-05 00:08:46.647926 bitroom-0.1.2/src/bitroom/auth/auth.py
+-rw-r--r--   0        0        0    18654 2023-05-05 00:08:46.647926 bitroom-0.1.2/src/bitroom/auth/encrypt_js.py
+-rw-r--r--   0        0        0     2532 2023-05-05 00:08:46.647926 bitroom-0.1.2/src/bitroom/cli.py
+-rw-r--r--   0        0        0     1642 2023-05-05 00:08:46.647926 bitroom-0.1.2/src/bitroom/config.py
+-rw-r--r--   0        0        0     7312 2023-05-05 00:08:46.647926 bitroom-0.1.2/src/bitroom/room.py
+-rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 bitroom-0.1.2/PKG-INFO
```

### Comparing `bitroom-0.1.1/src/bitroom/auth/auth.py` & `bitroom-0.1.2/src/bitroom/auth/auth.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.1/src/bitroom/auth/encrypt_js.py` & `bitroom-0.1.2/src/bitroom/auth/encrypt_js.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.1/src/bitroom/cli.py` & `bitroom-0.1.2/src/bitroom/cli.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.1/src/bitroom/config.py` & `bitroom-0.1.2/src/bitroom/config.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.1/src/bitroom/room.py` & `bitroom-0.1.2/src/bitroom/room.py`

 * *Files identical despite different names*

