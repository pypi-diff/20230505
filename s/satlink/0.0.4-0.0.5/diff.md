# Comparing `tmp/satlink-0.0.4.tar.gz` & `tmp/satlink-0.0.5.tar.gz`

## Comparing `satlink-0.0.4.tar` & `satlink-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 satlink-0.0.4/demo.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 satlink-0.0.4/src/satlink/__init__.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 satlink-0.0.4/src/satlink/components/downlink.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 satlink-0.0.4/src/satlink/components/houston.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 satlink-0.0.4/src/satlink/components/satellite.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 satlink-0.0.4/src/satlink/components/server.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 satlink-0.0.4/src/satlink/components/type.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 satlink-0.0.4/src/satlink/components/uplink.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 satlink-0.0.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 satlink-0.0.4/LICENSE
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 satlink-0.0.4/README.md
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 satlink-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 satlink-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 satlink-0.0.5/demo.py
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 satlink-0.0.5/publish.sh
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 satlink-0.0.5/src/satlink/__init__.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 satlink-0.0.5/src/satlink/components/datalink.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 satlink-0.0.5/src/satlink/components/downlink.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 satlink-0.0.5/src/satlink/components/satellite.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 satlink-0.0.5/src/satlink/components/uplink.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 satlink-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 satlink-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 satlink-0.0.5/README.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 satlink-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 satlink-0.0.5/PKG-INFO
```

### Comparing `satlink-0.0.4/.gitignore` & `satlink-0.0.5/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -123,7 +123,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# MacOS
+.DS_Store
```

### Comparing `satlink-0.0.4/LICENSE` & `satlink-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `satlink-0.0.4/README.md` & `satlink-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -45,22 +45,21 @@
 
 Step 4: Now, populate the sat.py file with the following code:
 ```python
 from satlink import Satellite
 
 sat = Satellite()
 
-@sat.get("/")
+@sat.datalink("/")
 def index(uplink, downlink):
-  return downlink.text("Hello, World!")
+  return downlink.text("Hello, Earth!")
 
 sat.transmit()
-# Alternatively: sat.transmit(3000, "localhost")
 ```
 
 Step 5: Lastly, let's boot up our satellite.
 ```bash
-python3 app.py
+python3 sat.py
 ```
-When you visit [http://localhost:3000/](http://localhost:3000/) you should see the text "Hello, World!".
+When you visit [http://localhost:3000/](http://localhost:3000/) you should see the text "Hello, Earth!".
 
 To learn more, take a look at the [API documentation](https://github.com/olejorga/satlink/wiki).
```

### Comparing `satlink-0.0.4/pyproject.toml` & `satlink-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "satlink"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="olejorga" },
 ]
 description = "A light web framework - originally developed as a project in Frameworks at HiØ, written with love in Python <3"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.11"
```

### Comparing `satlink-0.0.4/PKG-INFO` & `satlink-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: satlink
-Version: 0.0.4
+Version: 0.0.5
 Summary: A light web framework - originally developed as a project in Frameworks at HiØ, written with love in Python <3
 Project-URL: Documentation, https://github.com/olejorga/satlink/wiki
 Project-URL: Repository, https://github.com/olejorga/satlink
 Author: olejorga
+License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
@@ -59,22 +60,21 @@
 
 Step 4: Now, populate the sat.py file with the following code:
 ```python
 from satlink import Satellite
 
 sat = Satellite()
 
-@sat.get("/")
+@sat.datalink("/")
 def index(uplink, downlink):
-  return downlink.text("Hello, World!")
+  return downlink.text("Hello, Earth!")
 
 sat.transmit()
-# Alternatively: sat.transmit(3000, "localhost")
 ```
 
 Step 5: Lastly, let's boot up our satellite.
 ```bash
-python3 app.py
+python3 sat.py
 ```
-When you visit [http://localhost:3000/](http://localhost:3000/) you should see the text "Hello, World!".
+When you visit [http://localhost:3000/](http://localhost:3000/) you should see the text "Hello, Earth!".
 
 To learn more, take a look at the [API documentation](https://github.com/olejorga/satlink/wiki).
```

