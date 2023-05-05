# Comparing `tmp/AutoGenerateMKD-0.0.6.tar.gz` & `tmp/AutoGenerateMKD-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoGenerateMKD-0.0.6.tar", last modified: Fri May  5 16:34:12 2023, max compression
+gzip compressed data, was "AutoGenerateMKD-0.0.7.tar", last modified: Fri May  5 16:40:40 2023, max compression
```

## Comparing `AutoGenerateMKD-0.0.6.tar` & `AutoGenerateMKD-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:34:12.668110 AutoGenerateMKD-0.0.6/
--rw-r--r--   0 coseto     (501) staff       (20)       52 2023-05-05 14:55:45.000000 AutoGenerateMKD-0.0.6/.gitignore
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:34:12.659791 AutoGenerateMKD-0.0.6/AutoGenerateMKD/
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 14:51:10.000000 AutoGenerateMKD-0.0.6/AutoGenerateMKD/__init__.py
--rw-r--r--   0 coseto     (501) staff       (20)     2369 2023-05-05 16:22:41.000000 AutoGenerateMKD-0.0.6/AutoGenerateMKD/main.py
--rw-r--r--   0 coseto     (501) staff       (20)     1239 2023-05-04 17:27:12.000000 AutoGenerateMKD-0.0.6/AutoGenerateMKD/mkdocs.yml
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:34:12.664174 AutoGenerateMKD-0.0.6/AutoGenerateMKD.egg-info/
--rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 16:34:12.000000 AutoGenerateMKD-0.0.6/AutoGenerateMKD.egg-info/PKG-INFO
--rw-r--r--   0 coseto     (501) staff       (20)      467 2023-05-05 16:34:12.000000 AutoGenerateMKD-0.0.6/AutoGenerateMKD.egg-info/SOURCES.txt
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 16:34:12.000000 AutoGenerateMKD-0.0.6/AutoGenerateMKD.egg-info/dependency_links.txt
--rw-r--r--   0 coseto     (501) staff       (20)      146 2023-05-05 16:34:12.000000 AutoGenerateMKD-0.0.6/AutoGenerateMKD.egg-info/entry_points.txt
--rw-r--r--   0 coseto     (501) staff       (20)      349 2023-05-05 16:34:12.000000 AutoGenerateMKD-0.0.6/AutoGenerateMKD.egg-info/requires.txt
--rw-r--r--   0 coseto     (501) staff       (20)       41 2023-05-05 16:34:12.000000 AutoGenerateMKD-0.0.6/AutoGenerateMKD.egg-info/top_level.txt
--rw-r--r--   0 coseto     (501) staff       (20)     1054 2023-05-04 15:54:56.000000 AutoGenerateMKD-0.0.6/LICENSE
--rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 16:34:12.667484 AutoGenerateMKD-0.0.6/PKG-INFO
--rw-r--r--   0 coseto     (501) staff       (20)       52 2023-05-04 15:56:36.000000 AutoGenerateMKD-0.0.6/Readme.md
--rw-r--r--   0 coseto     (501) staff       (20)      314 2023-05-05 16:20:54.000000 AutoGenerateMKD-0.0.6/SUMMARY.md
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:34:12.666240 AutoGenerateMKD-0.0.6/mkdocs_pagenav_generator/
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.6/mkdocs_pagenav_generator/__init__.py
--rw-r--r--   0 coseto     (501) staff       (20)      993 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.6/mkdocs_pagenav_generator/plugin.py
--rw-r--r--   0 coseto     (501) staff       (20)     1371 2023-05-04 15:36:15.000000 AutoGenerateMKD-0.0.6/pyproject.toml
--rw-r--r--   0 coseto     (501) staff       (20)      225 2023-05-04 15:24:17.000000 AutoGenerateMKD-0.0.6/requirements.txt
--rw-r--r--   0 coseto     (501) staff       (20)       38 2023-05-05 16:34:12.668372 AutoGenerateMKD-0.0.6/setup.cfg
--rw-r--r--   0 coseto     (501) staff       (20)     1215 2023-05-05 16:33:57.000000 AutoGenerateMKD-0.0.6/setup.py
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:40:40.363118 AutoGenerateMKD-0.0.7/
+-rw-r--r--   0 coseto     (501) staff       (20)       52 2023-05-05 14:55:45.000000 AutoGenerateMKD-0.0.7/.gitignore
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:40:40.355452 AutoGenerateMKD-0.0.7/AutoGenerateMKD/
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 14:51:10.000000 AutoGenerateMKD-0.0.7/AutoGenerateMKD/__init__.py
+-rw-r--r--   0 coseto     (501) staff       (20)     2369 2023-05-05 16:22:41.000000 AutoGenerateMKD-0.0.7/AutoGenerateMKD/main.py
+-rw-r--r--   0 coseto     (501) staff       (20)     1239 2023-05-04 17:27:12.000000 AutoGenerateMKD-0.0.7/AutoGenerateMKD/mkdocs.yml
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:40:40.360047 AutoGenerateMKD-0.0.7/AutoGenerateMKD.egg-info/
+-rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 16:40:40.000000 AutoGenerateMKD-0.0.7/AutoGenerateMKD.egg-info/PKG-INFO
+-rw-r--r--   0 coseto     (501) staff       (20)      467 2023-05-05 16:40:40.000000 AutoGenerateMKD-0.0.7/AutoGenerateMKD.egg-info/SOURCES.txt
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 16:40:40.000000 AutoGenerateMKD-0.0.7/AutoGenerateMKD.egg-info/dependency_links.txt
+-rw-r--r--   0 coseto     (501) staff       (20)      146 2023-05-05 16:40:40.000000 AutoGenerateMKD-0.0.7/AutoGenerateMKD.egg-info/entry_points.txt
+-rw-r--r--   0 coseto     (501) staff       (20)      349 2023-05-05 16:40:40.000000 AutoGenerateMKD-0.0.7/AutoGenerateMKD.egg-info/requires.txt
+-rw-r--r--   0 coseto     (501) staff       (20)       41 2023-05-05 16:40:40.000000 AutoGenerateMKD-0.0.7/AutoGenerateMKD.egg-info/top_level.txt
+-rw-r--r--   0 coseto     (501) staff       (20)     1054 2023-05-04 15:54:56.000000 AutoGenerateMKD-0.0.7/LICENSE
+-rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 16:40:40.362559 AutoGenerateMKD-0.0.7/PKG-INFO
+-rw-r--r--   0 coseto     (501) staff       (20)       52 2023-05-04 15:56:36.000000 AutoGenerateMKD-0.0.7/Readme.md
+-rw-r--r--   0 coseto     (501) staff       (20)      314 2023-05-05 16:20:54.000000 AutoGenerateMKD-0.0.7/SUMMARY.md
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:40:40.361664 AutoGenerateMKD-0.0.7/mkdocs_pagenav_generator/
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.7/mkdocs_pagenav_generator/__init__.py
+-rw-r--r--   0 coseto     (501) staff       (20)      993 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.7/mkdocs_pagenav_generator/plugin.py
+-rw-r--r--   0 coseto     (501) staff       (20)     1371 2023-05-04 15:36:15.000000 AutoGenerateMKD-0.0.7/pyproject.toml
+-rw-r--r--   0 coseto     (501) staff       (20)      225 2023-05-04 15:24:17.000000 AutoGenerateMKD-0.0.7/requirements.txt
+-rw-r--r--   0 coseto     (501) staff       (20)       38 2023-05-05 16:40:40.363283 AutoGenerateMKD-0.0.7/setup.cfg
+-rw-r--r--   0 coseto     (501) staff       (20)     1242 2023-05-05 16:40:32.000000 AutoGenerateMKD-0.0.7/setup.py
```

### Comparing `AutoGenerateMKD-0.0.6/AutoGenerateMKD/main.py` & `AutoGenerateMKD-0.0.7/AutoGenerateMKD/main.py`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.6/AutoGenerateMKD/mkdocs.yml` & `AutoGenerateMKD-0.0.7/AutoGenerateMKD/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.6/LICENSE` & `AutoGenerateMKD-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.6/mkdocs_pagenav_generator/plugin.py` & `AutoGenerateMKD-0.0.7/mkdocs_pagenav_generator/plugin.py`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.6/pyproject.toml` & `AutoGenerateMKD-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.6/setup.py` & `AutoGenerateMKD-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="AutoGenerateMKD",
-    version="0.0.6",
+    version="0.0.7",
     author="E-NoR,Teng",
     description="Auto generate markdown api docs, base on dosc.",
     packages=find_packages(),
     install_requires=[
         "mkdocs>=1",
         "wcmatch>=7",
         "mkdocs-awesome-pages-plugin>=2.5.0",
@@ -19,15 +19,16 @@
         "mkdocs-material>=1.1.1",
         "mkdocstrings-python>=0.9.0",
         "pymdown-extensions>=9.11",
         "mkdocs>=1",
         "wcmatch>=7",
         "mkdocs-awesome-pages-plugin>=2.5.0",
     ],
-    data_files=[("data", ["AutoGenerateMKD/mkdocs.yml"])],
+    include_package_data=True,
+    data_files=[("", ["AutoGenerateMKD/mkdocs.yml"])],
     entry_points={
         "mkdocs.plugins": ["pagenav-generator = mkdocs_pagenav_generator.plugin:NavGeneratorPlugin"],
         "console_scripts": [
             "AutoGenMKD=AutoGenerateMKD.main:main",
         ],
     },
     classifiers=[
```

