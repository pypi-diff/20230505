# Comparing `tmp/dream_helpers-0.0.268.tar.gz` & `tmp/dream_helpers-0.0.269.tar.gz`

## Comparing `dream_helpers-0.0.268.tar` & `dream_helpers-0.0.269.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/.bumpversion.cfg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/Makefile
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/src/dream_helpers/__init__.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/src/dream_helpers/datahub_helper.py
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/src/dream_helpers/kubeflow_helper.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/src/dream_helpers/minio_helper.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/README.md
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/pyproject.toml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.268/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/.bumpversion.cfg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/Makefile
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/src/dream_helpers/__init__.py
+-rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/src/dream_helpers/datahub_helper.py
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/src/dream_helpers/kubeflow_helper.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/src/dream_helpers/minio_helper.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/README.md
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/pyproject.toml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.269/PKG-INFO
```

### Comparing `dream_helpers-0.0.268/src/dream_helpers/datahub_helper.py` & `dream_helpers-0.0.269/src/dream_helpers/datahub_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,17 @@
 def load_csv_dataset_as_pandas_dataframe(dataset:str, 
                                          minio_endpoint:str, 
                                          datahub_endpoint:str) -> pd.DataFrame:
     dataset_source_url = get_dataset_source_url(
         endpoint=datahub_endpoint,
         dataset_name=dataset
     )
-    dataset_source_url = "sources/get-sources-example/new%20zealand%20statistical%20areas%20--%20generalised"
+    dataset_source_url = "s3://sources/get-sources-example/new%20zealand%20statistical%20areas%20--%20generalised"
     logger.info("Dataset source url -> %s" % dataset_source_url)
+
     return pd.read_csv(
         dataset_source_url,
         storage_options={
             "client_kwargs": {"endpoint_url": minio_endpoint}
         }
     )
```

### Comparing `dream_helpers-0.0.268/src/dream_helpers/kubeflow_helper.py` & `dream_helpers-0.0.269/src/dream_helpers/kubeflow_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.268/src/dream_helpers/minio_helper.py` & `dream_helpers-0.0.269/src/dream_helpers/minio_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.268/.gitignore` & `dream_helpers-0.0.269/.gitignore`

 * *Files identical despite different names*

