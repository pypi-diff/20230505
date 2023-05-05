# Comparing `tmp/heaserver-trash-aws-s3-1.0.0a3.tar.gz` & `tmp/heaserver-trash-aws-s3-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a3.tar", last modified: Wed May  3 03:59:55 2023, max compression
+gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a4.tar", last modified: Fri May  5 17:26:54 2023, max compression
```

## Comparing `heaserver-trash-aws-s3-1.0.0a3.tar` & `heaserver-trash-aws-s3-1.0.0a4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.470519 heaserver-trash-aws-s3-1.0.0a3/
--rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/LICENSE
--rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0     4352 2023-05-03 03:59:55.469519 heaserver-trash-aws-s3-1.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 03:59:55.470519 heaserver-trash-aws-s3-1.0.0a3/setup.cfg
--rw-rw-rw-   0        0        0     1869 2023-05-03 03:59:21.000000 heaserver-trash-aws-s3-1.0.0a3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.431800 heaserver-trash-aws-s3-1.0.0a3/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.430230 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.443520 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/__init__.py
--rw-rw-rw-   0        0        0    47564 2023-05-03 03:58:45.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/service.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.444520 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/wstl/
--rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.465518 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     4352 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 03:59:55.000000 heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.432802 heaserver-trash-aws-s3-1.0.0a3/tests/
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.432802 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:55.468519 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/__init__.py
--rw-rw-rw-   0        0        0    69298 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/test_all.py
--rw-rw-rw-   0        0        0     6276 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/testcase.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.631208 heaserver-trash-aws-s3-1.0.0a4/
+-rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4352 2023-05-05 17:26:54.630208 heaserver-trash-aws-s3-1.0.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 17:26:54.631208 heaserver-trash-aws-s3-1.0.0a4/setup.cfg
+-rw-rw-rw-   0        0        0     1869 2023-05-05 17:26:10.000000 heaserver-trash-aws-s3-1.0.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.574209 heaserver-trash-aws-s3-1.0.0a4/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.573208 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/
+drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.593213 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/__init__.py
+-rw-rw-rw-   0        0        0    48628 2023-05-05 17:24:22.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/service.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.594209 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/wstl/
+-rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.626207 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     4352 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.575209 heaserver-trash-aws-s3-1.0.0a4/tests/
+drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.576209 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.629208 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/__init__.py
+-rw-rw-rw-   0        0        0    69298 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/test_all.py
+-rw-rw-rw-   0        0        0     6276 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/testcase.py
```

### Comparing `heaserver-trash-aws-s3-1.0.0a3/LICENSE` & `heaserver-trash-aws-s3-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a3/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a3/README.md` & `heaserver-trash-aws-s3-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a3/setup.py` & `heaserver-trash-aws-s3-1.0.0a4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-trash-aws-s3',
-    version='1.0.0a3',
+    version='1.0.0a4',
     description="deleted file management",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=['heaserver.trashawss3'],
       package_data={'heaserver.trashawss3': ['wstl/*.json']},
       install_requires=[
-          'heaserver>=1.0.0a115, <1.0.0a116'
+          'heaserver>=1.0.0a116, <1.0.0a117'
       ],
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Environment :: Console',
           'Intended Audience :: Developers',
           'Natural Language :: English',
           'License :: OSI Approved :: Apache Software License',
```

### Comparing `heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/service.py` & `heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,14 +425,30 @@
     """
     return await response.get_all(request, [i async for i in _get_deleted_items(request)])
 
 
 
 @routes.get('/volumes/{volume_id}/awss3trash/')
 @routes.get('/volumes/{volume_id}/awss3trash')
+@action(name='heaserver-awss3trash-item-get-open-choices',
+        rel='hea-opener-choices hea-context-menu',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/opener',
+        itemif='isheaobject(heaobject.folder.AWSS3Folder)')
+@action('heaserver-awss3trash-item-get-properties',
+        rel='hea-properties hea-context-menu')
+@action('heaserver-awss3trash-item-restore',
+        rel='hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/restorer')
+@action('heaserver-awss3trash-item-permanently-delete',
+        rel='hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}/deleter')
+@action('heaserver-awss3trash-item-get-self', rel='self',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trash/{id}')
+@action('heaserver-awss3trash-do-empty-trash', rel='hea-trash-emptier',
+        path='/volumes/{volume_id}/buckets/{bucket_id}/awss3trashemptier')
 async def get_all_deleted_items_all_buckets(request: web.Request) -> web.Response:
     """
     Gets a list of all deleted items in a volume.
 
     :param request: the HTTP request.
     :return: the list of items with delete markers.
     ---
```

### Comparing `heaserver-trash-aws-s3-1.0.0a3/src/heaserver/trashawss3/wstl/all.json` & `heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a3/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt` & `heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/test_all.py` & `heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a3/tests/heaserver/trashawss3test/testcase.py` & `heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/testcase.py`

 * *Files identical despite different names*

