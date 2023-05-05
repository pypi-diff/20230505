# Comparing `tmp/ALifeStdDev-0.3.0.tar.gz` & `tmp/ALifeStdDev-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ALifeStdDev-0.3.0.tar", last modified: Thu May  4 23:28:41 2023, max compression
+gzip compressed data, was "ALifeStdDev-0.3.3.tar", last modified: Fri May  5 03:25:01 2023, max compression
```

## Comparing `ALifeStdDev-0.3.0.tar` & `ALifeStdDev-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:28:41.576547 ALifeStdDev-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:28:41.576547 ALifeStdDev-0.3.0/ALifeStdDev/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 23:28:13.000000 ALifeStdDev-0.3.0/ALifeStdDev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:28:41.576547 ALifeStdDev-0.3.0/ALifeStdDev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-04 23:28:41.000000 ALifeStdDev-0.3.0/ALifeStdDev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-04 23:28:41.000000 ALifeStdDev-0.3.0/ALifeStdDev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:28:41.000000 ALifeStdDev-0.3.0/ALifeStdDev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:28:40.000000 ALifeStdDev-0.3.0/ALifeStdDev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 23:28:41.000000 ALifeStdDev-0.3.0/ALifeStdDev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 23:28:41.000000 ALifeStdDev-0.3.0/ALifeStdDev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-04 23:28:13.000000 ALifeStdDev-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-04 23:28:41.576547 ALifeStdDev-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-04 23:28:13.000000 ALifeStdDev-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 23:28:41.576547 ALifeStdDev-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-04 23:28:13.000000 ALifeStdDev-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:01.064870 ALifeStdDev-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:01.064870 ALifeStdDev-0.3.3/ALifeStdDev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:01.064870 ALifeStdDev-0.3.3/ALifeStdDev/ALifeStdDev/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 03:24:36.000000 ALifeStdDev-0.3.3/ALifeStdDev/ALifeStdDev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-05 03:24:36.000000 ALifeStdDev-0.3.3/ALifeStdDev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:01.064870 ALifeStdDev-0.3.3/ALifeStdDev/phylogeny/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 03:24:36.000000 ALifeStdDev-0.3.3/ALifeStdDev/phylogeny/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-05 03:24:36.000000 ALifeStdDev-0.3.3/ALifeStdDev/phylogeny/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-05 03:24:36.000000 ALifeStdDev-0.3.3/ALifeStdDev/phylogeny/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30491 2023-05-05 03:24:36.000000 ALifeStdDev-0.3.3/ALifeStdDev/phylogeny/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:01.064870 ALifeStdDev-0.3.3/ALifeStdDev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-05 03:25:01.000000 ALifeStdDev-0.3.3/ALifeStdDev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-05 03:25:01.000000 ALifeStdDev-0.3.3/ALifeStdDev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:25:01.000000 ALifeStdDev-0.3.3/ALifeStdDev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:25:00.000000 ALifeStdDev-0.3.3/ALifeStdDev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 03:25:01.000000 ALifeStdDev-0.3.3/ALifeStdDev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 03:25:01.000000 ALifeStdDev-0.3.3/ALifeStdDev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-05 03:24:36.000000 ALifeStdDev-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-05 03:25:01.064870 ALifeStdDev-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-05 03:24:36.000000 ALifeStdDev-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:25:01.064870 ALifeStdDev-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-05 03:24:36.000000 ALifeStdDev-0.3.3/setup.py
```

### Comparing `ALifeStdDev-0.3.0/ALifeStdDev.egg-info/PKG-INFO` & `ALifeStdDev-0.3.3/ALifeStdDev.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,50 @@
 Metadata-Version: 2.1
 Name: ALifeStdDev
-Version: 0.3.0
+Version: 0.3.3
 Summary: Python development tools for working with standardized ALife data.
 Home-page: https://github.com/alife-data-standards/alife-std-dev-python
 Author: Emily Dolson, Alex Lalejini, Matthew Andres Moreno
 Author-email: dolsonem@msu.edu, lalejini@msu.edu, morenoma@umich.edu
 License: MIT
 Description: # ALife Data Standards - Python Development Utilities
         
         [![CI](https://github.com/alife-data-standards/alife-std-dev-python/actions/workflows/CI.yaml/badge.svg)](https://github.com/alife-data-standards/alife-std-dev-python/actions/workflows/CI.yaml)
         [![Codacy Badge](https://app.codacy.com/project/badge/Grade/0305e8a814e04d4395c25a70b2908651)](https://www.codacy.com/gh/alife-data-standards/alife-std-dev-python/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=alife-data-standards/alife-std-dev-python&amp;utm_campaign=Badge_Grade)
         [![codecov](https://codecov.io/gh/alife-data-standards/alife-std-dev-python/branch/master/graph/badge.svg?token=FGMQICJ2SK)](https://codecov.io/gh/alife-data-standards/alife-std-dev-python)
+        ![PyPI](https://img.shields.io/pypi/v/ALifeStdDev?color=blue)
         
         This is the repository for the ALifeStdDev Python package, which contains Python
         development utilities for working with [standardized](https://github.com/alife-data-standards/alife-data-standards)
         ALife data.
         
+        # Installation Instructions
+        
+        ALifeStdDev can be installed using pip:
+        
+        ```
+        pip install ALifeStdDev
+        ```
+        
+        # Usage Instructions
+        
+        To load a single submodule,
+        
+        ```python3
+        from ALifeStdDev import phylogeny as asd_phylo
+        asd_phylo.load_phylogeny_to_pandas_df("myfile.csv")
+        ```
+        
+        To load the library as a flat namespace,
+        
+        ```python3
+        from ALifeStdDev import ALifeStdDev as asd
+        asd.load_phylogeny_to_pandas_df("myfile.csv")
+        ```
+        
 Keywords: artificial life
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ALifeStdDev-0.3.0/LICENSE` & `ALifeStdDev-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ALifeStdDev-0.3.0/PKG-INFO` & `ALifeStdDev-0.3.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,50 @@
 Metadata-Version: 2.1
 Name: ALifeStdDev
-Version: 0.3.0
+Version: 0.3.3
 Summary: Python development tools for working with standardized ALife data.
 Home-page: https://github.com/alife-data-standards/alife-std-dev-python
 Author: Emily Dolson, Alex Lalejini, Matthew Andres Moreno
 Author-email: dolsonem@msu.edu, lalejini@msu.edu, morenoma@umich.edu
 License: MIT
 Description: # ALife Data Standards - Python Development Utilities
         
         [![CI](https://github.com/alife-data-standards/alife-std-dev-python/actions/workflows/CI.yaml/badge.svg)](https://github.com/alife-data-standards/alife-std-dev-python/actions/workflows/CI.yaml)
         [![Codacy Badge](https://app.codacy.com/project/badge/Grade/0305e8a814e04d4395c25a70b2908651)](https://www.codacy.com/gh/alife-data-standards/alife-std-dev-python/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=alife-data-standards/alife-std-dev-python&amp;utm_campaign=Badge_Grade)
         [![codecov](https://codecov.io/gh/alife-data-standards/alife-std-dev-python/branch/master/graph/badge.svg?token=FGMQICJ2SK)](https://codecov.io/gh/alife-data-standards/alife-std-dev-python)
+        ![PyPI](https://img.shields.io/pypi/v/ALifeStdDev?color=blue)
         
         This is the repository for the ALifeStdDev Python package, which contains Python
         development utilities for working with [standardized](https://github.com/alife-data-standards/alife-data-standards)
         ALife data.
         
+        # Installation Instructions
+        
+        ALifeStdDev can be installed using pip:
+        
+        ```
+        pip install ALifeStdDev
+        ```
+        
+        # Usage Instructions
+        
+        To load a single submodule,
+        
+        ```python3
+        from ALifeStdDev import phylogeny as asd_phylo
+        asd_phylo.load_phylogeny_to_pandas_df("myfile.csv")
+        ```
+        
+        To load the library as a flat namespace,
+        
+        ```python3
+        from ALifeStdDev import ALifeStdDev as asd
+        asd.load_phylogeny_to_pandas_df("myfile.csv")
+        ```
+        
 Keywords: artificial life
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ALifeStdDev-0.3.0/setup.py` & `ALifeStdDev-0.3.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(name='ALifeStdDev',
-      version='0.3.0',
+      version='0.3.3',
       description='Python development tools for working with standardized ALife data.',
       url='https://github.com/alife-data-standards/alife-std-dev-python',
       author='Emily Dolson, Alex Lalejini, Matthew Andres Moreno',
       author_email='dolsonem@msu.edu, lalejini@msu.edu, morenoma@umich.edu',
       license='MIT',
       python_requires='>=3.7',
       classifiers=[
@@ -26,12 +26,12 @@
         # 'Programming Language :: Python :: 3.11',
       ],
       long_description=readme,
       long_description_content_type='text/markdown',
       include_package_data=True,
       keywords='artificial life',
       test_suite='tests',
-      packages=['ALifeStdDev'],
+      packages=find_packages(include=['ALifeStdDev', 'ALifeStdDev.*']),
       install_requires=['networkx', 'pandas'],
       tests_require=['pytest'],
       zip_safe=False,
 )
```

