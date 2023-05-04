# Comparing `tmp/dream_helpers-0.0.271.tar.gz` & `tmp/dream_helpers-0.0.272.tar.gz`

## Comparing `dream_helpers-0.0.271.tar` & `dream_helpers-0.0.272.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/.bumpversion.cfg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/Makefile
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/src/dream_helpers/__init__.py
--rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/src/dream_helpers/datahub_helper.py
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/src/dream_helpers/kubeflow_helper.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/src/dream_helpers/minio_helper.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/README.md
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/pyproject.toml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.271/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/.bumpversion.cfg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/Makefile
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/src/dream_helpers/__init__.py
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/src/dream_helpers/datahub_helper.py
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/src/dream_helpers/kubeflow_helper.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/src/dream_helpers/minio_helper.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/README.md
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/pyproject.toml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dream_helpers-0.0.272/PKG-INFO
```

### Comparing `dream_helpers-0.0.271/src/dream_helpers/datahub_helper.py` & `dream_helpers-0.0.272/src/dream_helpers/datahub_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,28 +78,29 @@
 def load_csv_dataset_as_pandas_dataframe(dataset:str, 
                                          minio_endpoint:str, 
                                          datahub_endpoint:str) -> pd.DataFrame:
     dataset_source_url = get_dataset_source_url(
         endpoint=datahub_endpoint,
         dataset_name=dataset
     )
-    dataset_source_url = "s3://%s" % urllib.parse.quote(dataset_source_url)
+    dataset_source_url = "s3://%s" % dataset_source_url    
     logger.info("Dataset source url -> %s" % dataset_source_url)
     return pd.read_csv(
         dataset_source_url,
         storage_options={
             "client_kwargs": {
                 "endpoint_url": minio_endpoint,
                 "aws_access_key_id": "minio",
                 "aws_secret_access_key": "minio123"
             }
         }
     )
 
 
+
 '''
 
 Dataset Helpers  
 
 '''
 def upsert_datasets(dataset_urns: List[str],
                    platform_urn: str,
```

### Comparing `dream_helpers-0.0.271/src/dream_helpers/kubeflow_helper.py` & `dream_helpers-0.0.272/src/dream_helpers/kubeflow_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.271/src/dream_helpers/minio_helper.py` & `dream_helpers-0.0.272/src/dream_helpers/minio_helper.py`

 * *Files identical despite different names*

### Comparing `dream_helpers-0.0.271/.gitignore` & `dream_helpers-0.0.272/.gitignore`

 * *Files identical despite different names*

