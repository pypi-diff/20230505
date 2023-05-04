# Comparing `tmp/frazzle-0.2.1.tar.gz` & `tmp/frazzle-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frazzle-0.2.1.tar", max compression
+gzip compressed data, was "frazzle-0.2.2.tar", max compression
```

## Comparing `frazzle-0.2.1.tar` & `frazzle-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-04 16:47:23.012784 frazzle-0.2.1/frazzle/__init__.py
--rw-r--r--   0        0        0       66 2023-05-04 16:48:25.089104 frazzle-0.2.1/frazzle/__main__.py
--rw-r--r--   0        0        0     1259 2023-05-04 16:48:13.852312 frazzle-0.2.1/frazzle/client.py
--rw-r--r--   0        0        0      492 2023-05-04 16:48:35.034491 frazzle-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       15 2023-05-04 16:45:06.940554 frazzle-0.2.1/README.md
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 frazzle-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-04 16:47:23.012784 frazzle-0.2.2/frazzle/__init__.py
+-rw-r--r--   0        0        0       66 2023-05-04 16:51:20.691459 frazzle-0.2.2/frazzle/__main__.py
+-rw-r--r--   0        0        0     1259 2023-05-04 16:51:38.615239 frazzle-0.2.2/frazzle/client.py
+-rw-r--r--   0        0        0      548 2023-05-04 22:36:59.102697 frazzle-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-05-04 22:34:52.447786 frazzle-0.2.2/README.md
+-rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 frazzle-0.2.2/PKG-INFO
```

### Comparing `frazzle-0.2.1/frazzle/client.py` & `frazzle-0.2.2/frazzle/client.py`

 * *Files identical despite different names*

