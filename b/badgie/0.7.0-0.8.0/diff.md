# Comparing `tmp/badgie-0.7.0.tar.gz` & `tmp/badgie-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgie-0.7.0.tar", last modified: Tue May  2 21:33:10 2023, max compression
+gzip compressed data, was "badgie-0.8.0.tar", last modified: Fri May  5 06:33:34 2023, max compression
```

## Comparing `badgie-0.7.0.tar` & `badgie-0.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.239818 badgie-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-02 21:33:05.000000 badgie-0.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4641 2023-05-02 21:33:10.239818 badgie-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3749 2023-05-02 21:33:05.000000 badgie-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.234818 badgie-0.7.0/badgie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-02 21:33:07.000000 badgie-0.7.0/badgie/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.237818 badgie-0.7.0/badgie/badges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/brettops.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/codestyle.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     6403 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.239818 badgie-0.7.0/badgie/finders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/files.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/pre_commit_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/remotes.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/project.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.235818 badgie-0.7.0/badgie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4641 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-02 21:33:10.240818 badgie-0.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-02 21:33:07.000000 badgie-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.547295 badgie-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-05 06:33:29.000000 badgie-0.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-05-05 06:33:34.547295 badgie-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2023-05-05 06:33:29.000000 badgie-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.542295 badgie-0.8.0/badgie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-05 06:33:31.000000 badgie-0.8.0/badgie/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.545295 badgie-0.8.0/badgie/badges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/brettops.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/codestyle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6403 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.547295 badgie-0.8.0/badgie/finders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/pre_commit_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/remotes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/project.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.544295 badgie-0.8.0/badgie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-05 06:33:34.548296 badgie-0.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1525 2023-05-05 06:33:31.000000 badgie-0.8.0/setup.py
```

### Comparing `badgie-0.7.0/LICENSE` & `badgie-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/badges/brettops.py` & `badgie-0.8.0/badgie/badges/brettops.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/badges/codestyle.py` & `badgie-0.8.0/badgie/badges/codestyle.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/badges/gitlab.py` & `badgie-0.8.0/badgie/badges/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/badges/precommit.py` & `badgie-0.8.0/badgie/badges/precommit.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/cli.py` & `badgie-0.8.0/badgie/cli.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/finders/files.py` & `badgie-0.8.0/badgie/finders/files.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/finders/gitlab.py` & `badgie-0.8.0/badgie/finders/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/finders/pre_commit_config.py` & `badgie-0.8.0/badgie/finders/pre_commit_config.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/finders/remotes.py` & `badgie-0.8.0/badgie/finders/remotes.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/models.py` & `badgie-0.8.0/badgie/models.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/parser.py` & `badgie-0.8.0/badgie/parser.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/project.py` & `badgie-0.8.0/badgie/project.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/tokens.py` & `badgie-0.8.0/badgie/tokens.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie/utils.py` & `badgie-0.8.0/badgie/utils.py`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/badgie.egg-info/SOURCES.txt` & `badgie-0.8.0/badgie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badgie-0.7.0/setup.py` & `badgie-0.8.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
 
@@ -26,20 +26,22 @@
             "badgie = badgie.cli:main",
         ],
     },
     install_requires=install_requires,
     python_requires=">=3.9",
     keywords=["badge", "template", "markdown"],
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Documentation",
+        "Topic :: Software Development :: Quality Assurance",
+        "Topic :: Utilities",
     ],
 )
```

