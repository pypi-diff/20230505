# Comparing `tmp/pbx_component_files_uploader-0.0.2.tar.gz` & `tmp/pbx_component_files_uploader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbx_component_files_uploader-0.0.2.tar", max compression
+gzip compressed data, was "pbx_component_files_uploader-0.0.3.tar", max compression
```

## Comparing `pbx_component_files_uploader-0.0.2.tar` & `pbx_component_files_uploader-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/LICENSE
--rw-r--r--   0        0        0      427 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/README.md
--rw-r--r--   0        0        0       22 2023-04-28 07:55:18.616871 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/__init__.py
--rw-r--r--   0        0        0      491 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/exceptions/errors.py
--rw-r--r--   0        0        0     2141 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/auth.py
--rw-r--r--   0        0        0     2045 2023-04-28 08:11:14.105329 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/selectel.py
--rw-r--r--   0        0        0     1610 2023-04-28 07:56:24.891596 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/token.py
--rw-r--r--   0        0        0      402 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/interfaces/base_uploader.py
--rw-r--r--   0        0        0      799 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/uploader.py
--rw-r--r--   0        0        0      638 2023-04-28 07:57:01.522893 pbx_component_files_uploader-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 pbx_component_files_uploader-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.3/LICENSE
+-rw-r--r--   0        0        0      427 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2023-05-04 12:43:47.462068 pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/__init__.py
+-rw-r--r--   0        0        0      491 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/exceptions/errors.py
+-rw-r--r--   0        0        0     2141 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/ext/selectel/auth.py
+-rw-r--r--   0        0        0     2043 2023-05-04 12:35:08.231673 pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/ext/selectel/selectel.py
+-rw-r--r--   0        0        0     1610 2023-04-28 07:56:24.891596 pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/ext/selectel/token.py
+-rw-r--r--   0        0        0      402 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/interfaces/base_uploader.py
+-rw-r--r--   0        0        0      799 2023-04-27 11:33:26.295002 pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/uploader.py
+-rw-r--r--   0        0        0      638 2023-05-04 12:43:56.629968 pbx_component_files_uploader-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 pbx_component_files_uploader-0.0.3/PKG-INFO
```

### Comparing `pbx_component_files_uploader-0.0.2/LICENSE` & `pbx_component_files_uploader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/auth.py` & `pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/ext/selectel/auth.py`

 * *Files identical despite different names*

### Comparing `pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/selectel.py` & `pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/ext/selectel/selectel.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,11 +47,11 @@
 
                 response = requests.put(
                     url=url, data=srcFile.open(mode='rb'), headers=headers)
 
                 if response.status_code == 201:
                     return response.url
             except Exception as e:
-                log.debug(f'Attempt [{i + 1}]. Failed to upload. Cause [{e.__cause__}]')
                 errorDesc = str(e)
+                log.debug(f'Attempt [{i + 1}]. Failed to upload. Cause [{errorDesc}]')
 
         raise UploadError(400, f'Failed upload file [{srcFilePath}]. Cause [{errorDesc}]')
```

### Comparing `pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/ext/selectel/token.py` & `pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/ext/selectel/token.py`

 * *Files identical despite different names*

### Comparing `pbx_component_files_uploader-0.0.2/pbx_component_files_uploader/uploader.py` & `pbx_component_files_uploader-0.0.3/pbx_component_files_uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `pbx_component_files_uploader-0.0.2/pyproject.toml` & `pbx_component_files_uploader-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbx-component-files-uploader"
-version = "0.0.2"
+version = "0.0.3"
 description = "Files uploader to custom storages"
 authors = [
     "Ivan Kalashnikov <ivan@leadvertex.ru>"
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/leadvertex/pbx-component-files-uploader"
```

### Comparing `pbx_component_files_uploader-0.0.2/PKG-INFO` & `pbx_component_files_uploader-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbx-component-files-uploader
-Version: 0.0.2
+Version: 0.0.3
 Summary: Files uploader to custom storages
 Home-page: https://github.com/leadvertex/pbx-component-files-uploader
 License: MIT
 Keywords: leadvertex,selectel,storage,remote storage,uploader
 Author: Ivan Kalashnikov
 Author-email: ivan@leadvertex.ru
 Requires-Python: >=3.7,<4.0
```

