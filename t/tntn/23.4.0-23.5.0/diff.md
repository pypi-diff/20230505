# Comparing `tmp/tntn-23.4.0.tar.gz` & `tmp/tntn-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tntn-23.4.0.tar", last modified: Mon Apr  3 07:01:48 2023, max compression
+gzip compressed data, was "tntn-23.5.0.tar", last modified: Fri May  5 10:11:28 2023, max compression
```

## Comparing `tntn-23.4.0.tar` & `tntn-23.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-04-03 04:56:00.576377 tntn-23.4.0/LICENSE.md
--rw-r--r--   0        0        0      989 2023-04-03 06:51:02.469114 tntn-23.4.0/pyproject.toml
--rw-r--r--   0        0        0     1302 2023-04-03 06:57:39.942299 tntn-23.4.0/README.md
--rw-r--r--   0        0        0      171 2023-04-03 06:25:30.548879 tntn-23.4.0/tntn/__init__.py
--rw-r--r--   0        0        0      838 2023-04-03 05:55:13.167892 tntn-23.4.0/tntn/__main__.py
--rw-r--r--   0        0        0       24 2023-04-03 06:58:33.888253 tntn-23.4.0/tntn/__version__.py
--rw-r--r--   0        0        0     3243 2023-04-03 06:42:45.600696 tntn-23.4.0/tntn/tntn.py
--rw-r--r--   0        0        0     2546 2023-04-03 05:43:39.706245 tntn-23.4.0/tntn/urls.toml
--rw-r--r--   0        0        0     2676 2023-04-03 06:25:54.206035 tntn-23.4.0/tntn/util.py
--rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 tntn-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-03 04:56:00.576377 tntn-23.5.0/LICENSE.md
+-rw-r--r--   0        0        0      989 2023-04-03 06:51:02.469114 tntn-23.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1302 2023-04-03 06:57:39.942299 tntn-23.5.0/README.md
+-rw-r--r--   0        0        0      171 2023-04-03 06:25:30.548879 tntn-23.5.0/tntn/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-03 05:55:13.167892 tntn-23.5.0/tntn/__main__.py
+-rw-r--r--   0        0        0       24 2023-05-05 10:08:51.864937 tntn-23.5.0/tntn/__version__.py
+-rw-r--r--   0        0        0     3619 2023-05-05 10:08:00.232931 tntn-23.5.0/tntn/tntn.py
+-rw-r--r--   0        0        0     2546 2023-04-03 05:43:39.706245 tntn-23.5.0/tntn/urls.toml
+-rw-r--r--   0        0        0     2676 2023-04-03 06:25:54.206035 tntn-23.5.0/tntn/util.py
+-rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 tntn-23.5.0/PKG-INFO
```

### Comparing `tntn-23.4.0/LICENSE.md` & `tntn-23.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tntn-23.4.0/pyproject.toml` & `tntn-23.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dependencies = [
     "tomli; python_version < '3.11'",
     "tqdm",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 dynamic = []
-version = "23.4.0"
+version = "23.5.0"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 tntn = "tntn.__main__:main"
```

### Comparing `tntn-23.4.0/README.md` & `tntn-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tntn-23.4.0/tntn/__main__.py` & `tntn-23.5.0/tntn/__main__.py`

 * *Files identical despite different names*

### Comparing `tntn-23.4.0/tntn/tntn.py` & `tntn-23.5.0/tntn/tntn.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,33 +7,38 @@
 from pathlib import Path
 from typing import NamedTuple
 
 from .util import download, get_info
 
 pattern = {
     "jprq": r"(?P<url>https?://\S+\.jprq\.live)",
-    "bore": r"(?P<url>bore\.pub:\d+)",
+    "bore": r"(?P<url>[^/ ]+\.\w+:\d+)",
 }
 
-argv = {"jprq": "http {port}", "bore": "local {port} --to bore.pub"}
+argv = {"jprq": "http {port}", "bore": "local {port}"}
 lines = {"jprq": 5, "bore": 2}
 
 
 class Urls(NamedTuple):
     tunnel: str
     process: subprocess.Popen
 
 
 class Tunnel:
     def __init__(self, app: str = "bore"):
         self.app = app.lower()
         self.running: dict[int, Urls] = {}
 
     def __call__(
-        self, port: int, token: str | None = None, verbose: bool = True
+        self,
+        port: int,
+        token: str | None = None,
+        verbose: bool = True,
+        bore_url: str = "bore.pub",
+        bore_port: int | None = None,
     ) -> Urls:
         if port in self.running:
             if verbose:
                 self._print(self.running[port].tunnel)
             return self.running[port]
 
         info = get_info(self.app)
@@ -42,17 +47,25 @@
 
         # if jprq, token is required
         if self.app == "jprq":
             if not token:
                 raise ValueError("jprq requires token")
 
             # always success even if given invalid token, so no need to 'check=True'
-            subprocess.run([info.executable, "auth", token])
+            subprocess.run(
+                [info.executable, "auth", token],
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+            )
 
         args = shlex.split(argv[self.app].format(port=port))
+        if self.app == "bore":
+            args += ["--to", bore_url]
+            if bore_port is not None:
+                args += ["--port", str(bore_port)]
         args = [info.executable, *args]
 
         process = subprocess.Popen(
             args, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding="utf-8"
         )
 
         atexit.register(process.terminate)
```

### Comparing `tntn-23.4.0/tntn/urls.toml` & `tntn-23.5.0/tntn/urls.toml`

 * *Files identical despite different names*

### Comparing `tntn-23.4.0/tntn/util.py` & `tntn-23.5.0/tntn/util.py`

 * *Files identical despite different names*

### Comparing `tntn-23.4.0/PKG-INFO` & `tntn-23.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tntn
-Version: 23.4.0
+Version: 23.5.0
 Summary: Python wrapper library for tunneling apps
 License: MIT
 Author-email: dowon <ks2515@naver.com>
 Requires-Python: >=3.7
 Project-URL: repository, https://github.com/Bing-su/tntn
 Description-Content-Type: text/markdown
```

