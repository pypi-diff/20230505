# Comparing `tmp/carchive-0.0.44.tar.gz` & `tmp/carchive-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.44.tar", last modified: Fri May  5 02:51:20 2023, max compression
+gzip compressed data, was "carchive-0.0.45.tar", last modified: Fri May  5 02:56:07 2023, max compression
```

## Comparing `carchive-0.0.44.tar` & `carchive-0.0.45.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:51:20.943880 carchive-0.0.44/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 02:51:16.000000 carchive-0.0.44/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:51:20.943880 carchive-0.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 02:51:16.000000 carchive-0.0.44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:51:20.943880 carchive-0.0.44/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9270 2023-05-05 02:51:16.000000 carchive-0.0.44/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:51:20.943880 carchive-0.0.44/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:51:20.943880 carchive-0.0.44/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3386 2023-05-05 02:51:16.000000 carchive-0.0.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:56:07.211802 carchive-0.0.45/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 02:56:01.000000 carchive-0.0.45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:56:07.211802 carchive-0.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 02:56:01.000000 carchive-0.0.45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:56:07.211802 carchive-0.0.45/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9255 2023-05-05 02:56:01.000000 carchive-0.0.45/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:56:07.211802 carchive-0.0.45/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:56:07.211802 carchive-0.0.45/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3386 2023-05-05 02:56:01.000000 carchive-0.0.45/setup.py
```

### Comparing `carchive-0.0.44/LICENSE` & `carchive-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.44/carchive/__init__.py` & `carchive-0.0.45/carchive/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	def __init__(self):
 		self.cur_status = None
 		self.now = None
 
 	@property
 	def status(self):
 		# curl -I https://api.github.com/users/octocat|grep x-ratelimit-reset
-		self.cur_status, self.now = requests.get("https://api.github.com/users/octocat").json()['data'].headers, datetime.datetime.now()
+		self.cur_status, self.now = requests.get("https://api.github.com/users/octocat").headers, datetime.datetime.now()
 		return {
 			'Reset': self.cur_status['X-RateLimit-Reset'],
 			'Used': self.cur_status['X-RateLimit-Used'],
 			'Total': self.cur_status['X-RateLimit-Limit'],
 			'Remaining': self.cur_status['X-RateLimit-Remaining'],
 			'RemainingDate':datetime.datetime.fromtimestamp(int(self.cur_status['X-RateLimit-Reset'])),
 			'WaitFor':datetime.datetime.fromtimestamp(int(self.cur_status['X-RateLimit-Reset'])) - self.now,
```

### Comparing `carchive-0.0.44/setup.py` & `carchive-0.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.44"
+VERSION = "0.0.45"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

