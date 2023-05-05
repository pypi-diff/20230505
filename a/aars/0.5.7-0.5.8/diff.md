# Comparing `tmp/aars-0.5.7.tar.gz` & `tmp/aars-0.5.8.tar.gz`

## Comparing `aars-0.5.7.tar` & `aars-0.5.8.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.5.7/docs-requirements.txt
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aars-0.5.7/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.7/py.typed
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.5.7/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.5.7/.github/workflows/mkdocs-gh-pages.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.5.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.5.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 aars-0.5.7/docs/FastAPI_Cookbook.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.7/docs/index.md -> ../README.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/Exceptions.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/utils.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/core/AARS.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/core/Index.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.5.7/docs/Code_Reference/core/Record.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.5.7/src/aars/__init__.py
--rw-r--r--   0        0        0    38261 2020-02-02 00:00:00.000000 aars-0.5.7/src/aars/core.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 aars-0.5.7/src/aars/exceptions.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 aars-0.5.7/src/aars/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.7/tests/__init__.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 aars-0.5.7/tests/aars.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aars-0.5.7/tests/fetch_all.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.5.7/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.5.7/LICENSE
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 aars-0.5.7/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 aars-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.5.8/docs-requirements.txt
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aars-0.5.8/mkdocs.yml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.5.8/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.5.8/.github/workflows/mkdocs-gh-pages.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.5.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.5.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 aars-0.5.8/docs/FastAPI_Cookbook.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.8/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/Exceptions.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/utils.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/core/AARS.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/core/Index.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.5.8/docs/Code_Reference/core/Record.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/__init__.py
+-rw-r--r--   0        0        0    38516 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/core.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/py.typed
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 aars-0.5.8/src/aars/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.8/tests/__init__.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 aars-0.5.8/tests/aars.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.5.8/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.5.8/LICENSE
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 aars-0.5.8/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 aars-0.5.8/PKG-INFO
```

### Comparing `aars-0.5.7/mkdocs.yml` & `aars-0.5.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/.github/workflows/mkdocs-gh-pages.yml` & `aars-0.5.8/.github/workflows/mkdocs-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/.github/workflows/publish.yml` & `aars-0.5.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/.github/workflows/python-publish.yml` & `aars-0.5.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/docs/FastAPI_Cookbook.md` & `aars-0.5.8/docs/FastAPI_Cookbook.md`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/src/aars/core.py` & `aars-0.5.8/src/aars/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -964,14 +964,19 @@
         for message in aleph_resp.messages:
             yield message.item_hash
 
         if page == 1:
             # If there are more pages, fetch them
             total_items = aleph_resp.pagination_total
             per_page = aleph_resp.pagination_per_page
+            # log the total number of items and pages
+            logger.debug(
+                f"Found {total_items} items in {channel or 'all channels'}"
+            )
+            logger.debug(f"Fetching {math.ceil(total_items / per_page)} pages")
             if total_items > per_page:
                 for next_page in range(2, math.ceil(total_items / per_page) + 1):
                     async for item_hash in cls.fetch_revisions(
                         record_type=record_type,
                         ref=ref,
                         channel=channel,
                         owner=owner,
```

### Comparing `aars-0.5.7/src/aars/exceptions.py` & `aars-0.5.8/src/aars/exceptions.py`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/src/aars/utils.py` & `aars-0.5.8/src/aars/utils.py`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/tests/aars.py` & `aars-0.5.8/tests/aars.py`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/.gitignore` & `aars-0.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/LICENSE` & `aars-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/README.md` & `aars-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `aars-0.5.7/pyproject.toml` & `aars-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aars"
-version = "0.5.7"
+version = "0.5.8"
 authors = [
   { name="Mike Hukiewitz", email="mike.hukiewitz@robotter.ai" },
 ]
 description = "Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aars-0.5.7/PKG-INFO` & `aars-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aars
-Version: 0.5.7
+Version: 0.5.8
 Summary: Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im
 Project-URL: Homepage, https://github.com/aleph-im/active-record-sdk
 Project-URL: Bug Tracker, https://github.com/aleph-im/active-record-sdk/issues
 Author-email: Mike Hukiewitz <mike.hukiewitz@robotter.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

