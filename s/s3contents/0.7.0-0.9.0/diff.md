# Comparing `tmp/s3contents-0.7.0.tar.gz` & `tmp/s3contents-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3contents-0.7.0.tar", last modified: Sun Aug 15 00:55:14 2021, max compression
+gzip compressed data, was "s3contents-0.9.0.tar", max compression
```

## Comparing `s3contents-0.7.0.tar` & `s3contents-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,24 @@
-drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2021-08-15 00:55:14.133293 s3contents-0.7.0/
-drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2021-08-15 00:55:14.118803 s3contents-0.7.0/.github/
-drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2021-08-15 00:55:14.125119 s3contents-0.7.0/.github/workflows/
--rw-r--r--   0 danielfrg   (501) staff       (20)     2120 2021-08-14 23:43:57.000000 s3contents-0.7.0/.github/workflows/test.yml
--rw-r--r--   0 danielfrg   (501) staff       (20)     1642 2021-08-14 23:19:03.000000 s3contents-0.7.0/.gitignore
--rw-r--r--   0 danielfrg   (501) staff       (20)      699 2021-08-15 00:54:21.000000 s3contents-0.7.0/CHANGELOG.md
--rw-r--r--   0 danielfrg   (501) staff       (20)      913 2021-08-14 23:23:43.000000 s3contents-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 danielfrg   (501) staff       (20)    11358 2021-08-14 23:19:03.000000 s3contents-0.7.0/LICENSE.txt
--rw-r--r--   0 danielfrg   (501) staff       (20)     2089 2021-08-14 23:50:35.000000 s3contents-0.7.0/Makefile
--rw-r--r--   0 danielfrg   (501) staff       (20)    10808 2021-08-15 00:55:14.133590 s3contents-0.7.0/PKG-INFO
--rw-r--r--   0 danielfrg   (501) staff       (20)     8326 2021-08-14 23:19:03.000000 s3contents-0.7.0/README.md
--rw-r--r--   0 danielfrg   (501) staff       (20)      918 2021-08-14 23:19:03.000000 s3contents-0.7.0/RELEASE.md
--rw-r--r--   0 danielfrg   (501) staff       (20)      419 2021-08-15 00:20:46.000000 s3contents-0.7.0/environment.yml
--rw-r--r--   0 danielfrg   (501) staff       (20)     1097 2021-08-14 23:19:03.000000 s3contents-0.7.0/pyproject.toml
--rw-r--r--   0 danielfrg   (501) staff       (20)      292 2021-08-15 00:20:48.000000 s3contents-0.7.0/requirements-dev.txt
--rw-r--r--   0 danielfrg   (501) staff       (20)      107 2021-08-14 23:35:04.000000 s3contents-0.7.0/requirements.txt
-drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2021-08-15 00:55:14.128247 s3contents-0.7.0/s3contents/
--rw-r--r--   0 danielfrg   (501) staff       (20)     1090 2021-08-14 23:19:03.000000 s3contents-0.7.0/s3contents/__init__.py
--rw-r--r--   0 danielfrg   (501) staff       (20)      142 2021-08-15 00:55:13.000000 s3contents-0.7.0/s3contents/_generated_version.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1601 2021-08-14 23:19:03.000000 s3contents-0.7.0/s3contents/chunks.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     7073 2021-08-15 00:43:03.000000 s3contents-0.7.0/s3contents/gcs_fs.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1231 2021-08-14 23:19:03.000000 s3contents-0.7.0/s3contents/gcsmanager.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1876 2021-08-14 23:19:03.000000 s3contents-0.7.0/s3contents/genericfs.py
--rw-r--r--   0 danielfrg   (501) staff       (20)    15084 2021-08-15 00:15:59.000000 s3contents-0.7.0/s3contents/genericmanager.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1630 2021-08-15 00:27:44.000000 s3contents-0.7.0/s3contents/ipycompat.py
--rw-r--r--   0 danielfrg   (501) staff       (20)    10695 2021-08-15 00:42:18.000000 s3contents-0.7.0/s3contents/s3_fs.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     5037 2021-08-14 23:19:03.000000 s3contents-0.7.0/s3contents/s3manager.py
-drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2021-08-15 00:55:14.133028 s3contents-0.7.0/s3contents/tests/
--rw-r--r--   0 danielfrg   (501) staff       (20)        0 2021-08-14 23:19:03.000000 s3contents-0.7.0/s3contents/tests/__init__.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1147 2021-08-15 00:26:05.000000 s3contents-0.7.0/s3contents/tests/hooks.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1021 2021-08-15 00:26:52.000000 s3contents-0.7.0/s3contents/tests/test_gcsmanager.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1385 2021-08-15 00:26:27.000000 s3contents-0.7.0/s3contents/tests/test_gcsmanager_chunked.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1069 2021-08-15 00:26:47.000000 s3contents-0.7.0/s3contents/tests/test_gcsmanager_with_prefix.py
--rw-r--r--   0 danielfrg   (501) staff       (20)      176 2021-08-14 23:19:03.000000 s3contents-0.7.0/s3contents/tests/test_import.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     2921 2021-08-15 00:27:05.000000 s3contents-0.7.0/s3contents/tests/test_s3manager.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1539 2021-08-15 00:26:32.000000 s3contents-0.7.0/s3contents/tests/test_s3manager_chunked.py
--rw-r--r--   0 danielfrg   (501) staff       (20)     1222 2021-08-15 00:26:57.000000 s3contents-0.7.0/s3contents/tests/test_s3manager_with_prefix.py
-drwxr-xr-x   0 danielfrg   (501) staff       (20)        0 2021-08-15 00:55:14.130073 s3contents-0.7.0/s3contents.egg-info/
--rw-r--r--   0 danielfrg   (501) staff       (20)    10808 2021-08-15 00:55:13.000000 s3contents-0.7.0/s3contents.egg-info/PKG-INFO
--rw-r--r--   0 danielfrg   (501) staff       (20)      982 2021-08-15 00:55:13.000000 s3contents-0.7.0/s3contents.egg-info/SOURCES.txt
--rw-r--r--   0 danielfrg   (501) staff       (20)        1 2021-08-15 00:55:13.000000 s3contents-0.7.0/s3contents.egg-info/dependency_links.txt
--rw-r--r--   0 danielfrg   (501) staff       (20)        1 2021-08-14 23:31:23.000000 s3contents-0.7.0/s3contents.egg-info/not-zip-safe
--rw-r--r--   0 danielfrg   (501) staff       (20)      350 2021-08-15 00:55:13.000000 s3contents-0.7.0/s3contents.egg-info/requires.txt
--rw-r--r--   0 danielfrg   (501) staff       (20)       11 2021-08-15 00:55:13.000000 s3contents-0.7.0/s3contents.egg-info/top_level.txt
--rw-r--r--   0 danielfrg   (501) staff       (20)      175 2021-08-15 00:55:14.134617 s3contents-0.7.0/setup.cfg
--rw-r--r--   0 danielfrg   (501) staff       (20)     1487 2021-08-14 23:19:03.000000 s3contents-0.7.0/setup.py
+-rw-r--r--   0        0        0    11358 2021-09-22 01:51:37.909694 s3contents-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     9439 2021-11-24 02:45:15.594957 s3contents-0.9.0/README.md
+-rw-r--r--   0        0        0     2555 2021-11-30 16:48:19.551164 s3contents-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2021-11-30 16:48:14.689231 s3contents-0.9.0/s3contents/__init__.py
+-rw-r--r--   0        0        0     1620 2021-09-22 03:51:31.669379 s3contents-0.9.0/s3contents/chunks.py
+-rw-r--r--   0        0        0      261 2021-11-24 02:52:38.991009 s3contents-0.9.0/s3contents/gcs/__init__.py
+-rw-r--r--   0        0        0     7258 2021-11-24 05:12:34.670631 s3contents-0.9.0/s3contents/gcs/gcs_fs.py
+-rw-r--r--   0        0        0     1235 2021-11-24 01:41:52.342844 s3contents-0.9.0/s3contents/gcs/gcsmanager.py
+-rw-r--r--   0        0        0     1876 2021-09-22 01:51:37.910743 s3contents-0.9.0/s3contents/genericfs.py
+-rw-r--r--   0        0        0    17443 2021-11-29 23:25:24.208435 s3contents-0.9.0/s3contents/genericmanager.py
+-rw-r--r--   0        0        0     1641 2021-09-22 03:51:31.670307 s3contents-0.9.0/s3contents/ipycompat.py
+-rw-r--r--   0        0        0    10962 2021-11-29 23:25:24.208639 s3contents-0.9.0/s3contents/s3_fs.py
+-rw-r--r--   0        0        0     5421 2021-11-24 02:19:31.826751 s3contents-0.9.0/s3contents/s3manager.py
+-rw-r--r--   0        0        0        0 2021-09-22 01:51:37.911095 s3contents-0.9.0/s3contents/tests/__init__.py
+-rw-r--r--   0        0        0     1084 2021-11-24 02:51:31.437792 s3contents-0.9.0/s3contents/tests/gcs/test_gcsmanager.py
+-rw-r--r--   0        0        0     1458 2021-11-24 02:51:04.844234 s3contents-0.9.0/s3contents/tests/gcs/test_gcsmanager_chunked.py
+-rw-r--r--   0        0        0     1132 2021-11-24 02:51:27.457816 s3contents-0.9.0/s3contents/tests/gcs/test_gcsmanager_with_prefix.py
+-rw-r--r--   0        0        0     1161 2021-09-22 03:51:31.670939 s3contents-0.9.0/s3contents/tests/hooks.py
+-rw-r--r--   0        0        0      221 2021-09-29 23:46:57.766467 s3contents-0.9.0/s3contents/tests/test_pkg.py
+-rw-r--r--   0        0        0     2923 2021-11-24 03:02:50.767614 s3contents-0.9.0/s3contents/tests/test_s3manager.py
+-rw-r--r--   0        0        0     1548 2021-09-22 03:51:31.672000 s3contents-0.9.0/s3contents/tests/test_s3manager_chunked.py
+-rw-r--r--   0        0        0     1222 2021-09-22 03:51:31.672188 s3contents-0.9.0/s3contents/tests/test_s3manager_with_prefix.py
+-rw-r--r--   0        0        0    10632 1970-01-01 00:00:00.000000 s3contents-0.9.0/setup.py
+-rw-r--r--   0        0        0    10618 1970-01-01 00:00:00.000000 s3contents-0.9.0/PKG-INFO
```

### Comparing `s3contents-0.7.0/LICENSE.txt` & `s3contents-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `s3contents-0.7.0/PKG-INFO` & `s3contents-0.9.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,248 +1,299 @@
-Metadata-Version: 2.1
-Name: s3contents
-Version: 0.7.0
-Summary: S3 Contents Manager for Jupyter
-Home-page: https://github.com/danielfrg/s3contents
-Maintainer: Daniel Rodriguez
-Maintainer-email: daniel@danielfrg.com
-License: Apache License, Version 2.0
-Description: # S3Contents
-        
-        [![pypi](https://badge.fury.io/py/s3contents.svg)](https://pypi.org/project/s3contents/)
-        [![build](https://github.com/danielfrg/s3contents/workflows/test/badge.svg)](https://github.com/danielfrg/s3contents/actions/workflows/test.yml)
-        [![coverage](https://codecov.io/gh/danielfrg/s3contents/branch/master/graph/badge.svg)](https://codecov.io/gh/danielfrg/s3contents?branch=master)
-        [![licence](https://img.shields.io/:license-Apache%202-blue.svg)](http://github.com/danielfrg/s3contents/blob/master/LICENSE.txt)
-        
-        An S3 and GCS backed ContentsManager implementation for Jupyter.
-        
-        It aims to a be a transparent, drop-in replacement for Jupyter standard filesystem-backed storage system.
-        With this implementation of a Jupyter Contents Manager you can save all your notebooks, regular files, directories
-        structure directly to a S3/GCS bucket, this could be on AWS/GCP or a self hosted S3 API compatible like [minio](http://minio.io).
-        
-        ## Prerequisites
-        
-        Write access (valid credentials) to an S3/GCS bucket, this could be on AWS/GCP or a self hosted S3 like [minio](http://minio.io).
-        
-        ## Installation
-        
-        ```
-        pip install s3contents
-        ```
-        
-        ## Jupyter config
-        
-        Edit `~/.jupyter/jupyter_notebook_config.py` based on the backend you want to
-        based on the examples below. Replace credentials as needed.
-        
-        ## AWS S3
-        
-        ```python
-        from s3contents import S3ContentsManager
-        
-        c = get_config()
-        
-        # Tell Jupyter to use S3ContentsManager for all storage.
-        c.NotebookApp.contents_manager_class = S3ContentsManager
-        c.S3ContentsManager.access_key_id = "{{ AWS Access Key ID / IAM Access Key ID }}"
-        c.S3ContentsManager.secret_access_key = "{{ AWS Secret Access Key / IAM Secret Access Key }}"
-        c.S3ContentsManager.session_token = "{{ AWS Session Token / IAM Session Token }}"
-        c.S3ContentsManager.bucket = "{{ S3 bucket name }}"
-        
-        # Optional settings:
-        c.S3ContentsManager.prefix = "this/is/a/prefix/on/the/s3/bucket"
-        c.S3ContentsManager.sse = "AES256"
-        c.S3ContentsManager.signature_version = "s3v4"
-        c.S3ContentsManager.init_s3_hook = init_function  # See AWS key refresh
-        ```
-        
-        Example for `play.minio.io:9000`:
-        
-        ```python
-        from s3contents import S3ContentsManager
-        
-        c = get_config()
-        
-        # Tell Jupyter to use S3ContentsManager for all storage.
-        c.NotebookApp.contents_manager_class = S3ContentsManager
-        c.S3ContentsManager.access_key_id = "Q3AM3UQ867SPQQA43P2F"
-        c.S3ContentsManager.secret_access_key = "zuf+tfteSlswRu7BJ86wekitnifILbZam1KYY3TG"
-        c.S3ContentsManager.endpoint_url = "http://play.minio.io:9000"
-        c.S3ContentsManager.bucket = "s3contents-demo"
-        c.S3ContentsManager.prefix = "notebooks/test"
-        ```
-        
-        ### AWS EC2 role auth setup
-        
-        It also possible to use IAM Role-based access to the S3 bucket from an Amazon EC2 instance.
-        
-        To do that just leave `access_key_id` and `secret_access_key` set to their default values (`None`),
-        and ensure that the EC2 instance has an IAM role which provides sufficient permissions for the bucket and the operations necessary.
-        
-        ### AWS key refresh
-        
-        The optional `init_s3_hook` configuration can be used to enable AWS key rotation (described [here](https://dev.to/li_chastina/auto-refresh-aws-tokens-using-iam-role-and-boto3-2cjf) and [here](https://www.owenrumney.co.uk/2019/01/15/implementing-refreshingawscredentials-python/)) as follows:
-        
-        ```python
-        from s3contents import S3ContentsManager
-        from botocore.credentials import RefreshableCredentials
-        from botocore.session import get_session
-        import botocore
-        import boto3
-        from configparser import ConfigParser
-        
-        def refresh_external_credentials():
-            config = ConfigParser()
-            config.read('/home/jovyan/.aws/credentials')
-            return {
-                "access_key": config['default']['aws_access_key_id'],
-                "secret_key": config['default']['aws_secret_access_key'],
-                "token": config['default']['aws_session_token'],
-                "expiry_time": config['default']['aws_expiration']
-            }
-        
-        session_credentials = RefreshableCredentials.create_from_metadata(
-                metadata = refresh_external_credentials(),
-                refresh_using = refresh_external_credentials,
-                method = 'custom-refreshing-key-file-reader'
-        )
-        
-        def make_key_refresh_boto3(this_s3contents_instance):
-            refresh_session =  get_session() # from botocore.session
-            refresh_session._credentials = session_credentials
-            my_s3_session =  boto3.Session(botocore_session=refresh_session)
-            this_s3contents_instance.boto3_session = my_s3_session
-        
-        # Tell Jupyter to use S3ContentsManager for all storage.
-        c.NotebookApp.contents_manager_class = S3ContentsManager
-        
-        c.S3ContentsManager.init_s3_hook = make_key_refresh_boto3
-        ```
-        
-        ## GCP Cloud Storage
-        
-        ```python
-        from s3contents import GCSContentsManager
-        
-        c = get_config(
-        
-        c.NotebookApp.contents_manager_class = GCSContentsManager
-        c.GCSContentsManager.project = "{{ your-project }}"
-        c.GCSContentsManager.token = "~/.config/gcloud/application_default_credentials.json"
-        c.GCSContentsManager.bucket = "{{ GCP bucket name }}"
-        ```
-        
-        Note that the file `~/.config/gcloud/application_default_credentials.json` assumes a posix system
-        when you did `gcloud init`
-        
-        ## Access local files
-        
-        To access local file as well as remote files in S3 you can use [hybridcontents](https://github.com/viaduct-ai/hybridcontents).
-        
-        First install it:
-        
-        ```
-        pip install hybridcontents
-        ```
-        
-        Use a configuration similar to this:
-        
-        ```python
-        from s3contents import S3ContentsManager
-        from hybridcontents import HybridContentsManager
-        from notebook.services.contents.largefilemanager import LargeFileManager
-        
-        c = get_config()
-        
-        c.NotebookApp.contents_manager_class = HybridContentsManager
-        
-        c.HybridContentsManager.manager_classes = {
-            # Associate the root directory with an S3ContentsManager.
-            # This manager will receive all requests that don"t fall under any of the
-            # other managers.
-            "": S3ContentsManager,
-            # Associate /directory with a LargeFileManager.
-            "local_directory": LargeFileManager,
-        }
-        
-        c.HybridContentsManager.manager_kwargs = {
-            # Args for root S3ContentsManager.
-            "": {
-                "access_key_id": "{{ AWS Access Key ID / IAM Access Key ID }}",
-                "secret_access_key": "{{ AWS Secret Access Key / IAM Secret Access Key }}",
-                "bucket": "{{ S3 bucket name }}",
-            },
-            # Args for the LargeFileManager mapped to /directory
-            "local_directory": {
-                "root_dir": "/Users/danielfrg/Downloads",
-            },
-        }
-        ```
-        
-        ## File Save Hooks
-        
-        If you want to use pre/post file save hooks here are some examples.
-        
-        A `pre_save_hook` is written in the exact same way as normal, operating on the file in local storage before commiting it to the object store.
-        
-        ```python
-        def scrub_output_pre_save(model, **kwargs):
-            """scrub output before saving notebooks"""
-            # only run on notebooks
-            if model["type"] != "notebook":
-                return
-            # only run on nbformat v4
-            if model["content"]["nbformat"] != 4:
-                return
-        
-            for cell in model["content"]["cells"]:
-                if cell["cell_type"] != "code":
-                    continue
-                cell["outputs"] = []
-                cell["execution_count"] = None
-        
-        c.S3ContentsManager.pre_save_hook = scrub_output_pre_save
-        ```
-        
-        A `post_save_hook` instead operates on the file in object storage, because of this it is useful to use the file methods on the `contents_manager` for data manipulation. In addition, one must use the following function signature (unique to `s3contents`):
-        
-        ```python
-        def make_html_post_save(model, s3_path, contents_manager, **kwargs):
-            """
-            convert notebooks to HTML after saving via nbconvert
-            """
-            from nbconvert import HTMLExporter
-        
-            if model["type"] != "notebook":
-                return
-        
-            content, _format = contents_manager.fs.read(s3_path, format="text")
-            my_notebook = nbformat.reads(content, as_version=4)
-        
-            html_exporter = HTMLExporter()
-            html_exporter.template_name = "classic"
-        
-            (body, resources) = html_exporter.from_notebook_node(my_notebook)
-        
-            base, ext = os.path.splitext(s3_path)
-            contents_manager.fs.write(path=(base + ".html"), content=body, format=_format)
-        
-        c.S3ContentsManager.post_save_hook = make_html_post_save
-        ```
-        
-        ## Notes
-        
-        While there are some implementations of this already:
-        ([s3nb](https://github.com/monetate/s3nb) or [s3drive](https://github.com/stitchfix/s3drive)),
-        I wasn't able to make them work in newer versions of Jupyter Notebook.
-        This aims to be a more tested version and it's based on [PGContents](https://github.com/quantopian/pgcontents).
-        
-Keywords: jupyter,s3,contents-manager,gcs,aws,gcp
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
+<p align="center">
+    <img src="https://raw.githubusercontent.com/danielfrg/s3contents/main/docs/logo.png" width="450px">
+</p>
+
+<p align="center">
+    <a href="https://pypi.org/project/s3contents/">
+        <img src="https://badge.fury.io/py/s3contents.svg">
+    </a>
+    <a href="https://github.com/danielfrg/s3contents/actions/workflows/test.yml">
+        <img src="https://github.com/danielfrg/s3contents/workflows/test/badge.svg">
+    </a>
+    <a href="https://codecov.io/gh/danielfrg/s3contents?branch=main">
+        <img src="https://codecov.io/gh/danielfrg/s3contents/branch/main/graph/badge.svg">
+    </a>
+    <a href="http://github.com/danielfrg/s3contents/blob/main/LICENSE.txt">
+        <img src="https://img.shields.io/:license-Apache%202-blue.svg">
+    </a>
+</p>
+
+# S3Contents - Jupyter Notebooks in S3
+
+A transparent, drop-in replacement for Jupyter standard filesystem-backed storage system.
+With this implementation of a
+[Jupyter Contents Manager](https://jupyter-server.readthedocs.io/en/latest/developers/contents.html)
+you can save all your notebooks, files and directory structure directly to a
+S3/GCS bucket on AWS/GCP or a self hosted S3 API compatible like [MinIO](http://minio.io).
+
+## Installation
+
+```shell
+pip install s3contents
+```
+
+Install with GCS dependencies:
+
+```shell
+pip install s3contents[gcs]
+```
+
+## s3contents vs X
+
+While there are some implementations of an S3 Jupyter Content Manager such as
+[s3nb](https://github.com/monetate/s3nb) or [s3drive](https://github.com/stitchfix/s3drive)
+s3contents is the only one tested against new versions of Jupyter.
+It also supports more authentication methods and Google Cloud Storage.
+
+This aims to be a fully tested implementation and it's based on [PGContents](https://github.com/quantopian/pgcontents).
+
+## Configuration
+
+Create a `jupyter_notebook_config.py` file in one of the
+[Jupyter config directories](https://jupyter.readthedocs.io/en/latest/use/jupyter-directories.html#id1)
+for example: `~/.jupyter/jupyter_notebook_config.py`.
+
+**Jupyter Notebook Classic**: If you plan to use the Classic Jupyter Notebook
+interface you need to change `ServerApp` to `NotebookApp` for all the examples on this page.
+
+## AWS S3
+
+```python
+from s3contents import S3ContentsManager
+
+c = get_config()
+
+# Tell Jupyter to use S3ContentsManager
+c.ServerApp.contents_manager_class = S3ContentsManager
+c.S3ContentsManager.bucket = "<S3 bucket name>"
+
+# Fix JupyterLab dialog issues
+c.ServerApp.root_dir = ""
+```
+
+### Authentication
+
+Additionally you can configure multiple authentication methods:
+
+Access and secret keys:
+
+```python
+c.S3ContentsManager.access_key_id = "<AWS Access Key ID / IAM Access Key ID>"
+c.S3ContentsManager.secret_access_key = "<AWS Secret Access Key / IAM Secret Access Key>"
+```
+
+Session token:
+
+```python
+c.S3ContentsManager.session_token = "<AWS Session Token / IAM Session Token>"
+```
+
+### AWS EC2 role auth setup
+
+It also possible to use IAM Role-based access to the S3 bucket from an Amazon EC2 instance or AWS resource.
+
+To do that just leave any authentication options (`access_key_id`, `secret_access_key`) to their default of `None`
+and ensure that the EC2 instance has an IAM role which provides sufficient permissions (read and write) for the bucket.
+
+### Optional settings
+
+```python
+# A prefix in the S3 buckets to use as the root of the Jupyter file system
+c.S3ContentsManager.prefix = "this/is/a/prefix/on/the/s3/bucket"
+
+# Server-Side Encryption
+c.S3ContentsManager.sse = "AES256"
+
+# Authentication signature version
+c.S3ContentsManager.signature_version = "s3v4"
+
+# See AWS key refresh
+c.S3ContentsManager.init_s3_hook = init_function
+```
+
+### AWS key refresh
+
+The optional `init_s3_hook` configuration can be used to enable AWS key rotation (described [here](https://dev.to/li_chastina/auto-refresh-aws-tokens-using-iam-role-and-boto3-2cjf) and [here](https://www.owenrumney.co.uk/2019/01/15/implementing-refreshingawscredentials-python/)) as follows:
+
+```python
+import boto3
+import botocore
+from botocore.credentials import RefreshableCredentials
+from botocore.session import get_session
+from configparser import ConfigParser
+
+from s3contents import S3ContentsManager
+
+def refresh_external_credentials():
+    config = ConfigParser()
+    config.read('/home/jovyan/.aws/credentials')
+    return {
+        "access_key": config['default']['aws_access_key_id'],
+        "secret_key": config['default']['aws_secret_access_key'],
+        "token": config['default']['aws_session_token'],
+        "expiry_time": config['default']['aws_expiration']
+    }
+
+session_credentials = RefreshableCredentials.create_from_metadata(
+        metadata = refresh_external_credentials(),
+        refresh_using = refresh_external_credentials,
+        method = 'custom-refreshing-key-file-reader'
+)
+
+def make_key_refresh_boto3(this_s3contents_instance):
+    refresh_session =  get_session() # from botocore.session
+    refresh_session._credentials = session_credentials
+    my_s3_session =  boto3.Session(botocore_session=refresh_session)
+    this_s3contents_instance.boto3_session = my_s3_session
+
+# Tell Jupyter to use S3ContentsManager
+c.ServerApp.contents_manager_class = S3ContentsManager
+
+c.S3ContentsManager.init_s3_hook = make_key_refresh_boto3
+```
+
+### MinIO playground example
+
+You can test this using the [`play.minio.io:9000`](https://play.minio.io:9000) playground:
+
+Just be sure to create the bucket first.
+
+```python
+from s3contents import S3ContentsManager
+
+c = get_config()
+
+# Tell Jupyter to use S3ContentsManager
+c.ServerApp.contents_manager_class = S3ContentsManager
+c.S3ContentsManager.access_key_id = "Q3AM3UQ867SPQQA43P2F"
+c.S3ContentsManager.secret_access_key = "zuf+tfteSlswRu7BJ86wekitnifILbZam1KYY3TG"
+c.S3ContentsManager.endpoint_url = "https://play.minio.io:9000"
+c.S3ContentsManager.bucket = "s3contents-demo"
+c.S3ContentsManager.prefix = "notebooks/test"
+```
+
+## Access local files
+
+To access local file as well as remote files in S3 you can use [hybridcontents](https://github.com/viaduct-ai/hybridcontents).
+
+Install it:
+
+```shell
+pip install hybridcontents
+```
+
+Use a configuration similar to this:
+
+```python
+from s3contents import S3ContentsManager
+from hybridcontents import HybridContentsManager
+from notebook.services.contents.largefilemanager import LargeFileManager
+
+c = get_config()
+
+c.ServerApp.contents_manager_class = HybridContentsManager
+
+c.HybridContentsManager.manager_classes = {
+    # Associate the root directory with an S3ContentsManager.
+    # This manager will receive all requests that don"t fall under any of the
+    # other managers.
+    "": S3ContentsManager,
+    # Associate /local_directory with a LargeFileManager.
+    "local_directory": LargeFileManager,
+}
+
+c.HybridContentsManager.manager_kwargs = {
+    # Args for root S3ContentsManager.
+    "": {
+        "access_key_id": "<AWS Access Key ID / IAM Access Key ID>",
+        "secret_access_key": "<AWS Secret Access Key / IAM Secret Access Key>",
+        "bucket": "<S3 bucket name>",
+    },
+    # Args for the LargeFileManager mapped to /local_directory
+    "local_directory": {
+        "root_dir": "/Users/danielfrg/Downloads",
+    },
+}
+```
+
+## GCP - Google Cloud Storage
+
+Install the extra dependencies with:
+
+```shell
+pip install s3contents[gcs]
+```
+
+```python
+from s3contents.gcs import GCSContentsManager
+
+c = get_config(
+
+c.ServerApp.contents_manager_class = GCSContentsManager
+c.GCSContentsManager.project = "<your-project>"
+c.GCSContentsManager.token = "~/.config/gcloud/application_default_credentials.json"
+c.GCSContentsManager.bucket = "<GCP bucket name>"
+```
+
+Note that the file `~/.config/gcloud/application_default_credentials.json` assumes
+a POSIX system when you did `gcloud init`.
+
+## Other configuration
+
+### File Save Hooks
+
+If you want to use pre/post file save hooks here are some examples.
+
+A `pre_save_hook` is written in the exact same way as normal, operating on the
+file in local storage before committing it to the object store.
+
+```python
+def scrub_output_pre_save(model, **kwargs):
+    """
+    Scrub output before saving notebooks
+    """
+
+    # only run on notebooks
+    if model["type"] != "notebook":
+        return
+
+    # only run on nbformat v4
+    if model["content"]["nbformat"] != 4:
+        return
+
+    for cell in model["content"]["cells"]:
+        if cell["cell_type"] != "code":
+            continue
+        cell["outputs"] = []
+        cell["execution_count"] = None
+
+c.S3ContentsManager.pre_save_hook = scrub_output_pre_save
+```
+
+A `post_save_hook` instead operates on the file in object storage,
+because of this it is useful to use the file methods on the `contents_manager`
+for data manipulation.
+In addition, one must use the following function signature (unique to `s3contents`):
+
+```python
+def make_html_post_save(model, s3_path, contents_manager, **kwargs):
+    """
+    Convert notebooks to HTML after saving via nbconvert
+    """
+    from nbconvert import HTMLExporter
+
+    if model["type"] != "notebook":
+        return
+
+    content, _format = contents_manager.fs.read(s3_path, format="text")
+    my_notebook = nbformat.reads(content, as_version=4)
+
+    html_exporter = HTMLExporter()
+    html_exporter.template_name = "classic"
+
+    (body, resources) = html_exporter.from_notebook_node(my_notebook)
+
+    base, ext = os.path.splitext(s3_path)
+    contents_manager.fs.write(path=(base + ".html"), content=body, format=_format)
+
+c.S3ContentsManager.post_save_hook = make_html_post_save
+```
```

### Comparing `s3contents-0.7.0/README.md` & `s3contents-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,161 @@
-# S3Contents
+Metadata-Version: 2.1
+Name: s3contents
+Version: 0.9.0
+Summary: S3 Contents Manager for Jupyter
+Home-page: https://github.com/danielfrg/s3contents
+License: Apache License, Version 2.0
+Author: Daniel Rodriguez
+Maintainer: Daniel Rodriguez
+Requires-Python: >=3.7.1,<4
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Provides-Extra: gcs
+Requires-Dist: aiobotocore[boto3] (>=1.4.0,<2.0.0)
+Requires-Dist: gcsfs (>=2021.11.0,<2022.0.0); extra == "gcs"
+Requires-Dist: notebook (>=5.6,<7.0)
+Requires-Dist: s3fs (>=2021.11.0)
+Project-URL: Documentation, https://github.com/danielfrg/s3contents
+Project-URL: Repository, https://github.com/danielfrg/s3contents
+Description-Content-Type: text/markdown
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/danielfrg/s3contents/main/docs/logo.png" width="450px">
+</p>
+
+<p align="center">
+    <a href="https://pypi.org/project/s3contents/">
+        <img src="https://badge.fury.io/py/s3contents.svg">
+    </a>
+    <a href="https://github.com/danielfrg/s3contents/actions/workflows/test.yml">
+        <img src="https://github.com/danielfrg/s3contents/workflows/test/badge.svg">
+    </a>
+    <a href="https://codecov.io/gh/danielfrg/s3contents?branch=main">
+        <img src="https://codecov.io/gh/danielfrg/s3contents/branch/main/graph/badge.svg">
+    </a>
+    <a href="http://github.com/danielfrg/s3contents/blob/main/LICENSE.txt">
+        <img src="https://img.shields.io/:license-Apache%202-blue.svg">
+    </a>
+</p>
+
+# S3Contents - Jupyter Notebooks in S3
+
+A transparent, drop-in replacement for Jupyter standard filesystem-backed storage system.
+With this implementation of a
+[Jupyter Contents Manager](https://jupyter-server.readthedocs.io/en/latest/developers/contents.html)
+you can save all your notebooks, files and directory structure directly to a
+S3/GCS bucket on AWS/GCP or a self hosted S3 API compatible like [MinIO](http://minio.io).
 
-[![pypi](https://badge.fury.io/py/s3contents.svg)](https://pypi.org/project/s3contents/)
-[![build](https://github.com/danielfrg/s3contents/workflows/test/badge.svg)](https://github.com/danielfrg/s3contents/actions/workflows/test.yml)
-[![coverage](https://codecov.io/gh/danielfrg/s3contents/branch/master/graph/badge.svg)](https://codecov.io/gh/danielfrg/s3contents?branch=master)
-[![licence](https://img.shields.io/:license-Apache%202-blue.svg)](http://github.com/danielfrg/s3contents/blob/master/LICENSE.txt)
+## Installation
 
-An S3 and GCS backed ContentsManager implementation for Jupyter.
+```shell
+pip install s3contents
+```
 
-It aims to a be a transparent, drop-in replacement for Jupyter standard filesystem-backed storage system.
-With this implementation of a Jupyter Contents Manager you can save all your notebooks, regular files, directories
-structure directly to a S3/GCS bucket, this could be on AWS/GCP or a self hosted S3 API compatible like [minio](http://minio.io).
+Install with GCS dependencies:
 
-## Prerequisites
+```shell
+pip install s3contents[gcs]
+```
 
-Write access (valid credentials) to an S3/GCS bucket, this could be on AWS/GCP or a self hosted S3 like [minio](http://minio.io).
+## s3contents vs X
 
-## Installation
+While there are some implementations of an S3 Jupyter Content Manager such as
+[s3nb](https://github.com/monetate/s3nb) or [s3drive](https://github.com/stitchfix/s3drive)
+s3contents is the only one tested against new versions of Jupyter.
+It also supports more authentication methods and Google Cloud Storage.
 
-```
-pip install s3contents
-```
+This aims to be a fully tested implementation and it's based on [PGContents](https://github.com/quantopian/pgcontents).
+
+## Configuration
 
-## Jupyter config
+Create a `jupyter_notebook_config.py` file in one of the
+[Jupyter config directories](https://jupyter.readthedocs.io/en/latest/use/jupyter-directories.html#id1)
+for example: `~/.jupyter/jupyter_notebook_config.py`.
 
-Edit `~/.jupyter/jupyter_notebook_config.py` based on the backend you want to
-based on the examples below. Replace credentials as needed.
+**Jupyter Notebook Classic**: If you plan to use the Classic Jupyter Notebook
+interface you need to change `ServerApp` to `NotebookApp` for all the examples on this page.
 
 ## AWS S3
 
 ```python
 from s3contents import S3ContentsManager
 
 c = get_config()
 
-# Tell Jupyter to use S3ContentsManager for all storage.
-c.NotebookApp.contents_manager_class = S3ContentsManager
-c.S3ContentsManager.access_key_id = "{{ AWS Access Key ID / IAM Access Key ID }}"
-c.S3ContentsManager.secret_access_key = "{{ AWS Secret Access Key / IAM Secret Access Key }}"
-c.S3ContentsManager.session_token = "{{ AWS Session Token / IAM Session Token }}"
-c.S3ContentsManager.bucket = "{{ S3 bucket name }}"
+# Tell Jupyter to use S3ContentsManager
+c.ServerApp.contents_manager_class = S3ContentsManager
+c.S3ContentsManager.bucket = "<S3 bucket name>"
 
-# Optional settings:
-c.S3ContentsManager.prefix = "this/is/a/prefix/on/the/s3/bucket"
-c.S3ContentsManager.sse = "AES256"
-c.S3ContentsManager.signature_version = "s3v4"
-c.S3ContentsManager.init_s3_hook = init_function  # See AWS key refresh
+# Fix JupyterLab dialog issues
+c.ServerApp.root_dir = ""
 ```
 
-Example for `play.minio.io:9000`:
+### Authentication
+
+Additionally you can configure multiple authentication methods:
+
+Access and secret keys:
 
 ```python
-from s3contents import S3ContentsManager
+c.S3ContentsManager.access_key_id = "<AWS Access Key ID / IAM Access Key ID>"
+c.S3ContentsManager.secret_access_key = "<AWS Secret Access Key / IAM Secret Access Key>"
+```
 
-c = get_config()
+Session token:
 
-# Tell Jupyter to use S3ContentsManager for all storage.
-c.NotebookApp.contents_manager_class = S3ContentsManager
-c.S3ContentsManager.access_key_id = "Q3AM3UQ867SPQQA43P2F"
-c.S3ContentsManager.secret_access_key = "zuf+tfteSlswRu7BJ86wekitnifILbZam1KYY3TG"
-c.S3ContentsManager.endpoint_url = "http://play.minio.io:9000"
-c.S3ContentsManager.bucket = "s3contents-demo"
-c.S3ContentsManager.prefix = "notebooks/test"
+```python
+c.S3ContentsManager.session_token = "<AWS Session Token / IAM Session Token>"
 ```
 
 ### AWS EC2 role auth setup
 
-It also possible to use IAM Role-based access to the S3 bucket from an Amazon EC2 instance.
+It also possible to use IAM Role-based access to the S3 bucket from an Amazon EC2 instance or AWS resource.
+
+To do that just leave any authentication options (`access_key_id`, `secret_access_key`) to their default of `None`
+and ensure that the EC2 instance has an IAM role which provides sufficient permissions (read and write) for the bucket.
 
-To do that just leave `access_key_id` and `secret_access_key` set to their default values (`None`),
-and ensure that the EC2 instance has an IAM role which provides sufficient permissions for the bucket and the operations necessary.
+### Optional settings
+
+```python
+# A prefix in the S3 buckets to use as the root of the Jupyter file system
+c.S3ContentsManager.prefix = "this/is/a/prefix/on/the/s3/bucket"
+
+# Server-Side Encryption
+c.S3ContentsManager.sse = "AES256"
+
+# Authentication signature version
+c.S3ContentsManager.signature_version = "s3v4"
+
+# See AWS key refresh
+c.S3ContentsManager.init_s3_hook = init_function
+```
 
 ### AWS key refresh
 
 The optional `init_s3_hook` configuration can be used to enable AWS key rotation (described [here](https://dev.to/li_chastina/auto-refresh-aws-tokens-using-iam-role-and-boto3-2cjf) and [here](https://www.owenrumney.co.uk/2019/01/15/implementing-refreshingawscredentials-python/)) as follows:
 
 ```python
-from s3contents import S3ContentsManager
+import boto3
+import botocore
 from botocore.credentials import RefreshableCredentials
 from botocore.session import get_session
-import botocore
-import boto3
 from configparser import ConfigParser
 
+from s3contents import S3ContentsManager
+
 def refresh_external_credentials():
     config = ConfigParser()
     config.read('/home/jovyan/.aws/credentials')
     return {
         "access_key": config['default']['aws_access_key_id'],
         "secret_key": config['default']['aws_secret_access_key'],
         "token": config['default']['aws_session_token'],
@@ -100,111 +170,147 @@
 
 def make_key_refresh_boto3(this_s3contents_instance):
     refresh_session =  get_session() # from botocore.session
     refresh_session._credentials = session_credentials
     my_s3_session =  boto3.Session(botocore_session=refresh_session)
     this_s3contents_instance.boto3_session = my_s3_session
 
-# Tell Jupyter to use S3ContentsManager for all storage.
-c.NotebookApp.contents_manager_class = S3ContentsManager
+# Tell Jupyter to use S3ContentsManager
+c.ServerApp.contents_manager_class = S3ContentsManager
 
 c.S3ContentsManager.init_s3_hook = make_key_refresh_boto3
 ```
 
-## GCP Cloud Storage
+### MinIO playground example
+
+You can test this using the [`play.minio.io:9000`](https://play.minio.io:9000) playground:
+
+Just be sure to create the bucket first.
 
 ```python
-from s3contents import GCSContentsManager
+from s3contents import S3ContentsManager
 
-c = get_config(
+c = get_config()
 
-c.NotebookApp.contents_manager_class = GCSContentsManager
-c.GCSContentsManager.project = "{{ your-project }}"
-c.GCSContentsManager.token = "~/.config/gcloud/application_default_credentials.json"
-c.GCSContentsManager.bucket = "{{ GCP bucket name }}"
+# Tell Jupyter to use S3ContentsManager
+c.ServerApp.contents_manager_class = S3ContentsManager
+c.S3ContentsManager.access_key_id = "Q3AM3UQ867SPQQA43P2F"
+c.S3ContentsManager.secret_access_key = "zuf+tfteSlswRu7BJ86wekitnifILbZam1KYY3TG"
+c.S3ContentsManager.endpoint_url = "https://play.minio.io:9000"
+c.S3ContentsManager.bucket = "s3contents-demo"
+c.S3ContentsManager.prefix = "notebooks/test"
 ```
 
-Note that the file `~/.config/gcloud/application_default_credentials.json` assumes a posix system
-when you did `gcloud init`
-
 ## Access local files
 
 To access local file as well as remote files in S3 you can use [hybridcontents](https://github.com/viaduct-ai/hybridcontents).
 
-First install it:
+Install it:
 
-```
+```shell
 pip install hybridcontents
 ```
 
 Use a configuration similar to this:
 
 ```python
 from s3contents import S3ContentsManager
 from hybridcontents import HybridContentsManager
 from notebook.services.contents.largefilemanager import LargeFileManager
 
 c = get_config()
 
-c.NotebookApp.contents_manager_class = HybridContentsManager
+c.ServerApp.contents_manager_class = HybridContentsManager
 
 c.HybridContentsManager.manager_classes = {
     # Associate the root directory with an S3ContentsManager.
     # This manager will receive all requests that don"t fall under any of the
     # other managers.
     "": S3ContentsManager,
-    # Associate /directory with a LargeFileManager.
+    # Associate /local_directory with a LargeFileManager.
     "local_directory": LargeFileManager,
 }
 
 c.HybridContentsManager.manager_kwargs = {
     # Args for root S3ContentsManager.
     "": {
-        "access_key_id": "{{ AWS Access Key ID / IAM Access Key ID }}",
-        "secret_access_key": "{{ AWS Secret Access Key / IAM Secret Access Key }}",
-        "bucket": "{{ S3 bucket name }}",
+        "access_key_id": "<AWS Access Key ID / IAM Access Key ID>",
+        "secret_access_key": "<AWS Secret Access Key / IAM Secret Access Key>",
+        "bucket": "<S3 bucket name>",
     },
-    # Args for the LargeFileManager mapped to /directory
+    # Args for the LargeFileManager mapped to /local_directory
     "local_directory": {
         "root_dir": "/Users/danielfrg/Downloads",
     },
 }
 ```
 
-## File Save Hooks
+## GCP - Google Cloud Storage
+
+Install the extra dependencies with:
+
+```shell
+pip install s3contents[gcs]
+```
+
+```python
+from s3contents.gcs import GCSContentsManager
+
+c = get_config(
+
+c.ServerApp.contents_manager_class = GCSContentsManager
+c.GCSContentsManager.project = "<your-project>"
+c.GCSContentsManager.token = "~/.config/gcloud/application_default_credentials.json"
+c.GCSContentsManager.bucket = "<GCP bucket name>"
+```
+
+Note that the file `~/.config/gcloud/application_default_credentials.json` assumes
+a POSIX system when you did `gcloud init`.
+
+## Other configuration
+
+### File Save Hooks
 
 If you want to use pre/post file save hooks here are some examples.
 
-A `pre_save_hook` is written in the exact same way as normal, operating on the file in local storage before commiting it to the object store.
+A `pre_save_hook` is written in the exact same way as normal, operating on the
+file in local storage before committing it to the object store.
 
 ```python
 def scrub_output_pre_save(model, **kwargs):
-    """scrub output before saving notebooks"""
+    """
+    Scrub output before saving notebooks
+    """
+
     # only run on notebooks
     if model["type"] != "notebook":
         return
+
     # only run on nbformat v4
     if model["content"]["nbformat"] != 4:
         return
 
     for cell in model["content"]["cells"]:
         if cell["cell_type"] != "code":
             continue
         cell["outputs"] = []
         cell["execution_count"] = None
 
 c.S3ContentsManager.pre_save_hook = scrub_output_pre_save
 ```
 
-A `post_save_hook` instead operates on the file in object storage, because of this it is useful to use the file methods on the `contents_manager` for data manipulation. In addition, one must use the following function signature (unique to `s3contents`):
+A `post_save_hook` instead operates on the file in object storage,
+because of this it is useful to use the file methods on the `contents_manager`
+for data manipulation.
+In addition, one must use the following function signature (unique to `s3contents`):
 
 ```python
 def make_html_post_save(model, s3_path, contents_manager, **kwargs):
     """
-    convert notebooks to HTML after saving via nbconvert
+    Convert notebooks to HTML after saving via nbconvert
     """
     from nbconvert import HTMLExporter
 
     if model["type"] != "notebook":
         return
 
     content, _format = contents_manager.fs.read(s3_path, format="text")
@@ -217,13 +323,7 @@
 
     base, ext = os.path.splitext(s3_path)
     contents_manager.fs.write(path=(base + ".html"), content=body, format=_format)
 
 c.S3ContentsManager.post_save_hook = make_html_post_save
 ```
 
-## Notes
-
-While there are some implementations of this already:
-([s3nb](https://github.com/monetate/s3nb) or [s3drive](https://github.com/stitchfix/s3drive)),
-I wasn't able to make them work in newer versions of Jupyter Notebook.
-This aims to be a more tested version and it's based on [PGContents](https://github.com/quantopian/pgcontents).
```

### Comparing `s3contents-0.7.0/s3contents/chunks.py` & `s3contents-0.9.0/s3contents/chunks.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 See https://jupyter-notebook.readthedocs.io/en/stable/extending/contents.html#chunked-saving
 """
 
 import base64
 import contextvars
 import time
 
-
 # Used as a "registry" for uploads.
-content_chunks = contextvars.ContextVar("jupyterlab_content_chunks", default={})
+content_chunks = contextvars.ContextVar(
+    "jupyterlab_content_chunks", default={}
+)
 
 
 def store_content_chunk(path: str, content: str):
     """Store a base64 chunk in the registry as bytes"""
 
     current_value = content_chunks.get()
 
@@ -29,15 +30,17 @@
     """Assemble the chunk bytes into a single base64 string"""
 
     current_value = content_chunks.get()
 
     if path not in current_value:
         raise ValueError(f"No chunk for path {path}")
 
-    return base64.b64encode(b"".join(current_value[path]["chunks"])).decode("ascii")
+    return base64.b64encode(b"".join(current_value[path]["chunks"])).decode(
+        "ascii"
+    )
 
 
 def delete_chunks(path):
     """Should be called once the upload is complete to free the memory"""
 
     current_value = content_chunks.get()
     del current_value[path]
```

### Comparing `s3contents-0.7.0/s3contents/gcs_fs.py` & `s3contents-0.9.0/s3contents/gcs/gcs_fs.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 from s3contents.genericfs import GenericFS, NoSuchFile
 from s3contents.ipycompat import Unicode
 
 
 class GCSFS(GenericFS):
 
-    project = Unicode(help="GCP Project", allow_none=True, default_value=None).tag(
-        config=True, env="JPYNB_GCS_PROJECT"
-    )
+    project = Unicode(
+        help="GCP Project", allow_none=True, default_value=None
+    ).tag(config=True, env="JPYNB_GCS_PROJECT")
     token = Unicode(
         help="Path to the GCP token", allow_none=True, default_value=None
     ).tag(config=True, env="JPYNB_GCS_TOKEN_PATH")
 
     region_name = Unicode("us-east-1", help="Region name").tag(
         config=True, env="JPYNB_GCS_REGION_NAME"
     )
@@ -43,23 +43,23 @@
         self.fs = gcsfs.GCSFileSystem(project=self.project, token=token)
 
         self.init()
 
     def init(self):
         self.mkdir("")
         self.ls("")
-        assert self.isdir(""), "The root directory should exists :)"
+        assert self.isdir(""), "The root directory should exists"
 
     #  GenericFS methods -----------------------------------------------------------------------------------------------
 
     def ls(self, path):
         path_ = self.path(path)
         self.log.debug("S3contents.GCSFS: Listing directory: `%s`", path_)
         files = self.fs.ls(path_)
-        return self.unprefix(files)
+        return self.remove_prefix(files)
 
     def isfile(self, path):
         path_ = self.path(path)
         is_file = False
 
         exists = self.fs.exists(path_)
         if not exists:
@@ -74,31 +74,39 @@
         return is_file
 
     def isdir(self, path):
         # GCSFS doesnt return exists=True for a directory with no files so
         # we need to check if the dir_keep_file exists
         is_dir = self.isfile(path + self.separator + self.dir_keep_file)
         path_ = self.path(path)
-        self.log.debug("S3contents.GCSFS: `%s` is a directory: %s", path_, is_dir)
+        self.log.debug(
+            "S3contents.GCSFS: `%s` is a directory: %s", path_, is_dir
+        )
         return is_dir
 
     def mv(self, old_path, new_path):
-        self.log.debug("S3contents.GCSFS: Move file `%s` to `%s`", old_path, new_path)
+        self.log.debug(
+            "S3contents.GCSFS: Move file `%s` to `%s`", old_path, new_path
+        )
         self.cp(old_path, new_path)
         self.rm(old_path)
 
     def cp(self, old_path, new_path):
         old_path_, new_path_ = self.path(old_path), self.path(new_path)
-        self.log.debug("S3contents.GCSFS: Coping `%s` to `%s`", old_path_, new_path_)
+        self.log.debug(
+            "S3contents.GCSFS: Coping `%s` to `%s`", old_path_, new_path_
+        )
 
         if self.isdir(old_path):
             old_dir_path, new_dir_path = old_path, new_path
             for obj in self.ls(old_dir_path):
                 old_item_path = obj
-                new_item_path = old_item_path.replace(old_dir_path, new_dir_path, 1)
+                new_item_path = old_item_path.replace(
+                    old_dir_path, new_dir_path, 1
+                )
                 self.cp(old_item_path, new_item_path)
         elif self.isfile(old_path):
             self.fs.copy(old_path_, new_path_)
 
     def rm(self, path):
         path_ = self.path(path)
         self.log.debug("S3contents.GCSFS: Removing: `%s`", path_)
@@ -141,15 +149,15 @@
         info = self.fs.info(path_)
         ret = {}
         if "updated" in info:
             ret["ST_MTIME"] = info["updated"]
         return ret
 
     def write(self, path, content, format):
-        path_ = self.path(self.unprefix(path))
+        path_ = self.path(self.remove_prefix(path))
         self.log.debug("S3contents.GCSFS: Writing file: `%s`", path_)
         with self.fs.open(path_, mode="wb") as f:
             if format == "base64":
                 b64_bytes = content.encode("ascii")
                 content_ = base64.b64decode(b64_bytes)
             else:
                 content_ = content.encode("utf8")
@@ -172,28 +180,32 @@
         prefix = self.bucket
         if self.prefix:
             prefix += self.separator + self.prefix
         return prefix
 
     prefix_ = property(get_prefix)
 
-    def unprefix(self, path):
+    def remove_prefix(self, path):
         """Remove the self.prefix_ (if present) from a path or list of paths"""
         path = self.strip(path)
         if isinstance(path, str):
-            path = path[len(self.prefix_) :] if path.startswith(self.prefix_) else path
+            path = (
+                path[len(self.prefix_) :]
+                if path.startswith(self.prefix_)
+                else path
+            )
             path = path[1:] if path.startswith(self.separator) else path
             return path
         if isinstance(path, (list, tuple)):
             path = [
                 p[len(self.prefix_) :] if p.startswith(self.prefix_) else p
                 for p in path
             ]
             path = [p[1:] if p.startswith(self.separator) else p for p in path]
             return path
 
     def path(self, *path):
         """Utility to join paths including the bucket and prefix"""
         path = list(filter(None, path))
-        path = self.unprefix(path)
+        path = self.remove_prefix(path)
         items = [self.prefix_] + path
         return self.join(*items)
```

### Comparing `s3contents-0.7.0/s3contents/gcsmanager.py` & `s3contents-0.9.0/s3contents/gcs/gcsmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from s3contents.gcs_fs import GCSFS
+from s3contents.gcs.gcs_fs import GCSFS
 from s3contents.genericmanager import GenericContentsManager
 from s3contents.ipycompat import Unicode
 
 
 class GCSContentsManager(GenericContentsManager):
 
-    project = Unicode(help="GCP Project", allow_none=True, default_value=None).tag(
-        config=True, env="JPYNB_GCS_PROJECT"
-    )
+    project = Unicode(
+        help="GCP Project", allow_none=True, default_value=None
+    ).tag(config=True, env="JPYNB_GCS_PROJECT")
     token = Unicode(
         help="Path to the GCP token", allow_none=True, default_value=None
     ).tag(config=True, env="JPYNB_GCS_TOKEN_PATH")
 
     region_name = Unicode("us-east-1", help="Region name").tag(
         config=True, env="JPYNB_GCS_REGION_NAME"
     )
```

### Comparing `s3contents-0.7.0/s3contents/genericfs.py` & `s3contents-0.9.0/s3contents/genericfs.py`

 * *Files identical despite different names*

### Comparing `s3contents-0.7.0/s3contents/genericmanager.py` & `s3contents-0.9.0/s3contents/genericmanager.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     from_dict,
     import_item,
     reads,
     string_types,
     validate,
 )
 
-
 DUMMY_CREATED_DATE = datetime.datetime.fromtimestamp(86400)
 NBFORMAT_VERSION = 4
 
 
 class GenericContentsManager(ContentsManager, HasTraits):
 
     # This makes the checkpoints get saved on this directory
@@ -71,52 +70,70 @@
 
     def no_such_entity(self, path):
         self.do_error("No such entity: [{path}]".format(path=path), 404)
 
     def already_exists(self, path):
         thing = "File" if self.file_exists(path) else "Directory"
         self.do_error(
-            "{thing} already exists: [{path}]".format(thing=thing, path=path), 409
+            "{thing} already exists: [{path}]".format(thing=thing, path=path),
+            409,
         )
 
     def guess_type(self, path, allow_directory=True):
         """
         Guess the type of a file.
         If allow_directory is False, don't consider the possibility that the
         file is a directory.
 
         Parameters
         ----------
             obj: s3.Object or string
         """
+        self.log.debug(
+            f"guess_type with path={path} and allow_directory={allow_directory}"
+        )
         if path.endswith(".ipynb"):
             return "notebook"
         elif allow_directory and self.dir_exists(path):
             return "directory"
         else:
             return "file"
 
     def file_exists(self, path):
         # Does a file exist at the given path?
         self.log.debug("S3contents.GenericManager.file_exists: ('%s')", path)
         return self.fs.isfile(path)
 
     def dir_exists(self, path):
         # Does a directory exist at the given path?
-        self.log.debug("S3contents.GenericManager.dir_exists: path('%s')", path)
+        self.log.debug(
+            "S3contents.GenericManager.dir_exists: path('%s')", path
+        )
         return self.fs.isdir(path)
 
     def get(self, path, content=True, type=None, format=None):
         # Get a file or directory model.
         self.log.debug(
-            "S3contents.GenericManager.get] path('%s') type(%s) format(%s)",
+            "S3contents.GenericManager.get: path('%s') type(%s) format(%s)",
             path,
             type,
             format,
         )
+
+        # This is a hack to remove some startup dialog error from JupyterLab
+        # TODO: Figure out why is this happening
+        if self.parent:
+            if path.startswith(self.parent.root_dir):
+                self.log.debug(
+                    "S3contents.GenericManager.get: removing root_dir (%s) from path",
+                    self.parent.root_dir,
+                )
+                path = path[len(self.parent.root_dir) :]
+        # END hack
+
         path = path.strip("/")
 
         if type is None:
             type = self.guess_type(path)
         try:
             func = {
                 "directory": self._get_directory,
@@ -140,78 +157,120 @@
     def _get_notebook(self, path, content=True, format=None):
         self.log.debug(
             "S3contents.GenericManager._get_notebook: path('%s') type(%s) format(%s)",
             path,
             content,
             format,
         )
-        return self._notebook_model_from_path(path, content=content, format=format)
+        return self._notebook_model_from_path(
+            path, content=content, format=format
+        )
 
     def _get_file(self, path, content=True, format=None):
         self.log.debug(
             "S3contents.GenericManager._get_file: path('%s') type(%s) format(%s)",
             path,
             content,
             format,
         )
         return self._file_model_from_path(path, content=content, format=format)
 
     def _directory_model_from_path(self, path, content=False):
         def s3_detail_to_model(s3_detail):
             model_path = s3_detail["Key"]
-            model = base_model(self.fs.unprefix(model_path))
+            model = base_model(self.fs.remove_prefix(model_path))
             if s3_detail["StorageClass"] == "DIRECTORY":
                 model["created"] = model["last_modified"] = DUMMY_CREATED_DATE
                 model["type"] = "directory"
                 lstat = self.fs.lstat(model_path)
                 if "ST_MTIME" in lstat and lstat["ST_MTIME"]:
-                    model["created"] = model["last_modified"] = lstat["ST_MTIME"]
+                    model["created"] = model["last_modified"] = lstat[
+                        "ST_MTIME"
+                    ]
             else:
                 model["last_modified"] = s3_detail.get("LastModified").replace(
                     microsecond=0, tzinfo=tzutc()
                 )
                 model["created"] = model["last_modified"]
                 # model["size"] = s3_detail.get("Size")
-                model["type"] = "notebook" if model_path.endswith(".ipynb") else "file"
+                model["type"] = (
+                    "notebook" if model_path.endswith(".ipynb") else "file"
+                )
             return model
 
         self.log.debug(
             "S3contents.GenericManager._directory_model_from_path: path('%s') type(%s)",
             path,
             content,
         )
         model = base_directory_model(path)
         if self.fs.isdir(path):
             lstat = self.fs.lstat(path)
+
+            self.log.debug(
+                f"s3_detail_to_model={s3_detail_to_model}"
+                f"dir_s3_detail: path='{path}', lstat={lstat}"
+            )
+
             if "ST_MTIME" in lstat and lstat["ST_MTIME"]:
                 model["created"] = model["last_modified"] = lstat["ST_MTIME"]
         if content:
             if not self.dir_exists(path):
                 self.no_such_entity(path)
             model["format"] = "json"
             prefixed_path = self.fs.path(path)
-            files_s3_detail = sync(self.fs.fs.loop, self.fs.fs._lsdir, prefixed_path)
+            files_s3_detail = sync(
+                self.fs.fs.loop, self.fs.fs._lsdir, prefixed_path
+            )
+            # filter out .s3keep files
             filtered_files_s3_detail = list(
                 filter(
                     lambda detail: os.path.basename(detail["Key"])
                     != self.fs.dir_keep_file,
                     files_s3_detail,
                 )
             )
-            model["content"] = list(map(s3_detail_to_model, filtered_files_s3_detail))
+
+            # filter out delete_markers in versioned buckets
+            def is_delete_marker(detail):
+                lstat = self.fs.lstat(detail["Key"])
+                return bool("ST_MTIME" in lstat and lstat["ST_MTIME"])
+
+            filtered_files_s3_detail = list(
+                filter(
+                    lambda detail: is_delete_marker(detail),
+                    filtered_files_s3_detail,
+                )
+            )
+
+            for file_s3_detail in filtered_files_s3_detail:
+                self.log.debug(
+                    f"\n file_s3_detail: {file_s3_detail}"
+                    f"lstat={self.fs.lstat(file_s3_detail['Key'])}"
+                    f"is_delete_marker = {is_delete_marker(file_s3_detail)}"
+                )
+
+            model["content"] = list(
+                map(s3_detail_to_model, filtered_files_s3_detail)
+            )
         return model
 
     def _notebook_model_from_path(self, path, content=False, format=None):
         """
         Build a notebook model from database record.
         """
+        self.log.debug(
+            f"_notebook_model_from_path with path={path}, content={content}, format={format}"
+        )
         model = base_model(path)
         model["type"] = "notebook"
         if self.fs.isfile(path):
-            model["created"] = model["last_modified"] = self.fs.lstat(path)["ST_MTIME"]
+            model["created"] = model["last_modified"] = self.fs.lstat(path)[
+                "ST_MTIME"
+            ]
         else:
             self.do_error("Not Found", 404)
         if content:
             if not self.fs.isfile(path):
                 self.no_such_entity(path)
             file_content, _ = self.fs.read(path, format)
             nb_content = reads(file_content, as_version=NBFORMAT_VERSION)
@@ -221,18 +280,23 @@
             self.validate_notebook_model(model)
         return model
 
     def _file_model_from_path(self, path, content=False, format=None):
         """
         Build a file model from database record.
         """
+        self.log.debug(
+            f"_file_model_from_path with path={path}, content={content}, format={format}"
+        )
         model = base_model(path)
         model["type"] = "file"
         if self.fs.isfile(path):
-            model["created"] = model["last_modified"] = self.fs.lstat(path)["ST_MTIME"]
+            model["created"] = model["last_modified"] = self.fs.lstat(path)[
+                "ST_MTIME"
+            ]
         else:
             model["created"] = model["last_modified"] = DUMMY_CREATED_DATE
         if content:
             try:
                 # Get updated format from fs.read()
                 content, format_ = self.fs.read(path, format)
             except NoSuchFile as e:
@@ -243,19 +307,23 @@
             model["content"] = content
             model["mimetype"] = mimetypes.guess_type(path)[0] or "text/plain"
         return model
 
     def save(self, model, path):
         """Save a file or directory model to path."""
 
+        self.log.debug(f"save with path={path}, model={model}")
+
         # Chunked uploads
         # See https://jupyter-notebook.readthedocs.io/en/stable/extending/contents.html#chunked-saving
         chunk = model.get("chunk", None)
         if chunk is not None:
-            return self._save_large_file(chunk, model, path, model.get("format"))
+            return self._save_large_file(
+                chunk, model, path, model.get("format")
+            )
 
         self.log.debug("S3contents.GenericManager.save %s: '%s'", model, path)
         if "type" not in model:
             self.do_error("No model type provided", 400)
         if "content" not in model and model["type"] != "directory":
             self.do_error("No file content provided", 400)
 
@@ -268,16 +336,20 @@
             if model["type"] == "notebook":
                 validation_message = self._save_notebook(model, path)
             elif model["type"] == "file":
                 validation_message = self._save_file(model, path)
             else:
                 validation_message = self._save_directory(path)
         except Exception as e:
-            self.log.error("Error while saving file: %s %s", path, e, exc_info=True)
-            self.do_error("Unexpected error while saving file: %s %s" % (path, e), 500)
+            self.log.error(
+                "Error while saving file: %s %s", path, e, exc_info=True
+            )
+            self.do_error(
+                "Unexpected error while saving file: %s %s" % (path, e), 500
+            )
 
         model = self.get(path, type=model["type"], content=False)
 
         self.run_post_save_hook(model=model, s3_path=model["path"])
 
         if validation_message is not None:
             model["message"] = validation_message
@@ -294,21 +366,25 @@
                 400,
             )
         if "content" not in model and model["type"] != "directory":
             self.do_error("No file content provided", 400)
 
         if format not in {"text", "base64"}:
             self.do_error(
-                "Must specify format of file contents as 'text' or 'base64'", 400
+                "Must specify format of file contents as 'text' or 'base64'",
+                400,
             )
 
         prune_stale_chunks()
 
         self.log.debug(
-            "S3contents.GenericManager.save (chunk %s) %s: '%s'", chunk, model, path
+            "S3contents.GenericManager.save (chunk %s) %s: '%s'",
+            chunk,
+            model,
+            path,
         )
 
         try:
             if chunk == 1:
                 self.run_pre_save_hook(model=model, path=path)
             # Store the chunk in our registry
             store_content_chunk(path, model["content"])
@@ -392,19 +468,24 @@
         return value
 
     def run_post_save_hook(self, model, s3_path):
         """Run the post-save hook if defined, and log errors"""
         if self.post_save_hook:
             try:
                 self.log.debug("Running post-save hook on %s", s3_path)
-                self.post_save_hook(s3_path=s3_path, model=model, contents_manager=self)
+                self.post_save_hook(
+                    s3_path=s3_path, model=model, contents_manager=self
+                )
             except Exception as e:
-                self.log.error("Post-save hook failed o-n %s", s3_path, exc_info=True)
+                self.log.error(
+                    "Post-save hook failed o-n %s", s3_path, exc_info=True
+                )
                 raise HTTPError(
-                    500, "Unexpected error while running post hook save: %s" % e
+                    500,
+                    "Unexpected error while running post hook save: %s" % e,
                 ) from e
 
 
 def base_model(path):
     return {
         "name": path.rsplit("/", 1)[-1],
         "path": path,
```

### Comparing `s3contents-0.7.0/s3contents/ipycompat.py` & `s3contents-0.9.0/s3contents/ipycompat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """
 Utilities for managing compat between notebook versions.
 
 Taken from: https://github.com/quantopian/pgcontents/blob/master/pgcontents/utils/ipycompat.py
 """
 
+import notebook
 from ipython_genutils.importstring import import_item
 from ipython_genutils.py3compat import string_types
 from nbformat import from_dict, reads, writes
 from nbformat.v4.nbbase import (
     new_code_cell,
     new_markdown_cell,
     new_notebook,
     new_raw_cell,
 )
-from notebook.utils import to_os_path
 from nbformat.v4.rwbase import strip_transient
-from notebook.services.contents.manager import ContentsManager
-from notebook.services.contents.filemanager import FileContentsManager
+from notebook.services.contents.checkpoints import (
+    Checkpoints,
+    GenericCheckpointsMixin,
+)
 from notebook.services.contents.filecheckpoints import GenericFileCheckpoints
-from notebook.services.contents.checkpoints import Checkpoints, GenericCheckpointsMixin
-
+from notebook.services.contents.filemanager import FileContentsManager
+from notebook.services.contents.manager import ContentsManager
+from notebook.utils import to_os_path
 from traitlets import (
     Any,
     Bool,
     Dict,
     HasTraits,
     Instance,
     Integer,
     TraitError,
     Unicode,
     validate,
 )
 from traitlets.config import Config
 
-import notebook
-
 if notebook.version_info[0] >= 7:  # noqa
     raise ImportError("Jupyter Notebook versions 6 and up are not supported.")
 
 
 __all__ = [
     "Any",
     "Bool",
```

### Comparing `s3contents-0.7.0/s3contents/s3_fs.py` & `s3contents-0.9.0/s3contents/s3_fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Utilities to make S3 look like a regular file system
 """
+
+import base64
+import datetime
 import os
 import re
 import sys
-import base64
-import datetime
 
 import s3fs
-from traitlets import Any
-from tornado.web import HTTPError
 from botocore.exceptions import ClientError
+from tornado.web import HTTPError
+from traitlets import Any
 
 from s3contents.genericfs import GenericFS, NoSuchFile
 from s3contents.ipycompat import Unicode
 
-
 SAMPLE_ACCESS_POLICY = """
 {{
     "Sid": "S3contentsKeepFile",
     "Action": [
         "s3:*"
     ],
     "Effect": "Allow",
@@ -45,16 +45,20 @@
     region_name = Unicode("us-east-1", help="Region name").tag(
         config=True, env="JPYNB_S3_REGION_NAME"
     )
     bucket = Unicode("notebooks", help="Bucket name to store notebooks").tag(
         config=True, env="JPYNB_S3_BUCKET"
     )
     signature_version = Unicode(help="").tag(config=True)
-    sse = Unicode(help="Type of server-side encryption to use").tag(config=True)
-    kms_key_id = Unicode(help="KMS ID to use to encrypt workbooks").tag(config=True)
+    sse = Unicode(help="Type of server-side encryption to use").tag(
+        config=True
+    )
+    kms_key_id = Unicode(help="KMS ID to use to encrypt workbooks").tag(
+        config=True
+    )
 
     prefix = Unicode("", help="Prefix path inside the specified bucket").tag(
         config=True
     )
     delimiter = Unicode("/", help="Path delimiter").tag(config=True)
 
     dir_keep_file = Unicode(
@@ -132,46 +136,54 @@
 
     #  GenericFS methods -----------------------------------------------------------------------------------------------
 
     def ls(self, path=""):
         path_ = self.path(path)
         self.log.debug("S3contents.S3FS.ls: Listing directory: `%s`", path_)
         files = self.fs.ls(path_, refresh=True)
-        return self.unprefix(files)
+        return self.remove_prefix(files)
 
     def isfile(self, path):
         path_ = self.path(path)
         # FileNotFoundError handled by s3fs
         is_file = self.fs.isfile(path_)
 
         self.log.debug("S3contents.S3FS: `%s` is a file: %s", path_, is_file)
         return is_file
 
     def isdir(self, path):
         path_ = self.path(path)
         # FileNotFoundError handled by s3fs
         is_dir = self.fs.isdir(path_)
 
-        self.log.debug("S3contents.S3FS: `%s` is a directory: %s", path_, is_dir)
+        self.log.debug(
+            "S3contents.S3FS: `%s` is a directory: %s", path_, is_dir
+        )
         return is_dir
 
     def mv(self, old_path, new_path):
-        self.log.debug("S3contents.S3FS: Move file `%s` to `%s`", old_path, new_path)
+        self.log.debug(
+            "S3contents.S3FS: Move file `%s` to `%s`", old_path, new_path
+        )
         self.cp(old_path, new_path)
         self.rm(old_path)
 
     def cp(self, old_path, new_path):
         old_path_, new_path_ = self.path(old_path), self.path(new_path)
-        self.log.debug("S3contents.S3FS: Coping `%s` to `%s`", old_path_, new_path_)
+        self.log.debug(
+            "S3contents.S3FS: Copying `%s` to `%s`", old_path_, new_path_
+        )
 
         if self.isdir(old_path):
             old_dir_path, new_dir_path = old_path, new_path
             for obj in self.ls(old_dir_path):
                 old_item_path = obj
-                new_item_path = old_item_path.replace(old_dir_path, new_dir_path, 1)
+                new_item_path = old_item_path.replace(
+                    old_dir_path, new_dir_path, 1
+                )
                 self.cp(old_item_path, new_item_path)
             self.mkdir(new_path)  # Touch with dir_keep_file
         elif self.isfile(old_path):
             self.fs.copy(old_path_, new_path_)
 
     def rm(self, path):
         path_ = self.path(path)
@@ -231,15 +243,15 @@
             st_time.minute,
             st_time.second,
             tzinfo=st_time.tzinfo,
         )
         return {"ST_MTIME": st_time}
 
     def write(self, path, content, format):
-        path_ = self.path(self.unprefix(path))
+        path_ = self.path(self.remove_prefix(path))
         self.log.debug("S3contents.S3FS: Writing file: `%s`", path_)
         if format not in {"text", "base64"}:
             raise HTTPError(
                 400,
                 "Must specify format of file contents as 'text' or 'base64'",
             )
         try:
@@ -250,15 +262,15 @@
                 content_ = base64.b64decode(b64_bytes)
         except Exception as e:
             raise HTTPError(400, "Encoding error saving %s: %s" % (path_, e))
         with self.fs.open(path_, mode="wb") as f:
             f.write(content_)
 
     def writenotebook(self, path, content):
-        path_ = self.path(self.unprefix(path))
+        path_ = self.path(self.remove_prefix(path))
         self.log.debug("S3contents.S3FS: Writing notebook: `%s`", path_)
         with self.fs.open(path_, mode="wb") as f:
             f.write(content.encode("utf-8"))
 
     #  Utilities -------------------------------------------------------------------------------------------------------
 
     def get_prefix(self):
@@ -268,33 +280,41 @@
             prefix = prefix[5:]
         if self.prefix:
             prefix += self.delimiter + self.prefix
         return prefix
 
     prefix_ = property(get_prefix)
 
-    def unprefix(self, path):
-        """Remove the self.prefix_ (if present) from a path or list of paths"""
-        self.log.debug(f"S3FS.unprefix: self.prefix_: {self.prefix_} path: {path}")
+    def remove_prefix(self, path):
+        """
+        Remove the self.prefix_ (if present) from a path or list of paths
+        """
+        self.log.debug(
+            f"S3FS.remove_prefix: self.prefix_: {self.prefix_} path: {path}"
+        )
         if isinstance(path, str):
-            path = path[len(self.prefix_) :] if path.startswith(self.prefix_) else path
+            path = (
+                path[len(self.prefix_) :]
+                if path.startswith(self.prefix_)
+                else path
+            )
             path = path[1:] if path.startswith(self.delimiter) else path
             return path
         if isinstance(path, (list, tuple)):
             path = [
                 p[len(self.prefix_) :] if p.startswith(self.prefix_) else p
                 for p in path
             ]
             path = [p[1:] if p.startswith(self.delimiter) else p for p in path]
             return path
 
     def path(self, *path):
         """Utility to join paths including the bucket and prefix"""
         path = list(filter(None, path))
-        path = self.unprefix(path)
+        path = self.remove_prefix(path)
         items = [self.prefix_] + path
         return self.delimiter.join(items)
 
     @staticmethod
     def must_be_dictionary(dictionary):
         if type(dictionary) is dict:
             pass
```

### Comparing `s3contents-0.7.0/s3contents/s3manager.py` & `s3contents-0.9.0/s3contents/s3manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,116 @@
 import json
 from urllib.parse import urlparse
 
 from traitlets import Any
 
 from s3contents.genericmanager import GenericContentsManager, from_dict
-from s3contents.ipycompat import Unicode
+from s3contents.ipycompat import Bool, Unicode
 from s3contents.s3_fs import S3FS
 
 
 class S3ContentsManager(GenericContentsManager):
 
     access_key_id = Unicode(
         help="S3/AWS access key ID", allow_none=True, default_value=None
-    ).tag(config=True, env="JPYNB_S3_ACCESS_KEY_ID")
-    secret_access_key = Unicode(
-        help="S3/AWS secret access key", allow_none=True, default_value=None
-    ).tag(config=True, env="JPYNB_S3_SECRET_ACCESS_KEY")
+    ).tag(config=True, env="JPY_S3_ACCESS_KEY_ID")
 
-    endpoint_url = Unicode("https://s3.amazonaws.com", help="S3 endpoint URL").tag(
-        config=True, env="JPYNB_S3_ENDPOINT_URL"
+    anon = Bool(help="S3/AWS session token", default_value=False).tag(
+        config=True, env="JPY_S3_ANON"
     )
-    region_name = Unicode("us-east-1", help="Region name").tag(
-        config=True, env="JPYNB_S3_REGION_NAME"
+
+    boto3_session = Any(
+        help="Place to store custom boto3 session (passed to S3_FS) - could be set by init_s3_hook"
     )
+
     bucket = Unicode("notebooks", help="Bucket name to store notebooks").tag(
-        config=True, env="JPYNB_S3_BUCKET"
+        config=True, env="JPY_S3_BUCKET"
     )
+
+    delimiter = Unicode("/", help="Path delimiter").tag(config=True)
+
+    endpoint_url = Unicode(
+        "https://s3.amazonaws.com", help="S3 endpoint URL"
+    ).tag(config=True, env="JPY_S3_ENDPOINT_URL")
+
+    kms_key_id = Unicode(help="KMS ID to use to encrypt workbooks").tag(
+        config=True, env="JPY_S3_KMS_KEY_ID"
+    )
+
+    init_s3_hook = Any(help="optional hook for init'ing s3").tag(config=True)
+
     prefix = Unicode("", help="Prefix path inside the specified bucket").tag(
-        config=True
+        config=True, env="JPY_S3_PREFIX"
     )
-    signature_version = Unicode(help="").tag(config=True)
-    delimiter = Unicode("/", help="Path delimiter").tag(config=True)
-    sse = Unicode(help="Type of server-side encryption to use").tag(config=True)
 
-    kms_key_id = Unicode(help="KMS ID to use to encrypt workbooks").tag(config=True)
+    region_name = Unicode("us-east-1", help="Region name").tag(
+        config=True, env="JPY_S3_REGION_NAME"
+    )
+
+    secret_access_key = Unicode(
+        help="S3/AWS secret access key", allow_none=True, default_value=None
+    ).tag(config=True, env="JPY_S3_SECRET_ACCESS_KEY")
 
     session_token = Unicode(
         help="S3/AWS session token", allow_none=True, default_value=None
-    ).tag(config=True, env="JPYNB_S3_SESSION_TOKEN")
+    ).tag(config=True, env="JPY_S3_SESSION_TOKEN")
 
-    boto3_session = Any(
-        help="Place to store custom boto3 session (passed to S3_FS) - could be set by init_s3_hook"
+    signature_version = Unicode(help="Signature Version").tag(
+        config=True, env="JPY_S3_SIGNATURE_VERSION"
+    )
+
+    sse = Unicode(help="Type of server-side encryption to use").tag(
+        config=True, env="JPY_S3_SSE"
     )
-    init_s3_hook = Any(help="optional hook for init'ing s3").tag(config=True)
 
     s3fs_additional_kwargs = Any(
         help="optional dictionary to be appended to s3fs additional kwargs"
     ).tag(config=True)
 
     def __init__(self, *args, **kwargs):
         super(S3ContentsManager, self).__init__(*args, **kwargs)
 
         self.run_init_s3_hook()
-        self.bucket = _validate_bucket(self.bucket, self.log)
+        self.bucket = validate_bucket(self.bucket, self.log)
+
         self._fs = S3FS(
-            log=self.log,
             access_key_id=self.access_key_id,
-            secret_access_key=self.secret_access_key,
-            endpoint_url=self.endpoint_url,
-            region_name=self.region_name,
+            anon=self.anon,
+            boto3_session=self.boto3_session,
             bucket=self.bucket,
+            delimiter=self.delimiter,
+            endpoint_url=self.endpoint_url,
+            kms_key_id=self.kms_key_id,
+            log=self.log,
             prefix=self.prefix,
+            region_name=self.region_name,
+            secret_access_key=self.secret_access_key,
             session_token=self.session_token,
             signature_version=self.signature_version,
-            delimiter=self.delimiter,
             sse=self.sse,
-            kms_key_id=self.kms_key_id,
-            boto3_session=self.boto3_session,
             s3fs_additional_kwargs=self.s3fs_additional_kwargs,
         )
 
     def run_init_s3_hook(self):
         if self.init_s3_hook is not None:
             self.init_s3_hook(self)
 
     def _save_notebook(self, model, path):
         nb_contents = from_dict(model["content"])
         self.check_and_sign(nb_contents, path)
+
         file_contents = json.dumps(model["content"])
-        self._fs.writenotebook(path, file_contents)
+        self.fs.writenotebook(path, file_contents)
         self.validate_notebook_model(model)
-        return model.get("message")
 
+        return model.get("message")
 
-def _validate_bucket(user_bucket, log):
-    """Helper function to strip off schemas and keys from your bucket.
 
-    Another approach may be to use regexes, but then you have to
-    think about regexes...
+def validate_bucket(user_bucket, log):
+    """Helper function to strip off schemas and keys from the bucket name
 
     Parameters
     ----------
     user_bucket : str
         The bucket that the user provided in their jupyter_notebook_config.py
     log :
         The logger hanging off of GenericContentsManager
@@ -104,37 +123,52 @@
     Raises
     ------
     ValueError
         * When I'm not sure how to parse out a bucket from the provided input
         * When the user provides an empty bucket
     """
     if not user_bucket:
-        raise ValueError(f"user_bucket function argument is empty: {user_bucket}")
-    log.debug(f"s3manager._validate_bucket: User provided bucket: {user_bucket}")
+        raise ValueError(
+            f"user_bucket function argument is empty: {user_bucket}"
+        )
+    log.debug(
+        f"s3manager.validate_bucket: User provided bucket: {user_bucket}"
+    )
     res = urlparse(user_bucket)
     scheme, netloc, path, params, query, fragment = res
     if netloc:
         bucket = netloc
         log.warning(
-            "s3manager._validate_bucket: "
+            "s3manager.validate_bucket: "
             f"Assuming you meant {bucket} for your bucket. "
             f"Using that. Please set bucket={bucket} "
             "in your jupyter_notebook_config.py file"
         )
         return bucket
     if scheme or netloc or params or query or fragment:
-        log.error("s3manager._validate_bucket: " f"Invalid bucket specification: {res}")
+        log.error(
+            "s3manager.validate_bucket: "
+            f"Invalid bucket specification: {res}"
+        )
         raise ValueError(f"Invalid bucket specification: {res}")
 
     bucket = path
     if "/" not in bucket:
         return bucket
 
     bucket, key = bucket.split("/", maxsplit=1)
     log.warning(
-        "s3manager._validate_bucket: "
+        "s3manager.validate_bucket: "
         f"Assuming you meant {bucket} for your bucket name. Don't "
         f"include '/' in your bucket name. Removing /{key} "
         f"from your bucket name. Please set bucket={bucket} "
         "in your jupyter_notebook_config.py file"
     )
     return bucket
+
+
+if __name__ == "__main__":
+    import sys
+
+    from jupyterlab.labapp import main
+
+    sys.exit(main())
```

### Comparing `s3contents-0.7.0/s3contents/tests/hooks.py` & `s3contents-0.9.0/s3contents/tests/hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,8 +37,10 @@
 
     html_exporter = HTMLExporter()
     html_exporter.template_name = "classic"
 
     (body, resources) = html_exporter.from_notebook_node(my_notebook)
 
     base, ext = os.path.splitext(s3_path)
-    contents_manager.fs.write(path=(base + ".html"), content=body, format=_format)
+    contents_manager.fs.write(
+        path=(base + ".html"), content=body, format=_format
+    )
```

### Comparing `s3contents-0.7.0/s3contents/tests/test_gcsmanager.py` & `s3contents-0.9.0/s3contents/tests/gcs/test_gcsmanager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import pytest
-
-from s3contents import GCSContentsManager
 from notebook.services.contents.tests.test_manager import TestContentsManager
 
+try:
+    from s3contents.gcs import GCSContentsManager
+except ImportError:
+    GCSContentsManager = None
+
 
 @pytest.mark.gcs
 class GCSContentsManagerTestCase(TestContentsManager):
     def setUp(self):
         """
         This setup is a hardcoded to run on my laptop and GCP account :)
         """
```

### Comparing `s3contents-0.7.0/s3contents/tests/test_gcsmanager_chunked.py` & `s3contents-0.9.0/s3contents/tests/gcs/test_gcsmanager_chunked.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import time
 
 import pytest
+from notebook.services.contents.tests.test_largefilemanager import (
+    TestLargeFileManager,
+)
 
-from s3contents import GCSContentsManager
 from s3contents.chunks import content_chunks
-from notebook.services.contents.tests.test_largefilemanager import TestLargeFileManager
+
+try:
+    from s3contents.gcs import GCSContentsManager
+except ImportError:
+    GCSContentsManager = None
 
 
 @pytest.mark.gcs
 class GcsContentsManagerLargeFileTestCase(TestLargeFileManager):
     def setUp(self):
         """
         This setup is a hardcoded to run on my laptop and GCP account :)
```

### Comparing `s3contents-0.7.0/s3contents/tests/test_gcsmanager_with_prefix.py` & `s3contents-0.9.0/s3contents/tests/gcs/test_gcsmanager_with_prefix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import pytest
-
-from s3contents import GCSContentsManager
 from notebook.services.contents.tests.test_manager import TestContentsManager
 
+try:
+    from s3contents.gcs import GCSContentsManager
+except ImportError:
+    GCSContentsManager = None
+
 
 @pytest.mark.gcs
 class GCSContentsManagerTestCase_prefix(TestContentsManager):
     def setUp(self):
         """
         This setup is a hardcoded to run on my laptop and GCP account :)
         """
```

### Comparing `s3contents-0.7.0/s3contents/tests/test_s3manager.py` & `s3contents-0.9.0/s3contents/tests/test_s3manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 
 import pytest
+from notebook.services.contents.tests.test_manager import TestContentsManager
 
 from s3contents import S3ContentsManager
-from s3contents.s3manager import _validate_bucket
-from notebook.services.contents.tests.test_manager import TestContentsManager
+from s3contents.s3manager import validate_bucket
 from s3contents.tests.hooks import make_html_post_save, scrub_output_pre_save
 
 
 @pytest.mark.minio
 class S3ContentsManagerTestCase(TestContentsManager):
     def setUp(self):
         """
@@ -76,25 +76,26 @@
 
 
 # Needs to be removed or else we'll run the main IPython tests as well
 del TestContentsManager
 
 
 @pytest.mark.parametrize(
-    "user_bucket", ("s3://BUCKET/some/key/", "BUCKET/some/", "BUCKET", "//BUCKET")
+    "user_bucket",
+    ("s3://BUCKET/some/key/", "BUCKET/some/", "BUCKET", "//BUCKET"),
 )
 def test_bucket_validation(user_bucket, caplog):
     import logging
 
     logger = logging.getLogger()
-    validated_bucket = _validate_bucket(user_bucket, logger)
+    validated_bucket = validate_bucket(user_bucket, logger)
     assert (
         validated_bucket == "BUCKET"
     ), "ContentsManager's bucket should be parsed properly"
 
 
 def test_bucket_validation_empty_bucket_name(caplog):
     import logging
 
     logger = logging.getLogger()
     with pytest.raises(ValueError):
-        _validate_bucket("", logger)
+        validate_bucket("", logger)
```

### Comparing `s3contents-0.7.0/s3contents/tests/test_s3manager_chunked.py` & `s3contents-0.9.0/s3contents/tests/test_s3manager_chunked.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import time
 
 import pytest
+from notebook.services.contents.tests.test_largefilemanager import (
+    TestLargeFileManager,
+)
 
 from s3contents import S3ContentsManager
 from s3contents.chunks import content_chunks
-from notebook.services.contents.tests.test_largefilemanager import TestLargeFileManager
 
 
 @pytest.mark.minio
 class S3ContentsManagerLargeFileTestCase(TestLargeFileManager):
     def setUp(self):
         """
         This setup is a hardcoded to the use a minio server running in localhost
```

### Comparing `s3contents-0.7.0/s3contents/tests/test_s3manager_with_prefix.py` & `s3contents-0.9.0/s3contents/tests/test_s3manager_with_prefix.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
+from notebook.services.contents.tests.test_manager import TestContentsManager
 
 from s3contents import S3ContentsManager
-from notebook.services.contents.tests.test_manager import TestContentsManager
 
 
 @pytest.mark.minio
 class S3ContentsManagerTestCase_prefix(TestContentsManager):
     def setUp(self):
         """
         This setup is a hardcoded to the use a minio server running in localhost
```

