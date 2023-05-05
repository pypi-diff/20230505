# Comparing `tmp/cluedin-0.1.0.tar.gz` & `tmp/cluedin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluedin-0.1.0.tar", max compression
+gzip compressed data, was "cluedin-0.1.1.tar", max compression
```

## Comparing `cluedin-0.1.0.tar` & `cluedin-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-02 20:10:19.990177 cluedin-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-02 20:10:19.990135 cluedin-0.1.0/cluedin/__init__.py
--rw-r--r--   0        0        0      544 2023-05-04 20:05:12.355081 cluedin-0.1.0/cluedin/cluedin.py
--rw-r--r--   0        0        0      293 2023-05-02 20:14:31.481276 cluedin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 cluedin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-02 20:10:19.990177 cluedin-0.1.1/README.md
+-rw-r--r--   0        0        0       41 2023-05-05 20:11:46.996331 cluedin-0.1.1/cluedin/__init__.py
+-rw-r--r--   0        0        0      684 2023-05-05 20:46:12.499526 cluedin-0.1.1/cluedin/auth.py
+-rw-r--r--   0        0        0      292 2023-05-05 18:02:53.064080 cluedin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 cluedin-0.1.1/PKG-INFO
```

