# Comparing `tmp/volvo-jira-0.1.1.tar.gz` & `tmp/volvo-jira-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volvo-jira-0.1.1.tar", last modified: Thu May  4 12:22:03 2023, max compression
+gzip compressed data, was "volvo-jira-0.1.3.tar", last modified: Fri May  5 15:33:02 2023, max compression
```

## Comparing `volvo-jira-0.1.1.tar` & `volvo-jira-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.577893 volvo-jira-0.1.1/
--rw-r--r--   0 PROBERT4   (502) staff       (20)     1075 2023-04-18 07:10:23.000000 volvo-jira-0.1.1/LICENSE
--rw-r--r--   0 PROBERT4   (502) staff       (20)      947 2023-05-04 12:22:03.578033 volvo-jira-0.1.1/PKG-INFO
--rw-r--r--   0 PROBERT4   (502) staff       (20)      280 2023-04-28 16:17:04.000000 volvo-jira-0.1.1/README.md
--rw-r--r--   0 PROBERT4   (502) staff       (20)      457 2023-05-02 15:16:53.000000 volvo-jira-0.1.1/pyproject.toml
--rw-r--r--   0 PROBERT4   (502) staff       (20)     1068 2023-05-04 12:22:03.584249 volvo-jira-0.1.1/setup.cfg
--rw-r--r--   0 PROBERT4   (502) staff       (20)       69 2023-04-18 07:13:11.000000 volvo-jira-0.1.1/setup.py
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.553365 volvo-jira-0.1.1/src/
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.566498 volvo-jira-0.1.1/src/vira/
--rw-r--r--   0 PROBERT4   (502) staff       (20)      149 2023-04-28 15:58:32.000000 volvo-jira-0.1.1/src/vira/__init__.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)        0 2023-04-18 07:34:47.000000 volvo-jira-0.1.1/src/vira/py.typed
--rw-r--r--   0 PROBERT4   (502) staff       (20)     2421 2023-05-03 11:00:44.000000 volvo-jira-0.1.1/src/vira/vira_add_parent.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     1178 2023-04-27 16:12:57.000000 volvo-jira-0.1.1/src/vira/vira_base.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     3325 2023-05-03 10:42:14.000000 volvo-jira-0.1.1/src/vira/vira_copy.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     6709 2023-05-03 10:48:47.000000 volvo-jira-0.1.1/src/vira/vira_deep_copy.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)      559 2023-05-03 14:47:20.000000 volvo-jira-0.1.1/src/vira/vira_error.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     3173 2023-05-03 15:16:54.000000 volvo-jira-0.1.1/src/vira/vira_issue.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     1483 2023-04-28 15:14:01.000000 volvo-jira-0.1.1/src/vira/vira_script_utils.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)    18705 2023-05-03 17:33:47.000000 volvo-jira-0.1.1/src/vira/vira_vira.py
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.572608 volvo-jira-0.1.1/src/volvo_jira.egg-info/
--rw-r--r--   0 PROBERT4   (502) staff       (20)      947 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/PKG-INFO
--rw-r--r--   0 PROBERT4   (502) staff       (20)      643 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/SOURCES.txt
--rw-r--r--   0 PROBERT4   (502) staff       (20)        1 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/dependency_links.txt
--rw-r--r--   0 PROBERT4   (502) staff       (20)      136 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/entry_points.txt
--rw-r--r--   0 PROBERT4   (502) staff       (20)        1 2023-05-03 17:00:24.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/not-zip-safe
--rw-r--r--   0 PROBERT4   (502) staff       (20)       81 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/requires.txt
--rw-r--r--   0 PROBERT4   (502) staff       (20)        5 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/top_level.txt
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.577002 volvo-jira-0.1.1/tests/
--rw-r--r--   0 PROBERT4   (502) staff       (20)     2683 2023-04-28 09:40:42.000000 volvo-jira-0.1.1/tests/test_connection.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     4996 2023-05-03 16:08:47.000000 volvo-jira-0.1.1/tests/test_issue.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)      317 2023-04-18 11:44:54.000000 volvo-jira-0.1.1/tests/test_logging.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     1526 2023-05-03 11:06:38.000000 volvo-jira-0.1.1/tests/test_scripts.py
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-05 15:33:02.592314 volvo-jira-0.1.3/
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1075 2023-04-18 07:10:23.000000 volvo-jira-0.1.3/LICENSE
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      899 2023-05-05 15:33:02.592458 volvo-jira-0.1.3/PKG-INFO
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      280 2023-04-28 16:17:04.000000 volvo-jira-0.1.3/README.md
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      457 2023-05-02 15:16:53.000000 volvo-jira-0.1.3/pyproject.toml
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1031 2023-05-05 15:33:02.593501 volvo-jira-0.1.3/setup.cfg
+-rw-r--r--   0 PROBERT4   (502) staff       (20)       69 2023-04-18 07:13:11.000000 volvo-jira-0.1.3/setup.py
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-05 15:33:02.521429 volvo-jira-0.1.3/src/
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-05 15:33:02.565835 volvo-jira-0.1.3/src/vira/
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      205 2023-05-04 12:34:47.000000 volvo-jira-0.1.3/src/vira/__init__.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)        0 2023-04-18 07:34:47.000000 volvo-jira-0.1.3/src/vira/py.typed
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     2421 2023-05-03 11:00:44.000000 volvo-jira-0.1.3/src/vira/vira_add_parent.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1178 2023-04-27 16:12:57.000000 volvo-jira-0.1.3/src/vira/vira_base.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     3339 2023-05-04 12:36:49.000000 volvo-jira-0.1.3/src/vira/vira_copy.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     6733 2023-05-04 12:32:12.000000 volvo-jira-0.1.3/src/vira/vira_deep_copy.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      606 2023-05-04 12:40:12.000000 volvo-jira-0.1.3/src/vira/vira_error.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     3173 2023-05-05 10:55:09.000000 volvo-jira-0.1.3/src/vira/vira_issue.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1483 2023-04-28 15:14:01.000000 volvo-jira-0.1.3/src/vira/vira_script_utils.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)    18154 2023-05-05 11:19:04.000000 volvo-jira-0.1.3/src/vira/vira_vira.py
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-05 15:33:02.578645 volvo-jira-0.1.3/src/volvo_jira.egg-info/
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      899 2023-05-05 15:33:02.000000 volvo-jira-0.1.3/src/volvo_jira.egg-info/PKG-INFO
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      643 2023-05-05 15:33:02.000000 volvo-jira-0.1.3/src/volvo_jira.egg-info/SOURCES.txt
+-rw-r--r--   0 PROBERT4   (502) staff       (20)        1 2023-05-05 15:33:02.000000 volvo-jira-0.1.3/src/volvo_jira.egg-info/dependency_links.txt
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      136 2023-05-05 15:33:02.000000 volvo-jira-0.1.3/src/volvo_jira.egg-info/entry_points.txt
+-rw-r--r--   0 PROBERT4   (502) staff       (20)        1 2023-05-03 17:00:24.000000 volvo-jira-0.1.3/src/volvo_jira.egg-info/not-zip-safe
+-rw-r--r--   0 PROBERT4   (502) staff       (20)       81 2023-05-05 15:33:02.000000 volvo-jira-0.1.3/src/volvo_jira.egg-info/requires.txt
+-rw-r--r--   0 PROBERT4   (502) staff       (20)        5 2023-05-05 15:33:02.000000 volvo-jira-0.1.3/src/volvo_jira.egg-info/top_level.txt
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-05 15:33:02.591837 volvo-jira-0.1.3/tests/
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     2759 2023-05-05 15:32:01.000000 volvo-jira-0.1.3/tests/test_connection.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     4992 2023-05-04 12:30:34.000000 volvo-jira-0.1.3/tests/test_issue.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      317 2023-04-18 11:44:54.000000 volvo-jira-0.1.3/tests/test_logging.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1505 2023-05-04 12:30:54.000000 volvo-jira-0.1.3/tests/test_scripts.py
```

### Comparing `volvo-jira-0.1.1/LICENSE` & `volvo-jira-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.1/PKG-INFO` & `volvo-jira-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: volvo-jira
-Version: 0.1.1
+Version: 0.1.3
 Summary: Volvo JIRA (VIRA) package and helper scripts. Contains scripts for deep copy, change parent and more
 Author: Per-Ola Robertsson
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE
 
 # VIRA
 A python project to handle VIRA (Volvo Cars version of JIRA) issues.
```

### Comparing `volvo-jira-0.1.1/setup.cfg` & `volvo-jira-0.1.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [metadata]
 name = volvo-jira
-version = 0.1.1
+version = 0.1.3
 description = Volvo JIRA (VIRA) package and helper scripts. Contains scripts for deep copy, change parent and more
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 author = Per-Ola Robertsson
 license = MIT
 license_files = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = 
 	vira
 install_requires = 
 	jira>=3
-python_requires = >=3.8
+python_requires = >=3.11
 package_dir = 
 	=src
 zip_safe = no
 entry_points = 
 	[console_scripts]
 	vira_deep_copy=vira.vira_deep_copy:main
 	vira_copy=vira.vira_copy:main
@@ -38,13 +37,13 @@
 	flake8>=3.9
 	tox>=3.24
 
 [options.package_data]
 vira = py.typed
 
 [flake8]
-max-line-length = 160
+max-line-length = 180
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `volvo-jira-0.1.1/src/vira/vira_add_parent.py` & `volvo-jira-0.1.3/src/vira/vira_add_parent.py`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.1/src/vira/vira_base.py` & `volvo-jira-0.1.3/src/vira/vira_base.py`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.1/src/vira/vira_copy.py` & `volvo-jira-0.1.3/src/vira/vira_copy.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         description=f"{SCRIPT_NAME} {SCRIPT_VERSION}. Deep Copies a VIRA issue. Created by {SCRIPT_AURTOUR}.\nRelease notes:\n{SCRIPT_RELEASE_NOTES}"
     )
 
     parser.add_argument("src_issue", help="The issue to copy from")
     parser.add_argument(
         "-p",
         "--parent_issue",
-        help="If specified the copy will be added to the parent. Need to be a one level up issuetype as the --src_issue aragument. If not specified the copy will not have a parent",
+        help="If specified the copy will be added to the parent. Need to be a one level up issuetype as the --src_issue aragument. \
+            If not specified the copy will not have a parent",
     )
 
     vira_script_utils.add_common_arguments(parser)
 
     # Parse the arguments
     args = parser.parse_args()
```

### Comparing `volvo-jira-0.1.1/src/vira/vira_deep_copy.py` & `volvo-jira-0.1.3/src/vira/vira_deep_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,25 +58,27 @@
         description=f"{SCRIPT_NAME} {SCRIPT_VERSION}. Deep Copies a VIRA issue. Created by {SCRIPT_AUTHOUR}"
     )
 
     parser.add_argument("src_issue", help="The issue to copy from")
     parser.add_argument(
         "-p",
         "--parent_issue",
-        help="If specified only sub issues of --src_issue will be copied to this issue. Need to be of same VIRA issuetype as the --src_issue aragument. If not specified a complete deep copy of --src_issue will be done.",
+        help="If specified only sub issues of --src_issue will be copied to this issue. Need to be of \
+        same VIRA issuetype as the --src_issue aragument. If not specified a complete deep copy of --src_issue will be done.",
     )
     parser.add_argument(
         "-c",
         "--capability_replace_text",
         help="Replaces the <capability> string of the template issues with this text. Tip: Use the name of the capability",
     )
     parser.add_argument(
         "-sm",
         "--sm_replace_text",
-        help="Replaces the <SM> string of the template issues with this text. Tip: Use the name of a Specific Module (node) that is part of the capability. Example: HP, HI, EthSw, SGA, VIU",
+        help="Replaces the <SM> string of the template issues with this text. \
+            Tip: Use the name of a Specific Module (node) that is part of the capability. Example: HP, HI, EthSw, SGA, VIU",
     )
     parser.add_argument(
         "-version",
         "--version",
         action="store_true",
         help="Detailed version information. Exits after printing",
     )
```

### Comparing `volvo-jira-0.1.1/src/vira/vira_error.py` & `volvo-jira-0.1.3/src/vira/vira_error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from jira import JIRAError
 
+
 class VIRAError(Exception):
     """Exception raised for generic VIRA errors.
 
     Attributes:
         message -- The error message
         status_code -- The error status code. Can be None
         jira_exception -- The underlying JIRA error (JIRAError). Can be None
     """
 
     def __init__(
-        self, message: str, *, status_code: int = None, jira_error: JIRAError = None
+        self,
+        message: str,
+        *,
+        status_code: int | None = None,
+        jira_error: JIRAError | None = None
     ):
         self.message = message
         self.status_code = status_code
         self.jira_error = jira_error
         super().__init__(self.message)
```

### Comparing `volvo-jira-0.1.1/src/vira/vira_issue.py` & `volvo-jira-0.1.3/src/vira/vira_issue.py`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.1/src/vira/vira_script_utils.py` & `volvo-jira-0.1.3/src/vira/vira_script_utils.py`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.1/src/vira/vira_vira.py` & `volvo-jira-0.1.3/src/vira/vira_vira.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import getpass
 from jira import JIRA
 from jira import JIRAError
 from vira.vira_base import getViraLogger, get_os_identifier
 from vira.vira_issue import VIRAIssue
 from vira.vira_error import VIRAError
 import os
 
@@ -11,26 +12,25 @@
 
 g_logger = getViraLogger()
 
 
 class VIRA:
     """Represent a VIRA instance."""
 
-    def __init__(self, vira_url: str = None):
+    def __init__(self, vira_url: str | None = None):
         """If vira_url is not provided, the VIRA_URL environment variable is used."""
-        self._jira = None
+        # self._jira = None
         if vira_url is None:
             vira_url = os.environ.get("VIRA_URL")
         assert vira_url is not None
         self.vira_url = vira_url
-        self.dry_run = False
         self.create_comment = None
         self.replacements = None
 
-    def connect_with_token(self, *, token: str = None):
+    def connect_with_token(self, *, token: str | None = None):
         # Connects to Jira/Vira using Personal Authentication Token (PAT)
         """If token is not provided, the VIRA_ACCESS_TOKEN environment variable is used."""
         if token is None:
             token = os.environ.get("VIRA_ACCESS_TOKEN")
         try:
             self._jira = JIRA(server=self.vira_url, token_auth=token)
         except JIRAError as e:
@@ -54,30 +54,30 @@
                     jira_error=e,
                 )
 
         g_logger.info(
             f"Connected to {self.vira_url} using PAT. OS:{get_os_identifier()}"
         )
 
-    def connect(self, *, user: str = None, password: str = None):
+    def connect(self, *, user: str | None = None, password: str | None = None):
         """If a parameter is not provided, the corresponding OS environment variable is used. If these are not found the user is prompted to enter the
         URL and credentials.
         After a sucessfull connection, the values are stored as OS environemnt variables. Next call will then not need to specify a URL and credentials
 
         VIRA_USER,
         VIRA_PASSWORD
         """
         if user is None:
             user = os.environ.get("VIRA_USER")
         if password is None:
             password = os.environ.get("VIRA_PASSWORD")
         if user is None:
             user = input("Please enter your VIRA username:")
         if password is None:
-            password = input("Please enter your VIRA password:")
+            password = getpass.getpass(prompt="Please enter your VIRA password:")
 
         # Connects to Jira/Vira
         try:
             self._jira = JIRA(server=self.vira_url, auth=(user, password))
         except JIRAError as e:
             raise VIRAError(
                 f'Could not connect to VIRA server "{self.vira_url}" as "{user}".',
@@ -116,15 +116,15 @@
             return src_str
 
         for matching, replacement in self.replacements:
             src_str = src_str.replace(matching, replacement)
         return src_str
 
     def can_be_child_to_parent(
-        self, *, parent_issue: VIRAIssue, child_issue: VIRAIssue
+        self, *, parent_issue: VIRAIssue | None, child_issue: VIRAIssue
     ):
         if parent_issue is None:
             return (True, "")
 
         if child_issue.is_feature:
             if not parent_issue.is_capability:
                 return (
@@ -255,72 +255,61 @@
             dst_field_value = {"id": src_field_value.id}
         else:
             g_logger.warning(f"Unhandled type: {type(src_field_value)}")
             dst_field_value = src_field_value
 
         return dst_field_value
 
-    def set_dry_run(self, dry_run=True):
-        self.dry_run = dry_run
-
     def set_create_comment(self, comment):
         self.create_comment = comment
 
-    def create_issue(self, issue_dict: dict):
-        if not self.dry_run:
-            try:
-                new_jira_issue = self._jira.create_issue(fields=issue_dict)
-            except JIRAError as e:
-                g_logger.error(
-                    f"Could not create issue. Details:\n{e.response.status_code} {e.response.content}",
-                    extra={"no_console": True},
-                )
-                raise VIRAError(
-                    "Could not create issue",
-                    status_code=e.response.status_code,
-                    jira_error=e,
-                )
-            if self.create_comment is not None:
-                self._jira.add_comment(new_jira_issue, self.create_comment)
-            new_issue = VIRAIssue(new_jira_issue, self._jira)
-            g_logger.debug(f"Created issue {new_issue.short_str}")
-            return new_issue
-        g_logger.debug(f"Simulated the creation of issue {issue_dict}")
-        return None
+    def create_issue(self, issue_dict: dict) -> VIRAIssue:
+        try:
+            new_jira_issue = self._jira.create_issue(fields=issue_dict)
+        except JIRAError as e:
+            g_logger.error(
+                f"Could not create issue. Details:\n{e.response.status_code} {e.response.content}",
+                extra={"no_console": True},
+            )
+            raise VIRAError(
+                "Could not create issue",
+                status_code=e.response.status_code,
+                jira_error=e,
+            )
+        if self.create_comment is not None:
+            self._jira.add_comment(new_jira_issue, self.create_comment)
+        new_issue = VIRAIssue(new_jira_issue, self._jira)
+        g_logger.debug(f"Created issue {new_issue.short_str}")
+        return new_issue
 
-    def copy_issue_by_key(self, src_issue_key: str, *, parent_issue_key: str = None):
+    def copy_issue_by_key(
+        self, src_issue_key: str, *, parent_issue_key: str | None = None
+    ):
         src_issue = self.get_issue(src_issue_key)
         parent_issue = None
         if parent_issue_key is not None:
             parent_issue = self.get_issue(parent_issue_key)
 
         return self.copy_issue(src_issue=src_issue, parent_issue=parent_issue)
 
     def copy_issue(
-        self, src_issue: VIRAIssue, *, parent_issue: VIRAIssue = None
+        self, src_issue: VIRAIssue, *, parent_issue: VIRAIssue | None = None
     ) -> VIRAIssue:
         """Copies a single issue from another. If parent_issue is supplied it will make the copy a child of the parent issue.
         parent_issue must be one hirarcial level up of src_issue."""
 
         # Check that this is possible so that it will not fail after we made the copy (that can't be undone)
         can_be_child, error_str = self.can_be_child_to_parent(
             child_issue=src_issue, parent_issue=parent_issue
         )
         if not can_be_child:
             raise VIRAError(error_str)
 
         dst_summary = self.replace_strings(src_issue.fields.summary)
 
-        if self.dry_run:
-            log_str = f'Dry run: Would have copied {src_issue.indent_str}{src_issue.short_str} but changed the summary to "{dst_summary}"'
-            if parent_issue is not None:
-                log_str += f" and added it as child to {parent_issue.short_str}"
-            g_logger.debug(log_str, extra={"console_only": True})
-            return None
-
         # TODO(probert4) Check these
         read_only_fields = [
             "lastViewed",
             "creator",
             "customfield_15100",
             "subtasks",
             "created",
@@ -408,15 +397,15 @@
         if parent_issue is not None:
             log_string += f" and made it child to {parent_issue.short_str}"
         g_logger.info(log_string)
 
         return new_issue
 
     def copy_issue_recursive(
-        self, src_issue: VIRAIssue, *, copy_parent_issue: VIRAIssue = None
+        self, src_issue: VIRAIssue, *, copy_parent_issue: VIRAIssue | None = None
     ) -> VIRAIssue:
         """Makes a deep copy of src_issue. If copy_parent_issue is provided then only sub-issues are copied and added to the copy_parent_issue.
         Will return the top parent of the copy. i.e. will return copy_parent_issue if not None.
         """
 
         if copy_parent_issue is None:
             copy_parent_issue = self.copy_issue(src_issue, parent_issue=None)
```

### Comparing `volvo-jira-0.1.1/src/volvo_jira.egg-info/PKG-INFO` & `volvo-jira-0.1.3/src/volvo_jira.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: volvo-jira
-Version: 0.1.1
+Version: 0.1.3
 Summary: Volvo JIRA (VIRA) package and helper scripts. Contains scripts for deep copy, change parent and more
 Author: Per-Ola Robertsson
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE
 
 # VIRA
 A python project to handle VIRA (Volvo Cars version of JIRA) issues.
```

### Comparing `volvo-jira-0.1.1/src/volvo_jira.egg-info/SOURCES.txt` & `volvo-jira-0.1.3/src/volvo_jira.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.1/tests/test_connection.py` & `volvo-jira-0.1.3/tests/test_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # Production VIRA tests
 @pytest.mark.usefixtures("no_environment_variables_set")
 def test_connection_to_production_with_cridentials(no_environment_variables_set):
     vira = VIRA(VIRA_URL)
     vira.connect(user=VIRA_TEST_USER, password=VIRA_TEST_USER_PASSWORD)
 
 
+@pytest.mark.skip("Fix this. monkeypatch can't emulate getpass.getpass() input.")
 @pytest.mark.usefixtures("no_environment_variables_set")
 def test_connection_to_production_using_console_input(
     no_environment_variables_set, monkeypatch
 ):
     inputs = iter([VIRA_TEST_USER, VIRA_TEST_USER_PASSWORD])
     monkeypatch.setattr("builtins.input", lambda _: next(inputs))
     vira = VIRA(VIRA_URL)
@@ -67,9 +68,9 @@
     with pytest.raises(VIRAError) as e_info:
         # Even with the correct environment variables set, parameters take precidence
         vira.connect(user="WrongUser", password=VIRA_TEST_USER_PASSWORD)
     assert e_info.value.status_code == 401
 
     with pytest.raises(VIRAError) as e_info:
         # Even with the correct environment variables set, parameters take precidence
-        vira.connect_with_token(token=VIRA_TEST_ACCESS_TOKEN + "Wrong")
+        vira.connect_with_token(token="WrongPersonalAccessToken")
     assert e_info.value.status_code == 401
```

### Comparing `volvo-jira-0.1.1/tests/test_issue.py` & `volvo-jira-0.1.3/tests/test_issue.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     fields = {
         "project": {"key": VIRA_PROJECT_KEY},
         "issuetype": "Story",
         "summary": "My own Story summary",
         "description": "My own Story description",
     }
 
-    vira.set_create_comment(f"This issue was created by unit test test_create_issue")
+    vira.set_create_comment("This issue was created by unit test test_create_issue")
 
     issue = vira.create_issue(fields)
 
     assert issue.fields.project.key == VIRA_PROJECT_KEY
     assert issue.fields.issuetype.name == "Story"
     assert issue.fields.summary == "My own Story summary"
     assert issue.fields.description == "My own Story description"
@@ -86,30 +86,30 @@
     assert issue.fields.status.name == "Open"
 
     assert issue.is_story
 
 
 def test_copy_issue(vira):
     src_issue = vira.get_issue("SOLSWEP-803")
-    vira.set_create_comment(f"This issue was created by unit test test_copy_issue")
+    vira.set_create_comment("This issue was created by unit test test_copy_issue")
 
     cpy_issue = vira.copy_issue(src_issue)
 
     assert cpy_issue.key != src_issue.key
     assert cpy_issue.id != src_issue.id
     assert cpy_issue.short_str != src_issue.short_str
     assert len(cpy_issue.get_children()) == 0
     assert cpy_issue.fields.project.key == src_issue.fields.project.key
     assert cpy_issue.fields.summary == src_issue.fields.summary
     assert cpy_issue.fields.description == src_issue.fields.description
     # TODO add more fileds test, status. Maybe even add a cmp overload to VIRAIssue?
 
 
 def test_deep_copy(vira, src_capability_issue):
-    vira.set_create_comment(f"This issue was created by unit test test_deep_copy")
+    vira.set_create_comment("This issue was created by unit test test_deep_copy")
     # def copy_issue_recursive(self, src_issue: VIRAIssue, *, copy_parent_issue: VIRAIssue = None) -> VIRAIssue:
     cpy_issue = vira.copy_issue_recursive(src_capability_issue)
 
     assert cpy_issue.is_capability
 
     assert cpy_issue.fields.summary == src_capability_issue.fields.summary
     assert cpy_issue.fields.description == src_capability_issue.fields.description
@@ -120,15 +120,15 @@
         src_capability_issue
     )
 
 
 def test_deep_copy_to_parent(vira, src_capability_issue):
     parent_capability_issue = vira.copy_issue_by_key("SOLSWEP-803")
     vira.set_create_comment(
-        f"This issue was created by unit test test_deep_copy_to_parent"
+        "This issue was created by unit test test_deep_copy_to_parent"
     )
     parent_n_children_before = calculate_n_children_recursive(parent_capability_issue)
 
     cpy_issue = vira.copy_issue_recursive(
         src_capability_issue, copy_parent_issue=parent_capability_issue
     )
```

### Comparing `volvo-jira-0.1.1/tests/test_scripts.py` & `volvo-jira-0.1.3/tests/test_scripts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import os
 import sys
 import pytest
-from unittest.mock import MagicMock, patch
+from unittest.mock import patch
 
 from tests.credentials import (
     VIRA_TEST_URL,
     VIRA_TEST_ACCESS_TOKEN,
 )
 
 import vira.vira_deep_copy as vira_deep_copy
```

