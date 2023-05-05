# Comparing `tmp/raphtory-0.0.9-cp39-none-win_amd64.whl.zip` & `tmp/raphtory-0.2.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2052474 bytes, number of entries: 7
--rw-r--r--  4.6 unx     8906 b- defN 23-Apr-14 13:05 raphtory-0.0.9.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-14 13:05 raphtory-0.0.9.dist-info/WHEEL
--rw-r--r--  4.6 unx     2005 b- defN 23-Apr-14 13:05 raphtory/nullmodels.py
--rw-r--r--  4.6 unx     7447 b- defN 23-Apr-14 13:05 raphtory/vis.py
--rw-r--r--  4.6 unx      311 b- defN 23-Apr-14 13:05 raphtory/__init__.py
--rwxr-xr-x  4.6 unx  5557760 b- defN 23-Apr-14 13:05 raphtory/raphtory.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      532 b- defN 23-Apr-14 13:05 raphtory-0.0.9.dist-info/RECORD
-7 files, 5577057 bytes uncompressed, 2051546 bytes compressed:  63.2%
+Zip file size: 2849769 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     9133 b- defN 23-May-05 17:42 raphtory-0.2.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-May-05 17:42 raphtory-0.2.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     2052 b- defN 23-May-05 17:42 raphtory/nullmodels.py
+-rw-r--r--  4.6 unx     7531 b- defN 23-May-05 17:42 raphtory/vis.py
+-rw-r--r--  4.6 unx      537 b- defN 23-May-05 17:42 raphtory/__init__.py
+-rwxr-xr-x  4.6 unx  8158208 b- defN 23-May-05 17:42 raphtory/raphtory.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      532 b- defN 23-May-05 17:42 raphtory-0.2.0.dist-info/RECORD
+7 files, 8178089 bytes uncompressed, 2848841 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: raphtory-0.0.9.dist-info/METADATA
+Filename: raphtory-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: raphtory-0.0.9.dist-info/WHEEL
+Filename: raphtory-0.2.0.dist-info/WHEEL
 Comment: 
 
 Filename: raphtory/nullmodels.py
 Comment: 
 
 Filename: raphtory/vis.py
 Comment: 
 
 Filename: raphtory/__init__.py
 Comment: 
 
 Filename: raphtory/raphtory.cp39-win_amd64.pyd
 Comment: 
 
-Filename: raphtory-0.0.9.dist-info/RECORD
+Filename: raphtory-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## raphtory/nullmodels.py

```diff
@@ -1,7 +1,11 @@
+"""
+Generate null models for a graph.
+"""
+
 import pandas as pd
 
 def shuffle_column(graph_df:pd.DataFrame, col_number=None, col_name=None, inplace=False):
     """
     returns a dataframe with a given column shuffled
     """
     assert col_number is not None or col_name is not None, f"No column number or name provided."
```

## raphtory/vis.py

```diff
@@ -1,7 +1,10 @@
+"""
+Generate a visualisation using matplotlib or pyvis from Raphtory graphs.
+"""
 from pyvis.network import Network
 import networkx as nx
 
 r"""Draw a graph with Pyvis.
 
 .. note::
```

## raphtory/__init__.py

```diff
@@ -5,8 +5,12 @@
 sys.modules["raphtory.graph_loader"] = graph_loader
 
 
 from .nullmodels import *
 
 __doc__ = raphtory.__doc__
 if hasattr(raphtory, "__all__"):
-    __all__ = raphtory.__all__
+    __all__ = raphtory.__all__
+
+algorithms.__doc__ = "Algorithmic functions that can be run on Raphtory graphs"
+graph_gen.__doc__ = "Generate Raphtory graphs from attachment models"
+graph_loader.__doc__ = "Load and save Raphtory graphs from/to file(s)"
```

