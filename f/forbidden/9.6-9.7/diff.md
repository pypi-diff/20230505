# Comparing `tmp/forbidden-9.6.tar.gz` & `tmp/forbidden-9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forbidden-9.6.tar", last modified: Thu May  4 11:15:56 2023, max compression
+gzip compressed data, was "forbidden-9.7.tar", last modified: Fri May  5 18:17:53 2023, max compression
```

## Comparing `forbidden-9.6.tar` & `forbidden-9.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:41:20.000000 forbidden-9.6/LICENSE
--rwxrwx---   0 root         (0) root         (0)      112 2023-04-28 13:41:20.000000 forbidden-9.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12639 2023-05-04 11:15:56.241732 forbidden-9.6/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)    12688 2023-05-04 09:58:59.000000 forbidden-9.6/README.md
--rwxrwx---   0 root         (0) root         (0)      833 2023-05-04 11:05:25.000000 forbidden-9.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 11:15:56.241732 forbidden-9.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/src/forbidden/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.6/src/forbidden/__init__.py
--rwxrwx---   0 root         (0) root         (0)    44751 2023-05-04 09:55:00.000000 forbidden-9.6/src/forbidden/forbidden.py
--rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.6/src/forbidden/user_agents.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/src/forbidden.egg-info/
--rwxrwx---   0 root         (0) root         (0)    12639 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)      430 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) root         (0)        1 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) root         (0)       89 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/entry_points.txt
--rwxrwx---   0 root         (0) root         (0)       79 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/requires.txt
--rwxrwx---   0 root         (0) root         (0)       19 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/src/stresser/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.6/src/stresser/__init__.py
--rwxrwx---   0 root         (0) root         (0)    19834 2023-05-04 09:56:11.000000 forbidden-9.6/src/stresser/stresser.py
--rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.6/src/stresser/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:17:53.250492 forbidden-9.7/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:41:20.000000 forbidden-9.7/LICENSE
+-rwxrwx---   0 root         (0) root         (0)      112 2023-04-28 13:41:20.000000 forbidden-9.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12795 2023-05-05 18:17:53.250492 forbidden-9.7/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)    12833 2023-05-05 18:17:29.000000 forbidden-9.7/README.md
+-rwxrwx---   0 root         (0) root         (0)      850 2023-05-05 17:25:05.000000 forbidden-9.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 18:17:53.250492 forbidden-9.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:17:53.250492 forbidden-9.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:17:53.250492 forbidden-9.7/src/forbidden/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.7/src/forbidden/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    45801 2023-05-05 18:17:15.000000 forbidden-9.7/src/forbidden/forbidden.py
+-rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.7/src/forbidden/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:17:53.250492 forbidden-9.7/src/forbidden.egg-info/
+-rwxrwx---   0 root         (0) root         (0)    12795 2023-05-05 18:17:53.000000 forbidden-9.7/src/forbidden.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)      430 2023-05-05 18:17:53.000000 forbidden-9.7/src/forbidden.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) root         (0)        1 2023-05-05 18:17:53.000000 forbidden-9.7/src/forbidden.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) root         (0)       89 2023-05-05 18:17:53.000000 forbidden-9.7/src/forbidden.egg-info/entry_points.txt
+-rwxrwx---   0 root         (0) root         (0)       79 2023-05-05 18:17:53.000000 forbidden-9.7/src/forbidden.egg-info/requires.txt
+-rwxrwx---   0 root         (0) root         (0)       19 2023-05-05 18:17:53.000000 forbidden-9.7/src/forbidden.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:17:53.250492 forbidden-9.7/src/stresser/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.7/src/stresser/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    19834 2023-05-05 17:26:56.000000 forbidden-9.7/src/stresser/stresser.py
+-rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.7/src/stresser/user_agents.txt
```

### Comparing `forbidden-9.6/LICENSE` & `forbidden-9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `forbidden-9.6/PKG-INFO` & `forbidden-9.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: forbidden
-Version: 9.6
-Summary: Bypass 4xx HTTP response status codes and more.
+Version: 9.7
+Summary: Bypass 4xx HTTP response status codes and more. Based on PycURL.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -113,15 +113,15 @@
 
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-9.6-py3-none-any.whl
+python3 -m pip install dist/forbidden-9.7-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -350,39 +350,39 @@
       "id":"570-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1"
       ],
       "body":null,
-      "agent":"Forbidden/9.6",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.7",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.7' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    },
    {
       "id":"571-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1:443"
       ],
       "body":null,
-      "agent":"Forbidden/9.6",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.7",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.7' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v9.6 ( github.com/ivan-sincek/forbidden )
+Forbidden v9.7 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -408,43 +408,49 @@
     -p <path> - /home/index.html | /README.txt | etc.
 EVIL
     Specify (strictly) evil domain name with no port to test URL overrides
     Scope: headers | redirects
     Default: github.com
     -e <evil> - xyz.interact.sh | xyz.burpcollaborator.net | etc.
 IGNORE
-    Filter out 200 OK false positive results by RegEx
-    Spacing will be stripped
+    Filter out 200 OK false positive results with a regual expression
     -i <ignore> - Forbidden | "Access Denied" | etc.
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Specify 'path' to ignore content length of accessible URL response
     Use comma separated values
     -l <lengths> - 12 | base | path | etc.
 THREADS
     Number of parallel threads to run
     More threads make it quicker but can give worse results
-    Heavily depends on network bandwidth and server capacity
+    Depends heavily on network bandwidth and server capacity
     Default: 5
     -th <threads> - 200 | etc.
+SLEEP
+    Sleep while queuing each request
+    Intended for a single thread use
+    -s <sleep> - 5 | etc.
 AGENT
     User agent to use
-    Default: Forbidden/9.6
+    Default: Forbidden/9.7
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
+DEBUG
+    Debug output
+    -dbg <debug> - yes
 ```
 
 ```fundamental
-Stresser v4.6 ( github.com/ivan-sincek/forbidden )
+Stresser v9.7 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -471,15 +477,15 @@
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Use comma separated values
     -l <lengths> - 12 | base | etc.
 AGENT
     User agent to use
-    Default: Stresser/4.6
+    Default: Stresser/9.7
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
```

### Comparing `forbidden-9.6/README.md` & `forbidden-9.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-9.6-py3-none-any.whl
+python3 -m pip install dist/forbidden-9.7-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -337,39 +337,39 @@
       "id":"570-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1"
       ],
       "body":null,
-      "agent":"Forbidden/9.6",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.7",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.7' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    },
    {
       "id":"571-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1:443"
       ],
       "body":null,
-      "agent":"Forbidden/9.6",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.7",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.7' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v9.6 ( github.com/ivan-sincek/forbidden )
+Forbidden v9.7 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -395,43 +395,49 @@
     -p <path> - /home/index.html | /README.txt | etc.
 EVIL
     Specify (strictly) evil domain name with no port to test URL overrides
     Scope: headers | redirects
     Default: github.com
     -e <evil> - xyz.interact.sh | xyz.burpcollaborator.net | etc.
 IGNORE
-    Filter out 200 OK false positive results by RegEx
-    Spacing will be stripped
+    Filter out 200 OK false positive results with a regual expression
     -i <ignore> - Forbidden | "Access Denied" | etc.
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Specify 'path' to ignore content length of accessible URL response
     Use comma separated values
     -l <lengths> - 12 | base | path | etc.
 THREADS
     Number of parallel threads to run
     More threads make it quicker but can give worse results
-    Heavily depends on network bandwidth and server capacity
+    Depends heavily on network bandwidth and server capacity
     Default: 5
     -th <threads> - 200 | etc.
+SLEEP
+    Sleep while queuing each request
+    Intended for a single thread use
+    -s <sleep> - 5 | etc.
 AGENT
     User agent to use
-    Default: Forbidden/9.6
+    Default: Forbidden/9.7
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
+DEBUG
+    Debug output
+    -dbg <debug> - yes
 ```
 
 ```fundamental
-Stresser v4.6 ( github.com/ivan-sincek/forbidden )
+Stresser v9.7 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -458,15 +464,15 @@
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Use comma separated values
     -l <lengths> - 12 | base | etc.
 AGENT
     User agent to use
-    Default: Stresser/4.6
+    Default: Stresser/9.7
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
```

### Comparing `forbidden-9.6/pyproject.toml` & `forbidden-9.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "forbidden"
-version = "9.6"
+version = "9.7"
 authors = [{ name = "Ivan Sincek" }]
-description = "Bypass 4xx HTTP response status codes and more."
+description = "Bypass 4xx HTTP response status codes and more. Based on PycURL."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent"
 ]
```

### Comparing `forbidden-9.6/src/forbidden/forbidden.py` & `forbidden-9.7/src/forbidden/forbidden.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import random
 import socket
 import base64
 import concurrent.futures
 import subprocess
 import io
 import requests
+import time
 import pycurl
 import termcolor
 import colorama
 import json
 
 start = datetime.datetime.now()
 
@@ -24,15 +25,15 @@
 colorama.init(autoreset = True)
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Forbidden v9.6 ( github.com/ivan-sincek/forbidden )")
+	print("Forbidden v9.7 ( github.com/ivan-sincek/forbidden )")
 	print("")
 	print("Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]")
 	print("Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]")
 
 def advanced():
 	basic()
 	print("")
@@ -61,39 +62,45 @@
 	print("    -p <path> - /home/index.html | /README.txt | etc.")
 	print("EVIL")
 	print("    Specify (strictly) evil domain name with no port to test URL overrides")
 	print("    Scope: headers | redirects")
 	print("    Default: github.com")
 	print("    -e <evil> - xyz.interact.sh | xyz.burpcollaborator.net | etc.")
 	print("IGNORE")
-	print("    Filter out 200 OK false positive results by RegEx")
-	print("    Spacing will be stripped")
+	print("    Filter out 200 OK false positive results with a regual expression")
 	print("    -i <ignore> - Forbidden | \"Access Denied\" | etc.")
 	print("LENGTHS")
 	print("    Filter out 200 OK false positive results by content lengths")
 	print("    Specify 'base' to ignore content length of base HTTP response")
 	print("    Specify 'path' to ignore content length of accessible URL response")
 	print("    Use comma separated values")
 	print("    -l <lengths> - 12 | base | path | etc.")
 	print("THREADS")
 	print("    Number of parallel threads to run")
 	print("    More threads make it quicker but can give worse results")
-	print("    Heavily depends on network bandwidth and server capacity")
+	print("    Depends heavily on network bandwidth and server capacity")
 	print("    Default: 5")
 	print("    -th <threads> - 200 | etc.")
+	print("SLEEP")
+	print("    Sleep while queuing each request")
+	print("    Intended for a single thread use")
+	print("    -s <sleep> - 5 | etc.")
 	print("AGENT")
 	print("    User agent to use")
-	print("    Default: Forbidden/9.6")
+	print("    Default: Forbidden/9.7")
 	print("    -a <agent> - curl/3.30.1 | random[-all] | etc.")
 	print("PROXY")
 	print("    Web proxy to use")
 	print("    -x <proxy> - 127.0.0.1:8080 | etc.")
 	print("OUT")
 	print("    Output file")
 	print("    -o <out> - results.json | etc.")
+	print("DEBUG")
+	print("    Debug output")
+	print("    -dbg <debug> - yes")
 
 # ------------------- MISCELENIOUS BEGIN -------------------
 
 def unique(sequence):
 	seen = set()
 	return [x for x in sequence if not (x in seen or seen.add(x))]
 
@@ -371,15 +378,15 @@
 def error(msg, help = False):
 	global proceed
 	proceed = False
 	print_error(msg)
 	if help:
 		print("Use -h for basic and --help for advanced info")
 
-args = {"url": None, "tests": None, "force": None, "values": None, "path": None, "evil": None, "ignore": None, "lengths": None, "threads": None, "agent": None, "proxy": None, "out": None}
+args = {"url": None, "tests": None, "force": None, "values": None, "path": None, "evil": None, "ignore": None, "lengths": None, "threads": None, "sleep": None, "agent": None, "proxy": None, "out": None, "debug": None}
 
 # TO DO: Better URL validation. Validate "evil" and "proxy" URLs.
 def validate(key, value):
 	global args
 	value = value.strip()
 	if len(value) > 0:
 		if key == "-u" and args["url"] is None:
@@ -424,25 +431,37 @@
 			args["threads"] = value
 			if not args["threads"].isdigit():
 				error("Number of parallel threads to run must be numeric")
 			else:
 				args["threads"] = int(args["threads"])
 				if args["threads"] < 1:
 					error("Number of parallel threads to run must be greater than zero")
+		elif key == "-s" and args["sleep"] is None:
+			args["sleep"] = value
+			if not args["sleep"].isdigit():
+				error("Sleep must be numeric")
+			else:
+				args["sleep"] = int(args["sleep"])
+				if args["sleep"] < 1:
+					error("Sleep must be greater than zero")
 		elif key == "-a" and args["agent"] is None:
 			args["agent"] = value
 			if args["agent"].lower() in ["random", "random-all"]:
 				file = os.path.join(os.path.abspath(os.path.split(__file__)[0]), "user_agents.txt")
 				if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
 					array = read_file(file)
 					args["agent"] = array[random.randint(0, len(array) - 1)] if args["agent"].lower() == "random" else array
 		elif key == "-x" and args["proxy"] is None:
 			args["proxy"] = value
 		elif key == "-o" and args["out"] is None:
 			args["out"] = value
+		elif key == "-dbg" and args["debug"] is None:
+			args["debug"] = value.lower()
+			if args["debug"] != "yes":
+				error("Specify 'yes' to enable debug output")
 
 def check(argc, args):
 	count = 0
 	for key in args:
 		if args[key] is not None:
 			count += 1
 	return argc - count == argc / 2
@@ -1038,15 +1057,17 @@
 
 def get_timestamp(text):
 	return print(("{0} - {1}").format(datetime.datetime.now().strftime("%H:%M:%S"), text))
 
 def progress(count, total):
 	print(("Progress: {0}/{1} | {2:.2f}%").format(count, total, (count / total) * 100), end = "\n" if count == total else "\r")
 
-def send_request(record):
+def send_request(record, sleep = None, debug = None):
+	if sleep:
+		time.sleep(sleep)
 	encoding = "UTF-8"
 	if record["body"]:
 		record["body"].encode(encoding)
 	headers = {}
 	if record["headers"]:
 		for header in record["headers"]:
 			array = header.split(": ", 1)
@@ -1065,23 +1086,26 @@
 		prepared = request.prepare()
 		prepared.url = record["url"]
 		response = session.send(prepared, proxies = proxies, timeout = (90, 180), verify = False, allow_redirects = True)
 		record["code"] = response.status_code
 		record["length"] = len(response.content)
 		if record["ignore"] and (record["ignore"]["text"] and re.search(record["ignore"]["text"], response.content.decode("ISO-8859-1"), re.MULTILINE | re.IGNORECASE) or record["ignore"]["lengths"] and any(record["length"] == length for length in record["ignore"]["lengths"])):
 			record["code"] = 0
-	except (requests.packages.urllib3.exceptions.LocationParseError, requests.exceptions.RequestException):
-		pass
+	except (requests.packages.urllib3.exceptions.LocationParseError, requests.exceptions.RequestException) as ex:
+		if debug:
+			print_error(("{0}\n{1}").format(ex, record["command"]))
 	finally:
 		if response is not None:
 			response.close()
 		session.close()
 	return record
 
-def send_curl(record):
+def send_curl(record, sleep = None, debug = None):
+	if sleep:
+		time.sleep(sleep)
 	encoding = "UTF-8"
 	response = io.BytesIO()
 	curl = pycurl.Curl()
 	curl.setopt(pycurl.CONNECTTIMEOUT, 90)
 	curl.setopt(pycurl.TIMEOUT, 180)
 	curl.setopt(pycurl.VERBOSE, False)
 	curl.setopt(pycurl.SSL_VERIFYPEER, False)
@@ -1102,16 +1126,17 @@
 	curl.setopt(pycurl.WRITEDATA, response)
 	try:
 		curl.perform()
 		record["code"] = int(curl.getinfo(pycurl.RESPONSE_CODE))
 		record["length"] = int(curl.getinfo(pycurl.SIZE_DOWNLOAD))
 		if record["ignore"] and (record["ignore"]["text"] and re.search(record["ignore"]["text"], response.getvalue().decode("ISO-8859-1"), re.MULTILINE | re.IGNORECASE) or record["ignore"]["lengths"] and any(record["length"] == length for length in record["ignore"]["lengths"])):
 			record["code"] = 0
-	except pycurl.error:
-		pass
+	except pycurl.error as ex:
+		if debug:
+			print_error(("{0}\n{1}").format(ex, record["command"]))
 	finally:
 		response.close()
 		curl.close()
 	return record
 
 def remove(array, keys):
 	for entry in array:
@@ -1182,23 +1207,25 @@
 			# continue
 			tmp.append(output(record, "green"))
 	# --------------------
 	display_table(table)
 	# --------------------
 	return tmp
 
-def bypass(collection, threads = 10):
+def bypass(collection, threads = 10, sleep = None, debug = None):
 	results = []
 	count = 0
 	total = len(collection)
 	print(("Number of created test records: {0}").format(total))
 	get_timestamp("Running tests...")
 	progress(count, total)
 	with concurrent.futures.ThreadPoolExecutor(max_workers = threads) as executor:
-		subprocesses = {executor.submit(send_curl if record["curl"] else send_request, record): record for record in collection}
+		subprocesses = []
+		for record in collection:
+			subprocesses.append(executor.submit(send_curl if record["curl"] else send_request, record, sleep, debug))
 		for subprocess in concurrent.futures.as_completed(subprocesses):
 			results.append(subprocess.result())
 			count += 1
 			progress(count, total)
 	return results
 
 def main():
@@ -1213,22 +1240,22 @@
 			advanced()
 		else:
 			error("Incorrect usage", True)
 	elif argc % 2 == 0 and argc <= len(args) * 2:
 		for i in range(1, argc, 2):
 			validate(sys.argv[i], sys.argv[i + 1])
 		if args["url"] is None or args["tests"] is None or not check(argc, args):
-			error("Missing a mandatory option (-u, -t) and/or optional (-f, -v, -p, -e, -i, -l, -th, -a, -x, -o)", True)
+			error("Missing a mandatory option (-u, -t) and/or optional (-f, -v, -p, -e, -i, -l, -th, -s, -a, -x, -o, -dbg)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed:
 		print("##########################################################################")
 		print("#                                                                        #")
-		print("#                             Forbidden v9.6                             #")
+		print("#                             Forbidden v9.7                             #")
 		print("#                                  by Ivan Sincek                        #")
 		print("#                                                                        #")
 		print("# Bypass 4xx HTTP response status codes and more.                        #")
 		print("# GitHub repository at github.com/ivan-sincek/forbidden.                 #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
 		print("#                                                                        #")
 		print("##########################################################################")
@@ -1236,15 +1263,15 @@
 		if not args["path"]:
 			args["path"] = ["/robots.txt"] # can have multiple
 		if not args["evil"]:
 			args["evil"] = "github.com"
 		if not args["threads"]:
 			args["threads"] = 5
 		if not args["agent"]:
-			args["agent"] = "Forbidden/9.6"
+			args["agent"] = "Forbidden/9.7"
 		# --------------------
 		url = parse_url(args["url"])
 		ignore = {"text": args["ignore"], "lengths": args["lengths"] if args["lengths"] else []}
 		# --------------------
 		# NOTE: Fetch content length of base HTTP response.
 		if "base" in ignore["lengths"]:
 			record = fetch(url["full"], args["force"] if args["force"] else "GET", None, None, None, args["agent"], None)
@@ -1266,15 +1293,15 @@
 		ips = fetch_ips(url["domain_no_port"])
 		values = args["values"] + ips if args["values"] else ips
 		# --------------------
 		collection = get_collection(url, args["tests"], accessible, args["evil"], args["force"], values, ignore, args["agent"], args["proxy"])
 		if not collection:
 			print("No test records were created")
 		else:
-			results = parse_results(bypass(filter(get_commands(collection)), args["threads"]))
+			results = parse_results(bypass(filter(get_commands(collection)), args["threads"], args["sleep"], args["debug"]))
 			if not results:
 				print("No result matched the validation criteria")
 			else:
 				print(("Number of valid results: {0}").format(len(results)))
 				if args["out"]:
 					write_file(jdump(results), args["out"])
 		print(("Script has finished in {0}").format(datetime.datetime.now() - start))
```

### Comparing `forbidden-9.6/src/forbidden/user_agents.txt` & `forbidden-9.7/src/forbidden/user_agents.txt`

 * *Files identical despite different names*

### Comparing `forbidden-9.6/src/forbidden.egg-info/PKG-INFO` & `forbidden-9.7/src/forbidden.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: forbidden
-Version: 9.6
-Summary: Bypass 4xx HTTP response status codes and more.
+Version: 9.7
+Summary: Bypass 4xx HTTP response status codes and more. Based on PycURL.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -113,15 +113,15 @@
 
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-9.6-py3-none-any.whl
+python3 -m pip install dist/forbidden-9.7-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -350,39 +350,39 @@
       "id":"570-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1"
       ],
       "body":null,
-      "agent":"Forbidden/9.6",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.7",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.7' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    },
    {
       "id":"571-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1:443"
       ],
       "body":null,
-      "agent":"Forbidden/9.6",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.7",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.7' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v9.6 ( github.com/ivan-sincek/forbidden )
+Forbidden v9.7 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -408,43 +408,49 @@
     -p <path> - /home/index.html | /README.txt | etc.
 EVIL
     Specify (strictly) evil domain name with no port to test URL overrides
     Scope: headers | redirects
     Default: github.com
     -e <evil> - xyz.interact.sh | xyz.burpcollaborator.net | etc.
 IGNORE
-    Filter out 200 OK false positive results by RegEx
-    Spacing will be stripped
+    Filter out 200 OK false positive results with a regual expression
     -i <ignore> - Forbidden | "Access Denied" | etc.
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Specify 'path' to ignore content length of accessible URL response
     Use comma separated values
     -l <lengths> - 12 | base | path | etc.
 THREADS
     Number of parallel threads to run
     More threads make it quicker but can give worse results
-    Heavily depends on network bandwidth and server capacity
+    Depends heavily on network bandwidth and server capacity
     Default: 5
     -th <threads> - 200 | etc.
+SLEEP
+    Sleep while queuing each request
+    Intended for a single thread use
+    -s <sleep> - 5 | etc.
 AGENT
     User agent to use
-    Default: Forbidden/9.6
+    Default: Forbidden/9.7
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
+DEBUG
+    Debug output
+    -dbg <debug> - yes
 ```
 
 ```fundamental
-Stresser v4.6 ( github.com/ivan-sincek/forbidden )
+Stresser v9.7 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -471,15 +477,15 @@
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Use comma separated values
     -l <lengths> - 12 | base | etc.
 AGENT
     User agent to use
-    Default: Stresser/4.6
+    Default: Stresser/9.7
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
```

### Comparing `forbidden-9.6/src/stresser/stresser.py` & `forbidden-9.7/src/stresser/stresser.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 colorama.init(autoreset = True)
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Stresser v4.6 ( github.com/ivan-sincek/forbidden )")
+	print("Stresser v9.7 ( github.com/ivan-sincek/forbidden )")
 	print("")
 	print("Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]")
 	print("Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]")
 
 def advanced():
 	basic()
 	print("")
@@ -58,15 +58,15 @@
 	print("LENGTHS")
 	print("    Filter out 200 OK false positive results by content lengths")
 	print("    Specify 'base' to ignore content length of base HTTP response")
 	print("    Use comma separated values")
 	print("    -l <lengths> - 12 | base | etc.")
 	print("AGENT")
 	print("    User agent to use")
-	print("    Default: Stresser/4.6")
+	print("    Default: Stresser/9.7")
 	print("    -a <agent> - curl/3.30.1 | random[-all] | etc.")
 	print("PROXY")
 	print("    Web proxy to use")
 	print("    -x <proxy> - 127.0.0.1:8080 | etc.")
 	print("OUT")
 	print("    Output file")
 	print("    -o <out> - results.json | etc.")
@@ -525,25 +525,25 @@
 	else:
 		error("Incorrect usage", True)
 
 	if proceed and check_directory(args["directory"]):
 		os.chdir(args["directory"])
 		print("###########################################################$$$$############")
 		print("#                                                                         #")
-		print("#                              Stresser v4.6                              #")
+		print("#                              Stresser v9.7                              #")
 		print("#                                  by Ivan Sincek                         #")
 		print("#                                                                         #")
 		print("# Bypass 4xx HTTP response status codes with stress testing.              #")
 		print("# GitHub repository at github.com/ivan-sincek/forbidden.                  #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
 		# --------------------
 		if not args["agent"]:
-			args["agent"] = "Stresser/4.6"
+			args["agent"] = "Stresser/9.7"
 		# --------------------
 		url = parse_url(args["url"])
 		ignore = {"text": args["ignore"], "lengths": args["lengths"] if args["lengths"] else []}
 		# --------------------
 		# NOTE: Fetch content length of base HTTP response.
 		if "base" in ignore["lengths"]:
 			record = fetch(url["full"], args["force"] if args["force"] else "GET", None, None, None, args["agent"], None)
```

### Comparing `forbidden-9.6/src/stresser/user_agents.txt` & `forbidden-9.7/src/stresser/user_agents.txt`

 * *Files identical despite different names*

