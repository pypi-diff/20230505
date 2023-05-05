# Comparing `tmp/xt_st_common-0.4.0.tar.gz` & `tmp/xt_st_common-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.4.0.tar", max compression
+gzip compressed data, was "xt_st_common-0.4.1.tar", max compression
```

## Comparing `xt_st_common-0.4.0.tar` & `xt_st_common-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      606 2023-05-05 03:38:29.753945 xt_st_common-0.4.0/README.md
--rw-r--r--   0        0        0     1541 2023-05-05 03:38:29.753945 xt_st_common-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-05 03:38:29.753945 xt_st_common-0.4.0/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5039 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/components.py
--rw-r--r--   0        0        0     1784 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/config.py
--rw-r--r--   0        0        0     7200 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/database.py
--rw-r--r--   0        0        0    14615 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/file_manager.py
--rw-r--r--   0        0        0     6269 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0     5938 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/session.py
--rw-r--r--   0        0        0     4871 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1774 2023-05-05 03:37:54.569437 xt_st_common-0.4.0/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 xt_st_common-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      606 2023-05-05 05:05:39.749835 xt_st_common-0.4.1/README.md
+-rw-r--r--   0        0        0     1541 2023-05-05 05:05:39.749835 xt_st_common-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-05 05:05:39.749835 xt_st_common-0.4.1/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5039 2023-05-05 05:05:07.689646 xt_st_common-0.4.1/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     1784 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     7200 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/database.py
+-rw-r--r--   0        0        0    14615 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/file_manager.py
+-rw-r--r--   0        0        0     6407 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0     5938 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     4871 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1774 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 xt_st_common-0.4.1/PKG-INFO
```

### Comparing `xt_st_common-0.4.0/README.md` & `xt_st_common-0.4.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.4.0
+# XT-STREAMLIT - 0.4.1
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ### Getting Started
```

### Comparing `xt_st_common-0.4.0/pyproject.toml` & `xt_st_common-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.4.0"
+version = "0.4.1"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `xt_st_common-0.4.0/src/xt_st_common/components.py` & `xt_st_common-0.4.1/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.4.0/src/xt_st_common/config.py` & `xt_st_common-0.4.1/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.4.0/src/xt_st_common/database.py` & `xt_st_common-0.4.1/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.4.0/src/xt_st_common/file_manager.py` & `xt_st_common-0.4.1/src/xt_st_common/file_manager.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.4.0/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.4.1/src/xt_st_common/fs_upload_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,24 +123,27 @@
     dir_list = sorted(set(dir_list), key=len, reverse=True)
     if "dir_list" not in st.session_state:
         st.session_state["dir_list"] = dir_list
     for path in dir_list:
         Path.rmdir(path)
 
 
-def upload_page(data_dir: str, accepted_ft: Union[None, str, List[str]] = None):
+def upload_page(data_dir: str, accepted_ft: Union[None, str, List[str]] = None, dl_prefix: str = "data"):
     """
     Render the upload page which uses the servers local filesystem for storage
 
     ### Parameters
         data_dir: str
             directory to store data in on the server
 
         accepted_ft: str or list of str or None
             Accepted filetypes for upload (passed to `st.file_uploader()`)
+
+        dl_prefix: str
+            Name of the zip when downloading will be `{dl_prefix}-Y-m-d_H.M.S.zip`
     """
     c1, c2 = st.columns(2)
 
     # Show file structure
     with c1:
         file_list = list_directory(data_dir + os.sep)
         file_tree = [
@@ -166,15 +169,15 @@
             dl_data = _prepare_download(ts["checked"], root_dir=data_dir)
 
         l_btn, r_btn, _ = st.columns([1, 1, 2])
         with l_btn:
             st.download_button(
                 "Zip & Download",
                 data=dl_data,
-                file_name=f"fracg-{datetime.now(tz=ZoneInfo(settings.TIMEZONE)).strftime('%Y-%m-%d_%H.%M.%S')}.zip",
+                file_name=f"{dl_prefix}-{datetime.now(tz=ZoneInfo(settings.TIMEZONE)).strftime('%Y-%m-%d_%H.%M.%S')}.zip",
                 disabled=not files_selected,
             )
         with r_btn:
             if st.button(
                 "Delete Selected", disabled=not files_selected, type="primary"
             ):
                 _delete_files(ts["checked"], root_dir=data_dir)
```

### Comparing `xt_st_common-0.4.0/src/xt_st_common/session.py` & `xt_st_common-0.4.1/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.4.0/src/xt_st_common/storage.py` & `xt_st_common-0.4.1/src/xt_st_common/storage.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.4.0/src/xt_st_common/utils.py` & `xt_st_common-0.4.1/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.4.0/PKG-INFO` & `xt_st_common-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.4.0
+Version: 0.4.1
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,15 +16,15 @@
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyjwt[crypto] (>=2.6.0,<3.0.0)
 Requires-Dist: streamlit (>=1.21.0,<2.0.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.4.0
+# XT-STREAMLIT - 0.4.1
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ### Getting Started
```

