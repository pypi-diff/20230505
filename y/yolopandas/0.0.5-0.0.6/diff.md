# Comparing `tmp/yolopandas-0.0.5.tar.gz` & `tmp/yolopandas-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolopandas-0.0.5.tar", max compression
+gzip compressed data, was "yolopandas-0.0.6.tar", max compression
```

## Comparing `yolopandas-0.0.5.tar` & `yolopandas-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-01-16 20:13:41.162755 yolopandas-0.0.5/LICENSE
--rw-r--r--   0        0        0     4436 2023-01-17 00:27:48.952984 yolopandas-0.0.5/README.md
--rw-r--r--   0        0        0      860 2023-01-28 14:06:21.128270 yolopandas-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      113 2023-01-16 20:13:41.172755 yolopandas-0.0.5/yolopandas/__init__.py
--rw-r--r--   0        0        0     2395 2023-01-28 14:02:23.568270 yolopandas-0.0.5/yolopandas/chains.py
--rw-r--r--   0        0        0     2203 2023-01-28 14:02:23.568270 yolopandas-0.0.5/yolopandas/llm_accessor.py
--rw-r--r--   0        0        0     5159 1970-01-01 00:00:00.000000 yolopandas-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-01-16 20:13:41.162755 yolopandas-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4436 2023-01-17 00:27:48.952984 yolopandas-0.0.6/README.md
+-rw-r--r--   0        0        0      855 2023-05-03 07:51:20.134425 yolopandas-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-01-16 20:13:41.172755 yolopandas-0.0.6/yolopandas/__init__.py
+-rw-r--r--   0        0        0     2395 2023-01-28 14:02:23.568270 yolopandas-0.0.6/yolopandas/chains.py
+-rw-r--r--   0        0        0     2203 2023-01-28 14:02:23.568270 yolopandas-0.0.6/yolopandas/llm_accessor.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:53:31.664373 yolopandas-0.0.6/yolopandas/utils/__init__.py
+-rw-r--r--   0        0        0     1267 2023-05-03 06:53:31.664373 yolopandas-0.0.6/yolopandas/utils/query_helpers.py
+-rw-r--r--   0        0        0     5149 1970-01-01 00:00:00.000000 yolopandas-0.0.6/PKG-INFO
```

### Comparing `yolopandas-0.0.5/LICENSE` & `yolopandas-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yolopandas-0.0.5/README.md` & `yolopandas-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `yolopandas-0.0.5/pyproject.toml` & `yolopandas-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "yolopandas"
-version = "0.0.5"
+version = "0.0.6"
 description = "Interact with Pandas objects via LLMs and langchain."
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/ccurme/yolopandas"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 ipython = "^8.8.0"
 langchain = ">= 0.0.60, < 1"
-openai = "^0.26.0"
+openai = "^0"
 pandas = "^1.4"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `yolopandas-0.0.5/yolopandas/chains.py` & `yolopandas-0.0.6/yolopandas/chains.py`

 * *Files identical despite different names*

### Comparing `yolopandas-0.0.5/yolopandas/llm_accessor.py` & `yolopandas-0.0.6/yolopandas/llm_accessor.py`

 * *Files identical despite different names*

### Comparing `yolopandas-0.0.5/PKG-INFO` & `yolopandas-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: yolopandas
-Version: 0.0.5
+Version: 0.0.6
 Summary: Interact with Pandas objects via LLMs and langchain.
 Home-page: https://www.github.com/ccurme/yolopandas
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipython (>=8.8.0,<9.0.0)
 Requires-Dist: langchain (>=0.0.60,<1)
-Requires-Dist: openai (>=0.26.0,<0.27.0)
+Requires-Dist: openai (>=0,<1)
 Requires-Dist: pandas (>=1.4,<2.0)
 Project-URL: Repository, https://www.github.com/ccurme/yolopandas
 Description-Content-Type: text/markdown
 
 # YOLOPandas
 
 Interact with Pandas objects via LLMs and [LangChain](https://github.com/hwchase17/langchain).
```

