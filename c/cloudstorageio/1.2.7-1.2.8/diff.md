# Comparing `tmp/cloudstorageio-1.2.7.tar.gz` & `tmp/cloudstorageio-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudstorageio-1.2.7.tar", last modified: Wed Oct  5 09:55:37 2022, max compression
+gzip compressed data, was "cloudstorageio-1.2.8.tar", last modified: Thu May  4 17:24:29 2023, max compression
```

## Comparing `cloudstorageio-1.2.7.tar` & `cloudstorageio-1.2.8.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.621055 cloudstorageio-1.2.7/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1068 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/LICENSE
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5272 2022-10-05 09:55:37.621055 cloudstorageio-1.2.7/PKG-INFO
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3516 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/README.md
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.617056 cloudstorageio-1.2.7/cloudstorageio/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      220 2022-10-05 09:55:02.000000 cloudstorageio-1.2.7/cloudstorageio/__init__.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.617056 cloudstorageio-1.2.7/cloudstorageio/configs/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       64 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/configs/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      401 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/configs/configs.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.617056 cloudstorageio-1.2.7/cloudstorageio/configs/resources/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/configs/resources/__init__.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.617056 cloudstorageio-1.2.7/cloudstorageio/enums/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       40 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/enums/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      142 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/enums/enums.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.617056 cloudstorageio-1.2.7/cloudstorageio/exceptions/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       50 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/exceptions/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      196 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/exceptions/exceptions.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.621055 cloudstorageio-1.2.7/cloudstorageio/interface/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      336 2022-10-05 09:25:25.000000 cloudstorageio-1.2.7/cloudstorageio/interface/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6654 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/interface/async_cloud.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    12492 2022-10-05 09:25:25.000000 cloudstorageio-1.2.7/cloudstorageio/interface/cloud_interface.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     9405 2022-10-05 09:25:25.000000 cloudstorageio-1.2.7/cloudstorageio/interface/drop_box.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    10673 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/interface/google_drive.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     9094 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/interface/google_storage.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5535 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/interface/local_storage.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    12221 2022-10-04 12:38:34.000000 cloudstorageio-1.2.7/cloudstorageio/interface/s3.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.621055 cloudstorageio-1.2.7/cloudstorageio/log/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/log/__init__.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.621055 cloudstorageio-1.2.7/cloudstorageio/tools/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/tools/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1033 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/tools/ci_collections.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2951 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/tools/decorators.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      236 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/cloudstorageio/tools/logger.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.617056 cloudstorageio-1.2.7/cloudstorageio.egg-info/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5272 2022-10-05 09:55:37.000000 cloudstorageio-1.2.7/cloudstorageio.egg-info/PKG-INFO
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1032 2022-10-05 09:55:37.000000 cloudstorageio-1.2.7/cloudstorageio.egg-info/SOURCES.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        1 2022-10-05 09:55:37.000000 cloudstorageio-1.2.7/cloudstorageio.egg-info/dependency_links.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       72 2022-10-05 09:55:37.000000 cloudstorageio-1.2.7/cloudstorageio.egg-info/requires.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       20 2022-10-05 09:55:37.000000 cloudstorageio-1.2.7/cloudstorageio.egg-info/top_level.txt
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2022-10-05 09:55:37.621055 cloudstorageio-1.2.7/docs/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/docs/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      792 2022-08-22 11:54:12.000000 cloudstorageio-1.2.7/docs/additional_docs.md
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      725 2022-10-05 09:55:37.621055 cloudstorageio-1.2.7/setup.cfg
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       38 2022-10-05 09:52:37.000000 cloudstorageio-1.2.7/setup.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1905 2023-05-04 17:16:09.000000 cloudstorageio-1.2.8/CHANGELOG.md
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1068 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/LICENSE
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5430 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3516 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/README.md
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      220 2023-05-04 17:16:20.000000 cloudstorageio-1.2.8/cloudstorageio/__init__.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/configs/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       64 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/configs/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      401 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/configs/configs.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/configs/resources/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/configs/resources/__init__.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/enums/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       40 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/enums/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      142 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/enums/enums.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/exceptions/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       50 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/exceptions/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      196 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/exceptions/exceptions.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/cloudstorageio/interface/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      336 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6654 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/async_cloud.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    12492 2023-05-04 16:51:03.000000 cloudstorageio-1.2.8/cloudstorageio/interface/cloud_interface.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     9405 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/drop_box.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    10673 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/google_drive.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     9094 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/google_storage.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5535 2023-05-04 16:51:03.000000 cloudstorageio-1.2.8/cloudstorageio/interface/local_storage.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    12626 2023-05-04 17:15:23.000000 cloudstorageio-1.2.8/cloudstorageio/interface/s3.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/cloudstorageio/log/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/log/__init__.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/cloudstorageio/tools/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/tools/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1033 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/tools/ci_collections.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2951 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/tools/decorators.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      236 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/tools/logger.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio.egg-info/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5430 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1045 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/SOURCES.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        1 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/dependency_links.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       72 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/requires.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       20 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/top_level.txt
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/docs/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/docs/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      792 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/docs/additional_docs.md
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      725 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/setup.cfg
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       38 2023-05-04 17:14:38.000000 cloudstorageio-1.2.8/setup.py
```

### Comparing `cloudstorageio-1.2.7/LICENSE` & `cloudstorageio-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/PKG-INFO` & `cloudstorageio-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstorageio
-Version: 1.2.7
+Version: 1.2.8
 Home-page: https://github.com/cognaize/cloudstorageio
 Author: cognaize
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cloudstorageio
 
@@ -184,7 +184,10 @@
 - Add AWS session token support
 ### [1.2.3] - 2020-11-10
 - Remove dropbox package dependency (dropbox will not be supported with this version)
 ### [1.2.4] - 2020-11-10
 - Add option include_files for listdir
 ### [1.2.7] - 2022-10-05
 - Updated build to setuptools
+### [1.2.8] - 2022-05-04
+- Fix error on listdir for s3 if the folder did not include subfolders
+- Add option include_files for listdir for non-recursive case
```

### Comparing `cloudstorageio-1.2.7/README.md` & `cloudstorageio-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/cloudstorageio/interface/async_cloud.py` & `cloudstorageio-1.2.8/cloudstorageio/interface/async_cloud.py`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/cloudstorageio/interface/cloud_interface.py` & `cloudstorageio-1.2.8/cloudstorageio/interface/cloud_interface.py`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/cloudstorageio/interface/drop_box.py` & `cloudstorageio-1.2.8/cloudstorageio/interface/drop_box.py`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/cloudstorageio/interface/google_drive.py` & `cloudstorageio-1.2.8/cloudstorageio/interface/google_drive.py`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/cloudstorageio/interface/google_storage.py` & `cloudstorageio-1.2.8/cloudstorageio/interface/google_storage.py`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/cloudstorageio/interface/local_storage.py` & `cloudstorageio-1.2.8/cloudstorageio/interface/local_storage.py`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/cloudstorageio/interface/s3.py` & `cloudstorageio-1.2.8/cloudstorageio/interface/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,24 +192,33 @@
             self._analyse_path(path)
             if include_folders:
                 folders_list = [f for f in self._listdir if f.endswith('/')]
                 self._listdir = self._object_key_list + folders_list
             else:
                 self._listdir = [f for f in self._object_key_list if not f.endswith('/')]
         else:
-            if not self.folder_exists(bucket=self._current_bucket, path=self._current_path):
-                raise FileNotFoundError(f'No such file or dictionary: {path}')
-            if self._current_bucket == self._current_path:
-                result = paginator.paginate(Bucket=self._current_bucket, Delimiter='/')
-                for prefix in result.search('CommonPrefixes'):
-                    folders.append(prefix.get('Prefix').split('/')[-2] + '/')
-            else:
-                result = paginator.paginate(Bucket=self._current_bucket, Delimiter='/', Prefix=current_path)
-                for prefix in result.search('CommonPrefixes'):
-                    folders.append(prefix.get('Prefix').split('/')[-2] + '/')
+            if include_folders:
+                if not self.folder_exists(bucket=self._current_bucket,
+                                          path=self._current_path):
+                    raise FileNotFoundError(
+                        f'No such file or dictionary: {path}')
+                if self._current_bucket == self._current_path:
+                    result = paginator.paginate(Bucket=self._current_bucket,
+                                                Delimiter='/')
+                    for prefix in result.search('CommonPrefixes'):
+                        folders.append(
+                            prefix.get('Prefix').split('/')[-2] + '/')
+                else:
+                    result = paginator.paginate(Bucket=self._current_bucket,
+                                                Delimiter='/',
+                                                Prefix=current_path)
+                    for prefix in result.search('CommonPrefixes'):
+                        if prefix is not None:
+                            folders.append(
+                                prefix.get('Prefix').split('/')[-2] + '/')
             if include_files:
                 for object_summary in self._bucket.objects.filter(Prefix=current_path, Delimiter='/'):
                     files.append(object_summary.key.split('/')[-1])
 
             self._listdir = folders + files
 
         return self._listdir
```

### Comparing `cloudstorageio-1.2.7/cloudstorageio/tools/ci_collections.py` & `cloudstorageio-1.2.8/cloudstorageio/tools/ci_collections.py`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/cloudstorageio/tools/decorators.py` & `cloudstorageio-1.2.8/cloudstorageio/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/cloudstorageio.egg-info/PKG-INFO` & `cloudstorageio-1.2.8/cloudstorageio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstorageio
-Version: 1.2.7
+Version: 1.2.8
 Home-page: https://github.com/cognaize/cloudstorageio
 Author: cognaize
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cloudstorageio
 
@@ -184,7 +184,10 @@
 - Add AWS session token support
 ### [1.2.3] - 2020-11-10
 - Remove dropbox package dependency (dropbox will not be supported with this version)
 ### [1.2.4] - 2020-11-10
 - Add option include_files for listdir
 ### [1.2.7] - 2022-10-05
 - Updated build to setuptools
+### [1.2.8] - 2022-05-04
+- Fix error on listdir for s3 if the folder did not include subfolders
+- Add option include_files for listdir for non-recursive case
```

### Comparing `cloudstorageio-1.2.7/cloudstorageio.egg-info/SOURCES.txt` & `cloudstorageio-1.2.8/cloudstorageio.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.md
 LICENSE
 README.md
 setup.cfg
 setup.py
 cloudstorageio/__init__.py
 cloudstorageio.egg-info/PKG-INFO
 cloudstorageio.egg-info/SOURCES.txt
```

### Comparing `cloudstorageio-1.2.7/docs/additional_docs.md` & `cloudstorageio-1.2.8/docs/additional_docs.md`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.7/setup.cfg` & `cloudstorageio-1.2.8/setup.cfg`

 * *Files identical despite different names*

