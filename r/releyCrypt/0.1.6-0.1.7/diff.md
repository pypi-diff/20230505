# Comparing `tmp/releyCrypt-0.1.6.tar.gz` & `tmp/releyCrypt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "releyCrypt-0.1.6.tar", last modified: Fri May  5 12:14:53 2023, max compression
+gzip compressed data, was "releyCrypt-0.1.7.tar", last modified: Fri May  5 19:28:25 2023, max compression
```

## Comparing `releyCrypt-0.1.6.tar` & `releyCrypt-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/
--rw-rw-rw-   0        0        0      145 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/releyCrypt/
--rw-rw-rw-   0        0        0      139 2023-04-29 19:29:24.000000 releyCrypt-0.1.6/releyCrypt/__init__.py
--rw-rw-rw-   0        0        0      846 2023-05-05 12:14:42.000000 releyCrypt-0.1.6/releyCrypt/decrypter.py
--rw-rw-rw-   0        0        0    35161 2023-04-23 19:09:26.000000 releyCrypt-0.1.6/releyCrypt/hypixel_api.py
--rw-rw-rw-   0        0        0      770 2023-04-20 19:34:26.000000 releyCrypt-0.1.6/releyCrypt/python_mc.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/releyCrypt.egg-info/
--rw-rw-rw-   0        0        0      145 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/releyCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/releyCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/releyCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/releyCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/releyCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 12:14:54.000000 releyCrypt-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-05-05 12:13:46.000000 releyCrypt-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/
+-rw-rw-rw-   0        0        0      145 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/releyCrypt/
+-rw-rw-rw-   0        0        0      139 2023-04-29 19:29:24.000000 releyCrypt-0.1.7/releyCrypt/__init__.py
+-rw-rw-rw-   0        0        0      846 2023-05-05 12:14:42.000000 releyCrypt-0.1.7/releyCrypt/decrypter.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/releyCrypt.egg-info/
+-rw-rw-rw-   0        0        0      145 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/releyCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/releyCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/releyCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/releyCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/releyCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 19:28:26.000000 releyCrypt-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-05-05 19:28:06.000000 releyCrypt-0.1.7/setup.py
```

### Comparing `releyCrypt-0.1.6/releyCrypt/decrypter.py` & `releyCrypt-0.1.7/releyCrypt/decrypter.py`

 * *Files identical despite different names*

