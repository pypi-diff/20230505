# Comparing `tmp/aiida-dataframe-0.1.2.tar.gz` & `tmp/aiida-dataframe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-dataframe-0.1.2.tar", last modified: Wed May  3 19:25:06 2023, max compression
+gzip compressed data, was "aiida-dataframe-0.1.3.tar", last modified: Fri May  5 09:08:09 2023, max compression
```

## Comparing `aiida-dataframe-0.1.2.tar` & `aiida-dataframe-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0      195 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.github/install_aiida_github.sh
--rw-r--r--   0        0        0     2240 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      762 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.github/workflows/publish-on-pypi.yml
--rw-r--r--   0        0        0      121 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.gitignore
--rw-r--r--   0        0        0      852 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      159 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.readthedocs.yml
--rw-r--r--   0        0        0     1073 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/LICENSE
--rw-r--r--   0        0        0     2424 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/README.md
--rw-r--r--   0        0        0       95 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/aiida_dataframe/__init__.py
--rw-r--r--   0        0        0     2171 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/aiida_dataframe/cli.py
--rw-r--r--   0        0        0      182 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/aiida_dataframe/data/__init__.py
--rw-r--r--   0        0        0     4711 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/aiida_dataframe/data/dataframe.py
--rw-r--r--   0        0        0      322 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/conftest.py
--rw-r--r--   0        0        0        7 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/docs/.gitignore
--rwxr-xr-x   0        0        0     1554 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/docs/Makefile
--rwxr-xr-x   0        0        0     7656 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/docs/source/conf.py
--rw-r--r--   0        0        0     3008 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/docs/source/developer_guide/index.rst
--rw-r--r--   0        0        0    76300 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/images/AiiDA_transparent_logo.png
--rwxr-xr-x   0        0        0     1269 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/index.rst
--rw-r--r--   0        0        0     2326 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/user_guide/get_started.rst
--rw-r--r--   0        0        0       94 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/user_guide/index.rst
--rw-r--r--   0        0        0      243 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/user_guide/tutorial.rst
--rw-r--r--   0        0        0     3371 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      215 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2016 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/test_cli.py
--rw-r--r--   0        0        0      143 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/test_cli/test_dataframe_export.csv
--rw-r--r--   0        0        0      488 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/test_cli/test_dataframe_show.txt
--rw-r--r--   0        0        0    12759 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/test_data.py
--rw-r--r--   0        0        0     4271 1970-01-01 00:00:00.000000 aiida-dataframe-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0      195 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/.github/install_aiida_github.sh
+-rw-r--r--   0        0        0     2240 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      762 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/.github/workflows/publish-on-pypi.yml
+-rw-r--r--   0        0        0      121 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/.gitignore
+-rw-r--r--   0        0        0      852 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      159 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/.readthedocs.yml
+-rw-r--r--   0        0        0     1073 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2424 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/README.md
+-rw-r--r--   0        0        0       95 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/aiida_dataframe/__init__.py
+-rw-r--r--   0        0        0     2171 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/aiida_dataframe/cli.py
+-rw-r--r--   0        0        0      182 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/aiida_dataframe/data/__init__.py
+-rw-r--r--   0        0        0     4927 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/aiida_dataframe/data/dataframe.py
+-rw-r--r--   0        0        0      322 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/conftest.py
+-rw-r--r--   0        0        0        7 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/docs/.gitignore
+-rwxr-xr-x   0        0        0     1554 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/docs/Makefile
+-rwxr-xr-x   0        0        0     7656 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/docs/source/conf.py
+-rw-r--r--   0        0        0     3008 2023-05-05 09:08:02.508503 aiida-dataframe-0.1.3/docs/source/developer_guide/index.rst
+-rw-r--r--   0        0        0    76300 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/docs/source/images/AiiDA_transparent_logo.png
+-rwxr-xr-x   0        0        0     1269 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/docs/source/index.rst
+-rw-r--r--   0        0        0     2326 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/docs/source/user_guide/get_started.rst
+-rw-r--r--   0        0        0       94 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/docs/source/user_guide/index.rst
+-rw-r--r--   0        0        0      243 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/docs/source/user_guide/tutorial.rst
+-rw-r--r--   0        0        0     3371 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2016 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/tests/test_cli.py
+-rw-r--r--   0        0        0      143 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/tests/test_cli/test_dataframe_export.csv
+-rw-r--r--   0        0        0      488 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/tests/test_cli/test_dataframe_show.txt
+-rw-r--r--   0        0        0    13695 2023-05-05 09:08:02.512503 aiida-dataframe-0.1.3/tests/test_data.py
+-rw-r--r--   0        0        0     4271 1970-01-01 00:00:00.000000 aiida-dataframe-0.1.3/PKG-INFO
```

### Comparing `aiida-dataframe-0.1.2/.github/workflows/ci.yml` & `aiida-dataframe-0.1.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/.github/workflows/publish-on-pypi.yml` & `aiida-dataframe-0.1.3/.github/workflows/publish-on-pypi.yml`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/.pre-commit-config.yaml` & `aiida-dataframe-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/LICENSE` & `aiida-dataframe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/README.md` & `aiida-dataframe-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/aiida_dataframe/cli.py` & `aiida-dataframe-0.1.3/aiida_dataframe/cli.py`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/aiida_dataframe/data/dataframe.py` & `aiida-dataframe-0.1.3/aiida_dataframe/data/dataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,12 +126,16 @@
         """
         Store the node. Before the node is stored
         sync the HDF5 storage with the _df attribute on the node
         This catches changes to the node made by using setitem
         on the dataframe e.g. `df["A"] = new_value`
         This is only done if the hashes of the DATA does not match up
         """
-        current_hash = self._hash_dataframe(self._df)
-        if current_hash != self.get_attribute("_pandas_data_hash"):
-            self._update_dataframe(self._df)
+        if not self.is_stored:
+            # Check if the dataframe directly attached to the node
+            # has been mutated in place before storing
+            # If so the underlying file is updated
+            current_hash = self._hash_dataframe(self._df)
+            if current_hash != self.get_attribute("_pandas_data_hash"):
+                self._update_dataframe(self._df)
 
         return super().store(*args, **kwargs)
```

### Comparing `aiida-dataframe-0.1.2/docs/Makefile` & `aiida-dataframe-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/docs/source/conf.py` & `aiida-dataframe-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/docs/source/developer_guide/index.rst` & `aiida-dataframe-0.1.3/docs/source/developer_guide/index.rst`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/docs/source/images/AiiDA_transparent_logo.png` & `aiida-dataframe-0.1.3/docs/source/images/AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/docs/source/index.rst` & `aiida-dataframe-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/docs/source/user_guide/get_started.rst` & `aiida-dataframe-0.1.3/docs/source/user_guide/get_started.rst`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/pyproject.toml` & `aiida-dataframe-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/tests/test_cli.py` & `aiida-dataframe-0.1.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.2/tests/test_data.py` & `aiida-dataframe-0.1.3/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,7 +490,44 @@
 
     assert node.list_object_names() == ["non_default.h5"]
 
     loaded = load_node(node.pk)
     assert loaded is not node
     assert loaded.list_object_names() == ["non_default.h5"]
     assert_frame_equal(loaded.df, df)
+
+
+@pytest.mark.parametrize(
+    "entry_point",
+    ("dataframe.frame",),
+)
+def test_modification_store_already_stored(entry_point):
+    """
+    Test that callign store on an already stroed node does nothing
+    (Including crashes)
+    """
+
+    PandasFrameData = DataFactory(entry_point)
+
+    # Example from pandas Docs
+    df = pd.DataFrame(
+        {
+            "A": 1.0,
+            "B": pd.Timestamp("20130102"),
+            "C": pd.Series(1, index=list(range(4)), dtype="float32"),
+            "D": np.array([3] * 4, dtype="int32"),
+            "E": pd.Categorical(["test", "train", "test", "train"]),
+            "F": "foo",
+        }
+    )
+
+    node = PandasFrameData(df)
+    node.store()
+    assert node.is_stored
+
+    loaded = load_node(node.pk)
+    assert loaded is not node
+    assert_frame_equal(loaded.df, df)
+
+    loaded_store = loaded.store()
+    assert loaded_store is loaded
+    assert_frame_equal(loaded_store.df, df)
```

### Comparing `aiida-dataframe-0.1.2/PKG-INFO` & `aiida-dataframe-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-dataframe
-Version: 0.1.2
+Version: 0.1.3
 Summary: AiiDA data plugin for pandas DataFrame objects
 Keywords: aiida,plugin
 Author-email: Henning Janßen <henning.janssen@gmx.net>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
```

