# Comparing `tmp/VikyTest-4.0.tar.gz` & `tmp/VikyTest-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VikyTest-4.0.tar", last modified: Fri May  5 06:25:08 2023, max compression
+gzip compressed data, was "VikyTest-5.0.tar", last modified: Fri May  5 06:36:43 2023, max compression
```

## Comparing `VikyTest-4.0.tar` & `VikyTest-5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:25:08.043882 VikyTest-4.0/
--rwx------   0 ec2-user  (1000) ec2-user  (1000)     1061 2023-05-04 05:18:17.000000 VikyTest-4.0/LICENSE.txt
--rw-------   0 ec2-user  (1000) ec2-user  (1000)      395 2023-05-05 06:25:08.039883 VikyTest-4.0/PKG-INFO
--rwx------   0 ec2-user  (1000) ec2-user  (1000)     8124 2023-05-04 05:18:17.000000 VikyTest-4.0/README.md
--rwx------   0 ec2-user  (1000) ec2-user  (1000)       86 2023-05-04 05:18:17.000000 VikyTest-4.0/pyproject.toml
--rw-------   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-05 06:25:08.043882 VikyTest-4.0/setup.cfg
--rwx------   0 ec2-user  (1000) ec2-user  (1000)      650 2023-05-05 06:24:33.000000 VikyTest-4.0/setup.py
-drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:25:08.039883 VikyTest-4.0/src/
-drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:25:08.039883 VikyTest-4.0/src/VikyTest/
--rwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-04 05:27:28.000000 VikyTest-4.0/src/VikyTest/__init__.py
--rwx------   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-05 05:46:55.000000 VikyTest-4.0/src/VikyTest/medToolkit.py
-drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:25:08.039883 VikyTest-4.0/src/VikyTest.egg-info/
--rw-------   0 ec2-user  (1000) ec2-user  (1000)      395 2023-05-05 06:25:07.000000 VikyTest-4.0/src/VikyTest.egg-info/PKG-INFO
--rw-------   0 ec2-user  (1000) ec2-user  (1000)      241 2023-05-05 06:25:08.000000 VikyTest-4.0/src/VikyTest.egg-info/SOURCES.txt
--rw-------   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-05 06:25:07.000000 VikyTest-4.0/src/VikyTest.egg-info/dependency_links.txt
--rw-------   0 ec2-user  (1000) ec2-user  (1000)        9 2023-05-05 06:25:07.000000 VikyTest-4.0/src/VikyTest.egg-info/top_level.txt
+drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:36:43.989111 VikyTest-5.0/
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)     1061 2023-05-04 05:18:17.000000 VikyTest-5.0/LICENSE.txt
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)      395 2023-05-05 06:36:43.989111 VikyTest-5.0/PKG-INFO
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)     8124 2023-05-04 05:18:17.000000 VikyTest-5.0/README.md
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)       86 2023-05-04 05:18:17.000000 VikyTest-5.0/pyproject.toml
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-05 06:36:43.989111 VikyTest-5.0/setup.cfg
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)     1133 2023-05-05 06:35:58.000000 VikyTest-5.0/setup.py
+drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:36:43.985111 VikyTest-5.0/src/
+drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:36:43.989111 VikyTest-5.0/src/VikyTest/
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-04 05:27:28.000000 VikyTest-5.0/src/VikyTest/__init__.py
+-rwx------   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-05 05:46:55.000000 VikyTest-5.0/src/VikyTest/medToolkit.py
+drwx------   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-05 06:36:43.989111 VikyTest-5.0/src/VikyTest.egg-info/
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)      395 2023-05-05 06:36:43.000000 VikyTest-5.0/src/VikyTest.egg-info/PKG-INFO
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)      241 2023-05-05 06:36:43.000000 VikyTest-5.0/src/VikyTest.egg-info/SOURCES.txt
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-05 06:36:43.000000 VikyTest-5.0/src/VikyTest.egg-info/dependency_links.txt
+-rw-------   0 ec2-user  (1000) ec2-user  (1000)        9 2023-05-05 06:36:43.000000 VikyTest-5.0/src/VikyTest.egg-info/top_level.txt
```

### Comparing `VikyTest-4.0/LICENSE.txt` & `VikyTest-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VikyTest-4.0/README.md` & `VikyTest-5.0/README.md`

 * *Files identical despite different names*

### Comparing `VikyTest-4.0/setup.py` & `VikyTest-5.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 from setuptools import setup, find_packages
+from setuptools.command.install import install
+import os
+import urllib.request
+
+class PostInstallCommand(install):
+    def run(self):
+        install.run(self)
+        print("Downloading data files....")
+        url = "https://sample-videos.com/zip/10mb.zip"
+        target_dir = os.path.join(self.install_lib, "VikyTest", "data")
+        os.makedirs(target_dir, exist_ok = True)
+        filename, headers = urllib.request.urlretrieve(url, os.path.join(target_dir, "10mb.zip"))
+
 
 setup(
     name = "VikyTest",
-    version = "4.0",
+    version = "5.0",
     author = "VigneshVallavan",
     author_email = "vigneshvallavan1999@gmail.com",
     description = "Medical NLP Toolkit",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir = {"": "src"},
     packages = find_packages(where="src"),
     python_requires = ">=3.6",
     include_package_data = True,
-    package_data = {
-        'VikyTest': ['*.zip'],
+    cmdclass = {
+        'install': PostInstallCommand,
     },
     download_url = 'https://sample-videos.com/zip/10mb.zip',
 )
```

