# Comparing `tmp/sppersist-0.1.5.tar.gz` & `tmp/sppersist-0.1.6.tar.gz`

## Comparing `sppersist-0.1.5.tar` & `sppersist-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.5/src/spPersist/__init__.py
--rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 sppersist-0.1.5/src/spPersist/dp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.5/LICENSE
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sppersist-0.1.5/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sppersist-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.6/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 sppersist-0.1.6/src/spPersist/dp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.6/LICENSE
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sppersist-0.1.6/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sppersist-0.1.6/PKG-INFO
```

### Comparing `sppersist-0.1.5/src/spPersist/dp.py` & `sppersist-0.1.6/src/spPersist/dp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import wget, tarfile, zipfile, os, shutil, requests
+import tarfile, zipfile, os, shutil, requests
 from zipfile import ZipFile
 from google.colab import auth
 import scanpy as sc
 import pandas as pd
 import anndata
 
 
-# id_to_url function, optimize package structure
 
 
 def Visium_FFPE_Mouse_Brain():
   '''
   Returns annotated data object of the Adult Mouse Brain (FFPE) dataset from 
   Visium, 10x Genomics.
   '''
@@ -48,14 +47,17 @@
 def Vizgen_V1(slice_num: int, replicate_num: int):
   '''
   Returns annotated data object of the dataset of 
   slice number slice_num and replicate number replicate_num  
   of the MERFISH Mouse Brain Receptor Map datasets from Vizgen.
   '''
 
+  if slice_num > 3 or replicate_num >3:
+    raise ValueError('Slice '+str(slice_num)+' Replicate '+str(replicate_num)+' does not exist.')
+
   auth.authenticate_user()
 
   # Paths to Data
   base_path = 'gs://public-datasets-vizgen-merfish/datasets/mouse_brain_map/BrainReceptorShowcase/'
 
   dataset_name = 'Slice' + str(slice_num) + '/Replicate' + str(replicate_num) + '/'
   dataset_suffix = '_S' + str(slice_num) + 'R' + str(replicate_num)
@@ -94,57 +96,56 @@
 
   adata.obs = pd.merge(adata.obs, coords, how="left", left_index=True, right_index=True)
   adata.obsm['spatial'] = adata.obs[["center_x", "center_y"]].values
   adata.obs.drop(columns=["center_x", "center_y"], inplace=True)
   return adata
 
 
-def zenodo_urls_from_doi(doi: str):
+def id_to_url(id_num: str):
   '''
-  zenodo_urls_from_doi takes a zenodo doi number doi and
-  returns a list of urls of the files in the repository.
+  id_to_url takes a GEO accession or Zenodo doi id_num
+  and returns the url path of the repository.
   '''
 
-  record_id = doi.split('.')[-1]
+  if 'GSE' in id_num:
+    path = 'https://ftp.ncbi.nlm.nih.gov/geo/series/GSE'+gse[3:6]+'nnn/'+gse+'/suppl/'
+  elif 'zenodo' in id_num:
+    record_id = doi.split('.')[-1]
+    r = requests.get(f"https://zenodo.org/api/records/{record_id}") 
+    urls = [f['links']['self'] for f in r.json()['files']]
+    path = os.path.commonprefix(urls)
+  else:
+    raise ValueError(id_num + ' is neither GEO accession or Zenodo doi.')
 
-  # get request (do not need to provide access token since public
-  r = requests.get(f"https://zenodo.org/api/records/{record_id}")  # params={'access_token': ACCESS_TOKEN})
-  return [f['links']['self'] for f in r.json()['files']]
+  return path
 
 
 def zenodo_to_h5(doi: str, filename: str, ttype: str):
   '''
   zenodo_to_h5 takes a zenodo doi number doi that 
   contains a tar or zip file named filename and ttype specifying
   if the technology type is Visium or MERFISH, and
   exports a zip file of annotated objects from 
   the Visium or MERFISH samples in the dataset as h5 files.
   '''
 
-  urls = zenodo_urls_from_doi(doi)
-  for url in urls:
-    if filename in url:
-      path = '/'.join(url.split('/')[:-1]) + '/'
-  
-  if path is None:
-    raise NameError('The repository does not contain a file named filename.')
-
+  path = id_to_url(doi)
   url_to_h5(path,filename=filename,ttype=ttype)
 
 
 def accession_to_h5(gse: str, filename: str, ttype: str):
   '''
   accession_to_h5 takes a GEO accession number gse that 
   contains a tar or zip file named filename and ttype specifying
   if the technology type is Visium or MERFISH, and
   exports a zip file of annotated objects from 
   the Visium or MERFISH samples in the dataset as h5 files.
   '''
 
-  path = 'https://ftp.ncbi.nlm.nih.gov/geo/series/GSE'+gse[3:6]+'nnn/'+gse+'/suppl/'
+  path = id_to_url(gse)
   url_to_h5(path, filename=filename, ttype=ttype)
 
 
 def url_to_h5(path: str, filename: str, ttype: str):
   '''
   url_to_h5 takes a url path that contains a 
   tar or zip file named filename and ttype specifying
@@ -154,17 +155,17 @@
 
   Note that the files in filename should contain samples of 
   gene expression counts and the corresponding spatial coordinates
   and the sample id should be prefix of these files separated by the
   underscore character.
   '''
 
-  url = path + filename
+  url = os.path.join(path,filename)
   if filename not in os.listdir():
-    wget.download(url, bar=wget.bar_adaptive)
+    open(filename, 'wb').write(requests.get(url).content)
 
   if tarfile.is_tarfile(filename):
     repository = tarfile.open(filename) 
     filenames = repository.getnames()
   elif zipfile.is_tarfile(filename):
     repository = ZipFile(filename)
     filenames = repository.namelist()
```

### Comparing `sppersist-0.1.5/LICENSE` & `sppersist-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.1.5/pyproject.toml` & `sppersist-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-0.1.5/PKG-INFO` & `sppersist-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.1.5
+Version: 0.1.6
 Summary: Spatial analysis package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

