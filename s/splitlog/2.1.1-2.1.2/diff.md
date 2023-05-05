# Comparing `tmp/splitlog-2.1.1.tar.gz` & `tmp/splitlog-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitlog-2.1.1.tar", max compression
+gzip compressed data, was "splitlog-2.1.2.tar", max compression
```

## Comparing `splitlog-2.1.1.tar` & `splitlog-2.1.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1092 2022-12-20 22:46:26.596527 splitlog-2.1.1/LICENSE
--rw-r--r--   0        0        0     1771 2022-12-20 22:46:26.596527 splitlog-2.1.1/README.md
--rw-r--r--   0        0        0     1161 2022-12-20 22:47:00.854463 splitlog-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    11993 2022-12-20 22:46:26.596527 splitlog-2.1.1/splitlog/__init__.py
--rw-r--r--   0        0        0     3456 2022-12-20 22:46:26.596527 splitlog-2.1.1/splitlog/__main__.py
--rw-r--r--   0        0        0     7460 2022-12-20 22:46:26.596527 splitlog-2.1.1/splitlog/outputfolder.py
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 splitlog-2.1.1/setup.py
--rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 splitlog-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-05 18:59:10.330361 splitlog-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1771 2023-05-05 18:59:10.330361 splitlog-2.1.2/README.md
+-rw-r--r--   0        0        0     1163 2023-05-05 18:59:46.558156 splitlog-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11993 2023-05-05 18:59:10.330361 splitlog-2.1.2/splitlog/__init__.py
+-rw-r--r--   0        0        0     3455 2023-05-05 18:59:10.330361 splitlog-2.1.2/splitlog/__main__.py
+-rw-r--r--   0        0        0     7460 2023-05-05 18:59:10.330361 splitlog-2.1.2/splitlog/outputfolder.py
+-rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 splitlog-2.1.2/PKG-INFO
```

### Comparing `splitlog-2.1.1/LICENSE` & `splitlog-2.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Sebastian Klemke <pypi@nerdheim.de>
+Copyright (c) 2022-2023 Sebastian Klemke <pypi@nerdheim.de>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `splitlog-2.1.1/README.md` & `splitlog-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `splitlog-2.1.1/pyproject.toml` & `splitlog-2.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splitlog"
-version = "2.1.1"
+version = "2.1.2"
 description = "Utility to split aggregated logs from Apache Hadoop Yarn applications into a folder hierarchy"
 authors = ["Sebastian Klemke <pypi@nerdheim.de>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -23,18 +23,18 @@
 pytz = ">=2022.1"
 importlib-metadata = "^5.1.0"
 
 [tool.poetry.scripts]
 splitlog = 'splitlog.__main__:main'
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^0.991"
-black = "^22.3.0"
-types-python-dateutil = "^2.8.15"
-pytest = "^7.2.0"
+mypy = "^1.2.0"
+black = "^23.3.0"
+types-python-dateutil = "^2.8.19.2"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 dirty = true
 
 [build-system]
```

### Comparing `splitlog-2.1.1/splitlog/__init__.py` & `splitlog-2.1.2/splitlog/__init__.py`

 * *Files identical despite different names*

### Comparing `splitlog-2.1.1/splitlog/__main__.py` & `splitlog-2.1.2/splitlog/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
     else:
         print(f"{_NAME} {version}")
 
     exit(0)
 
 
 def main(cli_args: Optional[List[str]] = None) -> None:
-
     import sys
 
     if cli_args is None:
         cli_args = sys.argv[1:]
 
     args = _parse_args(cli_args)
```

### Comparing `splitlog-2.1.1/splitlog/outputfolder.py` & `splitlog-2.1.2/splitlog/outputfolder.py`

 * *Files identical despite different names*

### Comparing `splitlog-2.1.1/PKG-INFO` & `splitlog-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitlog
-Version: 2.1.1
+Version: 2.1.2
 Summary: Utility to split aggregated logs from Apache Hadoop Yarn applications into a folder hierarchy
 Home-page: https://github.com/splitlog/splitlog.git
 License: MIT
 Author: Sebastian Klemke
 Author-email: pypi@nerdheim.de
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

