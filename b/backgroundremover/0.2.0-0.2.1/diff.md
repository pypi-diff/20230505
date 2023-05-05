# Comparing `tmp/backgroundremover-0.2.0.tar.gz` & `tmp/backgroundremover-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backgroundremover-0.2.0.tar", last modified: Fri May  5 19:23:18 2023, max compression
+gzip compressed data, was "dist/backgroundremover-0.2.1.tar", last modified: Fri May  5 19:51:39 2023, max compression
```

## Comparing `backgroundremover-0.2.0.tar` & `backgroundremover-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/
--rw-rw-r--   0 john      (1000) john      (1000)     1171 2022-03-30 21:01:22.000000 backgroundremover-0.2.0/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)      183 2022-03-30 21:01:22.000000 backgroundremover-0.2.0/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     8101 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     6149 2023-05-05 19:20:58.000000 backgroundremover-0.2.0/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     8101 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      677 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       70 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      364 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       10 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/cmd/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/cmd/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/cmd/cli.py
--rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/cmd/server.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/u2net/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/u2net/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/u2net/data_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/u2net/detect.py
--rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/u2net/u2net.py
--rw-rw-r--   0 john      (1000) john      (1000)      230 2022-03-30 21:01:23.000000 backgroundremover-0.2.0/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)      364 2023-04-30 21:22:20.000000 backgroundremover-0.2.0/requirements.txt
--rw-rw-r--   0 john      (1000) john      (1000)       78 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     1086 2023-05-05 19:23:15.000000 backgroundremover-0.2.0/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/
+-rw-rw-r--   0 john      (1000) john      (1000)     1171 2022-03-30 21:01:22.000000 backgroundremover-0.2.1/LICENSE.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      183 2022-03-30 21:01:22.000000 backgroundremover-0.2.1/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     8101 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     6149 2023-05-05 19:20:58.000000 backgroundremover-0.2.1/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover/
+-rw-rw-r--   0 john      (1000) john      (1000)      173 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6793 2023-05-05 19:18:41.000000 backgroundremover-0.2.1/backgroundremover/bg.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover/cmd/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/cmd/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/cmd/cli.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/cmd/server.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover/u2net/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/u2net/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/u2net/data_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/u2net/detect.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/u2net/u2net.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12586 2023-05-05 19:18:06.000000 backgroundremover-0.2.1/backgroundremover/utilities.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     8101 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)      654 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       70 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      364 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       18 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      230 2022-03-30 21:01:23.000000 backgroundremover-0.2.1/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)      364 2023-04-30 21:22:20.000000 backgroundremover-0.2.1/requirements.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       78 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     1018 2023-05-05 19:51:38.000000 backgroundremover-0.2.1/setup.py
```

### Comparing `backgroundremover-0.2.0/LICENSE.txt` & `backgroundremover-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.0/PKG-INFO` & `backgroundremover-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.0
+Version: 0.2.1
 Summary: Background remover from image and video
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 License: UNKNOWN
 Description: # BackgroundRemover
         ![Background Remover](/examplefiles/backgroundremoverexample.png)
```

### Comparing `backgroundremover-0.2.0/README.md` & `backgroundremover-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/PKG-INFO` & `backgroundremover-0.2.1/backgroundremover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.0
+Version: 0.2.1
 Summary: Background remover from image and video
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 License: UNKNOWN
 Description: # BackgroundRemover
         ![Background Remover](/examplefiles/backgroundremoverexample.png)
```

### Comparing `backgroundremover-0.2.0/backgroundremover/cmd/cli.py` & `backgroundremover-0.2.1/backgroundremover/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.0/backgroundremover/cmd/server.py` & `backgroundremover-0.2.1/backgroundremover/cmd/server.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.0/backgroundremover/u2net/data_loader.py` & `backgroundremover-0.2.1/backgroundremover/u2net/data_loader.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.0/backgroundremover/u2net/detect.py` & `backgroundremover-0.2.1/backgroundremover/u2net/detect.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.0/backgroundremover/u2net/u2net.py` & `backgroundremover-0.2.1/backgroundremover/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.0/setup.py` & `backgroundremover-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 with open("requirements.txt") as f:
     requireds = f.read().splitlines()
 
 setup(
     name="backgroundremover",
-    version="0.2.0",
+    version="0.2.1",
     description="Background remover from image and video",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nadermx/backgroundremover",
     author="Johnathan Nader",
     author_email="john@nader.mx",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="remove, background, u2net, remove background, background remover",
-    package_dir={"": "backgroundremover"},
-    packages=find_packages(where="backgroundremover"),
+    packages=find_packages(),
     python_requires=">=3.6, <4",
     install_requires=requireds,
     entry_points={
         "console_scripts": [
             "backgroundremover=backgroundremover.cmd.cli:main",
         ],
     },
```

