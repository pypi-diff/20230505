# Comparing `tmp/ou-container-content-1.1.2.tar.gz` & `tmp/ou_container_content-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou-container-content-1.1.2.tar", max compression
+gzip compressed data, was "ou_container_content-1.1.3.tar", max compression
```

## Comparing `ou-container-content-1.1.2.tar` & `ou_container_content-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      588 2022-11-16 15:07:07.682314 ou-container-content-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       57 2021-04-16 13:12:59.023757 ou-container-content-1.1.2/src/ou_container_content/__init__.py
--rw-r--r--   0        0        0     2846 2021-11-04 16:17:51.835860 ou-container-content-1.1.2/src/ou_container_content/__main__.py
--rw-r--r--   0        0        0     6505 2021-11-04 16:49:46.589609 ou-container-content-1.1.2/src/ou_container_content/distributor.py
--rw-r--r--   0        0        0       40 2021-05-14 13:42:10.374284 ou-container-content-1.1.2/src/ou_container_content/frontend/__init__.py
--rw-r--r--   0        0        0       40 2021-05-14 13:42:11.566244 ou-container-content-1.1.2/src/ou_container_content/frontend/build/__init__.py
--rw-r--r--   0        0        0     5544 2022-07-14 18:14:12.074134 ou-container-content-1.1.2/src/ou_container_content/frontend/build/bundle.css
--rw-r--r--   0        0        0     7148 2022-07-14 18:14:12.074134 ou-container-content-1.1.2/src/ou_container_content/frontend/build/bundle.js
--rw-r--r--   0        0        0    68795 2022-07-14 18:14:12.074134 ou-container-content-1.1.2/src/ou_container_content/frontend/build/bundle.js.map
--rw-r--r--   0        0        0      890 2022-07-14 18:14:12.074134 ou-container-content-1.1.2/src/ou_container_content/frontend/global.css
--rw-r--r--   0        0        0      642 2022-07-14 18:14:12.074134 ou-container-content-1.1.2/src/ou_container_content/frontend/index.html
--rw-r--r--   0        0        0      503 2022-07-14 18:14:12.074134 ou-container-content-1.1.2/src/ou_container_content/frontend/ou-favicon-1.png
--rw-r--r--   0        0        0      703 2022-07-14 18:14:12.074134 ou-container-content-1.1.2/src/ou_container_content/frontend/ou-favicon-2.png
--rw-r--r--   0        0        0      897 2022-07-14 18:14:12.074134 ou-container-content-1.1.2/src/ou_container_content/frontend/ou-favicon-3.png
--rw-r--r--   0        0        0     1601 2022-07-14 18:14:12.074134 ou-container-content-1.1.2/src/ou_container_content/frontend/ou-favicon-4.png
--rw-r--r--   0        0        0     2946 2021-10-01 15:59:53.817352 ou-container-content-1.1.2/src/ou_container_content/handlers.py
--rw-r--r--   0        0        0     1594 2021-11-04 16:17:42.372189 ou-container-content-1.1.2/src/ou_container_content/process.py
--rw-r--r--   0        0        0     1499 2021-06-24 15:01:11.746713 ou-container-content-1.1.2/src/ou_container_content/scripts.py
--rw-r--r--   0        0        0     1344 2021-06-24 15:03:26.806595 ou-container-content-1.1.2/src/ou_container_content/services.py
--rw-r--r--   0        0        0     3180 2021-06-25 12:36:17.192356 ou-container-content-1.1.2/src/ou_container_content/validator.py
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 ou-container-content-1.1.2/setup.py
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 ou-container-content-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      588 2023-05-05 10:04:12.063842 ou_container_content-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-05-05 10:04:12.063842 ou_container_content-1.1.3/src/ou_container_content/__init__.py
+-rw-r--r--   0        0        0     2846 2023-05-05 10:04:12.063842 ou_container_content-1.1.3/src/ou_container_content/__main__.py
+-rw-r--r--   0        0        0     6505 2023-05-05 10:04:12.063842 ou_container_content-1.1.3/src/ou_container_content/distributor.py
+-rw-r--r--   0        0        0       40 2023-05-05 10:04:12.064842 ou_container_content-1.1.3/src/ou_container_content/frontend/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-05 10:04:12.064842 ou_container_content-1.1.3/src/ou_container_content/frontend/build/__init__.py
+-rw-r--r--   0        0        0     5544 2023-05-05 10:04:12.064842 ou_container_content-1.1.3/src/ou_container_content/frontend/build/bundle.css
+-rw-r--r--   0        0        0     7148 2023-05-05 10:04:12.064842 ou_container_content-1.1.3/src/ou_container_content/frontend/build/bundle.js
+-rw-r--r--   0        0        0    68795 2023-05-05 10:04:12.064842 ou_container_content-1.1.3/src/ou_container_content/frontend/build/bundle.js.map
+-rw-r--r--   0        0        0      890 2023-05-05 10:04:12.064842 ou_container_content-1.1.3/src/ou_container_content/frontend/global.css
+-rw-r--r--   0        0        0      642 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/frontend/index.html
+-rw-r--r--   0        0        0      503 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/frontend/ou-favicon-1.png
+-rw-r--r--   0        0        0      703 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/frontend/ou-favicon-2.png
+-rw-r--r--   0        0        0      897 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/frontend/ou-favicon-3.png
+-rw-r--r--   0        0        0     1601 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/frontend/ou-favicon-4.png
+-rw-r--r--   0        0        0     2946 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/handlers.py
+-rw-r--r--   0        0        0     1594 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/process.py
+-rw-r--r--   0        0        0     1499 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/scripts.py
+-rw-r--r--   0        0        0     1345 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/services.py
+-rw-r--r--   0        0        0     3180 2023-05-05 10:04:12.065842 ou_container_content-1.1.3/src/ou_container_content/validator.py
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 ou_container_content-1.1.3/PKG-INFO
```

### Comparing `ou-container-content-1.1.2/pyproject.toml` & `ou_container_content-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ou-container-content"
-version = "1.1.2"
+version = "1.1.3"
 description = ""
 authors = ["Mark Hall <mark.hall@open.ac.uk>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = "^7.1.2"
 PyYAML = "^5.4.1"
```

### Comparing `ou-container-content-1.1.2/src/ou_container_content/__main__.py` & `ou_container_content-1.1.3/src/ou_container_content/__main__.py`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/distributor.py` & `ou_container_content-1.1.3/src/ou_container_content/distributor.py`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/frontend/build/bundle.css` & `ou_container_content-1.1.3/src/ou_container_content/frontend/build/bundle.css`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/frontend/build/bundle.js` & `ou_container_content-1.1.3/src/ou_container_content/frontend/build/bundle.js`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/frontend/build/bundle.js.map` & `ou_container_content-1.1.3/src/ou_container_content/frontend/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/frontend/global.css` & `ou_container_content-1.1.3/src/ou_container_content/frontend/global.css`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/frontend/index.html` & `ou_container_content-1.1.3/src/ou_container_content/frontend/index.html`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/frontend/ou-favicon-2.png` & `ou_container_content-1.1.3/src/ou_container_content/frontend/ou-favicon-2.png`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/frontend/ou-favicon-3.png` & `ou_container_content-1.1.3/src/ou_container_content/frontend/ou-favicon-3.png`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/frontend/ou-favicon-4.png` & `ou_container_content-1.1.3/src/ou_container_content/frontend/ou-favicon-4.png`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/handlers.py` & `ou_container_content-1.1.3/src/ou_container_content/handlers.py`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/process.py` & `ou_container_content-1.1.3/src/ou_container_content/process.py`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/scripts.py` & `ou_container_content-1.1.3/src/ou_container_content/scripts.py`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/src/ou_container_content/services.py` & `ou_container_content-1.1.3/src/ou_container_content/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     if 'services' in settings:
         for idx, service in enumerate(settings['services']):
             proc = await create_subprocess_exec('sudo', 'service', service, 'start')
             await proc.wait()
             send_message({
                 'component': 'services',
                 'state': 'active',
-                'progress': math.floor(100 / len(settings['scripts']) * idx),
+                'progress': math.floor(100 / len(settings['services']) * idx),
             })
     send_message({
         'component': 'services',
         'state': 'complete',
         'progress': 100,
     })
```

### Comparing `ou-container-content-1.1.2/src/ou_container_content/validator.py` & `ou_container_content-1.1.3/src/ou_container_content/validator.py`

 * *Files identical despite different names*

### Comparing `ou-container-content-1.1.2/PKG-INFO` & `ou_container_content-1.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ou-container-content
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
 Author: Mark Hall
 Author-email: mark.hall@open.ac.uk
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Cerberus (>=1.3.3,<2.0.0)
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: tornado (>=6.1,<7.0)
```

