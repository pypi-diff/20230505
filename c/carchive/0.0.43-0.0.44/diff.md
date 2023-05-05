# Comparing `tmp/carchive-0.0.43.tar.gz` & `tmp/carchive-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.43.tar", last modified: Fri May  5 02:41:31 2023, max compression
+gzip compressed data, was "carchive-0.0.44.tar", last modified: Fri May  5 02:51:20 2023, max compression
```

## Comparing `carchive-0.0.43.tar` & `carchive-0.0.44.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:41:31.208342 carchive-0.0.43/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 02:41:25.000000 carchive-0.0.43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:41:31.208342 carchive-0.0.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 02:41:25.000000 carchive-0.0.43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:41:31.208342 carchive-0.0.43/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9130 2023-05-05 02:41:25.000000 carchive-0.0.43/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:41:31.208342 carchive-0.0.43/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:41:31.000000 carchive-0.0.43/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 02:41:31.000000 carchive-0.0.43/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:41:31.000000 carchive-0.0.43/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 02:41:31.000000 carchive-0.0.43/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 02:41:31.000000 carchive-0.0.43/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:41:31.208342 carchive-0.0.43/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3386 2023-05-05 02:41:25.000000 carchive-0.0.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:51:20.943880 carchive-0.0.44/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 02:51:16.000000 carchive-0.0.44/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:51:20.943880 carchive-0.0.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 02:51:16.000000 carchive-0.0.44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:51:20.943880 carchive-0.0.44/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9270 2023-05-05 02:51:16.000000 carchive-0.0.44/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:51:20.943880 carchive-0.0.44/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 02:51:20.000000 carchive-0.0.44/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:51:20.943880 carchive-0.0.44/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3386 2023-05-05 02:51:16.000000 carchive-0.0.44/setup.py
```

### Comparing `carchive-0.0.43/LICENSE` & `carchive-0.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.43/carchive/__init__.py` & `carchive-0.0.44/carchive/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	def timing(self):
 		import time
 		if not hasattr(self, 'remaining') or self.remaining is None:
 			stats = self.status
 			print(stats)
 			self.remaining = int(stats['Remaining'])
 			self.wait_until = stats['WaitForNow']
+			self.timing
 		elif self.remaining >= 10:
 			self.remaining = self.remaining - 1
 		else:
 			time_to_sleep = self.wait_until
 			for itr in range(time_to_sleep):
 				print("{}/{}".format(itr,time_to_sleep))
 				time.sleep(1)
@@ -207,16 +208,18 @@
 		self.current_repo_itr = None
 		self.total_repo_len = None
 
 		def appr(string: mystring.string):
 			with open("mapping_file_{0}.csv".format(string.tobase64()), "a+") as writer:
 				writer.write(string)
 		self.appr = appr
+		self.api_watch = niceghapi()
 
 	def __call__(self, search_string:str):
+		self.api_watch.timing
 		search_string = mystring.string(search_string)
 
 		def process_prep(repo_itr:int, repo:Repository, search_string:str, appr:Callable, fin_queue:queue.Queue):
 			def process():
 				name = mystring.string("ITR:{0}_URL:{1}_STR:{2}\n".format(
 					repo_itr, repo.url, search_string
 				))
@@ -240,18 +243,21 @@
 
 				appr(name)
 				fin_queue.put(repo)
 
 			return process
 
 		repos = self.g.search_repositories(query=search_string)
-		self.total_repo_len = len(repos) - 1
-		for repo_itr, repo in enumerate(repos):
-			self.processor += process_prep(repo_itr, repo, search_string, self.appr, self.processed_paths)
-			self.current_repo_itr = repo_itr
+		self.total_repo_len = repos.totalCount
+		if self.total_repo_len > 0:
+			for repo_itr, repo in enumerate(repos):
+				self.processor += process_prep(repo_itr, repo, search_string, self.appr, self.processed_paths)
+				self.current_repo_itr = repo_itr
+		else:
+			print("No Repos Found")
 
 	def login(self):
 		os.environ['GH_TOKEN'] = self.token
 		try:
 			with open("~/.bashrc", "a+") as writer:
 				writer.write("GH_TOKEN={0}".format(self.token))
 		except:
```

### Comparing `carchive-0.0.43/setup.py` & `carchive-0.0.44/setup.py`

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
-VERSION = "0.0.43"
+VERSION = "0.0.44"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

