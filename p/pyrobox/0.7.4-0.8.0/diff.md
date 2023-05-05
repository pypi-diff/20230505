# Comparing `tmp/pyrobox-0.7.4.tar.gz` & `tmp/pyrobox-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrobox-0.7.4.tar", last modified: Sat Apr 22 19:18:07 2023, max compression
+gzip compressed data, was "pyrobox-0.8.0.tar", last modified: Fri May  5 20:56:15 2023, max compression
```

## Comparing `pyrobox-0.7.4.tar` & `pyrobox-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 19:18:07.409946 pyrobox-0.7.4/
--rw-rw-rw-   0        0        0     1062 2023-02-14 13:46:56.000000 pyrobox-0.7.4/LICENSE
--rw-rw-rw-   0        0        0    10271 2023-04-22 19:18:07.409946 pyrobox-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     9052 2023-04-19 11:03:38.000000 pyrobox-0.7.4/README.md
--rw-rw-rw-   0        0        0       90 2023-02-07 11:48:14.000000 pyrobox-0.7.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-22 19:18:07.400945 pyrobox-0.7.4/pyrobox.egg-info/
--rw-rw-rw-   0        0        0    10271 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1027 2023-04-22 19:18:07.410945 pyrobox-0.7.4/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-03-04 18:36:13.000000 pyrobox-0.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 19:18:07.408945 pyrobox-0.7.4/src/
--rw-rw-rw-   0        0        0       83 2023-03-04 18:36:13.000000 pyrobox-0.7.4/src/__init__.py
--rw-rw-rw-   0        0        0       20 2023-03-04 18:36:13.000000 pyrobox-0.7.4/src/__main__.py
--rw-rw-rw-   0        0        0     1812 2023-04-19 10:26:44.000000 pyrobox-0.7.4/src/arg_parser.py
--rw-rw-rw-   0        0        0      105 2023-04-22 14:53:09.000000 pyrobox-0.7.4/src/exceptions.py
--rw-rw-rw-   0        0        0     8154 2023-04-22 18:54:58.000000 pyrobox-0.7.4/src/fs_utils.py
--rw-rw-rw-   0        0        0    44164 2023-04-22 18:52:10.000000 pyrobox-0.7.4/src/page_templates.py
--rw-rw-rw-   0        0        0    46390 2023-04-22 18:57:57.000000 pyrobox-0.7.4/src/pyroboxCore.py
--rw-rw-rw-   0        0        0    32518 2023-04-22 19:14:09.000000 pyrobox-0.7.4/src/server.py
--rw-rw-rw-   0        0        0     2191 2023-02-07 11:48:14.000000 pyrobox-0.7.4/src/zipfly_local.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:56:15.065569 pyrobox-0.8.0/
+-rw-rw-rw-   0        0        0     1062 2023-02-14 13:46:56.000000 pyrobox-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0    10318 2023-05-05 20:56:15.066567 pyrobox-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9098 2023-04-23 13:48:06.000000 pyrobox-0.8.0/README.md
+-rw-rw-rw-   0        0        0       90 2023-02-07 11:48:14.000000 pyrobox-0.8.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-05 20:56:15.055592 pyrobox-0.8.0/pyrobox.egg-info/
+-rw-rw-rw-   0        0        0    10318 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1027 2023-05-05 20:56:15.069561 pyrobox-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      237 2023-03-04 18:36:12.000000 pyrobox-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:56:15.064574 pyrobox-0.8.0/src/
+-rw-rw-rw-   0        0        0       83 2023-03-04 18:36:12.000000 pyrobox-0.8.0/src/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-03-04 18:36:12.000000 pyrobox-0.8.0/src/__main__.py
+-rw-rw-rw-   0        0        0     1812 2023-04-19 10:26:44.000000 pyrobox-0.8.0/src/_arg_parser.py
+-rw-rw-rw-   0        0        0      105 2023-04-22 14:53:08.000000 pyrobox-0.8.0/src/_exceptions.py
+-rw-rw-rw-   0        0        0     8105 2023-05-05 20:50:11.000000 pyrobox-0.8.0/src/_fs_utils.py
+-rw-rw-rw-   0        0        0    44160 2023-05-05 20:25:55.000000 pyrobox-0.8.0/src/_page_templates.py
+-rw-rw-rw-   0        0        0     7165 2023-05-05 20:49:15.000000 pyrobox-0.8.0/src/_zipfly_manager.py
+-rw-rw-rw-   0        0        0    53479 2023-05-05 20:54:03.000000 pyrobox-0.8.0/src/pyroboxCore.py
+-rw-rw-rw-   0        0        0    29220 2023-05-05 20:34:07.000000 pyrobox-0.8.0/src/server.py
```

### Comparing `pyrobox-0.7.4/LICENSE` & `pyrobox-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrobox-0.7.4/PKG-INFO` & `pyrobox-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrobox
-Version: 0.7.4
+Version: 0.8.0
 Summary: Personal DropBox for Private Network
 Home-page: https://github.com/RaSan147/pyrobox
 Author-email: wwwqweasd147@gmail.com
 Project-URL: Bug Tracker, https://github.com/RaSan147/pyrobox/issues
 Project-URL: Documentation, https://github.com/RaSan147/pyrobox
 Project-URL: Source Code, https://github.com/RaSan147/pyrobox
 Project-URL: Release Notes, https://github.com/RaSan147/pyrobox/releases
@@ -150,14 +150,15 @@
 
 * https://github.com/RaSan147/pyrobox/issues/33 Show thumbnails, for png and jpg (how to do with just standard library?), For others, just show extension.
 * https://github.com/RaSan147/pyrobox/issues/34 Copy stream URL for videos to play with any video player
 * https://github.com/RaSan147/pyrobox/issues/36 Add side bar to do something 🤔
 * check output ip and port accuracy on multiple os  
 * https://github.com/RaSan147/pyrobox/issues/37 Backup code if Reload causes unhandled issue and can't be accessed
 * https://github.com/RaSan147/pyrobox/issues/39 User login and user based permission set. 🔑
+* Add more flags to disable specific features
 
 # Support for more features
 
 
 Context menu:
 --------------------------------------------------------------
   **Right click on any file link**
```

### Comparing `pyrobox-0.7.4/README.md` & `pyrobox-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
 * https://github.com/RaSan147/pyrobox/issues/33 Show thumbnails, for png and jpg (how to do with just standard library?), For others, just show extension.
 * https://github.com/RaSan147/pyrobox/issues/34 Copy stream URL for videos to play with any video player
 * https://github.com/RaSan147/pyrobox/issues/36 Add side bar to do something 🤔
 * check output ip and port accuracy on multiple os  
 * https://github.com/RaSan147/pyrobox/issues/37 Backup code if Reload causes unhandled issue and can't be accessed
 * https://github.com/RaSan147/pyrobox/issues/39 User login and user based permission set. 🔑
+* Add more flags to disable specific features
 
 # Support for more features
 
 
 Context menu:
 --------------------------------------------------------------
   **Right click on any file link**
```

### Comparing `pyrobox-0.7.4/pyrobox.egg-info/PKG-INFO` & `pyrobox-0.8.0/pyrobox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrobox
-Version: 0.7.4
+Version: 0.8.0
 Summary: Personal DropBox for Private Network
 Home-page: https://github.com/RaSan147/pyrobox
 Author-email: wwwqweasd147@gmail.com
 Project-URL: Bug Tracker, https://github.com/RaSan147/pyrobox/issues
 Project-URL: Documentation, https://github.com/RaSan147/pyrobox
 Project-URL: Source Code, https://github.com/RaSan147/pyrobox
 Project-URL: Release Notes, https://github.com/RaSan147/pyrobox/releases
@@ -150,14 +150,15 @@
 
 * https://github.com/RaSan147/pyrobox/issues/33 Show thumbnails, for png and jpg (how to do with just standard library?), For others, just show extension.
 * https://github.com/RaSan147/pyrobox/issues/34 Copy stream URL for videos to play with any video player
 * https://github.com/RaSan147/pyrobox/issues/36 Add side bar to do something 🤔
 * check output ip and port accuracy on multiple os  
 * https://github.com/RaSan147/pyrobox/issues/37 Backup code if Reload causes unhandled issue and can't be accessed
 * https://github.com/RaSan147/pyrobox/issues/39 User login and user based permission set. 🔑
+* Add more flags to disable specific features
 
 # Support for more features
 
 
 Context menu:
 --------------------------------------------------------------
   **Right click on any file link**
```

### Comparing `pyrobox-0.7.4/setup.cfg` & `pyrobox-0.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7972 6f62 6f78 0d0a 7665 7273   = pyrobox..vers
-00000020: 696f 6e20 3d20 302e 372e 340d 0a61 7574  ion = 0.7.4..aut
+00000020: 696f 6e20 3d20 302e 382e 300d 0a61 7574  ion = 0.8.0..aut
 00000030: 686f 7273 203d 2052 6173 616e 0d0a 6175  hors = Rasan..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 2077 7777  thor_email = www
 00000050: 7177 6561 7364 3134 3740 676d 6169 6c2e  qweasd147@gmail.
 00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000070: 203d 2050 6572 736f 6e61 6c20 4472 6f70   = Personal Drop
 00000080: 426f 7820 666f 7220 5072 6976 6174 6520  Box for Private 
 00000090: 4e65 7477 6f72 6b0d 0a6c 6f6e 675f 6465  Network..long_de
```

### Comparing `pyrobox-0.7.4/src/arg_parser.py` & `pyrobox-0.8.0/src/_arg_parser.py`

 * *Files identical despite different names*

### Comparing `pyrobox-0.7.4/src/fs_utils.py` & `pyrobox-0.8.0/src/_fs_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import os
 from queue import Queue
 import re
 import urllib.parse
 
 
-from .exceptions import LimitExceed
+from ._exceptions import LimitExceed
 
 
 
 
 def get_stat(path):
 	"""
 	Get the stat of a file.
@@ -190,20 +190,16 @@
 			total += entry.stat(follow_symlinks=False).st_size
 		except OSError:
 			continue
 
 		if limit and total>limit:
 			raise LimitExceed
 
-		if must_read:
-			try:
-				with open(entry.path, "rb") as f:
-					f.read(1)
-			except Exception:
-				continue
+		if must_read and not check_access(entry.path):
+			continue
 
 	return total
 
 def _get_tree_path_n_size(path, limit=-1, must_read=False, path_type="full"):
 	"""
 	returns a list of files[size, path] in a directory and its subdirectories.
 		[ [`path`, size], ... ]
```

### Comparing `pyrobox-0.7.4/src/page_templates.py` & `pyrobox-0.8.0/src/_page_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from string import Template as _Template # using this because js also use {$var} and {var} syntax and py .format is often unsafe
 
 __all__ = [
 	"directory_explorer_header",
 	"global_script",
 	"file_list",
 	"upload_form",
-	"js_script",
+	"file_list_script",
 	"video_script",
 	"zip_script",
 	"admin_page",
 	"error_page",
 ]
 
 
@@ -52,20 +52,20 @@
 
 def global_script():
 	return get_template("global_script.html")
 
 def file_list():
 	return global_script() + get_template("html_file_list.html")
 
+def file_list_script():
+	return get_template("html_script.html")
+
 def upload_form():
 	return get_template("html_upload.html")
 
-def js_script():
-	return global_script() + get_template("html_script.html")
-
 def video_script():
 	return global_script() + get_template("html_vid.html")
 
 def zip_script():
 	return global_script() + get_template("html_zip_page.html")
 
 def admin_page():
```

### Comparing `pyrobox-0.7.4/src/pyroboxCore.py` & `pyrobox-0.8.0/src/pyroboxCore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,101 +1,117 @@
-__version__ = "0.7.4"
+import traceback
+import json
+import string
+import random
+import base64
+import re
+from http import HTTPStatus
+from functools import partial
+import contextlib
+import urllib.request
+import urllib.parse
+import time
+import sys
+import socketserver
+import socket  # For gethostbyaddr()
+import shutil
+import posixpath
+import mimetypes
+import io
+import http.client
+import html
+import email.utils
+import datetime
+import argparse
+from string import Template
+from typing import Union
+from queue import Queue
+import logging
+import atexit
+import os
+
+__version__ = "0.8.0"
+
 enc = "utf-8"
 __all__ = [
 	"HTTPServer", "ThreadingHTTPServer", "BaseHTTPRequestHandler",
 	"SimpleHTTPRequestHandler",
-
 ]
 
-import os
-import atexit
-import logging
-from queue import Queue
-from typing import Union
-from string import Template
-
-import argparse
-
 
 logging.basicConfig(level=logging.INFO, format='%(levelname)s: \n%(message)s')
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 # set INFO to see all the requests
 # set WARNING to see only the requests that made change to the server
 # set ERROR to see only the requests that made the errors
 
 
-
 endl = "\n"
-T = t = true = True # too lazy to type
-F = f = false = False # too lazy to type
+T = t = true = True  # too lazy to type
+F = f = false = False  # too lazy to type
+
 
 class Config:
 	def __init__(self):
 		# DEFAULT DIRECTORY TO LAUNCH SERVER
-		self.ftp_dir = "." # DEFAULT DIRECTORY TO LAUNCH SERVER
+		self.ftp_dir = "."  # DEFAULT DIRECTORY TO LAUNCH SERVER
 
-		self.IP = None # will be assigned by checking
+		self.IP = None  # will be assigned by checking
 
 		# DEFAULT PORT TO LAUNCH SERVER
-		self.port= 6969  # DEFAULT PORT TO LAUNCH SERVER
+		self.port = 6969  # DEFAULT PORT TO LAUNCH SERVER
 
 		# UPLOAD PASSWORD SO THAT ANYONE RANDOM CAN'T UPLOAD
 		# CAN BE CHANGED BY USING --password NEW_PASSWORD
-		self.PASSWORD= "SECret"
+		self.PASSWORD = "SECret"
 
 		# LOGGING
 		self.log_location = "./"  # fallback log_location = "./"
-		self.allow_web_log = True # if you want to see some important LOG in browser, may contain your important information
-		self.write_log = False # if you want to write log to file
+		# if you want to see some important LOG in browser, may contain your important information
+		self.allow_web_log = True
+		self.write_log = False  # if you want to write log to file
 
 		# ZIP FEATURES
-		self.default_zip = "zipfile" # or "zipfile" to use python built in zip module
+		self.default_zip = "zipfile"  # or "zipfile" to use python built in zip module
 
 		# CHECK FOR MISSING REQUEIREMENTS
 		self.run_req_check = True
 
 		# FILE INFO
 		self.MAIN_FILE = os.path.realpath(__file__)
 		self.MAIN_FILE_dir = os.path.dirname(self.MAIN_FILE)
 
-
 		# OS DETECTION
 		self.OS = self.get_os()
 
-
 		# RUNNING SERVER STATS
 		self.ftp_dir = self.get_default_dir()
 		self.dev_mode = False
-		self.ASSETS = False # if you want to use assets folder, set this to True
+		self.ASSETS = False  # if you want to use assets folder, set this to True
 		self.ASSETS_dir = os.path.join(self.MAIN_FILE_dir, "/../assets/")
 		self.reload = False
 
-
 		self.disabled_func = {
 			"reload": False,
 		}
 
 		# TEMP FILE MAPPING
 		self.temp_file = set()
 
 		# CLEAN TEMP FILES ON EXIT
 		atexit.register(self.clear_temp)
 
-
 		# ASSET MAPPING
 		self.file_list = {}
 
 		# COMMANDLINE ARGUMENTS PARSER
 		self.parser = argparse.ArgumentParser(add_help=False)
 
-
-
-
 		# Default error message template
 		self.DEFAULT_ERROR_MESSAGE = Template("""
 		<!DOCTYPE HTML>
 		<html lang="en">
 		<html>
 			<head>
 				<meta charset="utf-8">
@@ -109,60 +125,54 @@
 				<h3>PyroBox Version: ${version}</h3>
 			</body>
 		</html>
 		""")
 
 		self.DEFAULT_ERROR_CONTENT_TYPE = "text/html;charset=utf-8"
 
-
-
 	def clear_temp(self):
 		for i in self.temp_file:
 			try:
 				os.remove(i)
 			except:
 				pass
 
-
-
 	def get_os(self):
 		from platform import system as platform_system
 
 		out = platform_system()
-		if out=="Linux":
-			if hasattr(sys, 'getandroidapilevel'):
-				#self.IP = "192.168.43.1"
-				return 'Android'
+		if out == "Linux" and hasattr(sys, 'getandroidapilevel'):
+			# self.IP = "192.168.43.1"
+			return 'Android'
 
 		return out
 
 	def get_default_dir(self):
 		return './'
 
-
 	def address(self):
-		return "http://%s:%i"%(self.IP, self.port)
+		return f"http://{self.IP}:{self.port}"
 
-	def parse_default_args(self, port = None, directory = None, bind = None, ):
-		if port is None:
+	def parse_default_args(self, port=0, directory="", bind=None):
+		if not port:
 			port = self.port
-		if directory is None:
+		if not directory:
 			directory = self.ftp_dir
-		if bind is None:
+		if not bind:
 			bind = None
 
 		parser = self.parser
 
 		parser.add_argument('--bind', '-b',
 							metavar='ADDRESS', default=bind,
 							help='Specify alternate bind address '
 								'[default: all interfaces]')
 		parser.add_argument('--directory', '-d', default=directory,
 							help='Specify alternative directory '
-							'[default: current directory]')
+								'[default: current directory]')
 		parser.add_argument('port', action='store',
 							default=port, type=int,
 							nargs='?',
 							help=f'Specify alternate port [default: {port}]')
 		parser.add_argument('--version', '-v', action='version',
 							version=__version__)
 
@@ -171,64 +181,28 @@
 								help=('show this help message and exit'))
 
 		args = parser.parse_known_args()[0]
 
 		return args
 
 
-
-
-
-
-
-
-
-import datetime
-import email.utils
-import html
-import http.client
-import io
-import mimetypes
-import posixpath
-import shutil
-import socket # For gethostbyaddr()
-import socketserver
-import sys
-import time
-import urllib.parse
-import urllib.request
-import contextlib
-from functools import partial
-from http import HTTPStatus
-
-import re
-import base64
-
-import random
-import string
-import json
-import traceback
-
-
-
-
 class Tools:
 	def __init__(self):
 		self.styles = {
-			"equal" : "=",
-			"star"    : "*",
-			"hash"  : "#",
-			"dash"  : "-",
+			"equal": "=",
+			"star": "*",
+			"hash": "#",
+			"dash": "-",
 			"udash": "_"
 		}
 
 	def term_width(self):
 		return shutil.get_terminal_size()[0]
 
-	def text_box(self, *text, style = "equal", sep=" "):
+	def text_box(self, *text, style="equal", sep=" "):
 		"""
 		Returns a string of text with a border around it.
 		"""
 		text = sep.join(map(str, text))
 		term_col = shutil.get_terminal_size()[0]
 
 		s = self.styles[style] if style in self.styles else style
@@ -237,14 +211,15 @@
 			tt += i.center(term_col) + '\n'
 		return (f"\n\n{s*term_col}\n{tt}{s*term_col}\n\n")
 
 	def random_string(self, length=10):
 		letters = string.ascii_lowercase
 		return ''.join(random.choice(letters) for i in range(length))
 
+
 tools = Tools()
 config = Config()
 
 
 class Callable_dict(dict):
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
@@ -255,34 +230,35 @@
 
 
 
 
 def reload_server():
 	"""reload the server process from file"""
 	file = config.MAIN_FILE
-	logger.info("Reloading...\n"+
+	logger.info("Reloading...\n" +
 				" ".join(
-					["RE-RUNNING: ", sys.executable, sys.executable, file, *sys.argv[1:]]
+					["RE-RUNNING: ", sys.executable,
+						sys.executable, file, *sys.argv[1:]]
 				))
 	try:
 		os.execl(sys.executable, sys.executable, file, *sys.argv[1:])
 	except:
 		traceback.print_exc()
 	sys.exit(0)
 
+
 def null(*args, **kwargs):
 	pass
 
 
-
-
 class Zfunc(object):
 	"""Thread safe sequncial printing/queue task handler class"""
 
 	__all__ = ["new", "update"]
+
 	def __init__(self, caller, store_return=False):
 		super().__init__()
 
 		self.queue = Queue()
 		# stores [args, kwargs], ...
 		self.store_return = store_return
 		self.returner = Queue()
@@ -306,31 +282,26 @@
 
 		self.BUSY = False
 
 		if not self.queue.empty():
 			# will make the loop continue running
 			return True
 
-
 	def update(self, *args, **kwargs):
 		""" Uses xprint and parse string"""
 
 		self.queue.put((args, kwargs))
 		while self.next() is True:
 			# use while instead of recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion.... error
 			pass
 
-
-
 	def new(self, caller, store_return=False):
 		self.__init__(caller=caller, store_return=store_return)
 
 
-
-
 """HTTP server classes.
 
 Note: BaseHTTPRequestHandler doesn't implement any HTTP request; see
 SimpleHTTPRequestHandler for simple implementations of GET, HEAD and POST,
 and CGIHTTPRequestHandler for CGI scripts.
 
 It does, however, optionally implement HTTP/1.1 persistent connections,
@@ -340,83 +311,82 @@
 
 - log requests even later (to capture byte count)
 - log user-agent header and other interesting goodies
 - send error log to separate file
 """
 
 
-
-
 ##############################################
 #         PAUSE AND RESUME FEATURE           #
 ##############################################
 
 def copy_byte_range(infile, outfile, start=None, stop=None, bufsize=16*1024):
 	'''
 	TO SUPPORT PAUSE AND RESUME FEATURE
 	Like shutil.copyfileobj, but only copy a range of the streams.
 	Both start and stop are inclusive.
 	'''
-	if start is not None: infile.seek(start)
+	if start is not None:
+		infile.seek(start)
 	while 1:
 		to_read = min(bufsize, stop + 1 - infile.tell() if stop else bufsize)
 		buf = infile.read(to_read)
 		if not buf:
 			break
 		outfile.write(buf)
 
 
 BYTE_RANGE_RE = re.compile(r'bytes=(\d+)-(\d+)?$')
+
+
 def parse_byte_range(byte_range):
 	'''Returns the two numbers in 'bytes=123-456' or throws ValueError.
 	The last number or both numbers may be None.
 	'''
 	if byte_range.strip() == '':
 		return None, None
 
 	m = BYTE_RANGE_RE.match(byte_range)
 	if not m:
 		raise ValueError('Invalid byte range %s' % byte_range)
 
-	#first, last = [x and int(x) for x in m.groups()] #
+	# first, last = [x and int(x) for x in m.groups()] #
 
 	first, last = map((lambda x: int(x) if x else None), m.groups())
 
 	if last and last < first:
 		raise ValueError('Invalid byte range %s' % byte_range)
 	return first, last
 
-#---------------------------x--------------------------------
-
+# ---------------------------x--------------------------------
 
 
-
-def URL_MANAGER(url:str):
+def URL_MANAGER(url: str):
 	"""
 	returns a tuple of (`path`, `query_dict`, `fragment`)\n
 
 	`url` = `'/store?page=10&limit=15&price=ASC#dskjfhs'`\n
 	`path` = `'/store'`\n
 	`query_dict` = `{'page': ['10'], 'limit': ['15'], 'price': ['ASC']}`\n
 	`fragment` = `dskjfhs`\n
 	"""
 
 	# url = '/store?page=10&limit=15&price#dskjfhs'
 	parse_result = urllib.parse.urlparse(url)
 
-
-	dict_result = Callable_dict(urllib.parse.parse_qs(parse_result.query, keep_blank_values=True))
+	dict_result = Callable_dict(urllib.parse.parse_qs(
+		parse_result.query, keep_blank_values=True))
 
 	return (parse_result.path, dict_result, parse_result.fragment)
 
 
 
 class HTTPServer(socketserver.TCPServer):
 
-	allow_reuse_address = True	# Seems to make sense in testing environment
+	allow_reuse_address = True  # Seems to make sense in testing environment
 
 	def server_bind(self):
 		"""Override server_bind to store the server name."""
 		socketserver.TCPServer.server_bind(self)
 		host, port = self.server_address[:2]
 		self.server_name = socket.getfqdn(host)
 		self.server_port = port
@@ -501,17 +471,17 @@
 			try:
 				if not version.startswith('HTTP/'):
 					raise ValueError
 				base_version_number = version.split('/', 1)[1]
 				version_number = base_version_number.split(".")
 				# RFC 2145 section 3.1 says there can be only one "." and
 				#   - major and minor numbers MUST be treated as
-				#	  separate integers;
+				#     separate integers;
 				#   - HTTP/2.4 is a lower version than HTTP/2.13, which in
-				#	  turn is lower than HTTP/12.3;
+				#     turn is lower than HTTP/12.3;
 				#   - Leading zeros MUST be ignored by recipients.
 				if len(version_number) != 2:
 					raise ValueError
 				version_number = int(version_number[0]), int(version_number[1])
 			except (ValueError, IndexError):
 				self.send_error(
 					HTTPStatus.BAD_REQUEST,
@@ -572,15 +542,15 @@
 			self.close_connection = True
 		elif (conntype.lower() == 'keep-alive' and
 			  self.protocol_version >= "HTTP/1.1"):
 			self.close_connection = False
 		# Examine the headers and look for an Expect directive
 		expect = self.headers.get('Expect', "")
 		if (expect.lower() == "100-continue" and
-				self.protocol_version >= "HTTP/1.1" and
+			self.protocol_version >= "HTTP/1.1" and
 				self.request_version >= "HTTP/1.1"):
 			if not self.handle_expect_100():
 				return False
 		return True
 
 	def handle_expect_100(self):
 		"""Decide what to do with an "Expect: 100-continue" header.
@@ -633,85 +603,85 @@
 			url_path, query, fragment = URL_MANAGER(self.path)
 			self.url_path = url_path
 			self.query = query
 			self.fragment = fragment
 
 			self.use_range = False
 
-
 			_hash = abs(hash((self.raw_requestline, tools.random_string(10))))
-			self.req_hash = base64.b64encode(str(_hash).encode('ascii')).decode()[:10]
+			self.req_hash = base64.b64encode(
+					str(_hash).encode('ascii')
+				).decode()[:10]
 
 			_w = tools.term_width()
-			w = _w - len(str(self.req_hash)) -2
+			w = _w - len(str(self.req_hash)) - 2
 			w = w//2
-			logger.info('='*w + f' {self.req_hash} ' + '='*w + '\n'+
-					'\n'.join(
-						[f'{self.req_hash}|=>\t request\t: {self.command}',
-						f'{self.req_hash}|=>\t url     \t: {url_path}',
-						f'{self.req_hash}|=>\t query   \t: {query}',
-						f'{self.req_hash}|=>\t fragment\t: {fragment}',
-						f'{self.req_hash}|=>\t full url \t: {self.path}',
-						]) + '\n'+
-					'+'*w + f' {self.req_hash} ' + '+'*w
-				)
-
-
-
+			logger.info('='*w + f' {self.req_hash} ' + '='*w + '\n' +
+						'\n'.join(
+								[f'{self.req_hash}|=>\t request\t: {self.command}',
+								 f'{self.req_hash}|=>\t url     \t: {url_path}',
+								 f'{self.req_hash}|=>\t query   \t: {query}',
+								 f'{self.req_hash}|=>\t fragment\t: {fragment}',
+								 f'{self.req_hash}|=>\t full url \t: {self.path}',
+								 ]) + '\n' +
+						'+'*w + f' {self.req_hash} ' + '+'*w
+						)
 
 			try:
 				method()
 			except Exception:
 				traceback.print_exc()
 
-			logger.info('-'*w + f' {self.req_hash} ' + '-'*w + '\n'+
+			logger.info('-'*w + f' {self.req_hash} ' + '-'*w + '\n' +
 						'#'*_w
 						)
-			self.wfile.flush() #actually send the response if not already done.
+			
+			# actually send the response if not already done.
+			self.wfile.flush()
+
 		except (TimeoutError, socket.timeout) as e:
-			#a read or a write timed out.  Discard this connection
+			# a read or a write timed out.  Discard this connection
 			self.log_error("Request timed out:", e)
 			self.close_connection = True
 			return
 
 	def handle(self):
 		"""Handle multiple requests if necessary."""
 		self.close_connection = True
 
 		self.handle_one_request()
 		while not self.close_connection:
 			self.handle_one_request()
 
-	def send_error(self, code, message=None, explain=None, error_message_format:Template=None):
+	def send_error(self, code, message=None, explain=None, error_message_format: Template = None):
 		"""Send and log an error reply.
 
 		Arguments are
 		* code:	an HTTP error code
-				   3 digits
+					3 digits
 		* message: a simple optional 1 line reason phrase.
-				   *( HTAB / SP / VCHAR / %x80-FF )
-				   defaults to short entry matching the response code
+					*( HTAB / SP / VCHAR / %x80-FF )
+					defaults to short entry matching the response code
 		* explain: a detailed message defaults to the long entry
-				   matching the response code.
+					matching the response code.
 		* error_message_format: a `string.Template` for the error message
-				   defaults to `config.DEFAULT_ERROR_MESSAGE`
+					defaults to `config.DEFAULT_ERROR_MESSAGE`
 
-				   auto-formatting values:
+					auto-formatting values:
 						`${code}`: the HTTP error code
 						`${message}`: the HTTP error message
 						`${explain}`: the detailed error message
 						`${version}`: the server software version string
 
 		This sends an error response (so it must be called before any
 		output has been generated), logs the error, and finally sends
 		a piece of HTML explaining the error to the user.
 
 		"""
 
-
 		error_message_format = error_message_format if error_message_format else config.DEFAULT_ERROR_MESSAGE
 
 		error_content_type = config.DEFAULT_ERROR_CONTENT_TYPE
 
 		try:
 			shortmsg, longmsg = self.responses[code]
 		except KeyError:
@@ -725,24 +695,24 @@
 		self.send_header('Connection', 'close')
 
 		# Message body is omitted for cases described in:
 		#  - RFC7230: 3.3. 1xx, 204(No Content), 304(Not Modified)
 		#  - RFC7231: 6.3.6. 205(Reset Content)
 		body = None
 		if (code >= 200 and
-			code not in (HTTPStatus.NO_CONTENT,
-						 HTTPStatus.RESET_CONTENT,
-						 HTTPStatus.NOT_MODIFIED)):
+				code not in (HTTPStatus.NO_CONTENT,
+							 HTTPStatus.RESET_CONTENT,
+							 HTTPStatus.NOT_MODIFIED)):
 			# HTML encode to prevent Cross Site Scripting attacks
 			# (see bug #1100201)
 			content = (error_message_format.safe_substitute(
-				code= code,
-				message= html.escape(message, quote=False),
-				explain= html.escape(explain, quote=False),
-				version= __version__
+				code=code,
+				message=html.escape(message, quote=False),
+				explain=html.escape(explain, quote=False),
+				version=__version__
 			))
 			body = content.encode('UTF-8', 'replace')
 			self.send_header("Content-Type", error_content_type)
 			self.send_header('Content-Length', str(len(body)))
 		self.end_headers()
 
 		if self.command != 'HEAD' and body:
@@ -768,16 +738,16 @@
 				if code in self.responses:
 					message = self.responses[code][0]
 				else:
 					message = ''
 			if not hasattr(self, '_headers_buffer'):
 				self._headers_buffer = []
 			self._headers_buffer.append(("%s %d %s\r\n" %
-					(self.protocol_version, code, message)).encode(
-						'utf-8', 'strict'))
+				(self.protocol_version, code, message)).encode(
+				'utf-8', 'strict'))
 
 	def send_header(self, keyword, value):
 		"""Send a MIME header to the headers buffer."""
 		if self.request_version != 'HTTP/0.9':
 			if not hasattr(self, '_headers_buffer'):
 				self._headers_buffer = []
 			self._headers_buffer.append(
@@ -817,74 +787,69 @@
 		default it passes the message on to log_message().
 
 		Arguments are the same as for log_message().
 
 		XXX This should go to the separate error log.
 
 		"""
-		self.log_message(args, error = True)
+		self.log_message(args, error=True)
 
 	def log_warning(self, *args):
 		"""Log a warning message [HIGH PRIORITY]"""
-		self.log_message(args, warning = True)
+		self.log_message(args, warning=True)
 
-	def log_debug(self, *args, write = True):
+	def log_debug(self, *args, write=True):
 		"""Log a debug message [LOWEST PRIORITY]"""
-		self.log_message(args, debug = True, write = write)
+		self.log_message(args, debug=True, write=write)
 
-	def log_info(self, *args, write = False):
+	def log_info(self, *args, write=False):
 		"""Default log message [MEDIUM PRIORITY]"""
-		self.log_message(args, write = write)
+		self.log_message(args, write=write)
 
 	def _log_writer(self, message):
 		os.makedirs(config.log_location, exist_ok=True)
-		with open(config.log_location + 'log.txt','a+') as f:
-			f.write((f"#{self.req_hash} by [{self.address_string()}] at [{self.log_date_time_string()}]|=> {message}\n"))
-
+		with open(config.log_location + 'log.txt', 'a+') as f:
+			f.write(
+				(f"#{self.req_hash} by [{self.address_string()}] at [{self.log_date_time_string()}]|=> {message}\n"))
 
-
-	def log_message(self, *args, error = False, warning = False, debug = False, write = True):
+	def log_message(self, *args, error=False, warning=False, debug=False, write=True):
 		"""Log an arbitrary message.
 
 		This is used by all other logging functions.  Override
 		it if you have specific logging wishes.
 
 		The client ip and current date/time are prefixed to
 		every message.
 
 		"""
 
 		message = ' '.join(map(str, args))
 
-		message = ("# %s by [%s] at [%s] %s\n" %
-						 (self.req_hash, self.address_string(),
-						  self.log_date_time_string(),
-						  message))
+		message = f"# {self.req_hash} by [{self.address_string()}] at [{self.log_date_time_string()}]|=> {message}\n"
+
 		if error:
 			logger.error(message)
 		elif warning:
 			logger.warning(message)
 		elif debug:
 			logger.debug(message)
 		else:
 			logger.info(message)
 
-
 		if not config.write_log:
 			return
 
 		if not hasattr(self, "Zlog_writer"):
 			self.Zlog_writer = Zfunc(self._log_writer)
 
 		try:
 			self.Zlog_writer.update(message)
 		except Exception:
 			traceback.print_exc()
 
-
 	def version_string(self):
 		"""Return the server software version string."""
 		return self.server_version + ' ' + self.sys_version
 
 	def date_time_string(self, timestamp=None):
 		"""Return the current date and time formatted for a message header."""
 		if timestamp is None:
@@ -892,15 +857,15 @@
 		return email.utils.formatdate(timestamp, usegmt=True)
 
 	def log_date_time_string(self):
 		"""Return the current time formatted for logging."""
 		now = time.time()
 		year, month, day, hh, mm, ss, x, y, z = time.localtime(now)
 		s = "%02d/%3s/%04d %02d:%02d:%02d" % (
-				day, self.monthname[month], year, hh, mm, ss)
+			day, self.monthname[month], year, hh, mm, ss)
 		return s
 
 	weekdayname = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 
 	monthname = [None,
 				 'Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
 				 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
@@ -938,105 +903,103 @@
 	request omits the actual contents of the file.
 
 	"""
 
 	server_version = "SimpleHTTP/" + __version__
 
 	if not mimetypes.inited:
-		mimetypes.init() # try to read system mime.types
+		mimetypes.init()  # try to read system mime.types
 	extensions_map = mimetypes.types_map.copy()
 	extensions_map.update({
-		'': 'application/octet-stream', # Default
-		'.py': 'text/plain',
-		'.c': 'text/plain',
-		'.h': 'text/plain',
-		'.css': 'text/css',
-
-		'.gz': 'application/gzip',
-		'.Z': 'application/octet-stream',
-		'.bz2': 'application/x-bzip2',
-		'.xz': 'application/x-xz',
-
-		'.webp': 'image/webp',
-
-		'opus': 'audio/opus',
-		'.oga': 'audio/ogg',
-		'.wav': 'audio/wav',
-
-		'.ogv': 'video/ogg',
-		'.ogg': 'application/ogg',
-		'm4a': 'audio/mp4',
+		'': 'application/octet-stream',  # Default
+			'.py': 'text/plain',
+			'.c': 'text/plain',
+			'.h': 'text/plain',
+			'.css': 'text/css',
+
+			'.gz': 'application/gzip',
+			'.Z': 'application/octet-stream',
+			'.bz2': 'application/x-bzip2',
+			'.xz': 'application/x-xz',
+
+			'.webp': 'image/webp',
+
+			'opus': 'audio/opus',
+			'.oga': 'audio/ogg',
+			'.wav': 'audio/wav',
+
+			'.ogv': 'video/ogg',
+			'.ogg': 'application/ogg',
+			'm4a': 'audio/mp4',
 	})
 
 	handlers = {
-			'HEAD': [],
-			'POST': [],
-		}
+		'HEAD': [],
+		'POST': [],
+	}
 
 	def __init__(self, *args, directory=None, **kwargs):
 		if directory is None:
 			directory = os.getcwd()
-		self.directory = os.fspath(directory) # same as directory, but str, new in 3.6
+		# os.fspath() same as directory, but str, new in 3.6
+		self.directory = os.fspath(directory)
 		super().__init__(*args, **kwargs)
 		self.query = Callable_dict()
 
-
 	def do_GET(self):
 		"""Serve a GET request."""
 		try:
 			f = self.send_head()
 		except Exception as e:
 			traceback.print_exc()
 			self.send_error(500, str(e))
 			return
 
 		if f:
 			try:
 				self.copyfile(f, self.wfile)
 			except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
-				self.log_info(tools.text_box(e.__class__.__name__, e,"\nby ", self.address_string()))
+				self.log_info(tools.text_box(e.__class__.__name__,
+							  e, "\nby ", self.address_string()))
 			finally:
 				f.close()
 
 	def do_(self):
 		'''incase of errored request'''
 		self.send_error(HTTPStatus.BAD_REQUEST, "Bad request.")
 
-
 	@staticmethod
-	def on_req(type='', url='', hasQ=(), QV={}, fragent='', url_regex = '', func=null):
+	def on_req(type='', url='', hasQ=(), QV={}, fragent='', url_regex='', func=null):
 		'''called when request is received
 		type: GET, POST, HEAD, ...
 		url: url (must start with /)
 		hasQ: if url has query
 		QV: match query value
 		fragent: fragent of request
 		url_regex: url regex (must start with /) url regex, the url must start and end with this regex
 
-		if query is tuple, it will only check existence of key
+		if query is tuple|list, it will only check existence of key
 		if query is dict, it will check value of key
 		'''
 		self = __class__
 
 		type = type.upper()
 		if type == 'GET':
 			type = 'HEAD'
 
-
 		if type not in self.handlers:
 			self.handlers[type] = []
 
 		# FIXING TYPE ISSUE
 		if isinstance(hasQ, str):
 			hasQ = (hasQ,)
 
-		if url=='' and url_regex=='':
+		if url == '' and url_regex == '':
 			url_regex = '.*'
 
-
 		to_check = (url, hasQ, QV, fragent, url_regex)
 
 		def decorator(func):
 			self.handlers[type].append((to_check, func))
 			return func
 		return decorator
 
@@ -1048,28 +1011,33 @@
 			hasQ: if url has query
 			QV: match query value
 			fragent: fragent of request
 			url_regex: url regex, the url must start and end with this regex
 
 
 		'''
-		if url_regex:
-			if not re.search("^"+url_regex+'$', self.url_path): return False
-		elif url and url!=self.url_path: return False
+		if url_regex and not re.search("^"+url_regex+'$', self.url_path):
+				return False
+		elif url and url != self.url_path:
+			return False
 
 		if isinstance(hasQ, str):
 			hasQ = (hasQ,)
 
-		if hasQ and self.query(*hasQ)==False: return False
+		if hasQ and self.query(*hasQ) == False:
+			return False
 		if QV:
 			for k, v in QV.items():
-				if not self.query(k): return False
-				if self.query[k] != v: return False
+				if not self.query(k):
+					return False
+				if self.query[k] != v:
+					return False
 
-		if fragent and self.fragment != fragent: return False
+		if fragent and self.fragment != fragent:
+			return False
 
 		return True
 
 	def do_HEAD(self):
 		"""Serve a HEAD request."""
 		try:
 			f = self.send_head()
@@ -1081,53 +1049,52 @@
 		if f:
 			f.close()
 
 	def do_POST(self):
 		"""Serve a POST request."""
 		self.range = None, None
 
-
 		path = self.translate_path(self.path)
 		# DIRECTORY DONT CONTAIN SLASH / AT END
 
 		url_path, query, fragment = self.url_path, self.query, self.fragment
 		spathsplit = self.url_path.split("/")
 
-
 		try:
 			for case, func in self.handlers['POST']:
 				if self.test_req(*case):
 					try:
-						f = func(self, url_path=url_path, query=query, fragment=fragment, path=path, spathsplit=spathsplit)
+						f = func(self, url_path=url_path, query=query,
+								 fragment=fragment, path=path, spathsplit=spathsplit)
 					except PostError:
 						traceback.print_exc()
-						break # break if error is raised and send BAD_REQUEST (at end of loop)
+						# break if error is raised and send BAD_REQUEST (at end of loop)
+						break
 
 					if f:
 						try:
 							self.copyfile(f, self.wfile)
 						except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
-							logger.info(tools.text_box(e.__class__.__name__, e,"\nby ", [self.address_string()]))
+							logger.info(tools.text_box(
+								e.__class__.__name__, e, "\nby ", [self.address_string()]))
 						finally:
 							f.close()
 					return
 
-
-
 			return self.send_error(HTTPStatus.BAD_REQUEST, "Invalid request.")
 
 		except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
-			logger.info(tools.text_box(e.__class__.__name__, e,"\nby ", [self.address_string()]))
+			logger.info(tools.text_box(e.__class__.__name__,
+						e, "\nby ", [self.address_string()]))
 			return
 		except Exception as e:
 			traceback.print_exc()
 			self.send_error(500, str(e))
 			return
 
-
 	def redirect(self, location):
 		'''redirect to location'''
 		self.send_response(HTTPStatus.FOUND)
 		self.send_header("Location", location)
 		self.end_headers()
 
 	def return_txt(self, code, msg, content_type="text/html; charset=utf-8"):
@@ -1149,26 +1116,30 @@
 		self.end_headers()
 		return f
 
 	def send_txt(self, code, msg, content_type="text/html; charset=utf-8"):
 		'''sends the head and file to client'''
 		f = self.return_txt(code, msg, content_type)
 		if self.command == "HEAD":
-			return # to avoid sending file on get request
+			return  # to avoid sending file on get request
 		self.copyfile(f, self.wfile)
 		f.close()
 
+	def send_text(self, code, msg, content_type="text/html; charset=utf-8"):
+		'''proxy to send_txt'''
+		self.send_txt(code, msg, content_type)
+
 	def send_json(self, obj):
 		"""send object as json
 		obj: json-able object or json.dumps() string"""
 		if not isinstance(obj, str):
 			obj = json.dumps(obj, indent=1)
 		f = self.return_txt(200, obj, content_type="application/json")
 		if self.command == "HEAD":
-			return # to avoid sending file on get request
+			return  # to avoid sending file on get request
 		self.copyfile(f, self.wfile)
 		f.close()
 
 	def return_file(self, path, filename=None, download=False):
 		f = None
 		is_attachment = "attachment;" if (self.query("dl") or download) else ""
 
@@ -1214,70 +1185,65 @@
 				first = self.range[0]
 				if first is None:
 					first = 0
 				last = self.range[1]
 				if last is None or last >= file_len:
 					last = file_len - 1
 
-				if first >= file_len: # PAUSE AND RESUME SUPPORT
+				if first >= file_len:  # PAUSE AND RESUME SUPPORT
 					self.send_error(416, 'Requested Range Not Satisfiable')
 					return None
 
 				self.send_response(206)
 				self.send_header('Content-Type', ctype)
 				self.send_header('Accept-Ranges', 'bytes')
 
-
 				response_length = last - first + 1
 
 				self.send_header('Content-Range',
-								'bytes %s-%s/%s' % (first, last, file_len))
+								 'bytes %s-%s/%s' % (first, last, file_len))
 				self.send_header('Content-Length', str(response_length))
 
-
-
 			else:
 				self.send_response(HTTPStatus.OK)
 				self.send_header("Content-Type", ctype)
 				self.send_header("Content-Length", str(file_len))
 
 			self.send_header("Last-Modified",
-							self.date_time_string(fs.st_mtime))
-			self.send_header("Content-Disposition", is_attachment+'filename="%s"' % (os.path.basename(path) if filename is None else filename))
+							 self.date_time_string(fs.st_mtime))
+			self.send_header("Content-Disposition", is_attachment+' filename="%s"' %
+							 (os.path.basename(path) if filename is None else filename))
 			self.end_headers()
 
 			return f
 
 		except PermissionError:
 			self.send_error(HTTPStatus.FORBIDDEN, "Permission denied")
 			return None
 
 		except OSError:
 			self.send_error(HTTPStatus.NOT_FOUND, "File not found")
 			return None
 
-
 		except Exception:
 			traceback.print_exc()
 
 			# if f and not f.closed(): f.close()
 			raise
 
 	def send_file(self, path, filename=None, download=False):
 		'''sends the head and file to client'''
 		f = self.return_file(path, filename, download)
 		if self.command == "HEAD":
-			return # to avoid sending file on get request
+			return  # to avoid sending file on get request
 		try:
 			self.copyfile(f, self.wfile)
 		finally:
 			f.close()
 
-
-
 	def send_head(self):
 		"""Common code for GET and HEAD commands.
 
 		This sends the response code and MIME headers.
 
 		Return value is either a file object (which has to be copied
 		to the outputfile by the caller unless the command was HEAD,
@@ -1298,86 +1264,75 @@
 			except ValueError as e:
 				self.send_error(400, 'Invalid byte range')
 				return None
 
 		path = self.translate_path(self.path)
 		# DIRECTORY DONT CONTAIN SLASH / AT END
 
-
 		url_path, query, fragment = self.url_path, self.query, self.fragment
 
 		spathsplit = self.url_path.split("/")
 
-
-
-		for case, func in self.handlers['HEAD']: # GET WILL Also BE HANDLED BY HEAD
+		# GET WILL Also BE HANDLED BY HEAD
+		for case, func in self.handlers['HEAD']:
 			if self.test_req(*case):
 				return func(self, url_path=url_path, query=query, fragment=fragment, path=path, spathsplit=spathsplit)
 
 		return self.send_error(HTTPStatus.NOT_FOUND, "File not found")
 
-
-
-
 	def get_displaypath(self, url_path):
 		"""
 		Helper to produce a display path for the directory listing.
 		"""
 
 		try:
-			displaypath = urllib.parse.unquote(url_path, errors='surrogatepass')
+			displaypath = urllib.parse.unquote(
+				url_path, errors='surrogatepass')
 		except UnicodeDecodeError:
 			displaypath = urllib.parse.unquote(url_path)
 		displaypath = html.escape(displaypath, quote=False)
 
 		return displaypath
 
-
-
-
-
-
 	def get_rel_path(self, filename):
 		"""Return the relative path to the file, FOR OS."""
 		return urllib.parse.unquote(posixpath.join(self.url_path, filename), errors='surrogatepass')
 
-
 	def translate_path(self, path):
 		"""Translate a /-separated PATH to the local filename syntax.
 
 		Components that mean special things to the local file system
 		(e.g. drive or directory names) are ignored.  (XXX They should
 		probably be diagnosed.)
 
 		"""
 		# abandon query parameters
-		path = path.split('?',1)[0]
-		path = path.split('#',1)[0]
+		path = path.split('?', 1)[0]
+		path = path.split('#', 1)[0]
 		# Don't forget explicit trailing slash when normalizing. Issue17324
 		trailing_slash = path.rstrip().endswith('/')
 
 		try:
 			path = urllib.parse.unquote(path, errors='surrogatepass')
 		except UnicodeDecodeError:
 			path = urllib.parse.unquote(path)
 		path = posixpath.normpath(path)
 		words = path.split('/')
 		words = filter(None, words)
 		path = self.directory
 
-
 		for word in words:
 			if os.path.dirname(word) or word in (os.curdir, os.pardir):
 				# Ignore components that are not a simple file/directory name
 				continue
 			path = os.path.join(path, word)
 		if trailing_slash:
 			path += '/'
 
-		return os.path.normpath(path) # fix OS based path issue
+		return os.path.normpath(path)  # fix OS based path issue
 
 	def copyfile(self, source, outputfile):
 		"""Copy all data between two file objects.
 
 		The SOURCE argument is a file object open for reading
 		(or anything with a read() method) and the DESTINATION
 		argument is a file object open for writing (or
@@ -1386,30 +1341,28 @@
 		The only reason for overriding this would be to change
 		the block size or perhaps to replace newlines by CRLF
 		-- note however that this the default server uses this
 		to copy binary data as well.
 
 		"""
 
-
 		if not self.range:
 			try:
 				source.read(1)
 			except:
 				traceback.print_exc()
 			source.seek(0)
 			shutil.copyfileobj(source, outputfile)
 
 		else:
 			# SimpleHTTPRequestHandler uses shutil.copyfileobj, which doesn't let
 			# you stop the copying before the end of the file.
 			start, stop = self.range  # set in send_head()
 			copy_byte_range(source, outputfile, start, stop)
 
-
 	def guess_type(self, path):
 		"""Guess the type of a file.
 
 		Argument is a PATH (a filename).
 
 		Return value is a string of the form type/subtype,
 		usable for a MIME Content-type header.
@@ -1427,22 +1380,68 @@
 		ext = ext.lower()
 		if ext in self.extensions_map:
 			return self.extensions_map[ext]
 		guess, _ = mimetypes.guess_type(path)
 		if guess:
 			return guess
 
-		return self.extensions_map[''] #return 'application/octet-stream'
-
+		return self.extensions_map['']  # return 'application/octet-stream'
 
 
 class PostError(Exception):
 	pass
 
 
+class ContentDisposition:
+	def __init__(self, content_disposition):
+		self.content_disposition = content_disposition
+		self.items = {}
+		self.parse()
+
+	def parse(self):
+		# Content-Disposition: form-data; name="post-type"
+		# Content-Disposition: form-data; name="file"; filename="C:\Users\user\Desktop\test.txt"
+		# Content-Disposition: form-data; name="file"; filename*=utf-8''%E6%B5%8B%E8%AF%95.txt
+
+		line = re.subn(r"Content-Disposition:", "",
+					   self.content_disposition, flags=re.IGNORECASE, count=1)[0]
+
+		# form-data; name="post-type"
+		# form-data; name="file"; filename="C:\Users\user\Desktop\test.txt"
+		# form-data; name="file"; filename*=utf-8''%E6%B5%8B%E8%AF%95.txt
+		parts = (i.strip() for i in line.split(";") if i.strip())
+
+		# form-data
+		# name="post-type"
+		# name="file"
+		# filename="C:\Users\user\Desktop\test.txt"
+		# filename*=utf-8''%E6%B5%8B%E8%AF%95.txt
+
+		for part in parts:
+			pair = [i.strip() for i in part.split("=", 1)]
+
+			key = pair[0]
+			value = pair[1] if len(pair) > 1 else ""
+
+			if key.lower() == "filename*" and value.lower().startswith("utf-8''"):
+				value = urllib.parse.unquote(
+					value[7:], encoding="utf-8", errors='surrogatepass')
+
+				key = "filename"
+
+			self.items[key.lower()] = value.strip('"')
+
+	def get(self, key, default=None):
+		return self.items.get(key.lower(), default)
+
+	def __getitem__(self, key):
+		return self.items[key.lower()]
+
+	def __contains__(self, key):
+		return key.lower() in self.items
 
 
 class DealPostData:
 	"""do_login
 
 #get starting boundary
 0: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa\r\n'
@@ -1456,162 +1455,384 @@
 8: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa\r\n'
 9: b'Content-Disposition: form-data; name="password"\r\n'
 10: b'\r\n'
 11: b'ccc\r\n'
 12: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa--\r\n'
 """
 
-
 	boundary = b''
 	num = 0
 	remainbytes = 0
 
-	def __init__(self, req:SimpleHTTPRequestHandler) -> None:
+	def __init__(self, req: SimpleHTTPRequestHandler) -> None:
+		"""After init, must call start() to get boundary and content_length"""
 		self.req = req
+		self.content_length = 0
+		self.content_type = ""
 
+		self.form = FormData(req, self, fake=True)
 
 	refresh = "<br><br><div class='pagination center' onclick='window.location.reload()'>Refresh &#128259;</div>"
 
+	def is_multipart(self):
+		return self.content_type.startswith("multipart/form-data")
 
-	def get(self, show=F, strip=F, Timeout=20):
+	def is_urlencoded(self):
+		return self.content_type.startswith("application/x-www-form-urlencoded")
+
+	def is_form_data(self):
+		return self.is_urlencoded() or self.is_multipart()
+
+	def is_json(self):
+		return self.content_type == "application/json"
+
+	def check_size_limit(self, max_size=-1):
+		"""
+		* check if content size is within limit
+		* return True if within limit
+		"""
+		if not max_size < 0 or self.content_length <= max_size:
+			raise PostError(
+				f"Content size limit exceeded: {self.content_length} > {max_size}")
+
+	def get(self, show=F, strip=F, Timeout=20, chunk_size=0):
 		"""
 		show: print line
 		strip: strip \r\n at end
 		Timeout: if having network issue on any side, will keep trying to get content until Timeout (in seconds)
 		"""
 		req = self.req
 
+		if self.remainbytes <= 0:
+			return b""
+
+		if chunk_size <= 0:
+			chunk_size = self.remainbytes
 
 		for _ in range(Timeout*2):
-			line = req.rfile.readline()
+			if self.is_multipart():
+				line = req.rfile.readline()
+			else:
+				line = req.rfile.read(chunk_size)
 			if line:
 				break
 			time.sleep(.5)
 		else:
 			raise ConnectionAbortedError
-		self.num+=1
+
 		if show:
 			print(f"{self.num}: {line}")
 		self.remainbytes -= len(line)
+		self.num += 1
 
-		if strip and line.endswith(b"\r\n"):
+		if strip and self.is_multipart() and line.endswith(b"\r\n"):
 			line = line.rpartition(b"\r\n")[0]
 
 		return line
 
-	def pass_bound(self):
-		line = self.get()
-		if not self.boundary in line:
-			self.req.log_error("Content NOT begin with boundary\n", [line, self.boundary])
+	def get_content(self, max_size=-1, chunk_size=0):
+		"""
+		* get content if not multipart
+		* return content
+		"""
 
-	def get_name(self, line=None, ):
-		if not line:
-			line = self.get()
-		try:
-			return re.findall(r'Content-Disposition.*name="(.*?)"', line.decode())[0]
-		except: return None
+		self.check_size_limit(max_size=max_size)
+
+		n = self.remainbytes
+		line = b""
+
+		while n > 0:
+			chunk = n % 1024
+			n -= chunk
 
-	def match_name(self, field_name:Union[None, str]=None):
+			_line = self.get(chunk_size=chunk)
+			if not _line:
+				break
+			line += _line
+
+		return line
+
+	def get_json(self, max_size=-1):
 		"""
-		field_name: name of the field (str)
-		* if None, skip checking field name
-		* if `empty string`, field name must be empty too
+		* get json data
+		* return parsed json data
 		"""
-		line = self.get()
 
-		if field_name is not None and self.get_name(line)!=field_name:
-			raise PostError(f"Invalid request: Expected {field_name} but got {self.get_name(line)}")
+		if not self.content_type == "application/json":
+			raise PostError("Content-Type is not application/json")
 
-		return line
+		line = self.get_content(max_size=max_size)
 
+		return json.loads(line)
 
 	def skip(self,):
 		self.get()
 
 	def start(self):
 		'''reads upto line 0'''
 		req = self.req
-		content_type = req.headers['content-type']
+		self.content_type = req.headers['content-type']
 
-		if not content_type:
-			raise PostError("Content-Type header doesn't contain boundary")
-		self.boundary = content_type.split("=")[1].encode()
+		if not self.content_type:
+			raise PostError("POST request without Content-Type")
+		if self.is_multipart():
+			self.boundary = self.content_type.split("=")[1].encode()
 
 		self.remainbytes = int(req.headers['content-length'])
+		self.content_length = self.remainbytes
+
+		# print(f"Content-Type: {self.content_type}")
+		# print(f"Content-Length: {self.content_length}")
+		# print(f"Request-header: {req.headers}")
+		# print(self.is_form_data())
+
+		if self.is_form_data():
+			self.form = FormData(req, self)
+
+
+class FormData:
+	"""
+	Handler for
+	`multipart/form-data` and
+	`application/x-www-form-urlencoded`
+	"""
+
+	def __init__(self, req: SimpleHTTPRequestHandler, dpd: DealPostData, fake=False) -> None:
+		"""
+		must be initialized from DealPostData
+		"""
+		self.req = req
+		self.dpd = dpd
+		self.fake = fake
+
+		self.content_length = dpd.content_length
+		self.content_type = dpd.content_type
+
+		if self.fake:
+			return
+		self.is_multipart = self.dpd.is_multipart()
+		self.boundary = dpd.boundary
+		if self.is_multipart:
+			# pass first boundary line (because after every field, there is a boundary line)
+			self.pass_bound()
+
+	def pass_bound(self):
+		"""
+		* pass boundary line in multipart
+		* raise error if boundary not found
+		"""
+		if self.fake:
+			raise PostError("Fake FormData")
+
+		if not self.is_multipart:
+			raise PostError("Not multipart")
+
+		line = self.dpd.get()
+		if not self.boundary in line:
+			self.req.log_error(f"Content boundary missing on line {self.dpd.num}\n", [
+							   line, self.boundary])
+
+	def get_a_dline(self, line: Union[bytes, str, None] = None):
+		"""
+		* get a line if not provided
+		* decoded if its in bytes
+		* return decoded line
+		"""
+		if self.fake:
+			raise PostError("Fake FormData")
+		# only these 2 needs fake check
+
+		if not line:
+			line = self.dpd.get()
+
+		if isinstance(line, bytes):
+			line = line.decode()
+
+		return line
+
+	def get_file_name(self, line: Union[bytes, str, None] = None):
+		"""
+		* get file name from Content-Disposition
+		* return file name
+		"""
+		line = self.get_a_dline(line)
+
+		cd = ContentDisposition(line)
+		fn = cd.get('filename')
+
+		if not fn:
+			raise PostError("Can't find out file name...")
+
+		return fn
 
+	def get_field_name(self, line=None):
+		"""
+		* get field name from Content-Disposition
+		* return field name
+		"""
+		line = self.get_a_dline(line)
+
+		# get name from Content-Disposition
+		return ContentDisposition(line).get('name')
+
+	def match_field_name(self, field_name: Union[None, str] = None):
+		"""
+		field_name: Expecting name of the field (str)
+		* if None, skip checking field name
+		* if `empty string`, field name must be empty too
+		"""
+		line = self.dpd.get()
+		got_field_name = self.get_field_name(line)
 
-		self.pass_bound()# LINE 0
+		if field_name is not None and got_field_name != field_name:
+			raise PostError(
+				f"Invalid request: Expected {field_name} but got {got_field_name}")
 
+		return line
 
-	def get_part(self, verify_name:Union[None, bytes, str] =None, verify_msg:Union[None, bytes, str] =None, decode=F):
+	def get_multi_field(self, verify_name: Union[None, bytes, str] = None, verify_msg: Union[None, bytes, str] = None, decode=F):
 		'''read a form field
 		ends at boundary
 		verify_name: name of the field (str|bytes|None)
 		verify_msg: message to verify (str|bytes)
 		decode: decode the message
 		* if None, skip checking field name
-		* if `empty string`, field name must be empty too'''
+		* if `empty string`, field name must be empty too
+
+		returns: field `(name, value)` (str|bytes)
+		'''
 		decoded = False
 
 		if isinstance(verify_name, bytes):
 			verify_name = verify_name.decode()
 
-		field_name = self.match_name(verify_name) # LINE 1 (field name)
+		# LINE 0 (boundary)
+		field_name = self.match_field_name(verify_name)  # LINE 1 (field name)
 		# if not verified, raise PostError
 
-		self.skip() # LINE 2 (blank line)
+		self.dpd.skip()  # LINE 2 (blank line)
 
 		line = b''
 		while 1:
-			_line = self.get() # from LINE 4 till boundary (form field value)
-			if self.boundary in _line: # boundary
+			_line = self.dpd.get()  # from LINE 3 till boundary (form field value)
+			if (not _line) or (self.boundary in _line):  # boundary
 				break
 			line += _line
 
-		line = line.rpartition(b"\r\n")[0] # remove \r\n at end
+		line = line.rpartition(b"\r\n")[0]  # remove \r\n at end
 		if decode:
 			line = line.decode()
 			decoded = True
 		if verify_msg is not None:
 			if not decoded:
 				if isinstance(verify_msg, str):
 					verify_msg = verify_msg.encode()
 
 			if line != verify_msg:
-				raise PostError(f"Invalid post request.\n Expected: {[verify_msg]}\n Got: {[line]}")
+				raise PostError(
+					f"Invalid post request.\n Expected: {[verify_msg]}\n Got: {[line]}")
 
 		# self.pass_bound() # LINE 5 (boundary)
 
 		return field_name, line
 
+	def get_urlencoded_field(self, verify_name: Union[None, bytes, str] = None, verify_msg: Union[None, bytes, str] = None):
+		"""
+		* get a field from form data
+		* return decoded name, value
+
+		"""
+		line = b""
+		data = self.dpd.get(chunk_size=1)
+		while data or data == b"&":
+			line += data
+
+			data = self.dpd.get(chunk_size=1)
+
+		name, value = line.split(b"=", 1)
+		# URL decode
+		name, value = urllib.parse.unquote(name), urllib.parse.unquote(value)
+
+		if verify_name is not None:
+			if isinstance(verify_name, bytes):
+				verify_name = verify_name.decode()
+
+			if name != verify_name:
+				raise PostError(
+					f"Invalid post request.\n Expected: {verify_name}\n Got: {name}")
+
+		if verify_msg is not None:
+			if isinstance(verify_msg, bytes):
+				verify_msg = verify_msg.decode()
+
+			if value != verify_msg:
+				raise PostError(
+					f"Invalid post request.\n Expected: {verify_msg}\n Got: {value}")
+		return name, value
+
+	def get_urlencoded_iter(self, max_size=-1):
+		"""
+		Generator that yields the parts of the form data as dict.
+		"""
+
+		self.dpd.check_size_limit(max_size)
+
+		data = self.dpd.get().decode()
+		for part in data.split("&"):
+			name, value = part.split("=")
+			name, value = urllib.parse.unquote(
+				name), urllib.parse.unquote(value)
+
+			yield name, value
+
+	def get_multipart_iter(self, max_size=-1):
+		"""
+		Generator that yields the parts of the form data as dict.
+		"""
 
+		self.dpd.check_size_limit(max_size)
 
+		while True:
+			field_name, value = self.get_multi_field(decode=True)
+			yield field_name, value
 
+	def get_parts(self, max_size=-1):
+		"""
+		Generator that yields the parts of the form data.
+		"""
+		if self.is_multipart:
+			g = self.get_multipart_iter
+		else:
+			g = self.get_urlencoded_iter
+
+		for part in g(max_size):
+			yield part
 
 
 def _get_best_family(*address):
 	infos = socket.getaddrinfo(
 		*address,
 		type=socket.SOCK_STREAM,
 		flags=socket.AI_PASSIVE
 	)
 	family, type, proto, canonname, sockaddr = next(iter(infos))
 	return family, sockaddr
 
+
 def get_ip(bind=None):
-	IP = bind # or "127.0.0.1"
+	IP = bind  # or "127.0.0.1"
 	s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 	s.settimeout(0)
 	try:
 		# doesn't even have to be reachable
 		s.connect(('10.255.255.255', 1))
 		IP = s.getsockname()[0]
 	except:
 		try:
-			if config.OS=="Android":
+			if config.OS == "Android":
 				IP = s.connect(("192.168.43.1",  1))
 				IP = s.getsockname()[0]
 				# Assigning this variable because Android does't return actual IP when hosting a hotspot
 		except (socket.herror, OSError):
 			pass
 	finally:
 		s.close()
@@ -1624,118 +1845,113 @@
 	"""Test the HTTP request handler class.
 
 	This runs an HTTP server on port 8000 (or the port argument).
 
 	"""
 
 	global httpd
-	if sys.version_info>=(3,8): # BACKWARD COMPATIBILITY
+	if sys.version_info >= (3, 8):  # BACKWARD COMPATIBILITY
 		ServerClass.address_family, addr = _get_best_family(bind, port)
 	else:
-		addr =(bind if bind!=None else '', port)
+		addr = (bind if bind != None else '', port)
 
 	device_ip = bind or "127.0.0.1"
 	# bind can be None (=> 127.0.0.1) or a string (=> 127.0.0.DDD)
 
 	HandlerClass.protocol_version = protocol
 	httpd = ServerClass(addr, HandlerClass)
 	host, port = httpd.socket.getsockname()[:2]
 	url_host = f'[{host}]' if ':' in host else host
 	hostname = socket.gethostname()
 	local_ip = config.IP if config.IP else get_ip(device_ip)
-	config.IP= local_ip
+	config.IP = local_ip
 
-
-	on_network = local_ip!=(device_ip)
+	on_network = local_ip != (device_ip)
 
 	logger.info(tools.text_box(
-		f"Serving HTTP on {host} port {port} \n", #TODO: need to check since the output is "Serving HTTP on :: port 6969"
-		f"(http://{url_host}:{port}/) ...\n", #TODO: need to check since the output is "(http://[::]:6969/) ..."
+		# TODO: need to check since the output is "Serving HTTP on :: port 6969"
+		f"Serving HTTP on {host} port {port} \n",
+		# TODO: need to check since the output is "(http://[::]:6969/) ..."
+		f"(http://{url_host}:{port}/) ...\n",
 		f"Server is probably running on\n",
 		(f"[over NETWORK] {config.address()}\n" if on_network else ""),
-		f"[on DEVICE] http://localhost:{config.port} & http://127.0.0.1:{config.port}"
-		, style="star", sep=""
-		)
+		f"[on DEVICE] http://localhost:{config.port} & http://127.0.0.1:{config.port}", style="star", sep=""
+	)
 	)
 	try:
 		httpd.serve_forever(poll_interval=0.1)
 	except KeyboardInterrupt:
 		logger.info("\nKeyboard interrupt received, exiting.")
 
 	except OSError:
 		logger.info("\nOSError received, exiting.")
 	finally:
 		if not config.reload:
 			sys.exit(0)
 
 
-class DualStackServer(ThreadingHTTPServer): # UNSUPPORTED IN PYTHON 3.7
+class DualStackServer(ThreadingHTTPServer):  # UNSUPPORTED IN PYTHON 3.7
 
 	def handle_error(self, request, client_address):
 		pass
 
 	def server_bind(self):
 		# suppress exception when protocol is IPv4
 		with contextlib.suppress(Exception):
 			self.socket.setsockopt(
 				socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
 		return super().server_bind()
 
 	def finish_request(self, request, client_address):
-			self.RequestHandlerClass(request, client_address, self,
-									directory=config.ftp_dir)
+		self.RequestHandlerClass(request, client_address, self,
+								 directory=config.ftp_dir)
 
 
-
-
-def run(port = None, directory = None, bind = None, arg_parse= True, handler = SimpleHTTPRequestHandler):
+def run(port=0, directory="", bind="", arg_parse=True, handler=SimpleHTTPRequestHandler):
 
 	if arg_parse:
-		args = config.parse_default_args(port=port, directory=directory, bind=bind)
+		args = config.parse_default_args(
+			port=port, directory=directory, bind=bind)
 
 		port = args.port
 		directory = args.directory
 		bind = args.bind
 
-
-
-	logger.info(tools.text_box("Running pyroboxCore: ", config.MAIN_FILE, "Version: ", __version__))
-
+	logger.info(tools.text_box("Running pyroboxCore: ",
+				config.MAIN_FILE, "Version: ", __version__))
 
 	if directory == config.ftp_dir and not os.path.isdir(config.ftp_dir):
-		logger.warning(config.ftp_dir, "not found!\nReseting directory to current directory")
+		logger.warning(
+			config.ftp_dir, "not found!\nReseting directory to current directory")
 		directory = "."
 
 	handler_class = partial(handler,
-								directory=directory)
+							directory=directory)
 
 	config.port = port
 	if port > 65535 or port < 0:
 		raise ValueError("Port must be between 0 and 65535")
 
 	config.ftp_dir = directory
 
 	if not config.reload:
-		if sys.version_info>(3,8):
+		if sys.version_info > (3, 8):
 			test(
-			HandlerClass=handler_class,
-			ServerClass=DualStackServer,
-			port=port,
-			bind=bind,
+				HandlerClass=handler_class,
+				ServerClass=DualStackServer,
+				port=port,
+				bind=bind,
 			)
-		else: # BACKWARD COMPATIBILITY
+		else:  # BACKWARD COMPATIBILITY
 			test(
-			HandlerClass=handler_class,
-			ServerClass=ThreadingHTTPServer,
-			port=port,
-			bind=bind,
+				HandlerClass=handler_class,
+				ServerClass=ThreadingHTTPServer,
+				port=port,
+				bind=bind,
 			)
 
-
 	if config.reload == True:
 		reload_server()
 
 
-
-
 if __name__ == '__main__':
 	run()
```

### Comparing `pyrobox-0.7.4/src/server.py` & `pyrobox-0.8.0/src/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
-enc = "utf-8"
+
+# TODO
+# ----------------------------------------------------------------
+# * ADD MORE FILE TYPES
+# * ADD SEARCH
 
 import html
 from string import Template
 import os
 import sys
 import posixpath
 import shutil
@@ -28,23 +32,26 @@
 import string
 import json
 from http import HTTPStatus
 
 import traceback
 import atexit
 
-from .pyroboxCore import config, logger, SimpleHTTPRequestHandler as SH_base, DealPostData as DPD, run as run_server, tools, Callable_dict, reload_server, __version__
-from .arg_parser import main as arg_parser
-from .fs_utils import get_titles, dir_navigator, get_dir_size, get_dir_m_time, get_stat, get_tree_count_n_size, _get_tree_path_n_size, fmbytes, humanbytes
+from .pyroboxCore import config, logger, SimpleHTTPRequestHandler as SH_base, DealPostData as DPD, run as run_server, tools, reload_server, __version__
 
-from . import page_templates as pt
+from ._fs_utils import get_titles, dir_navigator, get_dir_size, get_dir_m_time, get_stat, get_tree_count_n_size, _get_tree_path_n_size, fmbytes, humanbytes
+from ._arg_parser import main as arg_parser
+from . import _page_templates as pt
+from ._exceptions import LimitExceed
+from ._zipfly_manager import ZIP_Manager
 
 __version__ = __version__
 true = T = True
 false = F = False
+enc = "utf-8"
 
 ###########################################
 # ADD COMMAND LINE ARGUMENTS
 ###########################################
 arg_parser(config)
 cli_args = config.parser.parse_known_args()[0]
 config.PASSWORD = cli_args.password
@@ -64,32 +71,20 @@
 			"delete": False,
 			"download": False,
 			"upload": False,
 			"new_folder": False,
 			"rename": False,
 })
 
+########## ZIP MANAGER ################################
+config.max_zip_size = 6*1024*1024*1024
+zip_manager = ZIP_Manager(config, size_limit=config.max_zip_size)
 
-# FEATURES
-# ----------------------------------------------------------------
-# * PAUSE AND RESUME
-# * UPLOAD WITH PASSWORD
-# * FOLDER DOWNLOAD (uses temp folder)
-# * VIDEO PLAYER
-# * DELETE FILE FROM REMOTEp (RECYCLE BIN) # PERMANENTLY DELETE IS VULNERABLE
-# * File manager like NAVIGATION BAR
-# * RELOAD SERVER FROM REMOTE [DEBUG PURPOSE]
-# * MULTIPLE FILE UPLOAD
-# * FOLDER CREATION
-# * Pop-up messages (from my Web leach repo)
+#######################################################
 
-# TODO
-# ----------------------------------------------------------------
-# * ADD MORE FILE TYPES
-# * ADD SEARCH
 
 
 # INSTALL REQUIRED PACKAGES
 REQUEIREMENTS= ['send2trash', 'natsort']
 
 
 
@@ -156,17 +151,18 @@
 	def send_error(self, code, message=None, explain=None):
 		print("ERROR", code, message, explain)
 
 		displaypath = self.get_displaypath(self.url_path)
 
 		title = get_titles(displaypath)
 
-		_format = pt.error_page().safe_substitute(PY_PAGE_TITLE=title,
-													PY_PUBLIC_URL=config.address(),
-													PY_DIR_TREE_NO_JS=dir_navigator(displaypath))
+		_format = pt.error_page().safe_substitute(
+			PY_PAGE_TITLE=title,
+			PY_PUBLIC_URL=config.address(),
+			PY_DIR_TREE_NO_JS=dir_navigator(displaypath))
 
 		return super().send_error(code, message, explain, Template(_format))
 
 
 
 
 #############################################
@@ -329,170 +325,26 @@
 
 	r.append(pt.file_list().safe_substitute())
 
 	if not (cli_args.no_upload or cli_args.read_only or cli_args.view_only):
 
 		r.append(pt.upload_form().safe_substitute(PY_PUBLIC_URL=config.address()))
 
-	r.append(pt.js_script().safe_substitute(PY_LINK_LIST=str(r_li),
+	r.append(pt.file_list_script().safe_substitute(PY_LINK_LIST=str(r_li),
 										PY_FILE_LIST=str(f_li),
 										PY_FILE_SIZE =str(s_li)))
 
 
 	encoded = '\n'.join(r).encode(enc, 'surrogateescape')
 
 	return self.send_txt(HTTPStatus.OK, encoded)
 
 
 
 
-#############################################
-#               ZIP INITIALIZE              #
-#############################################
-
-from .zipfly_local import ZipFly
-
-class ZIP_Manager:
-	def __init__(self) -> None:
-		self.zip_temp_dir = tempfile.gettempdir() + '/zip_temp/'
-		self.zip_ids = Callable_dict()
-		self.zip_path_ids = Callable_dict()
-		self.zip_in_progress = Callable_dict()
-		self.zip_id_status = Callable_dict()
-
-		self.assigend_zid = Callable_dict()
-
-		self.cleanup()
-		atexit.register(self.cleanup)
-
-		self.init_dir()
-
-
-	def init_dir(self):
-		os.makedirs(self.zip_temp_dir, exist_ok=True)
-
-
-	def cleanup(self):
-		shutil.rmtree(self.zip_temp_dir, ignore_errors=True)
-
-	def get_id(self, path, size=None):
-		source_size = size if size else get_dir_size(path, must_read=True)
-		source_m_time = get_dir_m_time(path)
-
-		exist = 1
-
-		prev_zid, prev_size, prev_m_time = 0,0,0
-		if self.zip_path_ids(path):
-			prev_zid, prev_size, prev_m_time = self.zip_path_ids[path]
-
-		elif self.assigend_zid(path):
-			prev_zid, prev_size, prev_m_time = self.assigend_zid[path]
-
-		else:
-			exist=0
-
-
-		if exist and prev_m_time == source_m_time and prev_size == source_size:
-			return prev_zid
-
-
-		id = ''.join(random.choice(string.ascii_uppercase + string.digits) for _ in range(6))+'_'+ str(time.time())
-		id += '0'*(25-len(id))
-
-
-		self.assigend_zid[path] = (id, source_size, source_m_time)
-		return id
-
-
-
-
-	def archive(self, path, zid, size=None):
-		"""
-		archive the folder
-
-		`path`: path to archive
-		`zid`: id of the folder
-		`size`: size of the folder (optional)
-		"""
-		def err(msg):
-			self.zip_in_progress.pop(zid, None)
-			self.assigend_zid.pop(path, None)
-			self.zip_id_status[zid] = "ERROR: " + msg
-			return False
-		if config.disabled_func["zip"]:
-			return err("ZIP FUNTION DISABLED")
-
-
-
-
-		# run zipfly
-		self.zip_in_progress[zid] = 0
-
-		fs = _get_tree_path_n_size(path, must_read=True, path_type="both")
-		source_size = sum(i[1] for i in fs)
-		fm = [i[0] for i in fs]
-
-		if len(fm)==0:
-			return err("FOLDER HAS NO FILES")
-
-		source_m_time = get_dir_m_time(path)
-
-
-		dir_name = os.path.basename(path)
-
-
-
-		zfile_name = os.path.join(self.zip_temp_dir, "{dir_name}({zid})".format(dir_name=dir_name, zid=zid) + ".zip")
-
-		self.init_dir()
-
-
-		paths = []
-		for i,j in fm:
-			paths.append({"fs": i, "n":j})
-
-		zfly = ZipFly(paths = paths, chunksize=0x80000)
-
-
-
-		archived_size = 0
-
-		self.zip_id_status[zid] = "ARCHIVING"
-
-		try:
-			with open(zfile_name, "wb") as zf:
-				for chunk, c_size in zfly.generator():
-					zf.write(chunk)
-					archived_size += c_size
-					if source_size==0:
-						source_size+=1 # prevent division by 0
-					self.zip_in_progress[zid] = (archived_size/source_size)*100
-		except Exception as e:
-			traceback.print_exc()
-			return err(e)
-		self.zip_in_progress.pop(zid, None)
-		self.assigend_zid.pop(path, None)
-		self.zip_id_status[zid] = "DONE"
-
-
-
-		self.zip_path_ids[path] = zid, source_size, source_m_time
-		self.zip_ids[zid] = zfile_name
-		# zip_ids are never cleared in runtime due to the fact if someones downloading a zip, the folder content changed, other person asked for zip, new zip created and this id got removed, the 1st user wont be able to resume
-
-
-		return zid
-
-	def archive_thread(self, path, zid, size=None):
-		return threading.Thread(target=self.archive, args=(path, zid, size))
-
-zip_manager = ZIP_Manager()
-
-#---------------------------x--------------------------------
-
 
 if not os.path.isdir(config.log_location):
 	try:
 		os.mkdir(path=config.log_location)
 	except Exception:
 		config.log_location ="./"
 
@@ -679,36 +531,39 @@
 	path = kwargs.get('path', '')
 	url_path = kwargs.get('url_path', '')
 	spathsplit = kwargs.get('spathsplit', '')
 
 	if config.disabled_func["zip"]:
 		return self.return_txt(HTTPStatus.INTERNAL_SERVER_ERROR, "ERROR: ZIP FEATURE IS UNAVAILABLE !")
 
-	dir_size = get_dir_size(path, limit=6*1024*1024*1024)
+	# dir_size = get_dir_size(path, limit=6*1024*1024*1024)
 
-	if dir_size == -1:
-		msg = "Directory size is too large, please contact the host"
-		return self.return_txt(HTTPStatus.OK, msg)
+	# if dir_size == -1:
+	# 	msg = "Directory size is too large, please contact the host"
+	# 	return self.return_txt(HTTPStatus.OK, msg)
 
 	displaypath = self.get_displaypath(url_path)
 	filename = spathsplit[-2] + ".zip"
 
+	title = "Creating ZIP"
 
-	try:
-		zid = zip_manager.get_id(path, dir_size)
-		title = "Creating ZIP"
+	head = pt.directory_explorer_header().safe_substitute(PY_PAGE_TITLE=title,
+											PY_PUBLIC_URL=config.address(),
+											PY_DIR_TREE_NO_JS=dir_navigator(displaypath))
 
-		head = pt.directory_explorer_header().safe_substitute(PY_PAGE_TITLE=title,
-												PY_PUBLIC_URL=config.address(),
-												PY_DIR_TREE_NO_JS=dir_navigator(displaypath))
+	try:
+		zid = zip_manager.get_id(path)
 
 		tail = pt.zip_script().safe_substitute(PY_ZIP_ID = zid,
-		PY_ZIP_NAME = filename)
-		return self.return_txt(HTTPStatus.OK,
-		f"{head} {tail}")
+												PY_ZIP_NAME = filename)
+		return self.return_txt(HTTPStatus.OK, f"{head} {tail}")
+
+	except LimitExceed:
+		tail = "<h3>Directory size is too large, please contact the host</h3>"
+		return self.return_txt(HTTPStatus.SERVICE_UNAVAILABLE, f"{head} {tail}")
 	except Exception:
 		self.log_error(traceback.format_exc())
 		return self.return_txt(HTTPStatus.OK, "ERROR")
 
 @SH.on_req('HEAD', hasQ="zip")
 def get_zip(self: SH, *args, **kwargs):
 	"""Return ZIP file if available
@@ -732,14 +587,17 @@
 
 
 	filename = spathsplit[-2] + ".zip"
 
 	id = query["zid"][0]
 
 	# IF NOT STARTED
+	if zip_manager.calculating(id):
+		return reply("CALCULATING")
+
 	if not zip_manager.zip_id_status(id):
 		t = zip_manager.archive_thread(path, id)
 		t.start()
 
 		return reply("SUCCESS", "ARCHIVING")
 
 
@@ -890,26 +748,28 @@
 
 
 def AUTHORIZE_POST(req: SH, post:DPD, post_type=''):
 	"""Check if the user is authorized to post"""
 
 	# START
 	post.start()
+	form = post.form
 
-	verify_1 = post.get_part(verify_name='post-type', verify_msg=post_type, decode=T)
+	verify_1 = form.get_multi_field(verify_name='post-type', verify_msg=post_type, decode=T)
 
 
 	# GET UID
-	uid_verify = post.get_part(verify_name='post-uid', decode=T)
+	uid_verify = form.get_multi_field(verify_name='post-uid', decode=T)
 
-	if not uid_verify[0]:
+	uid = uid_verify[1]
+
+	if not uid:
 		raise PostError("Invalid request: No uid provided")
 
 
-	uid = uid_verify[1]
 
 
 	##################################
 
 	# HANDLE USER PERMISSION BY CHECKING UID
 
 	##################################
@@ -929,67 +789,65 @@
 
 	path = kwargs.get('path')
 	url_path = kwargs.get('url_path')
 
 
 	post = DPD(self)
 
+
 	# AUTHORIZE
 	uid = AUTHORIZE_POST(self, post, 'upload')
 
+	form = post.form
+
 	if not uid:
 		return None
 
 
 	uploaded_files = [] # Uploaded folder list
 
 
 
 	# PASSWORD SYSTEM
-	password = post.get_part(verify_name='password', decode=T)[1]
+	password = form.get_multi_field(verify_name='password', decode=T)[1]
 
 	self.log_debug(f'post password: {[password]} by client')
 	if password != config.PASSWORD: # readline returns password with \r\n at end
 		self.log_info(f"Incorrect password by {uid}")
 
 		return self.send_txt(HTTPStatus.UNAUTHORIZED, "Incorrect password")
 
 	while post.remainbytes > 0:
-		line = post.get()
-
-		fn = re.findall(r'Content-Disposition.*name="file"; filename="(.*)"', line.decode())
+		fn = form.get_file_name() # reads the next line and returns the file name
 		if not fn:
 			return self.send_error(HTTPStatus.BAD_REQUEST, "Can't find out file name...")
 
 
 		path = self.translate_path(self.path)
-		rltv_path = posixpath.join(url_path, fn[0])
-
-		if len(fn[0])==0:
-			return self.send_txt(HTTPStatus.BAD_REQUEST, "Invalid file name")
+		rltv_path = posixpath.join(url_path, fn)
 
 		temp_fn = os.path.join(path, ".LStemp-"+fn[0]+'.tmp')
 		config.temp_file.add(temp_fn)
 
 
-		fn = os.path.join(path, fn[0])
+		fn = os.path.join(path, fn)
 
 
 
-		line = post.get(F) # content type
-		line = post.get(F) # line gap
+		line = post.get() # content type
+		line = post.get() # line gap
 
 
 
 		# ORIGINAL FILE STARTS FROM HERE
 		try:
 			with open(temp_fn, 'wb') as out:
-				preline = post.get(F)
+				preline = post.get()
 				while post.remainbytes > 0:
-					line = post.get(F)
+					line = post.get()
 					if post.boundary in line:
 						preline = preline[0:-1]
 						if preline.endswith(b'\r'):
 							preline = preline[0:-1]
 						out.write(preline)
 						uploaded_files.append(rltv_path,)
 						break
@@ -1038,22 +896,23 @@
 	url_path = kwargs.get('url_path')
 
 
 	post = DPD(self)
 
 	# AUTHORIZE
 	uid = AUTHORIZE_POST(self, post, 'del-f')
+	form = post.form
 
 	if config.disabled_func["send2trash"]:
 		return self.send_json({"head": "Failed", "body": "Recycling unavailable! Try deleting permanently..."})
 
 
 
 	# File link to move to recycle bin
-	filename = post.get_part(verify_name='name', decode=T)[1].strip()
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
 
 	path = self.get_rel_path(filename)
 	xpath = self.translate_path(posixpath.join(url_path, filename))
 
 	self.log_warning(f'<-send2trash-> {xpath} by {[uid]}')
 
 	head = "Failed"
@@ -1083,19 +942,20 @@
 	url_path = kwargs.get('url_path')
 
 
 	post = DPD(self)
 
 	# AUTHORIZE
 	uid = AUTHORIZE_POST(self, post, 'del-p')
+	form = post.form
 
 
 
 	# File link to move to recycle bin
-	filename = post.get_part(verify_name='name', decode=T)[1].strip()
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
 	path = self.get_rel_path(filename)
 
 	xpath = self.translate_path(posixpath.join(url_path, filename))
 
 	self.log_warning(f'Perm. DELETED {xpath} by {[uid]}')
 
 
@@ -1128,21 +988,22 @@
 	url_path = kwargs.get('url_path')
 
 
 	post = DPD(self)
 
 	# AUTHORIZE
 	uid = AUTHORIZE_POST(self, post, 'rename')
+	form = post.form
 
 
 
 	# File link to move to recycle bin
-	filename = post.get_part(verify_name='name', decode=T)[1].strip()
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
 
-	new_name = post.get_part(verify_name='data', decode=T)[1].strip()
+	new_name = form.get_multi_field(verify_name='data', decode=T)[1].strip()
 
 	path = self.get_rel_path(filename)
 
 
 	xpath = self.translate_path(posixpath.join(url_path, filename))
 
 
@@ -1170,21 +1031,22 @@
 	script = None
 
 
 	post = DPD(self)
 
 	# AUTHORIZE
 	uid = AUTHORIZE_POST(self, post, 'info')
+	form = post.form
 
 
 
 
 
 	# File link to move to check info
-	filename = post.get_part(verify_name='name', decode=T)[1].strip()
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
 
 	path = self.get_rel_path(filename) # the relative path of the file or folder
 
 	xpath = self.translate_path(posixpath.join(url_path, filename)) # the absolute path of the file or folder
 
 
 	self.log_warning(f'Info Checked "{xpath}" by: {[uid]}')
@@ -1279,16 +1141,17 @@
 	path = kwargs.get('path')
 	url_path = kwargs.get('url_path')
 
 	post = DPD(self)
 
 	# AUTHORIZE
 	uid = AUTHORIZE_POST(self, post, 'new_folder')
+	form = post.form
 
-	filename = post.get_part(verify_name='name', decode=T)[1].strip()
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
 
 	path = self.get_rel_path(filename)
 
 	xpath = filename
 	if xpath.startswith(('../', '..\\', '/../', '\\..\\')) or '/../' in xpath or '\\..\\' in xpath or xpath.endswith(('/..', '\\..')):
 		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + path})
```

