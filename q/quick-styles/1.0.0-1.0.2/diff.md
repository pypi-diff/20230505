# Comparing `tmp/quick_styles-1.0.0.tar.gz` & `tmp/quick_styles-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_styles-1.0.0.tar", last modified: Fri May  5 15:34:54 2023, max compression
+gzip compressed data, was "quick_styles-1.0.2.tar", last modified: Fri May  5 18:16:59 2023, max compression
```

## Comparing `quick_styles-1.0.0.tar` & `quick_styles-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 15:34:54.179705 quick_styles-1.0.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1070 2023-05-05 15:32:55.000000 quick_styles-1.0.0/LICENSE.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3532 2023-05-05 15:34:54.179705 quick_styles-1.0.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3011 2023-05-05 15:32:55.000000 quick_styles-1.0.0/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 15:34:54.175705 quick_styles-1.0.0/quick_styles/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       37 2023-05-05 15:32:55.000000 quick_styles-1.0.0/quick_styles/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3169 2023-05-05 15:32:55.000000 quick_styles-1.0.0/quick_styles/functions.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 15:34:54.179705 quick_styles-1.0.0/quick_styles.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3532 2023-05-05 15:34:54.000000 quick_styles-1.0.0/quick_styles.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      224 2023-05-05 15:34:54.000000 quick_styles-1.0.0/quick_styles.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-05 15:34:54.000000 quick_styles-1.0.0/quick_styles.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-05 15:34:54.000000 quick_styles-1.0.0/quick_styles.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-05 15:34:54.179705 quick_styles-1.0.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      870 2023-05-05 15:32:55.000000 quick_styles-1.0.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 18:16:59.117262 quick_styles-1.0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1070 2023-05-05 15:32:55.000000 quick_styles-1.0.2/LICENSE.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3561 2023-05-05 18:16:59.117262 quick_styles-1.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3040 2023-05-05 17:56:01.000000 quick_styles-1.0.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 18:16:59.113262 quick_styles-1.0.2/quick_styles/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       37 2023-05-05 15:32:55.000000 quick_styles-1.0.2/quick_styles/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3169 2023-05-05 15:32:55.000000 quick_styles-1.0.2/quick_styles/functions.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 18:16:59.117262 quick_styles-1.0.2/quick_styles.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3561 2023-05-05 18:16:59.000000 quick_styles-1.0.2/quick_styles.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      224 2023-05-05 18:16:59.000000 quick_styles-1.0.2/quick_styles.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-05 18:16:59.000000 quick_styles-1.0.2/quick_styles.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-05 18:16:59.000000 quick_styles-1.0.2/quick_styles.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-05 18:16:59.117262 quick_styles-1.0.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      870 2023-05-05 18:16:36.000000 quick_styles-1.0.2/setup.py
```

### Comparing `quick_styles-1.0.0/LICENSE.md` & `quick_styles-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quick_styles-1.0.0/PKG-INFO` & `quick_styles-1.0.2/quick_styles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
-Name: quick_styles
-Version: 1.0.0
+Name: quick-styles
+Version: 1.0.2
 Summary: A ridiculously lightweight Python library for effortlessly applying ANSI escape color & style codes to Windows CMD.
 Home-page: https://github.com/imjamnotjelly/quick_styles
 Author: imjamnotjelly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Terminals
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-<img src="banner.png">
+<img src="https://raw.githubusercontent.com/imjamnotjelly/quick_styles/master/banner.png">
 
 <div align="center">
-  <h1>quick_styles (wip)</h1>
-  <label>An unbelievably lightweight Python library for effortlessly applying ANSI escape color & style codes to Windows CMD and other ANSI-supported terminals</label>
+  <h1>quick_styles</h1>
+  <p>An unbelievably lightweight Python library for effortlessly applying ANSI escape color & style codes to Windows CMD and other ANSI-supported terminals</p>
 </div>
 <br>
 <br>
 
 ## Description
 
 quick_styles enhances the experience of using the current unintuitive ANSI escape code system for text styling in Python. With quick_styles, you can easily generate ANSI codes with set parameters, save styles for future use, and implement custom codes for personalized styles.
 
 ## Download
 
 From PyPI using `pip`:
 
 ```shell
-pip install quick_styles
+pip install quick-styles
 ```
 
 ## Usage
 
 ### Example program
 
 Before we proceed to the explict info regarding the library's functionality, here's a preview of the core functions of quick_styles to get a sense of its capabilities:
@@ -81,9 +81,7 @@
 
 # Reset function returns defaults to initial values
 qs.defaults.reset()
 
 # Strings can also be styled without being immediately printed
 styled_string = qs.style_string("You can't see me...", styles="italic")
 ```
-
-### Function Refrence
```

### Comparing `quick_styles-1.0.0/README.md` & `quick_styles-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-<img src="banner.png">
+<img src="https://raw.githubusercontent.com/imjamnotjelly/quick_styles/master/banner.png">
 
 <div align="center">
-  <h1>quick_styles (wip)</h1>
-  <label>An unbelievably lightweight Python library for effortlessly applying ANSI escape color & style codes to Windows CMD and other ANSI-supported terminals</label>
+  <h1>quick_styles</h1>
+  <p>An unbelievably lightweight Python library for effortlessly applying ANSI escape color & style codes to Windows CMD and other ANSI-supported terminals</p>
 </div>
 <br>
 <br>
 
 ## Description
 
 quick_styles enhances the experience of using the current unintuitive ANSI escape code system for text styling in Python. With quick_styles, you can easily generate ANSI codes with set parameters, save styles for future use, and implement custom codes for personalized styles.
 
 ## Download
 
 From PyPI using `pip`:
 
 ```shell
-pip install quick_styles
+pip install quick-styles
 ```
 
 ## Usage
 
 ### Example program
 
 Before we proceed to the explict info regarding the library's functionality, here's a preview of the core functions of quick_styles to get a sense of its capabilities:
@@ -67,9 +67,7 @@
 
 # Reset function returns defaults to initial values
 qs.defaults.reset()
 
 # Strings can also be styled without being immediately printed
 styled_string = qs.style_string("You can't see me...", styles="italic")
 ```
-
-### Function Refrence
```

### Comparing `quick_styles-1.0.0/quick_styles/functions.py` & `quick_styles-1.0.2/quick_styles/functions.py`

 * *Files identical despite different names*

### Comparing `quick_styles-1.0.0/quick_styles.egg-info/PKG-INFO` & `quick_styles-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
-Name: quick-styles
-Version: 1.0.0
+Name: quick_styles
+Version: 1.0.2
 Summary: A ridiculously lightweight Python library for effortlessly applying ANSI escape color & style codes to Windows CMD.
 Home-page: https://github.com/imjamnotjelly/quick_styles
 Author: imjamnotjelly
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Terminals
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-<img src="banner.png">
+<img src="https://raw.githubusercontent.com/imjamnotjelly/quick_styles/master/banner.png">
 
 <div align="center">
-  <h1>quick_styles (wip)</h1>
-  <label>An unbelievably lightweight Python library for effortlessly applying ANSI escape color & style codes to Windows CMD and other ANSI-supported terminals</label>
+  <h1>quick_styles</h1>
+  <p>An unbelievably lightweight Python library for effortlessly applying ANSI escape color & style codes to Windows CMD and other ANSI-supported terminals</p>
 </div>
 <br>
 <br>
 
 ## Description
 
 quick_styles enhances the experience of using the current unintuitive ANSI escape code system for text styling in Python. With quick_styles, you can easily generate ANSI codes with set parameters, save styles for future use, and implement custom codes for personalized styles.
 
 ## Download
 
 From PyPI using `pip`:
 
 ```shell
-pip install quick_styles
+pip install quick-styles
 ```
 
 ## Usage
 
 ### Example program
 
 Before we proceed to the explict info regarding the library's functionality, here's a preview of the core functions of quick_styles to get a sense of its capabilities:
@@ -81,9 +81,7 @@
 
 # Reset function returns defaults to initial values
 qs.defaults.reset()
 
 # Strings can also be styled without being immediately printed
 styled_string = qs.style_string("You can't see me...", styles="italic")
 ```
-
-### Function Refrence
```

### Comparing `quick_styles-1.0.0/setup.py` & `quick_styles-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="quick_styles",
-    version="1.0.0",
+    version="1.0.2",
     description="A ridiculously lightweight Python library for effortlessly applying ANSI escape color & style codes to Windows CMD.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/imjamnotjelly/quick_styles",
     author="imjamnotjelly",
     license="MIT",
     classifiers=[
```

