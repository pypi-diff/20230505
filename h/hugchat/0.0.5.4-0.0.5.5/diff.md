# Comparing `tmp/hugchat-0.0.5.4.tar.gz` & `tmp/hugchat-0.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.5.4.tar", last modified: Fri May  5 13:53:29 2023, max compression
+gzip compressed data, was "hugchat-0.0.5.5.tar", last modified: Fri May  5 14:27:26 2023, max compression
```

## Comparing `hugchat-0.0.5.4.tar` & `hugchat-0.0.5.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 13:53:29.555837 hugchat-0.0.5.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2874 2023-05-05 13:53:29.555837 hugchat-0.0.5.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1854 2023-05-05 02:29:43.000000 hugchat-0.0.5.4/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-05 13:53:29.555837 hugchat-0.0.5.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1407 2023-05-05 13:53:22.000000 hugchat-0.0.5.4/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 13:53:29.543836 hugchat-0.0.5.4/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 13:53:29.551836 hugchat-0.0.5.4/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.4/src/hugchat/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.4/src/hugchat/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8764 2023-05-05 13:53:16.000000 hugchat-0.0.5.4/src/hugchat/hugchat.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 13:53:29.555837 hugchat-0.0.5.4/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2874 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 14:27:26.165608 hugchat-0.0.5.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2874 2023-05-05 14:27:26.161608 hugchat-0.0.5.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1854 2023-05-05 02:29:43.000000 hugchat-0.0.5.5/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-05 14:27:26.165608 hugchat-0.0.5.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1436 2023-05-05 14:26:47.000000 hugchat-0.0.5.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 14:27:26.161608 hugchat-0.0.5.5/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 14:27:26.161608 hugchat-0.0.5.5/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.5/src/hugchat/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.5/src/hugchat/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8764 2023-05-05 14:25:32.000000 hugchat-0.0.5.5/src/hugchat/hugchat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 14:27:26.161608 hugchat-0.0.5.5/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2874 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-05 14:27:26.000000 hugchat-0.0.5.5/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.5.4/LICENSE` & `hugchat-0.0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.5.4/PKG-INFO` & `hugchat-0.0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.4
+Version: 0.0.5.5
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hugchat-0.0.5.4/README.md` & `hugchat-0.0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.5.4/setup.py` & `hugchat-0.0.5.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.5.4",
+    version="0.0.5.5",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
@@ -16,14 +16,15 @@
     license="GNU Affero General Public License v3.0",
     packages=find_namespace_packages("src"),
     package_dir={"": "src"},
     py_modules=["hugchat"],
     package_data={"": ["*.json"]},
     install_requires=[
         "requests",
+        "requests_toolbelt",
     ],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "Natural Language :: English",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `hugchat-0.0.5.4/src/hugchat/hugchat.py` & `hugchat-0.0.5.5/src/hugchat/hugchat.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.5.4/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.5.5/src/hugchat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.4
+Version: 0.0.5.5
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

