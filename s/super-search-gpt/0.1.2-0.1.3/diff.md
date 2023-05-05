# Comparing `tmp/super_search_gpt-0.1.2.tar.gz` & `tmp/super_search_gpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_search_gpt-0.1.2.tar", last modified: Fri May  5 13:56:44 2023, max compression
+gzip compressed data, was "super_search_gpt-0.1.3.tar", last modified: Fri May  5 14:13:57 2023, max compression
```

## Comparing `super_search_gpt-0.1.2.tar` & `super_search_gpt-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:56:44.487926 super_search_gpt-0.1.2/
--rw-rw-rw-   0        0        0     2725 2023-05-05 13:56:44.487926 super_search_gpt-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1526 2023-05-03 20:45:45.000000 super_search_gpt-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 13:56:44.487926 super_search_gpt-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1525 2023-05-05 13:56:04.000000 super_search_gpt-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:56:44.487926 super_search_gpt-0.1.2/super_search_gpt.egg-info/
--rw-rw-rw-   0        0        0     2725 2023-05-05 13:56:43.000000 super_search_gpt-0.1.2/super_search_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-05 13:56:44.000000 super_search_gpt-0.1.2/super_search_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:56:43.000000 super_search_gpt-0.1.2/super_search_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-05 13:56:43.000000 super_search_gpt-0.1.2/super_search_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:56:43.000000 super_search_gpt-0.1.2/super_search_gpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 14:13:57.205001 super_search_gpt-0.1.3/
+-rw-rw-rw-   0        0        0       44 2023-05-05 14:12:06.000000 super_search_gpt-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2725 2023-05-05 14:13:57.203910 super_search_gpt-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1526 2023-05-03 20:45:45.000000 super_search_gpt-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 14:13:57.205915 super_search_gpt-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-05-05 14:13:23.000000 super_search_gpt-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:13:57.168049 super_search_gpt-0.1.3/super_search/
+-rw-rw-rw-   0        0        0     1203 2023-05-03 20:20:30.000000 super_search_gpt-0.1.3/super_search/NoneDecoder.py
+-rw-rw-rw-   0        0        0    12474 2023-05-03 21:30:44.000000 super_search_gpt-0.1.3/super_search/SuperSearch.py
+-rw-rw-rw-   0        0        0      116 2023-05-05 13:25:18.000000 super_search_gpt-0.1.3/super_search/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:13:57.200286 super_search_gpt-0.1.3/super_search_gpt.egg-info/
+-rw-rw-rw-   0        0        0     2725 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/top_level.txt
```

### Comparing `super_search_gpt-0.1.2/PKG-INFO` & `super_search_gpt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super_search_gpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: SuperSearch is a powerful Python package for advanced search and data extraction. It leverages the GPT-4 AI model, Google search, and web scraping to efficiently obtain information on various topics. Ideal for developers needing quick, accurate responses to complex queries and data extraction, analysis, and summarization from multiple web sources. Easy to integrate, SuperSearch enhances functionality and user experience, saving time on manual research and enabling smarter, more effective solutions.
 Home-page: https://github.com/gershonavi/super_search
 Author: Avi Gershon
 Author-email: gershonavi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `super_search_gpt-0.1.2/README.md` & `super_search_gpt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `super_search_gpt-0.1.2/setup.py` & `super_search_gpt-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="super_search_gpt",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
+    include_package_data=True,
     package_data={"super_search_gpt": ["*.py"]},
     install_requires=[
         "googlesearch-python",
         "beautifulsoup4",
         "openai",
         "pandas",
         "requests-html",
```

### Comparing `super_search_gpt-0.1.2/super_search_gpt.egg-info/PKG-INFO` & `super_search_gpt-0.1.3/super_search_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-search-gpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: SuperSearch is a powerful Python package for advanced search and data extraction. It leverages the GPT-4 AI model, Google search, and web scraping to efficiently obtain information on various topics. Ideal for developers needing quick, accurate responses to complex queries and data extraction, analysis, and summarization from multiple web sources. Easy to integrate, SuperSearch enhances functionality and user experience, saving time on manual research and enabling smarter, more effective solutions.
 Home-page: https://github.com/gershonavi/super_search
 Author: Avi Gershon
 Author-email: gershonavi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

