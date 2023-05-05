# Comparing `tmp/squirrels-0.1.0rc1.tar.gz` & `tmp/squirrels-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\squirrels-0.1.0rc1.tar", last modified: Wed Mar 22 15:14:00 2023, max compression
+gzip compressed data, was "squirrels-0.1.0rc2.tar", last modified: Fri May  5 13:53:39 2023, max compression
```

## Comparing `squirrels-0.1.0rc1.tar` & `squirrels-0.1.0rc2.tar`

### file list

```diff
@@ -1,67 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 15:14:00.000000 squirrels-0.1.0rc1/
--rw-rw-rw-   0        0        0     1269 2023-03-20 05:33:23.000000 squirrels-0.1.0rc1/.gitignore
--rw-rw-rw-   0        0        0     1087 2023-01-08 21:32:50.000000 squirrels-0.1.0rc1/LICENSE
--rw-rw-rw-   0        0        0     1396 2023-03-22 15:14:00.000000 squirrels-0.1.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0     1139 2023-03-19 16:57:12.000000 squirrels-0.1.0rc1/README.md
--rw-rw-rw-   0        0        0      114 2023-03-20 02:59:22.000000 squirrels-0.1.0rc1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/sample_project/
--rw-rw-rw-   0        0        0       16 2023-02-27 20:09:05.000000 squirrels-0.1.0rc1/sample_project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/sample_project/datasets/
--rw-rw-rw-   0        0        0      126 2023-03-05 02:09:17.000000 squirrels-0.1.0rc1/sample_project/datasets/sample_lu_data.csv
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/sample_project/datasets/stock_price_history/
--rw-rw-rw-   0        0        0     1093 2023-03-17 16:50:26.000000 squirrels-0.1.0rc1/sample_project/datasets/stock_price_history/context.py
--rw-rw-rw-   0        0        0      303 2023-03-12 15:54:54.000000 squirrels-0.1.0rc1/sample_project/datasets/stock_price_history/final_view.py
--rw-rw-rw-   0        0        0      211 2023-03-12 03:22:48.000000 squirrels-0.1.0rc1/sample_project/datasets/stock_price_history/final_view.sql.j2
--rw-rw-rw-   0        0        0     1961 2023-03-18 13:43:12.000000 squirrels-0.1.0rc1/sample_project/datasets/stock_price_history/parameters.py
--rw-rw-rw-   0        0        0      108 2023-03-12 03:03:14.000000 squirrels-0.1.0rc1/sample_project/datasets/stock_price_history/selections.cfg
--rw-rw-rw-   0        0        0      433 2023-03-12 03:03:14.000000 squirrels-0.1.0rc1/sample_project/datasets/stock_price_history/ticker_history.sql.j2
--rw-rw-rw-   0        0        0     1642 2023-03-17 15:28:39.000000 squirrels-0.1.0rc1/sample_project/functions.py
--rw-rw-rw-   0        0        0     2695 2023-03-17 15:30:27.000000 squirrels-0.1.0rc1/sample_project/parameter_options.py
--rw-rw-rw-   0        0        0       42 2023-03-22 15:14:00.000000 squirrels-0.1.0rc1/setup.cfg
--rw-rw-rw-   0        0        0     1304 2023-03-22 15:13:19.000000 squirrels-0.1.0rc1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels/
--rw-rw-rw-   0        0        0      578 2023-03-21 13:10:34.000000 squirrels-0.1.0rc1/squirrels/__init__.py
--rw-rw-rw-   0        0        0     5465 2023-03-19 20:10:45.000000 squirrels-0.1.0rc1/squirrels/api_server.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels/base_project/
--rw-rw-rw-   0        0        0       33 2023-03-21 13:14:13.000000 squirrels-0.1.0rc1/squirrels/base_project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels/base_project/database/
--rw-rw-rw-   0        0        0   188416 2023-03-18 14:11:28.000000 squirrels-0.1.0rc1/squirrels/base_project/database/seattle_weather.db
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels/base_project/datasets/
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels/base_project/datasets/sample_dataset/
--rw-rw-rw-   0        0        0      177 2023-03-20 05:41:37.000000 squirrels-0.1.0rc1/squirrels/base_project/datasets/sample_dataset/context.py
--rw-rw-rw-   0        0        0      491 2023-03-20 06:13:03.000000 squirrels-0.1.0rc1/squirrels/base_project/datasets/sample_dataset/database_view1.py
--rw-rw-rw-   0        0        0      152 2023-03-20 06:02:05.000000 squirrels-0.1.0rc1/squirrels/base_project/datasets/sample_dataset/database_view1.sql.j2
--rw-rw-rw-   0        0        0      318 2023-03-20 06:11:45.000000 squirrels-0.1.0rc1/squirrels/base_project/datasets/sample_dataset/final_view.py
--rw-rw-rw-   0        0        0       31 2023-03-20 06:10:47.000000 squirrels-0.1.0rc1/squirrels/base_project/datasets/sample_dataset/final_view.sql.j2
--rw-rw-rw-   0        0        0      224 2023-03-20 06:00:19.000000 squirrels-0.1.0rc1/squirrels/base_project/datasets/sample_dataset/parameters.py
--rw-rw-rw-   0        0        0      368 2023-03-20 07:19:32.000000 squirrels-0.1.0rc1/squirrels/base_project/squirrels.yaml
--rw-rw-rw-   0        0        0     5794 2023-03-21 13:02:34.000000 squirrels-0.1.0rc1/squirrels/command_line.py
--rw-rw-rw-   0        0        0     2007 2023-03-20 05:24:38.000000 squirrels-0.1.0rc1/squirrels/constants.py
--rw-rw-rw-   0        0        0     1336 2023-03-20 07:13:43.000000 squirrels-0.1.0rc1/squirrels/db_conn.py
--rw-rw-rw-   0        0        0     3704 2023-03-21 13:05:08.000000 squirrels-0.1.0rc1/squirrels/initializer.py
--rw-rw-rw-   0        0        0     1090 2023-03-12 05:38:34.000000 squirrels-0.1.0rc1/squirrels/manifest.py
--rw-rw-rw-   0        0        0     1233 2023-03-19 20:10:12.000000 squirrels-0.1.0rc1/squirrels/module_loader.py
--rw-rw-rw-   0        0        0    21803 2023-03-18 13:37:41.000000 squirrels-0.1.0rc1/squirrels/parameter_configs.py
--rw-rw-rw-   0        0        0     1856 2023-03-12 15:48:58.000000 squirrels-0.1.0rc1/squirrels/profile_manager.py
--rw-rw-rw-   0        0        0     9866 2023-03-20 07:01:59.000000 squirrels-0.1.0rc1/squirrels/renderer.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels/static/
--rw-rw-rw-   0        0        0     4638 2023-03-12 05:51:40.000000 squirrels-0.1.0rc1/squirrels/static/favicon.ico
--rw-rw-rw-   0        0        0     8663 2023-03-12 05:43:05.000000 squirrels-0.1.0rc1/squirrels/static/script.js
--rw-rw-rw-   0        0        0     1841 2023-03-12 03:03:14.000000 squirrels-0.1.0rc1/squirrels/static/style.css
-drwxrwxrwx   0        0        0        0 2023-03-22 15:14:00.000000 squirrels-0.1.0rc1/squirrels/templates/
--rw-rw-rw-   0        0        0     1253 2023-03-12 05:54:44.000000 squirrels-0.1.0rc1/squirrels/templates/index.html
--rw-rw-rw-   0        0        0      725 2023-03-07 01:22:12.000000 squirrels-0.1.0rc1/squirrels/templates/sandbox.html
--rw-rw-rw-   0        0        0        8 2023-03-22 15:13:19.000000 squirrels-0.1.0rc1/squirrels/version.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels.egg-info/
--rw-rw-rw-   0        0        0     1396 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1818 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-22 15:13:59.000000 squirrels-0.1.0rc1/squirrels.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 15:14:00.000000 squirrels-0.1.0rc1/tests/
--rw-rw-rw-   0        0        0      360 2023-03-19 21:59:29.000000 squirrels-0.1.0rc1/tests/conftest.py
--rw-rw-rw-   0        0        0      443 2023-03-12 05:36:35.000000 squirrels-0.1.0rc1/tests/test_db_conn.py
--rw-rw-rw-   0        0        0      593 2023-03-03 03:58:25.000000 squirrels-0.1.0rc1/tests/test_module_loader.py
--rw-rw-rw-   0        0        0     4028 2023-03-12 16:07:17.000000 squirrels-0.1.0rc1/tests/test_parameter_configs.py
--rw-rw-rw-   0        0        0      995 2023-03-12 16:11:48.000000 squirrels-0.1.0rc1/tests/test_profile_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.488018 squirrels-0.1.0rc2/
+-rw-rw-rw-   0        0        0     1088 2023-04-24 03:56:44.000000 squirrels-0.1.0rc2/LICENSE
+-rw-rw-rw-   0        0        0     2056 2023-05-05 13:53:39.486023 squirrels-0.1.0rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     1799 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 13:53:39.488018 squirrels-0.1.0rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1410 2023-04-24 03:56:44.000000 squirrels-0.1.0rc2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.392023 squirrels-0.1.0rc2/squirrels/
+-rw-rw-rw-   0        0        0     1007 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/__init__.py
+-rw-rw-rw-   0        0        0     5737 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/_command_line.py
+-rw-rw-rw-   0        0        0     6174 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/api_server.py
+-rw-rw-rw-   0        0        0     2269 2023-05-05 13:20:06.000000 squirrels-0.1.0rc2/squirrels/connection_set.py
+-rw-rw-rw-   0        0        0     1596 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/constants.py
+-rw-rw-rw-   0        0        0     3059 2023-04-22 22:12:54.000000 squirrels-0.1.0rc2/squirrels/credentials_manager.py
+-rw-rw-rw-   0        0        0     8682 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/dateutils.py
+-rw-rw-rw-   0        0        0     4283 2023-04-23 00:07:17.000000 squirrels-0.1.0rc2/squirrels/initializer.py
+-rw-rw-rw-   0        0        0     5209 2023-04-23 23:15:04.000000 squirrels-0.1.0rc2/squirrels/manifest.py
+-rw-rw-rw-   0        0        0     1261 2023-04-10 13:37:59.000000 squirrels-0.1.0rc2/squirrels/module_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.338017 squirrels-0.1.0rc2/squirrels/package_data/
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.429019 squirrels-0.1.0rc2/squirrels/package_data/base_project/
+-rw-rw-rw-   0        0        0       40 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/.gitignore
+-rw-rw-rw-   0        0        0      907 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/connections.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.435025 squirrels-0.1.0rc2/squirrels/package_data/base_project/database/
+-rw-rw-rw-   0        0        0     8192 2023-04-23 00:05:57.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/database/sample_database.db
+-rw-rw-rw-   0        0        0   188416 2023-03-18 14:11:28.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/database/seattle_weather.db
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.335032 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.459022 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/
+-rw-rw-rw-   0        0        0      296 2023-04-27 13:23:16.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/context.py
+-rw-rw-rw-   0        0        0      814 2023-04-27 13:23:30.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py
+-rw-rw-rw-   0        0        0      281 2023-04-27 13:23:34.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.sql.j2
+-rw-rw-rw-   0        0        0      299 2023-04-23 09:51:57.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/final_view.py
+-rw-rw-rw-   0        0        0       31 2023-03-20 06:10:47.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/final_view.sql.j2
+-rw-rw-rw-   0        0        0     1385 2023-04-27 13:22:31.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/parameters.py
+-rw-rw-rw-   0        0        0      142 2023-04-27 13:23:07.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/selections.cfg
+-rw-rw-rw-   0        0        0       56 2023-05-05 13:20:06.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/project_vars.yaml
+-rw-rw-rw-   0        0        0      264 2023-04-27 13:17:36.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/squirrels.yaml
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.466027 squirrels-0.1.0rc2/squirrels/package_data/static/
+-rw-rw-rw-   0        0        0     4638 2023-03-12 05:51:40.000000 squirrels-0.1.0rc2/squirrels/package_data/static/favicon.ico
+-rw-rw-rw-   0        0        0     9029 2023-04-23 18:22:58.000000 squirrels-0.1.0rc2/squirrels/package_data/static/script.js
+-rw-rw-rw-   0        0        0     1841 2023-03-12 03:03:14.000000 squirrels-0.1.0rc2/squirrels/package_data/static/style.css
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.469016 squirrels-0.1.0rc2/squirrels/package_data/templates/
+-rw-rw-rw-   0        0        0     1273 2023-04-24 03:56:44.000000 squirrels-0.1.0rc2/squirrels/package_data/templates/index.html
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.482024 squirrels-0.1.0rc2/squirrels/param_configs/
+-rw-rw-rw-   0        0        0        0 2023-04-14 00:13:00.000000 squirrels-0.1.0rc2/squirrels/param_configs/__init__.py
+-rw-rw-rw-   0        0        0    14672 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/param_configs/data_sources.py
+-rw-rw-rw-   0        0        0     8355 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/param_configs/parameter_options.py
+-rw-rw-rw-   0        0        0     1689 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/param_configs/parameter_set.py
+-rw-rw-rw-   0        0        0    18760 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/param_configs/parameters.py
+-rw-rw-rw-   0        0        0    14047 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/renderer.py
+-rw-rw-rw-   0        0        0     1148 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/timed_imports.py
+-rw-rw-rw-   0        0        0     2156 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/utils.py
+-rw-rw-rw-   0        0        0       95 2023-04-24 03:56:44.000000 squirrels-0.1.0rc2/squirrels/version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.418026 squirrels-0.1.0rc2/squirrels.egg-info/
+-rw-rw-rw-   0        0        0     2056 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1798 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       95 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `squirrels-0.1.0rc1/LICENSE` & `squirrels-0.1.0rc2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
```

### Comparing `squirrels-0.1.0rc1/setup.py` & `squirrels-0.1.0rc2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-from setuptools import setup
-from os import path
-
-with open('squirrels/version.txt') as f:
-    __version__ = f.read()
+from setuptools import setup, find_packages
+import os
 
 # The directory containing this file
-HERE = path.abspath(path.dirname(__file__))
+HERE = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
+with open(os.path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
+# Recursively get package data
+def package_files(directory):
+    paths = []
+    for (path, directories, filenames) in os.walk(directory):
+        for filename in filenames:
+            paths.append(os.path.join('..', path, filename))
+    return paths
+
+extra_files = package_files(os.path.join('squirrels', 'package_data'))
+
 setup(
     name='squirrels',
-    version=__version__,
-    packages=['squirrels'],
+    version='0.1.0rc2',
+    packages=find_packages(),
     description='Python Package for Configuring SQL Generating APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Tim Huang',
     author_email='tim.yuting@hotmail.com',
     license='MIT',
     install_requires=[
-        'inquirer', 'pwinput', 'cachetools', 'fastapi', 'uvicorn', 'Jinja2', 
-        'GitPython', 'pandasql', 'pandas', 'sqlalchemy<2', 'pyyaml'
+        'openpyxl', 'inquirer', 'pwinput', 'cachetools', 'fastapi', 'uvicorn', 
+        'Jinja2', 'GitPython', 'sqlalchemy', 'pandas', 'pyyaml'
     ],
     setup_requires=['pytest-runner==6.0.0'],
     tests_require=['pytest==7.2.0'],
     test_suite='tests',
-    package_data= {
-        'squirrels': ['static/*', 'templates/*', 'base_project/database/*', 'base_project/datasets/sample_dataset/*', 
-                      'base_project/.gitignore', 'base_project/*']
-    },
+    package_data= {'squirrels': extra_files},
     entry_points= {
-        'console_scripts': ['squirrels=squirrels.command_line:main']
+        'console_scripts': ['squirrels=squirrels._command_line:main']
     }
 )
```

### Comparing `squirrels-0.1.0rc1/squirrels/api_server.py` & `squirrels-0.1.0rc2/squirrels/api_server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,136 +1,128 @@
-import json, os
-from typing import Dict, List, FrozenSet, Tuple
+from typing import Dict, List, Tuple, Set
 from fastapi import FastAPI, Request
+from fastapi.datastructures import QueryParams
 from fastapi.responses import HTMLResponse, JSONResponse
 from fastapi.templating import Jinja2Templates
 from fastapi.staticfiles import StaticFiles
 from cachetools.func import ttl_cache
+import os, json
 
-from squirrels import major_version, constants as c, manifest as mf
-from squirrels.renderer import Renderer
-
-debug = False
-
-
-def normalize_name(name: str):
-    return name.replace('-', '_')
-
-def normalize_name_for_api(name: str):
-    return name.replace('_', '-')
-
-
-def load_selected_parameters(renderer: Renderer, query_params: FrozenSet[Tuple[str, str]]): # -> ParameterSet:
-    parameters = renderer.parameters
-    query_params_dict = dict(query_params)
-    for name, parameter in parameters._parameters_dict.items():
-        parameter.refresh(parameters)
-        selected_value = query_params_dict.get(name)
-        if selected_value is not None:
-            parameter.set_selection(selected_value)
-    return parameters
-
-
-def load_dataframe(renderer: Renderer):
-    renderer.set_job_context()
-    sql_by_view_name = renderer.get_rendered_sql_by_view()
-    
-    dataset_context = mf.get_dataset_parms(renderer.dataset)
-    final_view_name = dataset_context[c.FINAL_VIEW_KEY]
-    final_view_sql_str = renderer.get_final_view_sql_str(final_view_name, sql_by_view_name)
-    
-    _, df = renderer.get_all_results(sql_by_view_name, final_view_name, final_view_sql_str)
-    return df
-
-
-def template_function(dataset: str, request: Request, helper_func):
-    dataset = normalize_name(dataset)
-    query_params = frozenset((normalize_name(key), val) for key, val in request.query_params.items())
-    return helper_func(dataset, query_params)
-
-
-# Helper functions for "parameters" api
-def get_parameters_helper(dataset: str, query_params: FrozenSet[Tuple[str, str]]):
-    renderer = Renderer(dataset)
-    parameters = load_selected_parameters(renderer, query_params)
-    return parameters._to_dict(debug)
-    
-
-# Helper functions for "get_results" api
-def get_results_helper(dataset: str, query_params: FrozenSet[Tuple[str, str]]):
-    renderer = Renderer(dataset)
-    load_selected_parameters(renderer, query_params)
-    df = load_dataframe(renderer)
-    return json.loads(df.to_json(orient='table', index=False))
+from squirrels import major_version, constants as c, utils
+from squirrels.manifest import Manifest
+from squirrels.connection_set import ConnectionSet
+from squirrels.renderer import RendererIOWrapper, Renderer
+
+
+class ApiServer:
+    def __init__(self, manifest: Manifest, conn_set: ConnectionSet, no_cache: bool, debug: bool) -> None:
+        """
+        Constructor for ApiServer
+
+        Parameters:
+            manifest (Manifest): Manifest object produced from squirrels.yaml
+            conn_set (ConnectionSet): Set of all connection pools defined in connections.py
+            no_cache (bool): Whether to disable caching
+            debug (bool): Set to True to show "hidden" parameters in the /parameters endpoint response
+        """
+        self.manifest = manifest
+        self.conn_set = conn_set
+        self.no_cache = no_cache
+        self.debug = debug
         
+        self.datasets = manifest.get_all_dataset_names()
+        self.renderers: Dict[str, Renderer] = {}
+        for dataset in self.datasets:
+            rendererIO = RendererIOWrapper(dataset, manifest, conn_set)
+            self.renderers[dataset] = rendererIO.renderer
         
-def run(no_cache: bool, debug_value: bool, uvicorn_args: List[str]):
-    global debug
-    debug = debug_value
+    def _get_parameters_helper(self, dataset: str, query_params: Set[Tuple[str, str]]) -> Dict:
+        if len(query_params) > 1:
+            raise utils.InvalidInputError("The /parameters endpoint takes at most 1 query parameter")
+        renderer = self.renderers[dataset]
+        parameters = renderer.apply_selections(dict(query_params), updates_only = True)
+        return parameters.to_dict(self.debug)
+    
+    def _get_results_helper(self, dataset: str, query_params: Set[Tuple[str, str]]) -> Dict:
+        renderer = self.renderers[dataset]
+        _, _, _, _, df = renderer.load_results(dict(query_params))
+        return json.loads(df.to_json(orient='table', index=False))
+    
+    def _apply_dataset_api_function(self, api_function, dataset: str, raw_query_params: QueryParams):
+        dataset = utils.normalize_name(dataset)
+        query_params = set()
+        for key, val in raw_query_params.items():
+            query_params.add((utils.normalize_name(key), val))
+        query_params = frozenset(query_params)
+        return api_function(dataset, query_params)
+    
+    def run(self, uvicorn_args: List[str]) -> None:
+        """
+        Runs the API server with uvicorn for CLI "squirrels run"
+
+        Parameters:
+            uvicorn_args (List[str]): List of arguments to pass to uvicorn.run. Currently only supports "host" and "port"
+        """
+        app = FastAPI()
+
+        squirrels_version_path = f'/squirrels{major_version}'
+        config_base_path = utils.normalize_name_for_api(self.manifest.get_base_path())
+        base_path = squirrels_version_path + config_base_path
 
-    app = FastAPI()
+        static_dir = utils.join_paths(os.path.dirname(__file__), 'package_data', 'static')
+        app.mount('/static', StaticFiles(directory=static_dir), name='static')
 
-    mf.initialize(c.MANIFEST_FILE)
-    squirrels_version_path = f'/squirrels{major_version}'
-    config_base_path = normalize_name_for_api(mf.parms[c.BASE_PATH_KEY])
-    base_path = squirrels_version_path + config_base_path
+        templates_dir = utils.join_paths(os.path.dirname(__file__), 'package_data', 'templates')
+        templates = Jinja2Templates(directory=templates_dir)
 
-    static_dir = os.path.join(os.path.dirname(__file__), 'static')
-    app.mount('/static', StaticFiles(directory=static_dir), name='static')
-
-    templates_dir = os.path.join(os.path.dirname(__file__), 'templates')
-    templates = Jinja2Templates(directory=templates_dir)
-
-    # Parameters API
-    parameters_path = '/{dataset}/parameters'
-    
-    parameters_cache_size = mf.get_setting(c.PARAMETERS_CACHE_SIZE_SETTING, 1024)
-    parameters_cache_ttl = mf.get_setting(c.PARAMETERS_CACHE_TTL_SETTING, 24*60*60)
-
-    @ttl_cache(maxsize=parameters_cache_size, ttl=parameters_cache_ttl)
-    def get_parameters_cachable(*args):
-        return get_parameters_helper(*args)
-    
-    @app.get(base_path + parameters_path, response_class=JSONResponse)
-    async def get_parameters(dataset: str, request: Request):
-        helper_func = get_parameters_helper if no_cache else get_parameters_cachable
-        return template_function(dataset, request, helper_func)
-
-    # Results API
-    results_path = '/{dataset}'
-
-    results_cache_size = mf.get_setting(c.RESULTS_CACHE_SIZE_SETTING, 128)
-    results_cache_ttl = mf.get_setting(c.RESULTS_CACHE_TTL_SETTING, 60*60)
-
-    @ttl_cache(maxsize=results_cache_size, ttl=results_cache_ttl)
-    def get_results_cachable(*args):
-        return get_results_helper(*args)
-    
-    @app.get(base_path + results_path, response_class=JSONResponse)
-    async def get_results(dataset: str, request: Request):
-        helper_func = get_results_helper if no_cache else get_results_cachable
-        return template_function(dataset, request, helper_func)
-    
-    # Catalog API
-    @app.get(base_path, response_class=JSONResponse)
-    async def get_catalog():
-        all_dataset_contexts: Dict = mf.parms[c.DATASETS_KEY]
-        datasets = []
-        for dataset, dataset_context in all_dataset_contexts.items():
-            dataset_normalized = normalize_name_for_api(dataset)
-            datasets.append({
-                'dataset': dataset,
-                'label': dataset_context[c.DATASET_LABEL_KEY],
-                'parameters_path': base_path + parameters_path.format(dataset=dataset_normalized),
-                'result_path': base_path + results_path.format(dataset=dataset_normalized)
-            })
-        return {'project_variables': mf.parms[c.PROJ_VARS_KEY], 'resource_paths': datasets}
-    
-    # Squirrels UI
-    @app.get('/', response_class=HTMLResponse)
-    async def get_ui(request: Request):
-        return templates.TemplateResponse('index.html', {'request': request, 'base_path': base_path})
+        # Parameters API
+        parameters_path = base_path + '/{dataset}/parameters'
+        
+        parameters_cache_size = self.manifest.get_setting(c.PARAMETERS_CACHE_SIZE_SETTING, 1024)
+        parameters_cache_ttl = self.manifest.get_setting(c.PARAMETERS_CACHE_TTL_SETTING, 24*60*60)
 
-    
-    # Run API server
-    import uvicorn
-    uvicorn.run(app, host=uvicorn_args.host, port=uvicorn_args.port)
+        @ttl_cache(maxsize=parameters_cache_size, ttl=parameters_cache_ttl)
+        def get_parameters_cachable(*args):
+            return self._get_parameters_helper(*args)
+        
+        @app.get(parameters_path, response_class=JSONResponse)
+        async def get_parameters(dataset: str, request: Request):
+            api_function = self._get_parameters_helper if self.no_cache else get_parameters_cachable
+            return self._apply_dataset_api_function(api_function, dataset, request.query_params)
+
+        # Results API
+        results_path = base_path + '/{dataset}'
+
+        results_cache_size = self.manifest.get_setting(c.RESULTS_CACHE_SIZE_SETTING, 128)
+        results_cache_ttl = self.manifest.get_setting(c.RESULTS_CACHE_TTL_SETTING, 60*60)
+
+        @ttl_cache(maxsize=results_cache_size, ttl=results_cache_ttl)
+        def get_results_cachable(*args):
+            return self._get_results_helper(*args)
+        
+        @app.get(results_path, response_class=JSONResponse)
+        async def get_results(dataset: str, request: Request):
+            api_function = self._get_results_helper if self.no_cache else get_results_cachable
+            return self._apply_dataset_api_function(api_function, dataset, request.query_params)
+        
+        # Catalog API
+        @app.get(base_path, response_class=JSONResponse)
+        async def get_catalog():
+            datasets_info = []
+            for dataset in self.datasets:
+                dataset_normalized = utils.normalize_name_for_api(dataset)
+                datasets_info.append({
+                    'dataset': dataset,
+                    'label': self.manifest.get_dataset_label(dataset),
+                    'parameters_path': parameters_path.format(dataset=dataset_normalized),
+                    'result_path': results_path.format(dataset=dataset_normalized)
+                })
+            return {'project_variables': self.manifest.get_proj_vars(), 'resource_paths': datasets_info}
+        
+        # Squirrels UI
+        @app.get('/', response_class=HTMLResponse)
+        async def get_ui(request: Request):
+            return templates.TemplateResponse('index.html', {'request': request, 'base_path': base_path})
+        
+        # Run API server
+        import uvicorn
+        uvicorn.run(app, host=uvicorn_args.host, port=uvicorn_args.port)
```

### Comparing `squirrels-0.1.0rc1/squirrels/base_project/database/seattle_weather.db` & `squirrels-0.1.0rc2/squirrels/package_data/base_project/database/seattle_weather.db`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc1/squirrels/command_line.py` & `squirrels-0.1.0rc2/squirrels/_command_line.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,105 @@
-import sys, time
+from typing import List, Tuple, Optional
+from argparse import ArgumentParser
+import sys, time, pwinput
 sys.path.append('.')
 
-import pwinput
-from squirrels import constants as c, profile_manager as pm, __version__
-from squirrels import module_loader as ml, api_server
-from squirrels.renderer import Renderer
+from squirrels import constants as c, __version__
+from squirrels import module_loader as ml, manifest as mf, credentials_manager as cm, connection_set as cs
+from squirrels.api_server import ApiServer
+from squirrels.renderer import RendererIOWrapper
 from squirrels.initializer import Initializer
-from argparse import ArgumentParser
-
-
-def get_profiles():
-    for key, value in pm.get_profiles().items():
-        print(key + ": " + str(value))
+from squirrels.timed_imports import timer
 
 
-def set_profile(args):
-    profile = pm.Profile(args.name)
-    if args.values:
-        dialect, url, user, pw = args.values
+def _prompt_user_pw(args_values: Optional[List[str]]) -> Tuple[str, str]:
+    if args_values is not None:
+        user, pw = args_values
     else:
-        print("-- suggested PyPI packages for various sql drivers can be found here: " +
-              "https://superset.apache.org/docs/databases/installing-database-drivers/")
-
-        dialect = input("Enter sql dialect + driver: ")
-        url = input("Enter connection URL [host:port/database]: ")
         user = input("Enter username: ")
         pw = pwinput.pwinput("Enter password: ")
-    
-    profile.set(dialect, url, user, pw)
-    
-    print(f"\nProfile '{args.name}' has been set with following values:")
-    print(profile.get())
-
-
-def delete_profile(args):
-    profile_existed = pm.Profile(args.name).delete()
-    if profile_existed:
-        print(f"Profile '{args.name}' was deleted")
-    else:
-        print(f"Profile '{args.name}' does not exist")
+    return user, pw
 
 
 def main():
+    """
+    Main entry point for the squirrels command line utilities.
+    """
     start = time.time()
     parser = ArgumentParser(description="Command line utilities from the squirrels python package")
-    parser.add_argument('-V', '--version', action='store_true', help='Show the version and exit')
-    parser.add_argument('-v', '--verbose', action='store_true', help='Enable verbose output')
+    parser.add_argument('-v', '--version', action='store_true', help='Show the version and exit')
+    parser.add_argument('--verbose', action='store_true', help='Enable verbose output')
     subparsers = parser.add_subparsers(title='commands', dest='command')
 
-    def _add_profile_argument(parser):
-        parser.add_argument('name', type=str, help='Name of the database connection profile (provided in squirrels.yaml)')
-
     init_parser = subparsers.add_parser(c.INIT_CMD, help='Initialize a squirrels project')
-    init_parser.add_argument('--overwrite', action='store_true', help='Overwrite files if already exist')
+    init_parser.add_argument('--no-overwrite', action='store_true', help="Don't overwrite files if they already exist")
     init_parser.add_argument('--core', action='store_true', help='Include all core files')
     init_parser.add_argument('--context', action='store_true', help=f'Include the {c.CONTEXT_FILE} file')
+    init_parser.add_argument('--selections-cfg', action='store_true', help=f'Include the {c.SELECTIONS_CFG_FILE} file')
     init_parser.add_argument('--db-view', type=str, choices=['sql', 'py'], help='Create database view as sql (default) or python file')
     init_parser.add_argument('--final-view', type=str, choices=['sql', 'py'], help='Include final view as sql or python file')
     init_parser.add_argument('--sample-db', type=str, choices=['seattle-weather'], help='Sample sqlite database to include')
 
     subparsers.add_parser(c.LOAD_MODULES_CMD, help='Load all the modules specified in squirrels.yaml from git')
 
-    subparsers.add_parser(c.GET_PROFILES_CMD, help='Get all database connection profile names and values')
+    def _add_profile_argument(parser: ArgumentParser):
+        parser.add_argument('key', type=str, help='Key to the database connection credential')
+
+    subparsers.add_parser(c.GET_CREDS_CMD, help='Get all database connection credential keys')
 
-    set_profile_parser = subparsers.add_parser(c.SET_PROFILE_CMD, help='Set a database connection profile')
-    _add_profile_argument(set_profile_parser)
-    set_profile_parser.add_argument('--values', type=str, nargs=4, help='The sql dialect, connection url, username, and password')
+    set_cred_parser = subparsers.add_parser(c.SET_CRED_CMD, help='Set a database connection credential key')
+    _add_profile_argument(set_cred_parser)
+    set_cred_parser.add_argument('--values', type=str, nargs=2, help='The username and password')
 
-    delete_profile_parser = subparsers.add_parser(c.DELETE_PROFILE_CMD, help='Delete a database connection profile')
-    _add_profile_argument(delete_profile_parser)
+    delete_cred_parser = subparsers.add_parser(c.DELETE_CRED_CMD, help='Delete a database connection credential key')
+    _add_profile_argument(delete_cred_parser)
 
     test_parser = subparsers.add_parser(c.TEST_CMD, help='For a given dataset, create outputs for parameter API response and rendered sql queries')
     test_parser.add_argument('dataset', type=str, help='Name of dataset (provided in squirrels.yaml) to test. Results are written in an "outputs" folder')
-    test_parser.add_argument('-c', '--cfg', type=str, help='Configuration file for parameter selections. Path is relative to a specific dataset folder')
-    test_parser.add_argument('-d', '--data', type=str, help='Sample lookup data to avoid making a database connection. Path is relative to a specific dataset folder')
+    test_parser.add_argument('-c', '--cfg', type=str, help="Configuration file for parameter selections. Path is relative to the dataset's folder")
+    test_parser.add_argument('-d', '--data', type=str, help="Excel file with lookup data to avoid making a database connection. Path is relative to the dataset's folder")
     test_parser.add_argument('-r', '--runquery', action='store_true', help='Runs all database queries and final view, and produce the results as csv files')
 
     run_parser = subparsers.add_parser(c.RUN_CMD, help='Run the builtin API server')
     run_parser.add_argument('--no-cache', action='store_true', help='Do not cache any api results')
-    run_parser.add_argument('--debug', action='store_true', help='In debug mode, all "hidden parameters" show in parameters response')
+    run_parser.add_argument('--debug', action='store_true', help='In debug mode, all "hidden parameters" show in the parameters response')
     run_parser.add_argument('--host', type=str, default='127.0.0.1')
     run_parser.add_argument('--port', type=int, default=8000)
-    c.timer.add_activity_time('creating argparser', start)
 
-    start = time.time()
     args, _ = parser.parse_known_args()
+    timer.verbose = args.verbose
+    timer.add_activity_time('parsing arguments', start)
+
     if args.version:
         print(__version__)
-    elif args.command == c.GET_PROFILES_CMD:
-        get_profiles()
-    elif args.command == c.SET_PROFILE_CMD:
-        set_profile(args)
-    elif args.command == c.DELETE_PROFILE_CMD:
-        delete_profile(args)
-    elif args.command == c.TEST_CMD:
-        Renderer(args.dataset, args.cfg, args.data).write_outputs(args.runquery)
-        c.timer.add_activity_time('all of write_outputs', start)
-    elif args.command == c.RUN_CMD:
-        api_server.run(args.no_cache, args.debug, args)
-    elif args.command == c.LOAD_MODULES_CMD:
-        ml.load_modules()
     elif args.command == c.INIT_CMD:
-        Initializer(args.overwrite).init_project(args)
+        Initializer(not args.no_overwrite).init_project(args)
+    elif args.command == c.LOAD_MODULES_CMD:
+        manifest = mf.from_file()
+        ml.load_modules(manifest)
+    elif args.command == c.GET_CREDS_CMD: 
+        cm.squirrels_config_io.print_all_credentials()
+    elif args.command == c.SET_CRED_CMD:
+        user, pw = _prompt_user_pw(args.values)
+        cm.squirrels_config_io.set_credential(args.key, user, pw)
+    elif args.command == c.DELETE_CRED_CMD:
+        cm.squirrels_config_io.delete_credential(args.key)
+    elif args.command in [c.RUN_CMD, c.TEST_CMD]:
+        manifest = mf.from_file()
+        conn_set = cs.from_file(manifest)
+        if args.command == c.RUN_CMD:
+            server = ApiServer(manifest, conn_set, args.no_cache, args.debug)
+            server.run(args)
+        elif args.command == c.TEST_CMD:
+            rendererIO = RendererIOWrapper(args.dataset, manifest, conn_set, args.data)
+            rendererIO.write_outputs(args.cfg, args.runquery)
+        conn_set.dispose()
     elif args.command is None:
-        print(f'Error: Missing command. Enter "squirrels -h" for help.')
+        print(f'Command is missing. Enter "squirrels -h" for help.')
     else:
         print(f'Error: No such command "{args.command}". Enter "squirrels -h" for help.')
     
-    c.timer.report_times(args.verbose)
+    timer.report_times()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `squirrels-0.1.0rc1/squirrels/initializer.py` & `squirrels-0.1.0rc2/squirrels/initializer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,95 @@
 import inquirer, os, shutil
-from squirrels import major_version, constants as c
+from squirrels import major_version, constants as c, utils
 
-base_proj_dir = os.path.join(os.path.dirname(__file__), 'base_project')
-dataset_dir = os.path.join('datasets', 'sample_dataset')
+base_proj_dir = utils.join_paths(os.path.dirname(__file__), 'package_data', 'base_project')
+dataset_dir = utils.join_paths('datasets', 'sample_dataset')
 
 
 class Initializer:
     def __init__(self, overwrite: bool):
         self.overwrite = overwrite
 
-    def path_exists(self, filepath: str) -> bool:
+    def _path_exists(self, filepath: str) -> bool:
         if not self.overwrite and os.path.exists(filepath):
             print(f'File "{filepath}" already exists. Creation skipped.')
             return True
         return False
     
-    def copy_file(self, filepath: str):
-        if not self.path_exists(filepath):
+    def _copy_file(self, filepath: str):
+        if not self._path_exists(filepath):
             dest_dir = os.path.dirname(filepath)
             if dest_dir != '':
                 os.makedirs(dest_dir, exist_ok=True)
-            src_path = os.path.join(base_proj_dir, filepath)
+            src_path = utils.join_paths(base_proj_dir, filepath)
             shutil.copy(src_path, filepath)
 
-    def copy_dataset_file(self, filepath: str):
-        self.copy_file(os.path.join(dataset_dir, filepath))
+    def _copy_dataset_file(self, filepath: str):
+        self._copy_file(utils.join_paths(dataset_dir, filepath))
 
-    def copy_database_file(self, filepath: str):
-        self.copy_file(os.path.join('database', filepath))
+    def _copy_database_file(self, filepath: str):
+        self._copy_file(utils.join_paths('database', filepath))
 
-    def create_requirements_txt(self):
+    def _create_requirements_txt(self):
         filename = 'requirements.txt'
-        if not self.path_exists(filename):
+        if not self._path_exists(filename):
             next_major_version = int(major_version) + 1
             content = f'squirrels<{next_major_version}'
-            with open('requirements.txt', 'w') as f:
+            with open(filename, 'w') as f:
                 f.write(content)
 
     def init_project(self, args):
-        options = ['core', 'context', 'db_view', 'final_view', 'sample_db']
+        options = ['core', 'context', 'selections_cfg', 'db_view', 'final_view', 'sample_db']
         answers = { x: getattr(args, x) for x in options }
         if not any(answers.values()):
             questions = [
                 inquirer.Confirm('core',
                                 message="Include all core project files?",
                                 default=True),
                 inquirer.Confirm('context',
                                 message="Do you want to include a 'context.py' file?" ,
                                 default=False),
+                inquirer.Confirm('selections_cfg',
+                                message="Do you want to include a 'selections.cfg' file?" ,
+                                default=False),
                 inquirer.List('db_view', 
                             message="What's the file format for the database view? (ignore if core project files are not included)",
                             choices=['sql', 'py']),
                 inquirer.List('final_view', 
                             message="What's the file format for the final view (if any)?",
                             choices=['none', 'sql', 'py']),
                 inquirer.List('sample_db', 
                             message="What sample sqlite database do you wish to use (if any)?",
-                            choices=['none', 'seattle-weather'])
+                            choices=['none', 'sample_database', 'seattle_weather'])
             ]
             answers = inquirer.prompt(questions)
 
         if answers.get('core', False):
-            self.copy_file('.gitignore')
-            self.create_requirements_txt()
-            self.copy_file(c.MANIFEST_FILE)
-            self.copy_dataset_file(c.PARAMETERS_FILE)
+            self._copy_file('.gitignore')
+            self._copy_file(c.MANIFEST_FILE)
+            self._copy_file(c.PROJ_VARS_FILE)
+            self._copy_file(c.CONNECTIONS_FILE)
+            self._create_requirements_txt()
+            self._copy_dataset_file(c.PARAMETERS_FILE)
             if answers.get('db_view') == 'py':
-                self.copy_dataset_file(c.DATABASE_VIEW_NAME + '.py')
+                self._copy_dataset_file(c.DATABASE_VIEW_PY_FILE)
             else:
-                self.copy_dataset_file(c.DATABASE_VIEW_NAME + '.sql.j2')
+                self._copy_dataset_file(c.DATABASE_VIEW_SQL_FILE)
         
         if answers.get('context', False):
-            self.copy_dataset_file(c.CONTEXT_FILE)
+            self._copy_dataset_file(c.CONTEXT_FILE)
+        
+        if answers.get('selections_cfg', False):
+            self._copy_dataset_file(c.SELECTIONS_CFG_FILE)
         
         final_view_format = answers.get('final_view')
         if final_view_format == 'py':
-            self.copy_dataset_file(c.FINAL_VIEW_NAME + '.py')
+            self._copy_dataset_file(c.FINAL_VIEW_PY_NAME)
         elif final_view_format == 'sql':
-            self.copy_dataset_file(c.FINAL_VIEW_NAME + '.sql.j2')
+            self._copy_dataset_file(c.FINAL_VIEW_SQL_NAME)
 
         sample_db = answers.get('sample_db')
-        if sample_db == 'seattle-weather':
-            self.copy_database_file('seattle_weather.db')
+        if sample_db == 'sample_database':
+            self._copy_database_file('sample_database.db')
+        elif sample_db == 'seattle_weather':
+            self._copy_database_file('seattle_weather.db')
```

### Comparing `squirrels-0.1.0rc1/squirrels/module_loader.py` & `squirrels-0.1.0rc2/squirrels/module_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import List
+from typing import List, Tuple, Dict
 from squirrels import constants as c, manifest as mf
 import git, shutil, os, stat
 
 
-def parse_module_repo_strings(repo_strings):
+def parse_module_repo_strings(repo_strings: List[str]) -> List[Tuple[str]]:
     output = []
     for repo in repo_strings:
         try:
             url, tag = repo.split('@')
         except ValueError:
             raise RuntimeError(f'cannot split git repo "{repo}" into url and tag/branch... format must be like "url@tag"')
         
@@ -17,19 +17,16 @@
             name = url.split('/')[-1].replace('.git', '')
 
         output.append((name, url, tag))
     
     return output
 
 
-
-def load_modules():
-    mf.initialize(c.MANIFEST_FILE)
-    
-    repo_strings: List[str] = mf.parms[c.MODULES_KEY]
+def load_modules(manifest: mf.Manifest) -> None:
+    repo_strings: List[str] = manifest.get_modules()
 
     # Recreate the modules directory if it exists
     if os.path.exists(c.MODULES_FOLDER):
         def del_rw(action, name, exc):
             os.chmod(name, stat.S_IWRITE)
             os.remove(name)
         shutil.rmtree(c.MODULES_FOLDER, onerror=del_rw)
```

### Comparing `squirrels-0.1.0rc1/squirrels/static/favicon.ico` & `squirrels-0.1.0rc2/squirrels/package_data/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc1/squirrels/static/script.js` & `squirrels-0.1.0rc2/squirrels/package_data/static/script.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,15 @@
     loadingIndicator.style.display = 'flex';
     fetch(path)
         .then(response => response.json())
         .then(data => {
             func(data);
         })
         .catch(error => {
-            alert('Server error')
+            alert('Server error...')
             console.log(error)
         })
         .then(_ => {
             loadingIndicator.style.display = 'none'
         })
 }
 
@@ -40,23 +40,27 @@
         option.textContent = resource.label;
         datasetSelect.appendChild(option);
         datasetsMap.set(resource.dataset, resource);
     });
     changeDatasetSelection();
 }
 
-function refreshParameters() {
+function refreshParameters(provoker = null) {
     const selectedDatasetValue = datasetSelect.value;
     const parametersPath = datasetsMap.get(selectedDatasetValue).parameters_path;
-    const parametersRequest = parametersPath + '?' + getQueryParams()
+    const queryParameters = getQueryParams(provoker)
+    const parametersRequest = parametersPath + '?' + queryParameters
     console.log('Parameters request:', parametersRequest)
 
     callJsonAPI(parametersRequest, (jsonResponse) => {
-        generatedParamsDiv.innerHTML = "";
         jsonResponse.parameters.forEach(function(param) {
+            parametersMap.set(param.name, param);
+        })
+        generatedParamsDiv.innerHTML = "";
+        for (const param of parametersMap.values()) {
             const newDiv = document.createElement('div')
 
             const addLabel = function() {
                 const paramLabel = document.createElement('label')
                 paramLabel.innerHTML = param.label
                 newDiv.appendChild(paramLabel)
             }
@@ -122,16 +126,15 @@
                     selectOption.innerText = option.label;
                     multiSelect.appendChild(selectOption);
                 });
                 multiSelect.onchange = updateParameter
                 newDiv.appendChild(multiSelect);
             }
             generatedParamsDiv.appendChild(newDiv);
-            parametersMap.set(param.name, param);
-        })
+        }
     });
 }
 
 function updateParameter() {
     const param = parametersMap.get(this.id)
     if (param.widget_type === "DateField") {
         param.selected_date = this.value
@@ -142,34 +145,42 @@
     } else if (param.widget_type === "SingleSelect") {
         param.selected_id = this.options[this.selectedIndex].value
     } else if (param.widget_type === "MultiSelect") {
         param.selected_ids = [...this.selectedOptions].map(option => option.value)
     }
 
     if (param.trigger_refresh) {
-        refreshParameters()
+        refreshParameters(param)
     }
 }
 
-function getQueryParams() {
+function getQueryParams(provoker = null) {
     const queryParams = {}
-    for (const [key, value] of parametersMap.entries()) {
+
+    function addToQueryParams(key, value) {
         if (value.widget_type === "DateField") {
             queryParams[key] = value.selected_date
         } else if (value.widget_type === "NumberField") {
             queryParams[key] = value.selected_value
         } else if (value.widget_type === "RangeField") {
             // TODO
         } else if (value.widget_type === "SingleSelect") {
             queryParams[key] = value.selected_id
         } else if (value.widget_type === "MultiSelect") {
             result = value.selected_ids.join()
             if (result !== '') queryParams[key] = result
         }
     }
+    if (provoker !== null) {
+        addToQueryParams(provoker.name, provoker)
+    } else {
+        for (const [key, value] of parametersMap.entries()) {
+            addToQueryParams(key, value)
+        }
+    }
     console.log(queryParams)
     return new URLSearchParams(queryParams)
 }
 
 function getDatasetResults() {
     const selectedDatasetValue = datasetSelect.value;
     const resultPath = datasetsMap.get(selectedDatasetValue).result_path;
```

### Comparing `squirrels-0.1.0rc1/squirrels/static/style.css` & `squirrels-0.1.0rc2/squirrels/package_data/static/style.css`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc1/squirrels/templates/index.html` & `squirrels-0.1.0rc2/squirrels/package_data/templates/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html>
     <head>
         <title>Squirrels UI</title>
         <link id="favicon" rel="icon" type="image/x-icon" href="static/favicon.ico">
-        <link href="{{ url_for('static', path='/style.css') }}" rel="stylesheet">
-        <script src="{{ url_for('static', path='/script.js') }}" defer></script>
+        <link href="{{ url_for('static', path='/style.css?version=0') }}" rel="stylesheet">
+        <script src="{{ url_for('static', path='/script.js?version=0') }}" defer></script>
     </head>
     <body onload="callJsonAPI('{{ base_path }}', renderDatasetsSelection)">
     <div id="main-container">
         <div id="parameter-container">
             <label for="dataset-select">Select a Dataset:</label>
             <select id="dataset-select" onchange="changeDatasetSelection()"></select>
             <div id="generated-parameters"></div>
```

