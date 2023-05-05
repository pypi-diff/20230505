# Comparing `tmp/carchive-0.0.41.tar.gz` & `tmp/carchive-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.41.tar", last modified: Fri May  5 02:21:39 2023, max compression
+gzip compressed data, was "carchive-0.0.42.tar", last modified: Fri May  5 02:22:59 2023, max compression
```

## Comparing `carchive-0.0.41.tar` & `carchive-0.0.42.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:21:39.545486 carchive-0.0.41/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 02:21:35.000000 carchive-0.0.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:21:39.545486 carchive-0.0.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 02:21:35.000000 carchive-0.0.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:21:39.545486 carchive-0.0.41/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9130 2023-05-05 02:21:35.000000 carchive-0.0.41/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:21:39.545486 carchive-0.0.41/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:21:39.000000 carchive-0.0.41/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 02:21:39.000000 carchive-0.0.41/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:21:39.000000 carchive-0.0.41/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 02:21:39.000000 carchive-0.0.41/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 02:21:39.000000 carchive-0.0.41/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:21:39.545486 carchive-0.0.41/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3386 2023-05-05 02:21:35.000000 carchive-0.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:59.197385 carchive-0.0.42/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 02:22:53.000000 carchive-0.0.42/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:22:59.197385 carchive-0.0.42/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 02:22:53.000000 carchive-0.0.42/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:59.197385 carchive-0.0.42/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9130 2023-05-05 02:22:53.000000 carchive-0.0.42/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:59.197385 carchive-0.0.42/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:22:59.000000 carchive-0.0.42/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 02:22:59.000000 carchive-0.0.42/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:22:59.000000 carchive-0.0.42/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 02:22:59.000000 carchive-0.0.42/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 02:22:59.000000 carchive-0.0.42/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:22:59.197385 carchive-0.0.42/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3385 2023-05-05 02:22:53.000000 carchive-0.0.42/setup.py
```

### Comparing `carchive-0.0.41/LICENSE` & `carchive-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.41/carchive/__init__.py` & `carchive-0.0.42/carchive/__init__.py`

 * *Files identical despite different names*

### Comparing `carchive-0.0.41/setup.py` & `carchive-0.0.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.41"
+VERSION = "0.0.42"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -103,15 +103,15 @@
 	packages=find_packages(
 		exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 	entry_points={
 	},
 	install_requires=[
 		"PyGithub", 
 		#"git2net @ git+ssh://git@github.com/franceme/git2net/tarball/master@0ca0ce7db9c3a616096a250c9412a8780dd30768",
-		"git2net@git+http://@github.com/franceme/git2net"
+		"git2net@git+http://github.com/franceme/git2net"
 		"splittr",
 		"waybackpy",
 		"mystring",
 		"pygit2",
 	],
 	include_package_data=True,
 	classifiers=[
```

