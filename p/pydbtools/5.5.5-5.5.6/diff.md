# Comparing `tmp/pydbtools-5.5.5.tar.gz` & `tmp/pydbtools-5.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbtools-5.5.5.tar", max compression
+gzip compressed data, was "pydbtools-5.5.6.tar", max compression
```

## Comparing `pydbtools-5.5.5.tar` & `pydbtools-5.5.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10095 2023-05-02 16:10:43.329515 pydbtools-5.5.5/README.md
--rw-r--r--   0        0        0      855 2023-05-02 16:10:43.329515 pydbtools-5.5.5/pydbtools/__init__.py
--rw-r--r--   0        0        0     1130 2023-05-02 16:10:43.329515 pydbtools-5.5.5/pydbtools/_sql_render.py
--rw-r--r--   0        0        0    23104 2023-05-02 16:10:43.329515 pydbtools-5.5.5/pydbtools/_wrangler.py
--rw-r--r--   0        0        0     7265 2023-05-02 16:10:43.329515 pydbtools-5.5.5/pydbtools/utils.py
--rw-r--r--   0        0        0      663 2023-05-02 16:10:43.329515 pydbtools-5.5.5/pyproject.toml
--rw-r--r--   0        0        0    10938 1970-01-01 00:00:00.000000 pydbtools-5.5.5/PKG-INFO
+-rw-r--r--   0        0        0     9632 2023-05-05 15:48:50.967806 pydbtools-5.5.6/README.md
+-rw-r--r--   0        0        0      855 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pydbtools/__init__.py
+-rw-r--r--   0        0        0     1130 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pydbtools/_sql_render.py
+-rw-r--r--   0        0        0    23104 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pydbtools/_wrangler.py
+-rw-r--r--   0        0        0     6391 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pydbtools/utils.py
+-rw-r--r--   0        0        0      647 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pyproject.toml
+-rw-r--r--   0        0        0    10475 1970-01-01 00:00:00.000000 pydbtools-5.5.6/PKG-INFO
```

### Comparing `pydbtools-5.5.5/README.md` & `pydbtools-5.5.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -207,18 +207,14 @@
 user_id, out_path = pydb.get_user_id_and_table_dir()
 temp_db_name = pydb.get_database_name_from_userid(user_id)
 print(temp_db_name)
 pydb.create_temp_table()
 print(wr.catalog.delete_database(name=temp_db_name))
 ```
 
-### Setting the region
-
-In order to run queries, Athena needs to output its results into a staging bucket in S3. The aws region passed to awswrangler needs to be the same as the region of that bucket. This is usually the same as that set by the `AWS_DEFAULT_REGION` set within your underlying environment. However, in cases of cross-region working, you can specify the region for Athena to access by setting `AWS_ATHENA_QUERY_REGION` as an environment variable.
-
 # DEPRECATED
 
 ## Functions
 
 The functions:
 - `pydbtools.get_athena_query_response`
 - `pydbtools.read_sql`
```

### Comparing `pydbtools-5.5.5/pydbtools/__init__.py` & `pydbtools-5.5.6/pydbtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     create_table,
 )
 
 from ._sql_render import get_sql_from_file, render_sql_template  # noqa: F401
 
 from .utils import s3_path_join  # noqa: F401
 
-__version__ = "5.5.5"
+__version__ = "5.5.6"
```

### Comparing `pydbtools-5.5.5/pydbtools/_sql_render.py` & `pydbtools-5.5.6/pydbtools/_sql_render.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.5/pydbtools/_wrangler.py` & `pydbtools-5.5.6/pydbtools/_wrangler.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.5/pydbtools/utils.py` & `pydbtools-5.5.6/pydbtools/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,46 +2,29 @@
 import os
 import re
 import sqlparse
 from urllib.parse import urlparse, urljoin, urlunparse
 import sql_metadata
 import inspect
 import boto3
-from botocore.exceptions import NoCredentialsError
 from botocore.credentials import (
     InstanceMetadataProvider,
     InstanceMetadataFetcher,
 )
 from functools import reduce
 import awswrangler as wr
-import warnings
+
 
 # Set pydbtool params - if you were so inclined to change them
-bucket = os.getenv("ATHENA_QUERY_DUMP_BUCKET", "mojap-athena-query-dump")
-try:
-    bucket_region = wr.s3.get_bucket_region(bucket)
-except NoCredentialsError:
-    bucket_region = "eu-west-1"
+bucket = "mojap-athena-query-dump"
 temp_database_name_prefix = "mojap_de_temp_"
 aws_default_region = os.getenv(
-    "AWS_ATHENA_QUERY_REGION",
-    os.getenv("AWS_DEFAULT_REGION", os.getenv("AWS_REGION", "eu-west-1")),
+    "AWS_DEFAULT_REGION", os.getenv("AWS_REGION", "eu-west-1")
 )
 
-if aws_default_region != bucket_region:
-    warnings.warn(
-        f"""
-    Your aws region {aws_default_region} is different from the bucket where
-    the query results are saved: {bucket_region}. You can change this for this session
-    by setting pydb.utils.aws_default_region = "{bucket_region}".
-    You should also set the environment variable:
-    AWS_ATHENA_QUERY_REGION = "{bucket_region}" to ensure the correct region is set.
-    """
-    )
-
 
 def s3_path_join(base: str, *urls: [str]):
     return reduce(_s3_path_join, urls, base)
 
 
 def _s3_path_join(base: str, url: str, allow_fragments=True) -> str:
     """
@@ -151,43 +134,35 @@
             )
         )
     # Strip output for consistency, different versions of sqlparse
     # treat a trailing newline differently
     return "".join(new_query).strip()
 
 
-def clean_user_id(user_id: str) -> str:
-    username = user_id.split(":")[-1]
-    if "@" in username:
-        username = username.split("@")[0]
-    username = username.replace("-", "_")
-    return username
-
-
 def get_user_id_and_table_dir(
     boto3_session=None, force_ec2: bool = False, region_name: str = None
 ) -> Tuple[str, str]:
 
     region_name = _set_region_name(region_name)
 
     if boto3_session is None:
         boto3_session = get_boto_session(force_ec2=force_ec2, region_name=region_name)
 
     sts_client = boto3_session.client("sts")
     sts_resp = sts_client.get_caller_identity()
-    user_id = clean_user_id(sts_resp["UserId"])
-    out_path = s3_path_join("s3://" + bucket, user_id)
+    out_path = s3_path_join("s3://" + bucket, sts_resp["UserId"])
     if out_path[-1] != "/":
         out_path += "/"
 
-    return (user_id, out_path)
+    return (sts_resp["UserId"], out_path)
 
 
-def get_database_name_from_userid(clean_user_id: str) -> str:
-    unique_db_name = temp_database_name_prefix + clean_user_id
+def get_database_name_from_userid(user_id: str) -> str:
+    unique_db_name = user_id.split(":")[-1].split("-", 1)[-1].replace("-", "_")
+    unique_db_name = temp_database_name_prefix + unique_db_name
     return unique_db_name
 
 
 def get_database_name_from_sql(sql: str) -> str:
     """
     Obtains database name from SQL query for use
     by awswrangler.
```

### Comparing `pydbtools-5.5.5/pyproject.toml` & `pydbtools-5.5.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool]
 [tool.poetry]
 name = "pydbtools"
-version = "5.5.5"
+version = "5.5.6"
 description = "A python package to query data via amazon athena and bring it into a pandas df using aws-wrangler."
 license = "MIT"
 authors = ["Karik Isichei <karik.isichei@digital.justice.gov.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11" # wrangler dependency
 boto3 = ">=1.7.4"
 sqlparse = "^0.4.4"
-awswrangler = "^2.15.0"
+awswrangler = "^2.12.0"
 pyarrow = ">=5.0.0"
 Jinja2 = ">=3.1.0"
 sql-metadata = "^2.3.0"
 arrow-pd-parser = "^1.3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.1"
 toml = "^0.10"
-moto = "^4.1.8"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pydbtools-5.5.5/PKG-INFO` & `pydbtools-5.5.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pydbtools
-Version: 5.5.5
+Version: 5.5.6
 Summary: A python package to query data via amazon athena and bring it into a pandas df using aws-wrangler.
 License: MIT
 Author: Karik Isichei
 Author-email: karik.isichei@digital.justice.gov.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.0)
 Requires-Dist: arrow-pd-parser (>=1.3.7,<2.0.0)
-Requires-Dist: awswrangler (>=2.15.0,<3.0.0)
+Requires-Dist: awswrangler (>=2.12.0,<3.0.0)
 Requires-Dist: boto3 (>=1.7.4)
 Requires-Dist: pyarrow (>=5.0.0)
 Requires-Dist: sql-metadata (>=2.3.0,<3.0.0)
 Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
 Description-Content-Type: text/markdown
 
 # pydbtools
@@ -229,18 +229,14 @@
 user_id, out_path = pydb.get_user_id_and_table_dir()
 temp_db_name = pydb.get_database_name_from_userid(user_id)
 print(temp_db_name)
 pydb.create_temp_table()
 print(wr.catalog.delete_database(name=temp_db_name))
 ```
 
-### Setting the region
-
-In order to run queries, Athena needs to output its results into a staging bucket in S3. The aws region passed to awswrangler needs to be the same as the region of that bucket. This is usually the same as that set by the `AWS_DEFAULT_REGION` set within your underlying environment. However, in cases of cross-region working, you can specify the region for Athena to access by setting `AWS_ATHENA_QUERY_REGION` as an environment variable.
-
 # DEPRECATED
 
 ## Functions
 
 The functions:
 - `pydbtools.get_athena_query_response`
 - `pydbtools.read_sql`
```

