# Comparing `tmp/pycompete-0.0.0.tar.gz` & `tmp/pycompete-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompete-0.0.0.tar", last modified: Fri May  5 10:32:32 2023, max compression
+gzip compressed data, was "pycompete-0.0.4.tar", last modified: Fri May  5 12:18:58 2023, max compression
```

## Comparing `pycompete-0.0.0.tar` & `pycompete-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:32:32.800975 pycompete-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 10:32:25.000000 pycompete-0.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 10:32:32.800975 pycompete-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 10:32:25.000000 pycompete-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:32:32.800975 pycompete-0.0.0/pycompete.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 10:32:32.000000 pycompete-0.0.0/pycompete.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 10:32:32.000000 pycompete-0.0.0/pycompete.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:32:32.000000 pycompete-0.0.0/pycompete.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:32:32.000000 pycompete-0.0.0/pycompete.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:32:32.800975 pycompete-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-05 10:32:25.000000 pycompete-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.625822 pycompete-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-05 12:18:44.000000 pycompete-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-05 12:18:44.000000 pycompete-0.0.4/.github/workflows/syntax.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 12:18:44.000000 pycompete-0.0.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-05 12:18:44.000000 pycompete-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 12:18:44.000000 pycompete-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-05 12:18:44.000000 pycompete-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-05 12:18:58.629822 pycompete-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 12:18:44.000000 pycompete-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-05 12:18:44.000000 pycompete-0.0.4/notebooks/Untitled.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/pycompete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:44.000000 pycompete-0.0.4/pycompete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/pycompete/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 12:18:44.000000 pycompete-0.0.4/pycompete/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/pycompete/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 12:18:44.000000 pycompete-0.0.4/pycompete/model_selection/cv_splitters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/pycompete.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 12:18:58.000000 pycompete-0.0.4/pycompete.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-05 12:18:44.000000 pycompete-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 12:18:44.000000 pycompete-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:18:58.629822 pycompete-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:18:44.000000 pycompete-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.625822 pycompete-0.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.625822 pycompete-0.0.4/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:18:58.629822 pycompete-0.0.4/tests/unit/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-05 12:18:44.000000 pycompete-0.0.4/tests/unit/evaluation/test_metric.py
```

### Comparing `pycompete-0.0.0/LICENSE.txt` & `pycompete-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.0/README.md` & `pycompete-0.0.4/README.md`

 * *Files identical despite different names*

