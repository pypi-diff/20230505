# Comparing `tmp/sqlalchemy-orm-1.2.6.tar.gz` & `tmp/sqlalchemy-orm-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-orm-1.2.6.tar", last modified: Wed May  3 13:54:40 2023, max compression
+gzip compressed data, was "sqlalchemy-orm-1.2.7.tar", last modified: Thu May  4 23:45:10 2023, max compression
```

## Comparing `sqlalchemy-orm-1.2.6.tar` & `sqlalchemy-orm-1.2.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.118427 sqlalchemy-orm-1.2.6/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-03 13:54:40.118427 sqlalchemy-orm-1.2.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1036 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-03 13:54:39.000000 sqlalchemy-orm-1.2.6/VERSION
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-03 13:54:40.119427 sqlalchemy-orm-1.2.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.111426 sqlalchemy-orm-1.2.6/sqlalchemy_orm/
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.114426 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      855 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/base.py
--rwxrwxrwx   0 root         (0) root         (0)    14522 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/helper.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/mapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/custom_types.py
--rw-rw-rw-   0 root         (0) root         (0)     6265 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.117427 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/cst.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    10155 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/main.py
--rw-rw-rw-   0 root         (0) root         (0)     6089 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5089 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2732 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/version.py
--rwxrwxrwx   0 root         (0) root         (0)     1401 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/filter.py
--rwxrwxrwx   0 root         (0) root         (0)     1264 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/order_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.118427 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3635 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/tag.py
--rwxrwxrwx   0 root         (0) root         (0)     1718 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/tag_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      143 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/taggable.py
--rw-rw-rw-   0 root         (0) root         (0)     4983 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/query.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/session.py
--rw-rw-rw-   0 root         (0) root         (0)     2361 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/typemapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.113426 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:45:10.934597 sqlalchemy-orm-1.2.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-04 23:45:10.934597 sqlalchemy-orm-1.2.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1036 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-04 23:45:10.000000 sqlalchemy-orm-1.2.7/VERSION
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-04 23:45:10.934597 sqlalchemy-orm-1.2.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:45:10.927596 sqlalchemy-orm-1.2.7/sqlalchemy_orm/
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:45:10.929596 sqlalchemy-orm-1.2.7/sqlalchemy_orm/base/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      855 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/base/base.py
+-rwxrwxrwx   0 root         (0) root         (0)    14522 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/base/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/base/mapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/custom_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6265 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:45:10.932597 sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/cst.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10155 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5089 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/version.py
+-rwxrwxrwx   0 root         (0) root         (0)     1401 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1264 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/order_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:45:10.934597 sqlalchemy-orm-1.2.7/sqlalchemy_orm/patterns/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/patterns/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3635 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/patterns/tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     1718 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/patterns/tag_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      143 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/patterns/taggable.py
+-rw-rw-rw-   0 root         (0) root         (0)     4983 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/query.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     3073 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/typemapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2023-05-04 23:45:01.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:45:10.928596 sqlalchemy-orm-1.2.7/sqlalchemy_orm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-04 23:45:10.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-05-04 23:45:10.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 23:45:10.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-04 23:45:10.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-04 23:45:10.000000 sqlalchemy-orm-1.2.7/sqlalchemy_orm.egg-info/top_level.txt
```

### Comparing `sqlalchemy-orm-1.2.6/LICENSE` & `sqlalchemy-orm-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/PKG-INFO` & `sqlalchemy-orm-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-orm
-Version: 1.2.6
+Version: 1.2.7
 Summary: Data Relation Mapping framework for Python.
 Home-page: https://gitlab.com/parob/sqlalchemy-orm
-Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.6/sqlalchemy-orm-v1.2.6.tar.gz
+Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.7/sqlalchemy-orm-v1.2.7.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: SQLAlchemy,ORM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlalchemy-orm-1.2.6/README.md` & `sqlalchemy-orm-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/setup.py` & `sqlalchemy-orm-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Robert Parker",
     author_email="rob@parob.com",
     url="https://gitlab.com/parob/sqlalchemy-orm",
     download_url=f"https://gitlab.com/parob/sqlalchemy-orm/-/archive/v{version}"
-                 f"/sqlalchemy-orm-v{version}.tar.gz",
+    f"/sqlalchemy-orm-v{version}.tar.gz",
     keywords=["SQLAlchemy", "ORM"],
     description="Data Relation Mapping framework for Python.",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=["SQLAlchemy", "inflection", "cached-property", "typing_inspect"],
     extras_require={"dev": ["pytest", "pytest-cov", "coverage", "faker"]},
     classifiers=[
```

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/base.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/base/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/helper.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/base/helper.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/custom_types.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/custom_types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/database.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/database.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/cst.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/cst.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/helpers.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/main.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/main.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/models.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/models.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/parser.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/parser.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/sqla.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/eralchemy/sqla.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/filter.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/filter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/order_by.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/order_by.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/tag.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/patterns/tag.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/tag_mixin.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/patterns/tag_mixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/proxy.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/proxy.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/query.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm/utils.py` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/PKG-INFO` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-orm
-Version: 1.2.6
+Version: 1.2.7
 Summary: Data Relation Mapping framework for Python.
 Home-page: https://gitlab.com/parob/sqlalchemy-orm
-Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.6/sqlalchemy-orm-v1.2.6.tar.gz
+Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.7/sqlalchemy-orm-v1.2.7.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: SQLAlchemy,ORM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/SOURCES.txt` & `sqlalchemy-orm-1.2.7/sqlalchemy_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

