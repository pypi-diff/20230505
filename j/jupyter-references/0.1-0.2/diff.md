# Comparing `tmp/jupyter-references-0.1.tar.gz` & `tmp/jupyter-references-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-references-0.1.tar", last modified: Fri May  5 17:11:38 2023, max compression
+gzip compressed data, was "jupyter-references-0.2.tar", last modified: Fri May  5 17:14:13 2023, max compression
```

## Comparing `jupyter-references-0.1.tar` & `jupyter-references-0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:11:38.464957 jupyter-references-0.1/
--rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.1/LICENSE
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 17:11:38.464685 jupyter-references-0.1/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.1/README.md
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:11:38.459905 jupyter-references-0.1/jupyter_references/
--rw-r--r--   0 kmt        (501) staff       (20)     3275 2023-05-05 17:06:41.000000 jupyter-references-0.1/jupyter_references/__init__.py
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:11:38.464105 jupyter-references-0.1/jupyter_references.egg-info/
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 17:11:38.000000 jupyter-references-0.1/jupyter_references.egg-info/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)      225 2023-05-05 17:11:38.000000 jupyter-references-0.1/jupyter_references.egg-info/SOURCES.txt
--rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-05 17:11:38.000000 jupyter-references-0.1/jupyter_references.egg-info/dependency_links.txt
--rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-05 17:11:38.000000 jupyter-references-0.1/jupyter_references.egg-info/top_level.txt
--rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-05 17:11:38.465026 jupyter-references-0.1/setup.cfg
--rw-r--r--   0 kmt        (501) staff       (20)     1093 2023-05-05 17:09:45.000000 jupyter-references-0.1/setup.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:14:13.047169 jupyter-references-0.2/
+-rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.2/LICENSE
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 17:14:13.046932 jupyter-references-0.2/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.2/README.md
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:14:13.041507 jupyter-references-0.2/jupyter_references/
+-rw-r--r--   0 kmt        (501) staff       (20)     3275 2023-05-05 17:06:41.000000 jupyter-references-0.2/jupyter_references/__init__.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-05 17:14:13.046074 jupyter-references-0.2/jupyter_references.egg-info/
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)      266 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/SOURCES.txt
+-rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/dependency_links.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       26 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/requires.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-05 17:14:12.000000 jupyter-references-0.2/jupyter_references.egg-info/top_level.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-05 17:14:13.047228 jupyter-references-0.2/setup.cfg
+-rw-r--r--   0 kmt        (501) staff       (20)     1114 2023-05-05 17:14:08.000000 jupyter-references-0.2/setup.py
```

### Comparing `jupyter-references-0.1/LICENSE` & `jupyter-references-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.1/PKG-INFO` & `jupyter-references-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.1
+Version: 0.2
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.1/README.md` & `jupyter-references-0.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.1/jupyter_references/__init__.py` & `jupyter-references-0.2/jupyter_references/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.1/jupyter_references.egg-info/PKG-INFO` & `jupyter-references-0.2/jupyter_references.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.1
+Version: 0.2
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.1/setup.py` & `jupyter-references-0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,25 @@
     long_description = f.read()
 
 # package name must be the git repository name
 package_name = path.basename(this_directory)
 
 setuptools.setup(
     name=package_name,
-    version="0.1",
+    version="0.2",
     author="Kasper Munch",
     author_email="kaspermunch@birc.au.dk",
     description="Lightweight system for citing papers and making a reference list in jupyter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f'https://github.com/kaspermunch/{package_name}',
     packages=setuptools.find_packages(),
     # scripts=['script.py', 'other_script.py'],
     # entry_points = {
     #     'console_scripts': [f'commaneline_name={package_name}.function_name',
     #                         f'other_commaneline_name={package_name}.other_function_name']
     # },
     python_requires='>=3.7',
     install_requires=[
-        #   'numpy>=1.1',
+        'ipynbname',
+        'jupyterlab>=3.0'
     ])
```

