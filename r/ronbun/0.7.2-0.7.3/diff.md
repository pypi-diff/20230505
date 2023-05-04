# Comparing `tmp/ronbun-0.7.2.tar.gz` & `tmp/ronbun-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ronbun-0.7.2.tar", last modified: Sun Apr  9 15:33:46 2023, max compression
+gzip compressed data, was "ronbun-0.7.3.tar", max compression
```

## Comparing `ronbun-0.7.2.tar` & `ronbun-0.7.3.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:33:46.932200 ronbun-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 15:33:35.000000 ronbun-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-09 15:33:46.932200 ronbun-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 15:33:35.000000 ronbun-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:33:46.928200 ronbun-0.7.2/ronbun/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 15:33:35.000000 ronbun-0.7.2/ronbun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-04-09 15:33:35.000000 ronbun-0.7.2/ronbun/readme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:33:46.928200 ronbun-0.7.2/ronbun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 15:33:46.000000 ronbun-0.7.2/ronbun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:33:46.932200 ronbun-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-09 15:33:35.000000 ronbun-0.7.2/setup.py
+-rw-r--r--   0        0        0     1071 2023-05-04 23:50:21.644329 ronbun-0.7.3/LICENSE
+-rw-r--r--   0        0        0       82 2023-05-04 23:50:21.644329 ronbun-0.7.3/README.md
+-rw-r--r--   0        0        0      891 2023-05-04 23:50:21.644329 ronbun-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-04 23:50:21.644329 ronbun-0.7.3/ronbun/__init__.py
+-rw-r--r--   0        0        0     8671 2023-05-04 23:50:21.644329 ronbun-0.7.3/ronbun/readme.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 ronbun-0.7.3/PKG-INFO
```

### Comparing `ronbun-0.7.2/LICENSE` & `ronbun-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ronbun-0.7.2/ronbun/readme.py` & `ronbun-0.7.3/ronbun/readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     numeric_level = getattr(logging, args[1].upper(), None)
     if not isinstance(numeric_level, int):
         raise ValueError(f'Invalid log level: {args[1]}')
     logging.basicConfig(level=numeric_level)
     repo = Repo(sample_programs_repo_dir=args[0])
     readme_catalog = ReadMeCatalog(repo)
     for language, page in readme_catalog.pages.items():
-        page.dump("README", dir=f"{args[0]}/archive/{language[0]}/{language}")
+        page.dump("README", directory=f"{args[0]}/archive/{language[0]}/{language}")
 
 
 def _get_args() -> tuple:
     """
     A helper function which gets the log level from 
     the command line. Set as warning from default. 
     :return: the log level provided by the user
```

