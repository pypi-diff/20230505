# Comparing `tmp/aw-client-0.5.8.tar.gz` & `tmp/aw-client-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aw-client-0.5.8.tar", max compression
+gzip compressed data, was "aw-client-0.5.9.tar", max compression
```

## Comparing `aw-client-0.5.8.tar` & `aw-client-0.5.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    16726 2017-04-17 08:45:00.980472 aw-client-0.5.8/LICENSE.txt
--rw-r--r--   0        0        0     2792 2022-02-03 12:08:06.173023 aw-client-0.5.8/README.md
--rw-r--r--   0        0        0       48 2020-12-06 12:39:36.544625 aw-client-0.5.8/aw_client/__init__.py
--rw-r--r--   0        0        0       38 2019-03-04 09:02:29.668408 aw-client-0.5.8/aw_client/__main__.py
--rw-r--r--   0        0        0     1643 2021-11-22 13:23:24.726652 aw-client-0.5.8/aw_client/classes.py
--rwxr-xr-x   0        0        0     8447 2022-02-03 12:00:36.532258 aw-client-0.5.8/aw_client/cli.py
--rw-r--r--   0        0        0    15464 2022-03-03 08:19:34.223602 aw-client-0.5.8/aw_client/client.py
--rw-r--r--   0        0        0      326 2021-06-15 11:42:05.321369 aw-client-0.5.8/aw_client/config.py
--rw-r--r--   0        0        0        1 2021-05-12 09:46:26.642626 aw-client-0.5.8/aw_client/py.typed
--rw-r--r--   0        0        0     9180 2022-02-03 11:44:31.426215 aw-client-0.5.8/aw_client/queries.py
--rw-r--r--   0        0        0     1605 2022-02-03 11:50:56.686555 aw-client-0.5.8/aw_client/singleinstance.py
--rw-r--r--   0        0        0      955 2022-03-03 09:09:15.164839 aw-client-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3702 2022-03-03 09:10:39.974311 aw-client-0.5.8/setup.py
--rw-r--r--   0        0        0     3664 2022-03-03 09:10:39.974822 aw-client-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    16726 2017-04-17 08:45:00.980472 aw-client-0.5.9/LICENSE.txt
+-rw-r--r--   0        0        0     2792 2022-02-03 12:08:06.173023 aw-client-0.5.9/README.md
+-rw-r--r--   0        0        0       48 2020-12-06 12:39:36.544625 aw-client-0.5.9/aw_client/__init__.py
+-rw-r--r--   0        0        0       38 2019-03-04 09:02:29.668408 aw-client-0.5.9/aw_client/__main__.py
+-rw-r--r--   0        0        0     1643 2021-11-22 13:23:24.726652 aw-client-0.5.9/aw_client/classes.py
+-rwxr-xr-x   0        0        0     8447 2022-02-03 12:00:36.532258 aw-client-0.5.9/aw_client/cli.py
+-rw-r--r--   0        0        0    15655 2022-03-03 10:23:40.276340 aw-client-0.5.9/aw_client/client.py
+-rw-r--r--   0        0        0      326 2021-06-15 11:42:05.321369 aw-client-0.5.9/aw_client/config.py
+-rw-r--r--   0        0        0        1 2021-05-12 09:46:26.642626 aw-client-0.5.9/aw_client/py.typed
+-rw-r--r--   0        0        0     9180 2022-02-03 11:44:31.426215 aw-client-0.5.9/aw_client/queries.py
+-rw-r--r--   0        0        0     1605 2022-02-03 11:50:56.686555 aw-client-0.5.9/aw_client/singleinstance.py
+-rw-r--r--   0        0        0      955 2022-03-03 10:24:52.080297 aw-client-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3702 2022-03-03 10:28:38.474037 aw-client-0.5.9/setup.py
+-rw-r--r--   0        0        0     3664 2022-03-03 10:28:38.474384 aw-client-0.5.9/PKG-INFO
```

### Comparing `aw-client-0.5.8/LICENSE.txt` & `aw-client-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aw-client-0.5.8/README.md` & `aw-client-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `aw-client-0.5.8/aw_client/classes.py` & `aw-client-0.5.9/aw_client/classes.py`

 * *Files identical despite different names*

### Comparing `aw-client-0.5.8/aw_client/cli.py` & `aw-client-0.5.9/aw_client/cli.py`

 * *Files identical despite different names*

### Comparing `aw-client-0.5.8/aw_client/client.py` & `aw-client-0.5.9/aw_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,18 +135,24 @@
     #   Event get/post requests
     #
 
     def get_event(
         self,
         bucket_id: str,
         event_id: int,
-    ) -> Event:
+    ) -> Optional[Event]:
         endpoint = f"buckets/{bucket_id}/events/{event_id}"
-        event = self._get(endpoint).json()
-        return Event(**event)
+        try:
+            event = self._get(endpoint).json()
+            return Event(**event)
+        except req.exceptions.HTTPError as e:
+            if e.response.status_code == 404:
+                return None
+            else:
+                raise
 
     def delete_event(
         self,
         bucket_id: str,
         event_id: int,
     ) -> None:
         endpoint = f"buckets/{bucket_id}/events/{event_id}"
```

### Comparing `aw-client-0.5.8/aw_client/queries.py` & `aw-client-0.5.9/aw_client/queries.py`

 * *Files identical despite different names*

### Comparing `aw-client-0.5.8/aw_client/singleinstance.py` & `aw-client-0.5.9/aw_client/singleinstance.py`

 * *Files identical despite different names*

### Comparing `aw-client-0.5.8/pyproject.toml` & `aw-client-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aw-client"
-version = "0.5.8"
+version = "0.5.9"
 description = "Client library for ActivityWatch"
 authors = ["Erik Bjäreholt <erik@bjareho.lt>", "Johan Bjäreholt <johan@bjareho.lt>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://activitywatch.net/"
 repository = "https://github.com/ActivityWatch/aw-client/"
 documentation = "https://docs.activitywatch.net/"
```

### Comparing `aw-client-0.5.8/setup.py` & `aw-client-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'typing-extensions']
 
 entry_points = \
 {'console_scripts': ['aw-client = aw_client.cli:main']}
 
 setup_kwargs = {
     'name': 'aw-client',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'Client library for ActivityWatch',
     'long_description': 'aw-client\n=========\n\n[![GitHub Actions badge](https://github.com/ActivityWatch/aw-client/workflows/Build/badge.svg)](https://github.com/ActivityWatch/aw-client/actions)\n[![PyPI](https://img.shields.io/pypi/v/aw-client)](https://pypi.org/project/aw-client/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Typechecking: Mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n\nClient library for ActivityWatch in Python.\n\nPlease see [the documentation][docs] for usage, and take a look at `examples/`.\n\n - [Documentation][docs]\n - [API Reference][apiref]\n\n[docs]: https://docs.activitywatch.net/en/latest/\n[apiref]: https://docs.activitywatch.net/en/latest/api/python.html#aw-client\n\n## How to install\n\nInstall from pip: `pip install aw-client`\n\nInstall the latest version directly from github without cloning: `pip install git+https://github.com/ActivityWatch/aw-client.git`\n\nTo install from a cloned version:\n\n - clone repo: `git clone https://github.com/ActivityWatch/aw-client.git`\n - cd into the directory: `cd aw-client`\n - run `poetry install` (will create a virtualenv, if none activated)\n   - If you don\'t want to use poetry you can also use `pip install .`, but that might not get the exact version of the dependencies (due to not reading the `poetry.lock` file).\n\n## Usage\n\nFor the CLI:\n\n```\n$ aw-client --help\nUsage: aw-client [OPTIONS] COMMAND [ARGS]...\n\n  CLI utility for aw-client to aid in interacting with the ActivityWatch\n  server\n\nOptions:\n  --host TEXT     Address of host\n  --port INTEGER  Port to use\n  -v, --verbose   Verbosity\n  --testing       Set to use testing ports by default\n  --help          Show this message and exit.\n\nCommands:\n  buckets    List all buckets\n  canonical  Query \'canonical events\' for a single host (filtered,...\n  events     Query events from bucket with ID `bucket_id`\n  heartbeat  Send a heartbeat to bucket with ID `bucket_id` with JSON `data`\n  query      Run a query in file at `path` on the server\n  report     Generate an activity report\n```\n\n\n## Debugging\n\n* Run python with `LOG_LEVEL=debug` to get additional debugging output\n* If invalid events have been queued for submission, you may need to delete the file-based queues generated by this library\n* To use the development version of this library use `aw-client = {path = "../aw-client" }` in `pyproject.toml`\n\n## Examples\n\nThe `examples/` directory contains a couple of example scripts, including:\n\n - `time_spent_today.py` - fetches all non-afk events and sums their duration to get the total active time for the day.\n - `merge_buckets.py` - merges two buckets with non-intersecting events by moving all events from one into the other.\n - `redact_sensitive.py` - redact sensitive events.\n',
     'author': 'Erik Bjäreholt',
     'author_email': 'erik@bjareho.lt',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://activitywatch.net/',
```

### Comparing `aw-client-0.5.8/PKG-INFO` & `aw-client-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aw-client
-Version: 0.5.8
+Version: 0.5.9
 Summary: Client library for ActivityWatch
 Home-page: https://activitywatch.net/
 License: MPL-2.0
 Author: Erik Bjäreholt
 Author-email: erik@bjareho.lt
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved
```

