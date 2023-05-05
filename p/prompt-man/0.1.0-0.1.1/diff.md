# Comparing `tmp/prompt_man-0.1.0.tar.gz` & `tmp/prompt_man-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_man-0.1.0.tar", max compression
+gzip compressed data, was "prompt_man-0.1.1.tar", max compression
```

## Comparing `prompt_man-0.1.0.tar` & `prompt_man-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rwxr-xr-x   0        0        0        0 2023-05-03 21:37:45.485289 prompt_man-0.1.0/README.md
--rwxr-xr-x   0        0        0      170 2023-05-05 19:38:42.079268 prompt_man-0.1.0/prompt_man/__init__.py
--rwxr-xr-x   0        0        0      453 2023-05-05 19:01:37.778588 prompt_man-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 prompt_man-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2023-05-03 21:37:45.485289 prompt_man-0.1.1/README.md
+-rwxr-xr-x   0        0        0      118 2023-05-05 21:51:03.617623 prompt_man-0.1.1/prompt_man/__init__.py
+-rwxr-xr-x   0        0        0       81 2023-05-05 21:41:09.856134 prompt_man-0.1.1/prompt_man/hello.py
+-rwxr-xr-x   0        0        0      508 2023-05-05 21:52:44.327987 prompt_man-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 prompt_man-0.1.1/PKG-INFO
```

