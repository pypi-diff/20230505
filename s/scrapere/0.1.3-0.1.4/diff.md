# Comparing `tmp/scrapere-0.1.3.tar.gz` & `tmp/scrapere-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.1.3.tar", last modified: Thu May  4 15:05:25 2023, max compression
+gzip compressed data, was "scrapere-0.1.4.tar", last modified: Fri May  5 07:54:13 2023, max compression
```

## Comparing `scrapere-0.1.3.tar` & `scrapere-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-04 15:05:25.012432 scrapere-0.1.3/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      566 2023-05-04 15:05:25.012432 scrapere-0.1.3/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      356 2023-05-04 15:05:14.000000 scrapere-0.1.3/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-04 15:05:25.008432 scrapere-0.1.3/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.3/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     4741 2023-05-04 10:04:57.000000 scrapere-0.1.3/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.3/scrapere/user-agents-unique.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-04 15:05:25.012432 scrapere-0.1.3/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      566 2023-05-04 15:05:24.000000 scrapere-0.1.3/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-04 15:05:24.000000 scrapere-0.1.3/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-04 15:05:24.000000 scrapere-0.1.3/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-04 15:05:24.000000 scrapere-0.1.3/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-04 15:05:24.000000 scrapere-0.1.3/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-04 15:05:25.012432 scrapere-0.1.3/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      682 2023-05-04 15:05:10.000000 scrapere-0.1.3/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-05 07:54:13.379822 scrapere-0.1.4/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1042 2023-05-05 07:54:13.379822 scrapere-0.1.4/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      832 2023-05-05 07:53:15.000000 scrapere-0.1.4/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-05 07:54:13.375822 scrapere-0.1.4/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.4/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     4741 2023-05-05 07:53:35.000000 scrapere-0.1.4/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.4/scrapere/user-agents-unique.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-05 07:54:13.379822 scrapere-0.1.4/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1042 2023-05-05 07:54:13.000000 scrapere-0.1.4/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-05 07:54:13.000000 scrapere-0.1.4/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-05 07:54:13.000000 scrapere-0.1.4/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-05 07:54:13.000000 scrapere-0.1.4/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-05 07:54:13.000000 scrapere-0.1.4/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-05 07:54:13.379822 scrapere-0.1.4/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      682 2023-05-05 07:53:38.000000 scrapere-0.1.4/setup.py
```

### Comparing `scrapere-0.1.3/scrapere/toolbox.py` & `scrapere-0.1.4/scrapere/toolbox.py`

 * *Files identical despite different names*

### Comparing `scrapere-0.1.3/scrapere/user-agents-unique.txt` & `scrapere-0.1.4/scrapere/user-agents-unique.txt`

 * *Files identical despite different names*

### Comparing `scrapere-0.1.3/setup.py` & `scrapere-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='scrapere',
     packages=find_packages(),
-    version='0.1.3',
+    version='0.1.4',
     description='Small set of my web scraping python tools',
     author='vPere',
     license='MIT',
     readme='README.md',
     install_requires=[
         'requests',
         'beautifulsoup4',
```

