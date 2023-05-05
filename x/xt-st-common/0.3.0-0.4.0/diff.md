# Comparing `tmp/xt_st_common-0.3.0.tar.gz` & `tmp/xt_st_common-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.3.0.tar", max compression
+gzip compressed data, was "xt_st_common-0.4.0.tar", max compression
```

## Comparing `xt_st_common-0.3.0.tar` & `xt_st_common-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      606 2023-05-03 08:07:41.171007 xt_st_common-0.3.0/README.md
--rw-r--r--   0        0        0     1508 2023-05-03 08:07:41.171007 xt_st_common-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-03 08:07:41.171007 xt_st_common-0.3.0/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5039 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/components.py
--rw-r--r--   0        0        0     1699 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/config.py
--rw-r--r--   0        0        0     7200 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/database.py
--rw-r--r--   0        0        0    14615 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/file_manager.py
--rw-r--r--   0        0        0     5938 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/session.py
--rw-r--r--   0        0        0     4871 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1774 2023-05-03 08:07:04.010372 xt_st_common-0.3.0/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 xt_st_common-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      606 2023-05-05 03:38:29.753945 xt_st_common-0.4.0/README.md
+-rw-r--r--   0        0        0     1541 2023-05-05 03:38:29.753945 xt_st_common-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-05 03:38:29.753945 xt_st_common-0.4.0/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5039 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     1784 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     7200 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/database.py
+-rw-r--r--   0        0        0    14615 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/file_manager.py
+-rw-r--r--   0        0        0     6269 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0     5938 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     4871 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1774 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 xt_st_common-0.4.0/PKG-INFO
```

### Comparing `xt_st_common-0.3.0/README.md` & `xt_st_common-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.3.0
+# XT-STREAMLIT - 0.4.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ### Getting Started
```

### Comparing `xt_st_common-0.3.0/pyproject.toml` & `xt_st_common-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.3.0"
+version = "0.4.0"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 streamlit = "^1.21.0"
 pydantic = "^1.10.7"
 pyjwt = {extras = ["crypto"], version = "^2.6.0"}
 streamlit-js-eval = "^0.1.5"
 minio = { version = "^7.1.14", optional = true }
 odmantic = { version = "^0.9.2", optional = true }
 chardet = "^5.1.0"
+streamlit-tree-select = "^0.0.5"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 pytest = "^7.3.1"
 coverage = {extras = ["toml"], version = "^7.2.3"}
 pytest-cov = "^4.0.0"
```

### Comparing `xt_st_common-0.3.0/src/xt_st_common/components.py` & `xt_st_common-0.4.0/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.3.0/src/xt_st_common/config.py` & `xt_st_common-0.4.0/src/xt_st_common/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,12 +30,14 @@
     """Error message displayed when a user doesn't have permission to use the app"""
     STREAMLIT_SERVER_BASE_URL_PATH: str = ""
     """The base path for the URL where Streamlit should be served from"""
     MONGO_CONNECTION_STRING: str = ""
     """Mongo DB connection string"""
     DATABASE_NAME: str = ""
     """Mongo DB Database Name"""
+    TIMEZONE: str = "Australia/Perth"
+    """Default timezone used within the app"""
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
         case_sensitive = True
```

### Comparing `xt_st_common-0.3.0/src/xt_st_common/database.py` & `xt_st_common-0.4.0/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.3.0/src/xt_st_common/file_manager.py` & `xt_st_common-0.4.0/src/xt_st_common/file_manager.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.3.0/src/xt_st_common/session.py` & `xt_st_common-0.4.0/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.3.0/src/xt_st_common/storage.py` & `xt_st_common-0.4.0/src/xt_st_common/storage.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.3.0/src/xt_st_common/utils.py` & `xt_st_common-0.4.0/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.3.0/PKG-INFO` & `xt_st_common-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.3.0
+Version: 0.4.0
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,17 +13,18 @@
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
 Requires-Dist: minio (>=7.1.14,<8.0.0) ; extra == "storage"
 Requires-Dist: odmantic (>=0.9.2,<0.10.0) ; extra == "databases"
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyjwt[crypto] (>=2.6.0,<3.0.0)
 Requires-Dist: streamlit (>=1.21.0,<2.0.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
+Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.3.0
+# XT-STREAMLIT - 0.4.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ### Getting Started
```

