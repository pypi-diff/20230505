# Comparing `tmp/carchive-0.0.39.tar.gz` & `tmp/carchive-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.39.tar", last modified: Fri May  5 01:25:23 2023, max compression
+gzip compressed data, was "carchive-0.0.40.tar", last modified: Fri May  5 01:42:04 2023, max compression
```

## Comparing `carchive-0.0.39.tar` & `carchive-0.0.40.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.406494 carchive-0.0.39/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 01:25:18.000000 carchive-0.0.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 01:25:23.406494 carchive-0.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 01:25:18.000000 carchive-0.0.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.402494 carchive-0.0.39/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9130 2023-05-05 01:25:18.000000 carchive-0.0.39/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.406494 carchive-0.0.39/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:25:23.406494 carchive-0.0.39/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3593 2023-05-05 01:25:18.000000 carchive-0.0.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:42:04.546875 carchive-0.0.40/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 01:41:58.000000 carchive-0.0.40/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 01:42:04.546875 carchive-0.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 01:41:58.000000 carchive-0.0.40/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:42:04.542875 carchive-0.0.40/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9130 2023-05-05 01:41:58.000000 carchive-0.0.40/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:42:04.546875 carchive-0.0.40/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 01:42:04.000000 carchive-0.0.40/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 01:42:04.000000 carchive-0.0.40/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:42:04.000000 carchive-0.0.40/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 01:42:04.000000 carchive-0.0.40/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 01:42:04.000000 carchive-0.0.40/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:42:04.546875 carchive-0.0.40/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3334 2023-05-05 01:41:58.000000 carchive-0.0.40/setup.py
```

### Comparing `carchive-0.0.39/LICENSE` & `carchive-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.39/carchive/__init__.py` & `carchive-0.0.40/carchive/__init__.py`

 * *Files identical despite different names*

### Comparing `carchive-0.0.39/setup.py` & `carchive-0.0.40/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.39"
+VERSION = "0.0.40"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -101,19 +101,16 @@
 	python_requires=REQUIRES_PYTHON,
 	url=URL,
 	packages=find_packages(
 		exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 	entry_points={
 	},
 	install_requires=[
-		#https://pygithub.readthedocs.io/en/latest/introduction.html
-		"PyGithub", #To search for Repositories
-		#https://stackoverflow.com/questions/32688688/how-to-write-setup-py-to-include-a-git-repository-as-a-dependency/54701434#54701434
-		#https://git2net.readthedocs.io/en/latest/
-		"git2net @ git+https://github.com/franceme/git2net.git", #To gather and run metrics on the Repositories
+		"PyGithub", 
+		"git2net @ git+ssh://git@github.com/franceme/git2net/tarball/master@0ca0ce7db9c3a616096a250c9412a8780dd30768", 
 		"splittr",
 		"waybackpy",
 		"mystring",
 		"pygit2",
 	],
 	include_package_data=True,
 	classifiers=[
```

