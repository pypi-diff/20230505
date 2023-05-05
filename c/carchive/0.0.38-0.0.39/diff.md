# Comparing `tmp/carchive-0.0.38.tar.gz` & `tmp/carchive-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.38.tar", last modified: Thu May  4 15:47:14 2023, max compression
+gzip compressed data, was "carchive-0.0.39.tar", last modified: Fri May  5 01:25:23 2023, max compression
```

## Comparing `carchive-0.0.38.tar` & `carchive-0.0.39.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:47:14.963598 carchive-0.0.38/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 15:47:10.000000 carchive-0.0.38/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 15:47:14.963598 carchive-0.0.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 15:47:10.000000 carchive-0.0.38/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:47:14.959597 carchive-0.0.38/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9118 2023-05-04 15:47:10.000000 carchive-0.0.38/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:47:14.963598 carchive-0.0.38/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:47:14.963598 carchive-0.0.38/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3593 2023-05-04 15:47:10.000000 carchive-0.0.38/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.406494 carchive-0.0.39/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 01:25:18.000000 carchive-0.0.39/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 01:25:23.406494 carchive-0.0.39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 01:25:18.000000 carchive-0.0.39/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.402494 carchive-0.0.39/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9130 2023-05-05 01:25:18.000000 carchive-0.0.39/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.406494 carchive-0.0.39/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 01:25:23.000000 carchive-0.0.39/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:25:23.406494 carchive-0.0.39/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3593 2023-05-05 01:25:18.000000 carchive-0.0.39/setup.py
```

### Comparing `carchive-0.0.38/LICENSE` & `carchive-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.38/carchive/__init__.py` & `carchive-0.0.39/carchive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,19 +176,19 @@
 	@property
 	def webarchive_save_url(self,):
 		return mystring.string("https://web.archive.org/save/" + self.zip_url)
 
 T = TypeVar('T')
 class GRepo_Seed_Metric(ABC, Generic[T]):
 	@abstractmethod
-	def metric(filename: str, source_code: str) -> Dict[str, T]:
+	def metric(self, filename: str, source_code: str) -> Dict[str, T]:
 		pass
 
 	@abstractmethod
-	def diff(latest: T, previous: T):
+	def diff(self, latest: T, previous: T):
 		pass
 
 	def __call__(self):
 		setattr(self.metric, 'diff', self.diff)
 		return self.metric
```

### Comparing `carchive-0.0.38/setup.py` & `carchive-0.0.39/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.38"
+VERSION = "0.0.39"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

