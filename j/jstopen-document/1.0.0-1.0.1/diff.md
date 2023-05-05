# Comparing `tmp/jstopen-document-1.0.0.tar.gz` & `tmp/jstopen-document-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jstopen-document-1.0.0.tar", last modified: Mon Sep  6 06:22:19 2021, max compression
+gzip compressed data, was "jstopen-document-1.0.1.tar", last modified: Fri May  5 01:31:06 2023, max compression
```

## Comparing `jstopen-document-1.0.0.tar` & `jstopen-document-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
-drwxrwxrwx   0        0        0        0 2021-09-06 06:22:19.000000 jstopen-document-1.0.0/
--rw-rw-rw-   0        0        0      228 2021-09-06 06:22:19.000000 jstopen-document-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-09-06 06:22:19.000000 jstopen-document-1.0.0/jstopen/
-drwxrwxrwx   0        0        0        0 2021-09-06 06:22:19.000000 jstopen-document-1.0.0/jstopen/document/
--rw-rw-rw-   0        0        0      581 2021-09-05 10:43:34.000000 jstopen-document-1.0.0/jstopen/document/DocumentGetUriByIdRequest.py
--rw-rw-rw-   0        0        0      358 2021-09-05 10:43:42.000000 jstopen-document-1.0.0/jstopen/document/DocumentGetUriForUploadRequest.py
--rw-rw-rw-   0        0        0      172 2021-09-06 01:13:22.000000 jstopen-document-1.0.0/jstopen/document/__init__.py
--rw-rw-rw-   0        0        0      255 2021-09-06 04:01:55.000000 jstopen-document-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 01:31:06.239585 jstopen-document-1.0.1/
+-rw-rw-rw-   0        0        0      228 2023-05-05 01:31:06.239880 jstopen-document-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 01:31:06.234484 jstopen-document-1.0.1/jstopen/
+drwxrwxrwx   0        0        0        0 2023-05-05 01:31:06.238533 jstopen-document-1.0.1/jstopen/document/
+-rw-rw-rw-   0        0        0      670 2023-05-04 10:30:40.126086 jstopen-document-1.0.1/jstopen/document/DocumentAddRequest.py
+-rw-rw-rw-   0        0        0      581 2023-05-04 10:10:52.214718 jstopen-document-1.0.1/jstopen/document/DocumentGetUriByIdRequest.py
+-rw-rw-rw-   0        0        0      393 2023-05-04 10:24:04.813454 jstopen-document-1.0.1/jstopen/document/DocumentGetUriForUploadRequest.py
+-rw-rw-rw-   0        0        0      240 2023-05-04 10:36:00.642054 jstopen-document-1.0.1/jstopen/document/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-05-04 10:32:52.890223 jstopen-document-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jstopen-document-1.0.0/jstopen/document/DocumentGetUriByIdRequest.py` & `jstopen-document-1.0.1/jstopen/document/DocumentGetUriByIdRequest.py`

 * *Files identical despite different names*

