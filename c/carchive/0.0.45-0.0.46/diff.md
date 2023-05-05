# Comparing `tmp/carchive-0.0.45.tar.gz` & `tmp/carchive-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.45.tar", last modified: Fri May  5 02:56:07 2023, max compression
+gzip compressed data, was "carchive-0.0.46.tar", last modified: Fri May  5 03:20:43 2023, max compression
```

## Comparing `carchive-0.0.45.tar` & `carchive-0.0.46.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:56:07.211802 carchive-0.0.45/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 02:56:01.000000 carchive-0.0.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:56:07.211802 carchive-0.0.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 02:56:01.000000 carchive-0.0.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:56:07.211802 carchive-0.0.45/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9255 2023-05-05 02:56:01.000000 carchive-0.0.45/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:56:07.211802 carchive-0.0.45/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 02:56:07.000000 carchive-0.0.45/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:56:07.211802 carchive-0.0.45/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3386 2023-05-05 02:56:01.000000 carchive-0.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:20:43.786563 carchive-0.0.46/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 03:20:39.000000 carchive-0.0.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 03:20:43.786563 carchive-0.0.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 03:20:39.000000 carchive-0.0.46/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:20:43.786563 carchive-0.0.46/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9615 2023-05-05 03:20:39.000000 carchive-0.0.46/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:20:43.786563 carchive-0.0.46/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:20:43.786563 carchive-0.0.46/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-05 03:20:39.000000 carchive-0.0.46/setup.py
```

### Comparing `carchive-0.0.45/LICENSE` & `carchive-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.45/carchive/__init__.py` & `carchive-0.0.46/carchive/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os, requests, datetime, time, queue, threading
 from copy import deepcopy as dc
 from threading import Lock
 from typing import Dict, List, Callable, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 import mystring,splittr
-
+import pause
 from github import Github, Repository
 import git2net
 import pygit2 as git2
 
 class niceghapi(object):
 	def __init__(self):
 		self.cur_status = None
 		self.now = None
+		self.resetdate = None
 
 	@property
 	def status(self):
 		# curl -I https://api.github.com/users/octocat|grep x-ratelimit-reset
 		self.cur_status, self.now = requests.get("https://api.github.com/users/octocat").headers, datetime.datetime.now()
 		return {
 			'Reset': self.cur_status['X-RateLimit-Reset'],
@@ -34,22 +35,21 @@
 	def timing(self):
 		import time
 		if not hasattr(self, 'remaining') or self.remaining is None:
 			stats = self.status
 			print(stats)
 			self.remaining = int(stats['Remaining'])
 			self.wait_until = stats['WaitForNow']
+			self.resetdate = stats['RemainingDate']
 			self.timing
 		elif self.remaining >= 10:
 			self.remaining = self.remaining - 1
 		else:
-			time_to_sleep = self.wait_until
-			for itr in range(time_to_sleep):
-				print("{}/{}".format(itr,time_to_sleep))
-				time.sleep(1)
+			print("Waiting until: {0}".format(self.resetdate))
+			pause.until(self.resetdate)
 			delattr(self, 'remaining')
 			delattr(self, 'wait_until')
 		return
 
 class githuburl(object):
 	def __init__(self,url,token=None,verify=True,commit=None,tag=None):
 		self.url = mystring.string(dc(url))
@@ -209,17 +209,28 @@
 		self.total_repo_len = None
 
 		def appr(string: mystring.string):
 			with open("mapping_file_{0}.csv".format(string.tobase64()), "a+") as writer:
 				writer.write(string)
 		self.appr = appr
 		self.api_watch = niceghapi()
+	
+	@property
+	def timing(self):
+		self.api_watch.timing
+
+		extra_rate_limiting = self.g.get_rate_limit()
+		if hasattr(extra_rate_limiting, "search"):
+			search_limits = getattr(extra_rate_limiting, "search")
+			if search_limits.remaining < 2:
+				print("Waiting until: {0}".format(search_limits.reset))
+				pause.until(search_limits.reset)
 
 	def __call__(self, search_string:str):
-		self.api_watch.timing
+		self.timing
 		search_string = mystring.string(search_string)
 
 		def process_prep(repo_itr:int, repo:Repository, search_string:str, appr:Callable, fin_queue:queue.Queue):
 			def process():
 				name = mystring.string("ITR:{0}_URL:{1}_STR:{2}\n".format(
 					repo_itr, repo.url, search_string
 				))
```

### Comparing `carchive-0.0.45/setup.py` & `carchive-0.0.46/setup.py`

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
-VERSION = "0.0.45"
+VERSION = "0.0.46"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -108,14 +108,15 @@
 		"PyGithub", 
 		#"git2net @ git+ssh://git@github.com/franceme/git2net/tarball/master@0ca0ce7db9c3a616096a250c9412a8780dd30768",
 		"git2net@git+http://github.com/franceme/git2net",
 		"splittr",
 		"waybackpy",
 		"mystring",
 		"pygit2",
+		"pause",
 	],
 	include_package_data=True,
 	classifiers=[
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.8',
 	],
```

