# Comparing `tmp/django-ufilter-0.4.0.tar.gz` & `tmp/django_ufilter-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ufilter-0.4.0.tar", max compression
+gzip compressed data, was "django_ufilter-0.4.3.tar", max compression
```

## Comparing `django-ufilter-0.4.0.tar` & `django_ufilter-0.4.3.tar`

### file list

```diff
@@ -1,48 +1,47 @@
--rw-r--r--   0        0        0      500 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/AUTHORS.md
--rw-r--r--   0        0        0     1498 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1210 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     6063 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/README.rst
--rw-r--r--   0        0        0       22 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/__init__.py
--rw-r--r--   0        0        0        0 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/backends/__init__.py
--rw-r--r--   0        0        0     5198 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/backends/base.py
--rw-r--r--   0        0        0     3581 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/backends/django.py
--rw-r--r--   0        0        0     5189 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/backends/plain.py
--rw-r--r--   0        0        0      592 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/constants.py
--rw-r--r--   0        0        0      590 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/exceptions.py
--rw-r--r--   0        0        0     3759 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/fields.py
--rw-r--r--   0        0        0    19678 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/filters.py
--rw-r--r--   0        0        0       58 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/filtersets/__init__.py
--rw-r--r--   0        0        0    18325 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/filtersets/base.py
--rw-r--r--   0        0        0     4655 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/filtersets/django.py
--rw-r--r--   0        0        0     2414 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/filtersets/plain.py
--rw-r--r--   0        0        0        0 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/integrations/__init__.py
--rw-r--r--   0        0        0     5652 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/integrations/drf.py
--rw-r--r--   0        0        0     7572 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/utils.py
--rw-r--r--   0        0        0     1286 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/django_ufilter/validators.py
--rw-r--r--   0        0        0     7805 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/Makefile
--rw-r--r--   0        0        0      184 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.backends.base.rst
--rw-r--r--   0        0        0      190 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.backends.django.rst
--rw-r--r--   0        0        0      187 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.backends.plain.rst
--rw-r--r--   0        0        0      302 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.backends.rst
--rw-r--r--   0        0        0      175 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.exceptions.rst
--rw-r--r--   0        0        0      163 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.fields.rst
--rw-r--r--   0        0        0      166 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.filters.rst
--rw-r--r--   0        0        0      190 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.filtersets.base.rst
--rw-r--r--   0        0        0      193 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.filtersets.django.rst
--rw-r--r--   0        0        0      193 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.filtersets.plain.rst
--rw-r--r--   0        0        0      320 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.filtersets.rst
--rw-r--r--   0        0        0      193 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.integrations.drf.rst
--rw-r--r--   0        0        0      256 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.integrations.rst
--rw-r--r--   0        0        0      445 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.rst
--rw-r--r--   0        0        0      160 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.utils.rst
--rw-r--r--   0        0        0      175 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/django_ufilter.validators.rst
--rw-r--r--   0        0        0       84 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/api/modules.rst
--rw-r--r--   0        0        0     7534 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/big_picture.rst
--rw-r--r--   0        0        0     9604 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/conf.py
--rw-r--r--   0        0        0       78 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/history.rst
--rw-r--r--   0        0        0      271 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/index.rst
--rw-r--r--   0        0        0     9695 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/requirements.txt
--rw-r--r--   0        0        0     5189 2022-06-17 04:38:00.244048 django-ufilter-0.4.0/docs/usage.rst
--rw-r--r--   0        0        0     2323 2022-06-17 04:38:00.248048 django-ufilter-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7243 2022-06-17 04:38:16.308853 django-ufilter-0.4.0/setup.py
--rw-r--r--   0        0        0     7299 2022-06-17 04:38:16.309461 django-ufilter-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      500 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/AUTHORS.md
+-rw-r--r--   0        0        0     1981 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1210 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/LICENSE.md
+-rw-r--r--   0        0        0     6191 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/README.rst
+-rw-r--r--   0        0        0       22 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/backends/__init__.py
+-rw-r--r--   0        0        0     5198 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/backends/base.py
+-rw-r--r--   0        0        0     3581 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/backends/django.py
+-rw-r--r--   0        0        0     5189 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/backends/plain.py
+-rw-r--r--   0        0        0      592 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/constants.py
+-rw-r--r--   0        0        0      590 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/exceptions.py
+-rw-r--r--   0        0        0     3759 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/fields.py
+-rw-r--r--   0        0        0    19678 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/filters.py
+-rw-r--r--   0        0        0       58 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/filtersets/__init__.py
+-rw-r--r--   0        0        0    18325 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/filtersets/base.py
+-rw-r--r--   0        0        0     4655 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/filtersets/django.py
+-rw-r--r--   0        0        0     2414 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/filtersets/plain.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/integrations/__init__.py
+-rw-r--r--   0        0        0     5652 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/integrations/drf.py
+-rw-r--r--   0        0        0     7572 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/utils.py
+-rw-r--r--   0        0        0     1286 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/django_ufilter/validators.py
+-rw-r--r--   0        0        0     7805 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/Makefile
+-rw-r--r--   0        0        0      184 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.backends.base.rst
+-rw-r--r--   0        0        0      190 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.backends.django.rst
+-rw-r--r--   0        0        0      187 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.backends.plain.rst
+-rw-r--r--   0        0        0      302 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.backends.rst
+-rw-r--r--   0        0        0      175 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.exceptions.rst
+-rw-r--r--   0        0        0      163 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.fields.rst
+-rw-r--r--   0        0        0      166 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.filters.rst
+-rw-r--r--   0        0        0      190 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.filtersets.base.rst
+-rw-r--r--   0        0        0      193 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.filtersets.django.rst
+-rw-r--r--   0        0        0      193 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.filtersets.plain.rst
+-rw-r--r--   0        0        0      320 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.filtersets.rst
+-rw-r--r--   0        0        0      193 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.integrations.drf.rst
+-rw-r--r--   0        0        0      256 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.integrations.rst
+-rw-r--r--   0        0        0      445 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.rst
+-rw-r--r--   0        0        0      160 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.utils.rst
+-rw-r--r--   0        0        0      175 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/django_ufilter.validators.rst
+-rw-r--r--   0        0        0       84 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/api/modules.rst
+-rw-r--r--   0        0        0     7534 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/big_picture.rst
+-rw-r--r--   0        0        0     9604 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/conf.py
+-rw-r--r--   0        0        0       78 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/history.rst
+-rw-r--r--   0        0        0      271 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/index.rst
+-rw-r--r--   0        0        0     9695 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/requirements.txt
+-rw-r--r--   0        0        0     5189 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/docs/usage.rst
+-rw-r--r--   0        0        0     2247 2023-05-04 22:45:12.108016 django_ufilter-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     7440 1970-01-01 00:00:00.000000 django_ufilter-0.4.3/PKG-INFO
```

### Comparing `django-ufilter-0.4.0/CHANGELOG.md` & `django_ufilter-0.4.3/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,45 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 This project was originally forked from [django-url-filter](https://github.com/miki725/django-url-filter). If you wish to see the CHANGELOG pre-fork, visit [HISTORY.rst](https://github.com/miki725/django-url-filter/blob/master/HISTORY.rst).
 
 ## [Unreleased]
 
-## [0.4.0] - 2022-05-10
+## [0.4.3] - 2023-05-04
+
+### Added
+
+-   Support for Python3.11
+
+### Fixed
+
+-   README (Thanks @aseidma)
+-   CI - it had broke due to a django upgrade
+
+### Changed
+
+-   Do not enforce Django version according to the Python version (Thanks @arianesc)
+-   Upgraded Github Actions
+-   Upgraded Poetry
+-   Upgraded isort
+
+
+## [0.4.0] - 2022-06-17
 
 ### Added
 
 -   Support for Django v4
 -   Poetry for package management.
 -   Github Actions for CI.
 
 ### Changed
 
 -   Renamed forked package to `django-ufilter`.
+-   In `django_ufilter.integrations.drf`, renamed `DjangoFilterBackend` to `DRFFilterBackend`.
 -   Import sorter from `importanize` to `isort`.
 -   Pin versions on the hooks of the `pre-commit` configuration file.
 -   Moved all configurations to `pyproject.toml` on which support exists.
 -   `HISTORY.rst` to `CHANGELOG.md` following the KeepAChangelog format.
 -   `AUTHORS.rst` to `AUTHORS.md`
 
 ### Removed
@@ -32,9 +52,10 @@
 -   Support for CoreAPI.
 -   Support for all unsupported Python versions.
 -   Support for all unsupported Django versions.
 -   TravisCI and DroneCI.
 -   `setup.py`, `setup.cfg`, `requirements*.txt`, `MANIFEST.in`, `Makefile`.
 -   `__author__` and `__email__` - These are already available on `pyproject.toml`.
 
-[Unreleased]: https://github.com/Qu4tro/django-ufilter/compare/v0.4.0...HEAD
+[Unreleased]: https://github.com/Qu4tro/django-ufilter/compare/v0.4.3...HEAD
+[0.4.3]: https://github.com/Qu4tro/django-ufilter/releases/tag/v0.4.3
 [0.4.0]: https://github.com/Qu4tro/django-ufilter/releases/tag/v0.4.0
```

### Comparing `django-ufilter-0.4.0/LICENSE.md` & `django_ufilter-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/README.rst` & `django_ufilter-0.4.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 .. image:: https://badge.fury.io/py/django-ufilter.svg
    :target: http://badge.fury.io/py/django-ufilter
 .. image:: https://readthedocs.org/projects/django-ufilter/badge/?version=latest
    :target: http://django-ufilter.readthedocs.io/en/latest/?badge=latest
 
 Django UFilter provides a safe way to filter data via human-friendly URLs.
 
+This project was forked from https://github.com/miki725/django-url-filter, due to the lack of maintenance in the original one.
+
 * Free software: MIT license
 * GitHub: https://github.com/Qu4tro/django-ufilter/
 * Documentation: http://django-ufilter.readthedocs.io/
 
 Overview
 --------
```

### Comparing `django-ufilter-0.4.0/django_ufilter/backends/base.py` & `django_ufilter-0.4.3/django_ufilter/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/backends/django.py` & `django_ufilter-0.4.3/django_ufilter/backends/django.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/backends/plain.py` & `django_ufilter-0.4.3/django_ufilter/backends/plain.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/constants.py` & `django_ufilter-0.4.3/django_ufilter/constants.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/exceptions.py` & `django_ufilter-0.4.3/django_ufilter/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/fields.py` & `django_ufilter-0.4.3/django_ufilter/fields.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/filters.py` & `django_ufilter-0.4.3/django_ufilter/filters.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/filtersets/base.py` & `django_ufilter-0.4.3/django_ufilter/filtersets/base.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/filtersets/django.py` & `django_ufilter-0.4.3/django_ufilter/filtersets/django.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/filtersets/plain.py` & `django_ufilter-0.4.3/django_ufilter/filtersets/plain.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/integrations/drf.py` & `django_ufilter-0.4.3/django_ufilter/integrations/drf.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/utils.py` & `django_ufilter-0.4.3/django_ufilter/utils.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/django_ufilter/validators.py` & `django_ufilter-0.4.3/django_ufilter/validators.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/docs/Makefile` & `django_ufilter-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/docs/big_picture.rst` & `django_ufilter-0.4.3/docs/big_picture.rst`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/docs/conf.py` & `django_ufilter-0.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/docs/requirements.txt` & `django_ufilter-0.4.3/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/docs/usage.rst` & `django_ufilter-0.4.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django-ufilter-0.4.0/pyproject.toml` & `django_ufilter-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-ufilter"
-version = "0.4.0"
+version = "0.4.3"
 license = "MIT"
 include = ["AUTHORS.md", "CHANGELOG.md", "docs"]
 description = "django-ufilter provides a safe way to filter data."
 authors = ["Miroslav Shubernetskiy <miroslav@miki725.com>"]
 maintainers = ["Xavier Francisco <xavier.n.francisco@gmail.com>"]
 repository = "https://github.com/Qu4tro/django-ufilter"
 keywords = ["django", "django-rest-framework"]
@@ -23,28 +23,25 @@
     "Development Status :: 2 - Pre-Alpha",
 ]
 readme = "README.rst"
 
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
-django = [
-    {version = "^4", python = ">=3.8"},
-    {version = "^3.2", python = "<=3.9"},
-]
+django = ">=3.2"
 cached-property = "^1.5.2"
 
 [tool.poetry.dev-dependencies]
 bpython = "^0.22.1"
 pdbpp = "^0.10.3"
 isort = "^5.10.1"
 black = "^22.3.0"
 django-extensions = "^3.1.5"
-djangorestframework = "^3.13.1"
-pytz = "^2022.1" # Already required by djangorestframework, but not included due to some weird poetry bug
+djangorestframework = "^3.14.0"
+# pytz = "^2022.1" # Already required by djangorestframework, but not included due to some weird poetry bug
 django-debug-toolbar = "^3.4.0"
 mock = "^4.0.3"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pytest-django = "^4.5.2"
 flake8 = "^4.0.1"
 flake8-bugbear = "^22.4.25"
```

### Comparing `django-ufilter-0.4.0/setup.py` & `django_ufilter-0.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,218 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-ufilter
+Version: 0.4.3
+Summary: django-ufilter provides a safe way to filter data.
+Home-page: https://github.com/Qu4tro/django-ufilter
+License: MIT
+Keywords: django,django-rest-framework
+Author: Miroslav Shubernetskiy
+Author-email: miroslav@miki725.com
+Maintainer: Xavier Francisco
+Maintainer-email: xavier.n.francisco@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Requires-Dist: cached-property (>=1.5.2,<2.0.0)
+Requires-Dist: django (>=3.2)
+Project-URL: Repository, https://github.com/Qu4tro/django-ufilter
+Description-Content-Type: text/x-rst
 
-packages = \
-['django_ufilter',
- 'django_ufilter.backends',
- 'django_ufilter.filtersets',
- 'django_ufilter.integrations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cached-property>=1.5.2,<2.0.0']
-
-extras_require = \
-{':python_version <= "3.9"': ['django>=3.2,<4.0'],
- ':python_version >= "3.8"': ['django>=4,<5']}
-
-setup_kwargs = {
-    'name': 'django-ufilter',
-    'version': '0.4.0',
-    'description': 'django-ufilter provides a safe way to filter data.',
-    'long_description': '=================\nDjango UFilter\n=================\n\n.. image:: https://badge.fury.io/py/django-ufilter.svg\n   :target: http://badge.fury.io/py/django-ufilter\n.. image:: https://readthedocs.org/projects/django-ufilter/badge/?version=latest\n   :target: http://django-ufilter.readthedocs.io/en/latest/?badge=latest\n\nDjango UFilter provides a safe way to filter data via human-friendly URLs.\n\n* Free software: MIT license\n* GitHub: https://github.com/Qu4tro/django-ufilter/\n* Documentation: http://django-ufilter.readthedocs.io/\n\nOverview\n--------\n\nThe main goal of Django UFilter is to provide an easy URL interface\nfor filtering data. It allows the user to safely filter by model\nattributes and also allows to specify the lookup type for each filter\n(very much like Django\'s filtering system in ORM).\n\nFor example the following will retrieve all items where the id is\n``5`` and title contains ``"foo"``::\n\n    example.com/listview/?id=5&title__contains=foo\n\nIn addition to basic lookup types, Django UFilter allows to\nuse more sophisticated lookups such as ``in`` or ``year``.\nFor example::\n\n    example.com/listview/?id__in=1,2,3&created__year=2013\n\nRequirements\n------------\n\n* Python 2.7, 3.x, pypy or pypy3\n* Django 1.8+ (there are plans to support older Django versions)\n* Django REST Framework 2 or 3 (only if you want to use DRF integration)\n\nInstalling\n----------\n\nEasiest way to install this library is by using ``pip``::\n\n    $ pip install django-ufilter\n\nUsage Example\n-------------\n\nTo make example short, it demonstrates Django UFilter integration\nwith Django REST Framework but it can be used without DRF (see below).\n\n::\n\n  from django_ufilter.integrations.drf import DRFFilterBackend\n\n\n  class UserViewSet(ModelViewSet):\n      queryset = User.objects.all()\n      serializer_class = UserSerializer\n      filter_backends = [DjangoFilterBackend]\n      filter_fields = [\'username\', \'email\']\n\nAlternatively filterset can be manually created and used directly\nto filter querysets::\n\n  from django.http import QueryDict\n  from django_ufilter.filtersets import ModelFilterSet\n\n\n  class UserFilterSet(ModelFilterSet):\n      class Meta(object):\n          model = User\n\n  query = QueryDict(\'email__contains=gmail&joined__gt=2015-01-01\')\n  fs = UserFilterSet(data=query, queryset=User.objects.all())\n  filtered_users = fs.filter()\n\nAbove will automatically allow the use of all of the Django UFilter features.\nSome possibilities:\n\n* get user with id 5\n\n    example.com/users/?id=5\n\n* get user with id either 5, 10 or 15\n\n    example.com/users/?id__in=5,10,15\n\n* get user with id between 5 and 10\n\n    example.com/users/?id__range=5,10\n\n* get user with username "foo"\n\n    example.com/users/?username=foo\n\n* get user with username containing case insensitive "foo"\n\n    example.com/users/?username__icontains=foo\n\n* get user where username does NOT contain "foo"\n\n    example.com/users/?username__icontains!=foo\n\n* get user who joined in 2015 as per user profile\n\n    example.com/users/?profile__joined__year=2015\n\n* get user who joined in between 2010 and 2015 as per user profile\n\n    example.com/users/?profile__joined__range=2010-01-01,2015-12-31\n\n* get user who joined in after 2010 as per user profile\n\n    example.com/users/?profile__joined__gt=2010-01-01\n\nAvailable lookups:\n\n* contains: Match when string contains given substring.\n* day: Match by day of the month.\n* endswith: Match when string ends with given substring.\n* exact: Match exactly the value as is.\n* gt: Match when value is greater then given value.\n* gte: Match when value is greater or equal then given value.\n* hour: Match by the hour (24 hour) value of the timestamp.\n* icontains: Case insensitive match when string contains given substring.\n* iendswith: Case insensitive match when string ends with given substring.\n* iexact: Case insensitive match exactly the value as is.\n* iin: Case insensitive match when value is any of given comma separated values.\n* in: Match when value is any of given comma separated values.\n* iregex: Case insensitive match string by regex pattern.\n* isnull: Match when value is NULL.\n* istartswith: Case insensitive match when string starts with given substring.\n* lt: Match when value is less then given value.\n* lte: Match when value is less or equal then given value.\n* minute: Match by the minute value of the timestamp.\n* month: Match by the month value of the timestamp.\n* range: Match when value is within comma separated range.\n* regex: Match string by regex pattern.\n* second: Match by the second value of the timestamp.\n* startswith: Match when string starts with given substring.\n* week_day: Match by week day (1-Sunday to 7-Saturday) of the timestamp.\n* year: Match by the year value of the timestamp.\n* len: Match the length of a given ArrayField\n\nFeatures\n--------\n\n* **Human-friendly URLs**\n\n  Filter querystring format looks\n  very similar to syntax for filtering in Django ORM.\n  Even negated filters are supported! Some examples::\n\n    example.com/users/?email__contains=gmail&joined__gt=2015-01-01\n    example.com/users/?email__contains!=gmail  # note !\n\n* **Related models**\n\n  Support related fields so that filtering can be applied to related\n  models. For example::\n\n    example.com/users/?profile__nickname=foo\n\n* **Decoupled filtering**\n\n  How URLs are parsed and how data is filtered is decoupled.\n  This allows the actual filtering logic to be decoupled from Django\n  hence filtering is possible not only with Django ORM QuerySet but\n  any set of data can be filtered (e.g. plain Python objects)\n  assuming corresponding filtering backend is implemented.\n\n* **Usage-agnostic**\n\n  This library decouples filtering from any particular usage-pattern.\n  It implements all the basic building blocks for creating\n  filtersets but it does not assume how they will be used.\n  To make the library easy to use, it ships with some integrations\n  with common usage patterns like integration with Django REST Framework.\n  This means that its easy to use in custom applications with custom\n  requirements (which is probably most of the time!)\n',
-    'author': 'Miroslav Shubernetskiy',
-    'author_email': 'miroslav@miki725.com',
-    'maintainer': 'Xavier Francisco',
-    'maintainer_email': 'xavier.n.francisco@gmail.com',
-    'url': 'https://github.com/Qu4tro/django-ufilter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+=================
+Django UFilter
+=================
 
+.. image:: https://badge.fury.io/py/django-ufilter.svg
+   :target: http://badge.fury.io/py/django-ufilter
+.. image:: https://readthedocs.org/projects/django-ufilter/badge/?version=latest
+   :target: http://django-ufilter.readthedocs.io/en/latest/?badge=latest
+
+Django UFilter provides a safe way to filter data via human-friendly URLs.
+
+This project was forked from https://github.com/miki725/django-url-filter, due to the lack of maintenance in the original one.
+
+* Free software: MIT license
+* GitHub: https://github.com/Qu4tro/django-ufilter/
+* Documentation: http://django-ufilter.readthedocs.io/
+
+Overview
+--------
+
+The main goal of Django UFilter is to provide an easy URL interface
+for filtering data. It allows the user to safely filter by model
+attributes and also allows to specify the lookup type for each filter
+(very much like Django's filtering system in ORM).
+
+For example the following will retrieve all items where the id is
+``5`` and title contains ``"foo"``::
+
+    example.com/listview/?id=5&title__contains=foo
+
+In addition to basic lookup types, Django UFilter allows to
+use more sophisticated lookups such as ``in`` or ``year``.
+For example::
+
+    example.com/listview/?id__in=1,2,3&created__year=2013
+
+Requirements
+------------
+
+* Python 2.7, 3.x, pypy or pypy3
+* Django 1.8+ (there are plans to support older Django versions)
+* Django REST Framework 2 or 3 (only if you want to use DRF integration)
+
+Installing
+----------
+
+Easiest way to install this library is by using ``pip``::
+
+    $ pip install django-ufilter
+
+Usage Example
+-------------
+
+To make example short, it demonstrates Django UFilter integration
+with Django REST Framework but it can be used without DRF (see below).
+
+::
+
+  from django_ufilter.integrations.drf import DRFFilterBackend
+
+
+  class UserViewSet(ModelViewSet):
+      queryset = User.objects.all()
+      serializer_class = UserSerializer
+      filter_backends = [DjangoFilterBackend]
+      filter_fields = ['username', 'email']
+
+Alternatively filterset can be manually created and used directly
+to filter querysets::
+
+  from django.http import QueryDict
+  from django_ufilter.filtersets import ModelFilterSet
+
+
+  class UserFilterSet(ModelFilterSet):
+      class Meta(object):
+          model = User
+
+  query = QueryDict('email__contains=gmail&joined__gt=2015-01-01')
+  fs = UserFilterSet(data=query, queryset=User.objects.all())
+  filtered_users = fs.filter()
+
+Above will automatically allow the use of all of the Django UFilter features.
+Some possibilities:
+
+* get user with id 5
+
+    example.com/users/?id=5
+
+* get user with id either 5, 10 or 15
+
+    example.com/users/?id__in=5,10,15
+
+* get user with id between 5 and 10
+
+    example.com/users/?id__range=5,10
+
+* get user with username "foo"
+
+    example.com/users/?username=foo
+
+* get user with username containing case insensitive "foo"
+
+    example.com/users/?username__icontains=foo
+
+* get user where username does NOT contain "foo"
+
+    example.com/users/?username__icontains!=foo
+
+* get user who joined in 2015 as per user profile
+
+    example.com/users/?profile__joined__year=2015
+
+* get user who joined in between 2010 and 2015 as per user profile
+
+    example.com/users/?profile__joined__range=2010-01-01,2015-12-31
+
+* get user who joined in after 2010 as per user profile
+
+    example.com/users/?profile__joined__gt=2010-01-01
+
+Available lookups:
+
+* contains: Match when string contains given substring.
+* day: Match by day of the month.
+* endswith: Match when string ends with given substring.
+* exact: Match exactly the value as is.
+* gt: Match when value is greater then given value.
+* gte: Match when value is greater or equal then given value.
+* hour: Match by the hour (24 hour) value of the timestamp.
+* icontains: Case insensitive match when string contains given substring.
+* iendswith: Case insensitive match when string ends with given substring.
+* iexact: Case insensitive match exactly the value as is.
+* iin: Case insensitive match when value is any of given comma separated values.
+* in: Match when value is any of given comma separated values.
+* iregex: Case insensitive match string by regex pattern.
+* isnull: Match when value is NULL.
+* istartswith: Case insensitive match when string starts with given substring.
+* lt: Match when value is less then given value.
+* lte: Match when value is less or equal then given value.
+* minute: Match by the minute value of the timestamp.
+* month: Match by the month value of the timestamp.
+* range: Match when value is within comma separated range.
+* regex: Match string by regex pattern.
+* second: Match by the second value of the timestamp.
+* startswith: Match when string starts with given substring.
+* week_day: Match by week day (1-Sunday to 7-Saturday) of the timestamp.
+* year: Match by the year value of the timestamp.
+* len: Match the length of a given ArrayField
+
+Features
+--------
+
+* **Human-friendly URLs**
+
+  Filter querystring format looks
+  very similar to syntax for filtering in Django ORM.
+  Even negated filters are supported! Some examples::
+
+    example.com/users/?email__contains=gmail&joined__gt=2015-01-01
+    example.com/users/?email__contains!=gmail  # note !
+
+* **Related models**
+
+  Support related fields so that filtering can be applied to related
+  models. For example::
+
+    example.com/users/?profile__nickname=foo
+
+* **Decoupled filtering**
+
+  How URLs are parsed and how data is filtered is decoupled.
+  This allows the actual filtering logic to be decoupled from Django
+  hence filtering is possible not only with Django ORM QuerySet but
+  any set of data can be filtered (e.g. plain Python objects)
+  assuming corresponding filtering backend is implemented.
+
+* **Usage-agnostic**
+
+  This library decouples filtering from any particular usage-pattern.
+  It implements all the basic building blocks for creating
+  filtersets but it does not assume how they will be used.
+  To make the library easy to use, it ships with some integrations
+  with common usage patterns like integration with Django REST Framework.
+  This means that its easy to use in custom applications with custom
+  requirements (which is probably most of the time!)
 
-setup(**setup_kwargs)
```

