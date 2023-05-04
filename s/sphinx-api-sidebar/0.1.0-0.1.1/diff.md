# Comparing `tmp/sphinx_api_sidebar-0.1.0.tar.gz` & `tmp/sphinx_api_sidebar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_api_sidebar-0.1.0.tar", last modified: Thu May  4 23:27:13 2023, max compression
+gzip compressed data, was "sphinx_api_sidebar-0.1.1.tar", last modified: Thu May  4 23:41:32 2023, max compression
```

## Comparing `sphinx_api_sidebar-0.1.0.tar` & `sphinx_api_sidebar-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:27:13.662619 sphinx_api_sidebar-0.1.0/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1069 2023-05-04 06:26:37.000000 sphinx_api_sidebar-0.1.0/LICENSE
--rw-r--r--   0 yihengxiong   (501) staff       (20)        0 2023-05-04 06:32:13.000000 sphinx_api_sidebar-0.1.0/MANIFEST.in
--rw-r--r--   0 yihengxiong   (501) staff       (20)     4729 2023-05-04 23:27:13.661896 sphinx_api_sidebar-0.1.0/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)     2804 2023-05-04 23:16:02.000000 sphinx_api_sidebar-0.1.0/README.md
--rw-r--r--   0 yihengxiong   (501) staff       (20)      358 2023-05-04 23:26:35.000000 sphinx_api_sidebar-0.1.0/pyproject.toml
--rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-04 23:27:13.662800 sphinx_api_sidebar-0.1.0/setup.cfg
--rw-r--r--   0 yihengxiong   (501) staff       (20)      934 2023-05-04 16:40:41.000000 sphinx_api_sidebar-0.1.0/setup.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:27:13.654517 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar/
--rw-r--r--   0 yihengxiong   (501) staff       (20)       37 2023-05-04 06:28:19.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar/__init__.py
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1526 2023-05-04 23:02:49.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar/sphinx_api_sidebar.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:27:13.660058 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     4729 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)      412 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/SOURCES.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)        1 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/dependency_links.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       66 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/entry_points.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       12 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/requires.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       19 2023-05-04 23:27:13.000000 sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/top_level.txt
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:27:13.660824 sphinx_api_sidebar-0.1.0/tests/
--rw-r--r--   0 yihengxiong   (501) staff       (20)      555 2023-05-04 16:40:41.000000 sphinx_api_sidebar-0.1.0/tests/test_sphinx_api_sidebar.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:41:32.847503 sphinx_api_sidebar-0.1.1/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     1069 2023-05-04 06:26:37.000000 sphinx_api_sidebar-0.1.1/LICENSE
+-rw-r--r--   0 yihengxiong   (501) staff       (20)        0 2023-05-04 06:32:13.000000 sphinx_api_sidebar-0.1.1/MANIFEST.in
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     4730 2023-05-04 23:41:32.846940 sphinx_api_sidebar-0.1.1/PKG-INFO
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     2805 2023-05-04 23:38:29.000000 sphinx_api_sidebar-0.1.1/README.md
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      358 2023-05-04 23:39:35.000000 sphinx_api_sidebar-0.1.1/pyproject.toml
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-04 23:41:32.847670 sphinx_api_sidebar-0.1.1/setup.cfg
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      934 2023-05-04 16:40:41.000000 sphinx_api_sidebar-0.1.1/setup.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:41:32.837836 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       37 2023-05-04 06:28:19.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar/__init__.py
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     1526 2023-05-04 23:02:49.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar/sphinx_api_sidebar.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:41:32.845482 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     4730 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/PKG-INFO
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      412 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/SOURCES.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)        1 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/dependency_links.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       66 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/entry_points.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       12 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/requires.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       19 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/top_level.txt
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:41:32.845994 sphinx_api_sidebar-0.1.1/tests/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      555 2023-05-04 16:40:41.000000 sphinx_api_sidebar-0.1.1/tests/test_sphinx_api_sidebar.py
```

### Comparing `sphinx_api_sidebar-0.1.0/LICENSE` & `sphinx_api_sidebar-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_api_sidebar-0.1.0/PKG-INFO` & `sphinx_api_sidebar-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_api_sidebar
-Version: 0.1.0
+Version: 0.1.1
 Summary: Display any generated static API documentation in a sidebar
 Home-page: https://github.com/Yihengxiong6/sphinx_api_sidebar
 Author: Yiheng Xiong
 Author-email: Yiheng Xiong <georgex8866@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yiheng Xiong
@@ -64,15 +64,15 @@
     # Other extensions...
 ]
 ```
 
 2. To use a custom command to generate your API documentation or specify different directories, you can set the api_docs_generator configuration value in your conf.py file:
 
 ```python
-api_docs_generator = [
+api_docs_generators = [
   {
     'command': '<your_api_docs_build_command_1>',
     'outputs': [
             {
                 'name': '<generated_api_doc_name_1>',
                 'path': '<path_to_generated_api_doc_1>'
             },
```

### Comparing `sphinx_api_sidebar-0.1.0/README.md` & `sphinx_api_sidebar-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # Other extensions...
 ]
 ```
 
 2. To use a custom command to generate your API documentation or specify different directories, you can set the api_docs_generator configuration value in your conf.py file:
 
 ```python
-api_docs_generator = [
+api_docs_generators = [
   {
     'command': '<your_api_docs_build_command_1>',
     'outputs': [
             {
                 'name': '<generated_api_doc_name_1>',
                 'path': '<path_to_generated_api_doc_1>'
             },
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 ## Installation To install the `sphinx-api-sidebar` extension, you can use pip:
 ```sh pip install sphinx-api-sidebar ``` ## Usage 1. To enable the sphinx-api-
 sidebar extension in your Sphinx documentation project, add it to the
 extensions list in your conf.py file: ```python extensions =
 [ 'sphinx_api_sidebar', # Other extensions... ] ``` 2. To use a custom command
 to generate your API documentation or specify different directories, you can
 set the api_docs_generator configuration value in your conf.py file: ```python
-api_docs_generator = [ { 'command': '', 'outputs': [ { 'name': '', 'path': ''
+api_docs_generators = [ { 'command': '', 'outputs': [ { 'name': '', 'path': ''
 }, { 'name': '', 'path': '' }, # ... ] }, { 'command': '', 'outputs': [
 { 'name': '', 'path': '' }, # ... ] }, # more groups of generated api docs ]
 ``` Replace
 >,
 >, and
 > with the appropriate values for your project. 3. To make the different api
 documentation show up in the sidebar, you will need to copy the
```

### Comparing `sphinx_api_sidebar-0.1.0/setup.py` & `sphinx_api_sidebar-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_api_sidebar-0.1.0/sphinx_api_sidebar/sphinx_api_sidebar.py` & `sphinx_api_sidebar-0.1.1/sphinx_api_sidebar/sphinx_api_sidebar.py`

 * *Files identical despite different names*

### Comparing `sphinx_api_sidebar-0.1.0/sphinx_api_sidebar.egg-info/PKG-INFO` & `sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-api-sidebar
-Version: 0.1.0
+Version: 0.1.1
 Summary: Display any generated static API documentation in a sidebar
 Home-page: https://github.com/Yihengxiong6/sphinx_api_sidebar
 Author: Yiheng Xiong
 Author-email: Yiheng Xiong <georgex8866@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yiheng Xiong
@@ -64,15 +64,15 @@
     # Other extensions...
 ]
 ```
 
 2. To use a custom command to generate your API documentation or specify different directories, you can set the api_docs_generator configuration value in your conf.py file:
 
 ```python
-api_docs_generator = [
+api_docs_generators = [
   {
     'command': '<your_api_docs_build_command_1>',
     'outputs': [
             {
                 'name': '<generated_api_doc_name_1>',
                 'path': '<path_to_generated_api_doc_1>'
             },
```

### Comparing `sphinx_api_sidebar-0.1.0/tests/test_sphinx_api_sidebar.py` & `sphinx_api_sidebar-0.1.1/tests/test_sphinx_api_sidebar.py`

 * *Files identical despite different names*

