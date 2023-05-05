# Comparing `tmp/trata-1.0.0.tar.gz` & `tmp/trata-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trata-1.0.0.tar", max compression
+gzip compressed data, was "trata-1.0.1.tar", max compression
```

## Comparing `trata-1.0.0.tar` & `trata-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1545 2023-03-04 04:02:44.130319 trata-1.0.0/LICENSE
--rw-r--r--   0        0        0     5034 2023-04-18 01:23:07.929925 trata-1.0.0/README.md
--rw-r--r--   0        0        0     1420 2023-04-18 00:03:14.528215 trata-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      560 2023-04-12 21:52:42.348778 trata-1.0.0/trata/__init__.py
--rw-r--r--   0        0        0    18671 2023-03-31 02:05:18.160006 trata-1.0.0/trata/adaptive_sampler.py
--rw-r--r--   0        0        0    24605 2023-03-04 04:02:44.232304 trata-1.0.0/trata/composite_samples.py
--rw-r--r--   0        0        0    62845 2023-03-31 02:05:18.183947 trata-1.0.0/trata/sampler.py
--rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 trata-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1545 2023-03-04 04:02:44.130319 trata-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3316 2023-05-04 23:57:40.437007 trata-1.0.1/README.md
+-rw-r--r--   0        0        0     1759 2023-05-05 00:00:23.435107 trata-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-05-04 23:50:36.451451 trata-1.0.1/trata/__init__.py
+-rw-r--r--   0        0        0    18671 2023-05-04 23:50:36.453460 trata-1.0.1/trata/adaptive_sampler.py
+-rw-r--r--   0        0        0    24605 2023-03-04 04:02:44.232304 trata-1.0.1/trata/composite_samples.py
+-rw-r--r--   0        0        0    62845 2023-05-04 23:50:36.458451 trata-1.0.1/trata/sampler.py
+-rw-r--r--   0        0        0     4765 1970-01-01 00:00:00.000000 trata-1.0.1/PKG-INFO
```

### Comparing `trata-1.0.0/LICENSE` & `trata-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trata-1.0.0/pyproject.toml` & `trata-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "trata"
-version = "1.0.0"
+version = "1.0.1"
 description = "A tool to facilitate standard and adaptive Bayesian sampling."
 license = "BSD 3-Clause License"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers", "Intended Audience :: Education",
     "Intended Audience :: Science/Research", "Topic :: Scientific/Engineering",
@@ -51,7 +51,25 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/LLNL/trata/issues"
 "Discussions" = "https://github.com/LLNL/trata/discussions"
 
 [tool.black]
 line-length = 79
+
+[tool.bumpver]
+current_version = "2023.1001-alpha"
+version_pattern = "YYYY.BUILD[-TAG]"
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = true
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = [
+    'current_version = "{version}"',
+]
+"README.md" = [
+    "{version}",
+    "{pep440_version}",
+]
+
```

### Comparing `trata-1.0.0/trata/adaptive_sampler.py` & `trata-1.0.1/trata/adaptive_sampler.py`

 * *Files identical despite different names*

### Comparing `trata-1.0.0/trata/composite_samples.py` & `trata-1.0.1/trata/composite_samples.py`

 * *Files identical despite different names*

### Comparing `trata-1.0.0/trata/sampler.py` & `trata-1.0.1/trata/sampler.py`

 * *Files identical despite different names*

