# Comparing `tmp/UzbekNLP-0.0.1.tar.gz` & `tmp/UzbekNLP-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzbekNLP-0.0.1.tar", last modified: Fri May  5 09:54:45 2023, max compression
+gzip compressed data, was "UzbekNLP-0.0.2.tar", last modified: Fri May  5 10:18:12 2023, max compression
```

## Comparing `UzbekNLP-0.0.1.tar` & `UzbekNLP-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:54:45.934968 UzbekNLP-0.0.1/
--rw-rw-rw-   0        0        0     1096 2023-05-05 09:39:17.000000 UzbekNLP-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      754 2023-05-05 09:54:45.930775 UzbekNLP-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-05-05 09:37:06.000000 UzbekNLP-0.0.1/README.md
--rw-rw-rw-   0        0        0      552 2023-05-05 09:54:37.000000 UzbekNLP-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 09:54:45.934968 UzbekNLP-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-05-05 09:46:32.000000 UzbekNLP-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:54:45.915130 UzbekNLP-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 09:54:45.915130 UzbekNLP-0.0.1/src/UzbekNLP/
--rw-rw-rw-   0        0        0      187 2023-05-05 09:20:35.000000 UzbekNLP-0.0.1/src/UzbekNLP/Tokenizer.py
--rw-rw-rw-   0        0        0        0 2023-05-05 09:16:28.000000 UzbekNLP-0.0.1/src/UzbekNLP/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:54:45.930775 UzbekNLP-0.0.1/src/UzbekNLP.egg-info/
--rw-rw-rw-   0        0        0      754 2023-05-05 09:54:45.000000 UzbekNLP-0.0.1/src/UzbekNLP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-05 09:54:45.000000 UzbekNLP-0.0.1/src/UzbekNLP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:54:45.000000 UzbekNLP-0.0.1/src/UzbekNLP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 09:54:45.000000 UzbekNLP-0.0.1/src/UzbekNLP.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 10:18:12.938805 UzbekNLP-0.0.2/
+-rw-rw-rw-   0        0        0     1096 2023-05-05 09:39:17.000000 UzbekNLP-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      754 2023-05-05 10:18:12.938805 UzbekNLP-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2023-05-05 09:37:06.000000 UzbekNLP-0.0.2/README.md
+-rw-rw-rw-   0        0        0      552 2023-05-05 10:17:42.000000 UzbekNLP-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 10:18:12.938805 UzbekNLP-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1121 2023-05-05 10:17:27.000000 UzbekNLP-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:18:12.931570 UzbekNLP-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 10:18:12.935671 UzbekNLP-0.0.2/src/UzbekNLP/
+-rw-rw-rw-   0        0        0      187 2023-05-05 09:20:35.000000 UzbekNLP-0.0.2/src/UzbekNLP/Tokenizer.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 09:16:28.000000 UzbekNLP-0.0.2/src/UzbekNLP/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:18:12.937723 UzbekNLP-0.0.2/src/UzbekNLP.egg-info/
+-rw-rw-rw-   0        0        0      754 2023-05-05 10:18:12.000000 UzbekNLP-0.0.2/src/UzbekNLP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-05 10:18:12.000000 UzbekNLP-0.0.2/src/UzbekNLP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:18:12.000000 UzbekNLP-0.0.2/src/UzbekNLP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 10:18:12.000000 UzbekNLP-0.0.2/src/UzbekNLP.egg-info/top_level.txt
```

### Comparing `UzbekNLP-0.0.1/LICENSE` & `UzbekNLP-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UzbekNLP-0.0.1/PKG-INFO` & `UzbekNLP-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekNLP
-Version: 0.0.1
+Version: 0.0.2
 Summary: NLP library for Uzbek language
 Home-page: https://github.com/OllaberganYuldashov/UzbekNLP
 Author: Maksud Sharipov, Ollabergan Yuldashov
 Author-email: "Maksud Sharipov, Ollabergan Yuldashov" <maqsbek72@gmail.com>
 Project-URL: Homepage, https://github.com/OllaberganYuldashov/UzbekNLP
 Project-URL: Bug Tracker, https://github.com/OllaberganYuldashov/UzbekNLP/issues
 Keywords: python,UzbekNLP,uzbek words,NLP
```

### Comparing `UzbekNLP-0.0.1/pyproject.toml` & `UzbekNLP-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "UzbekNLP"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Maksud Sharipov, Ollabergan Yuldashov", email="maqsbek72@gmail.com" },
 ]
 description = "NLP library for Uzbek language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `UzbekNLP-0.0.1/setup.py` & `UzbekNLP-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="UzbekNLP",
-    version="0.0.1",
+    version="0.0.2",
     author="Maksud Sharipov, Ollabergan Yuldashov",
-    author_email="maqsbek72@gmail.com, ollaberganyuldashov@gmail.com",
+    author_email="maqsbek72@gmail.com",
     description="NLP library for Uzbek language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OllaberganYuldashov/UzbekNLP",
     project_urls={
         "Bug Tracker": "https://github.com/OllaberganYuldashov/UzbekNLP/issues",
     },
```

### Comparing `UzbekNLP-0.0.1/src/UzbekNLP.egg-info/PKG-INFO` & `UzbekNLP-0.0.2/src/UzbekNLP.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzbekNLP
-Version: 0.0.1
+Version: 0.0.2
 Summary: NLP library for Uzbek language
 Home-page: https://github.com/OllaberganYuldashov/UzbekNLP
 Author: Maksud Sharipov, Ollabergan Yuldashov
 Author-email: "Maksud Sharipov, Ollabergan Yuldashov" <maqsbek72@gmail.com>
 Project-URL: Homepage, https://github.com/OllaberganYuldashov/UzbekNLP
 Project-URL: Bug Tracker, https://github.com/OllaberganYuldashov/UzbekNLP/issues
 Keywords: python,UzbekNLP,uzbek words,NLP
```

