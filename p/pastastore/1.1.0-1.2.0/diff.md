# Comparing `tmp/pastastore-1.1.0.tar.gz` & `tmp/pastastore-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastastore-1.1.0.tar", last modified: Tue Mar 21 09:53:30 2023, max compression
+gzip compressed data, was "pastastore-1.2.0.tar", last modified: Fri May  5 14:06:23 2023, max compression
```

## Comparing `pastastore-1.1.0.tar` & `pastastore-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-21 09:53:30.591124 pastastore-1.1.0/
--rw-rw-r--   0 david     (1000) david     (1000)     1082 2020-05-01 14:40:40.000000 pastastore-1.1.0/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)     6356 2023-03-21 09:53:30.591124 pastastore-1.1.0/PKG-INFO
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-21 09:53:30.591124 pastastore-1.1.0/pastastore/
--rw-rw-r--   0 david     (1000) david     (1000)      181 2023-02-02 12:48:10.000000 pastastore-1.1.0/pastastore/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    62394 2023-03-20 14:00:43.000000 pastastore-1.1.0/pastastore/base.py
--rw-rw-r--   0 david     (1000) david     (1000)    23461 2023-03-17 15:38:56.000000 pastastore-1.1.0/pastastore/connectors.py
--rw-rw-r--   0 david     (1000) david     (1000)     6504 2023-03-20 14:08:46.000000 pastastore-1.1.0/pastastore/datasets.py
--rw-rw-r--   0 david     (1000) david     (1000)    41532 2023-03-03 15:03:32.000000 pastastore-1.1.0/pastastore/plotting.py
--rw-rw-r--   0 david     (1000) david     (1000)    34111 2023-03-20 14:09:34.000000 pastastore-1.1.0/pastastore/store.py
--rw-rw-r--   0 david     (1000) david     (1000)    29147 2023-02-08 13:00:07.000000 pastastore-1.1.0/pastastore/util.py
--rw-rw-r--   0 david     (1000) david     (1000)      203 2023-03-21 09:30:58.000000 pastastore-1.1.0/pastastore/version.py
--rw-rw-r--   0 david     (1000) david     (1000)    29564 2023-02-03 13:54:02.000000 pastastore-1.1.0/pastastore/yaml_interface.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-21 09:53:30.591124 pastastore-1.1.0/pastastore.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     6356 2023-03-21 09:53:30.000000 pastastore-1.1.0/pastastore.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      567 2023-03-21 09:53:30.000000 pastastore-1.1.0/pastastore.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-21 09:53:30.000000 pastastore-1.1.0/pastastore.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)      390 2023-03-21 09:53:30.000000 pastastore-1.1.0/pastastore.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-03-21 09:53:30.000000 pastastore-1.1.0/pastastore.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)     2433 2023-02-02 12:48:10.000000 pastastore-1.1.0/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)     3576 2023-02-21 09:16:04.000000 pastastore-1.1.0/readme.md
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-03-21 09:53:30.591124 pastastore-1.1.0/setup.cfg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-21 09:53:30.591124 pastastore-1.1.0/tests/
--rw-rw-r--   0 david     (1000) david     (1000)      170 2022-12-23 15:29:17.000000 pastastore-1.1.0/tests/test_001_import.py
--rw-rw-r--   0 david     (1000) david     (1000)     8299 2023-02-02 12:48:10.000000 pastastore-1.1.0/tests/test_002_connectors.py
--rw-rw-r--   0 david     (1000) david     (1000)     8588 2023-03-20 14:12:21.000000 pastastore-1.1.0/tests/test_003_pastastore.py
--rw-rw-r--   0 david     (1000) david     (1000)     4580 2023-02-06 09:35:01.000000 pastastore-1.1.0/tests/test_004_yaml.py
--rw-rw-r--   0 david     (1000) david     (1000)     1833 2023-02-08 12:44:18.000000 pastastore-1.1.0/tests/test_005_maps_plots.py
--rw-rw-r--   0 david     (1000) david     (1000)     6499 2023-03-20 16:46:28.000000 pastastore-1.1.0/tests/test_006_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:06:23.297315 pastastore-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-05 14:06:07.000000 pastastore-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-05 14:06:23.293315 pastastore-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:06:23.293315 pastastore-1.2.0/pastastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62394 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28727 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41622 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34111 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31168 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29490 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/yaml_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:06:23.293315 pastastore-1.2.0/pastastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-05 14:06:07.000000 pastastore-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-05 14:06:07.000000 pastastore-1.2.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:06:23.297315 pastastore-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:06:23.293315 pastastore-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_001_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_002_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_003_pastastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_004_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_005_maps_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_006_benchmark.py
```

### Comparing `pastastore-1.1.0/LICENSE` & `pastastore-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pastastore-1.1.0/PKG-INFO` & `pastastore-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastastore
-Version: 1.1.0
+Version: 1.2.0
 Summary: Tools for managing Pastas time series models.
 Author: D.A. Brakenhoff
 Maintainer-email: "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 D.A. Brakenhoff
         
@@ -49,14 +49,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: optional
 Provides-Extra: test
 Provides-Extra: pystore
 Provides-Extra: arctic
+Provides-Extra: arcticdb
 Provides-Extra: docs
 License-File: LICENSE
 
 ![pastastore](https://github.com/pastas/pastastore/workflows/pastastore/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/pastastore/badge/?version=latest)](https://pastastore.readthedocs.io/en/latest/?badge=latest)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/81b1e0294f5247cfa4eca657a8eebc61)](https://www.codacy.com/gh/pastas/pastastore?utm_source=github.com&utm_medium=referral&utm_content=pastas/pastastore&utm_campaign=Badge_Grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/81b1e0294f5247cfa4eca657a8eebc61)](https://www.codacy.com/gh/pastas/pastastore/dashboard?utm_source=github.com&utm_medium=referral&utm_content=pastas/pastastore&utm_campaign=Badge_Coverage)
@@ -113,14 +114,15 @@
 
 Now the user can add time series, models or analyze or visualize existing
 objects in the database. Some examples showing the functionality of the
 PastaStore object are shown below:
 
 ```python
 import pandas as pd
+import pastas as ps
 
 # load oseries from CSV and add to database
 oseries = pd.read_csv("oseries.csv")
 pstore.add_oseries(oseries, "my_oseries", metadata={"x": 100_000, "y": 400_000})
 
 # read oseries from database
 oseries = pstore.get_oseries("my_oseries")
@@ -132,15 +134,14 @@
 ax = pstore.maps.oseries()
 pstore.maps.add_background_map(ax)  # add a background map
 
 # plot my_oseries time series
 ax2 = pstore.plot.oseries(names=["my_oseries"])
 
 # create a model with pastas
-import pastas as ps
 ml = ps.Model(oseries, name="my_model")
 
 # add model to database
 pstore.add_model(ml)
 
 # load model from database
 ml2 = pstore.get_models("my_model")
```

### Comparing `pastastore-1.1.0/pastastore/base.py` & `pastastore-1.2.0/pastastore/base.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.1.0/pastastore/connectors.py` & `pastastore-1.2.0/pastastore/connectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -194,14 +194,195 @@
 
     @property
     def oseries_with_models(self):
         """List of oseries with models."""
         return self._get_library("oseries_models").list_symbols()
 
 
+class ArcticDBConnector(BaseConnector, ConnectorUtil):
+    conn_type = "arcticdb"
+
+    def __init__(self, name: str, uri: str):
+        """Create an ArcticDBConnector object using ArcticDB to store data.
+
+        Parameters
+        ----------
+        name : str
+            name of the database
+        uri : str
+            URI connection string (e.g. 'lmdb://<your path here>')
+        """
+        try:
+            import arcticdb
+        except ModuleNotFoundError as e:
+            print("Please install arcticdb with `pip install arcticdb`!")
+            raise e
+        self.uri = uri
+        self.name = name
+
+        self.libs: dict = {}
+        self.arc = arcticdb.Arctic(uri)
+        self._initialize()
+        self.models = ModelAccessor(self)
+        # for older versions of PastaStore, if oseries_models library is empty
+        # populate oseries - models database
+        self._update_all_oseries_model_links()
+
+    def _initialize(self) -> None:
+        """Internal method to initalize the libraries."""
+
+        for libname in self._default_library_names:
+            if self._library_name(libname) not in self.arc.list_libraries():
+                self.arc.create_library(self._library_name(libname))
+            else:
+                print(
+                    f"ArcticDBConnector: library "
+                    f"'{self._library_name(libname)}'"
+                    " already exists. Linking to existing library."
+                )
+            self.libs[libname] = self._get_library(libname)
+
+    def _library_name(self, libname: str) -> str:
+        """Internal method to get full library name according to ArcticDB."""
+        return ".".join([self.name, libname])
+
+    def _get_library(self, libname: str):
+        """Get ArcticDB library handle.
+
+        Parameters
+        ----------
+        libname : str
+            name of the library
+
+        Returns
+        -------
+        lib : arcticdb.Library handle
+            handle to the library
+        """
+        # get library handle
+        lib = self.arc.get_library(self._library_name(libname))
+        return lib
+
+    def _add_item(
+        self,
+        libname: str,
+        item: Union[FrameorSeriesUnion, Dict],
+        name: str,
+        metadata: Optional[Dict] = None,
+        **_,
+    ) -> None:
+        """Internal method to add item to library (time series or model).
+
+        Parameters
+        ----------
+        libname : str
+            name of the library
+        item : Union[FrameorSeriesUnion, Dict]
+            item to add, either time series or pastas.Model as dictionary
+        name : str
+            name of the item
+        metadata : Optional[Dict], optional
+            dictionary containing metadata, by default None
+        """
+        lib = self._get_library(libname)
+        # only normalizable datatypes can be written with write, else use write_pickle
+        # normalizable: Series, DataFrames, Numpy Arrays
+        if isinstance(item, (dict, list)):
+            lib.write_pickle(name, item, metadata=metadata)
+        else:
+            lib.write(name, item, metadata=metadata)
+
+    def _get_item(self, libname: str, name: str) -> Union[FrameorSeriesUnion, Dict]:
+        """Internal method to retrieve item from library.
+
+        Parameters
+        ----------
+        libname : str
+            name of the library
+        name : str
+            name of the item
+
+        Returns
+        -------
+        item : Union[FrameorSeriesUnion, Dict]
+            time series or model dictionary
+        """
+        lib = self._get_library(libname)
+        return lib.read(name).data
+
+    def _del_item(self, libname: str, name: str) -> None:
+        """Internal method to delete items (series or models).
+
+        Parameters
+        ----------
+        libname : str
+            name of library to delete item from
+        name : str
+            name of item to delete
+        """
+        lib = self._get_library(libname)
+        lib.delete(name)
+
+    def _get_metadata(self, libname: str, name: str) -> dict:
+        """Internal method to retrieve metadata for an item.
+
+        Parameters
+        ----------
+        libname : str
+            name of the library
+        name : str
+            name of the item
+
+        Returns
+        -------
+        dict
+            dictionary containing metadata
+        """
+        lib = self._get_library(libname)
+        return lib.read_metadata(name).metadata
+
+    @property
+    def oseries_names(self):
+        """List of oseries names.
+
+        Returns
+        -------
+        list
+            list of oseries in library
+        """
+        return self._get_library("oseries").list_symbols()
+
+    @property
+    def stresses_names(self):
+        """List of stresses names.
+
+        Returns
+        -------
+        list
+            list of stresses in library
+        """
+        return self._get_library("stresses").list_symbols()
+
+    @property
+    def model_names(self):
+        """List of model names.
+
+        Returns
+        -------
+        list
+            list of models in library
+        """
+        return self._get_library("models").list_symbols()
+
+    @property
+    def oseries_with_models(self):
+        """List of oseries with models."""
+        return self._get_library("oseries_models").list_symbols()
+
+
 class PystoreConnector(BaseConnector, ConnectorUtil):  # pragma: no cover
     conn_type = "pystore"
 
     def __init__(self, name: str, path: str):
         """Create a PystoreConnector object that points to a Pystore.
 
         Parameters
```

### Comparing `pastastore-1.1.0/pastastore/datasets.py` & `pastastore-1.2.0/pastastore/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,25 +172,28 @@
 def _default_connector(conntype: str):
     """Get default connector based on name.
 
     Parameters
     ----------
     conntype : str
         name of connector (DictConnector, PasConnector,
-        ArcticConnector or PystoreConnector)
+        ArcticConnector, ArcticDBConnector or PystoreConnector)
 
     Returns
     -------
     conn : Connector
         default Connector based on type.
     """
     Conn = getattr(pst, conntype)
     if Conn.conn_type == "arctic":
         connstr = "mongodb://localhost:27017/"
         conn = Conn("my_db", connstr)
+    elif Conn.conn_type == "arcticdb":
+        uri = "lmdb://./arctic_db"
+        conn = Conn("my_db", uri)
     elif Conn.conn_type == "pystore":
         conn = Conn("my_db", "./pystore_db")
     elif Conn.conn_type == "dict":
         conn = Conn("my_db")
     elif Conn.conn_type == "pas":
         conn = Conn("my_db", "./pas_db")
     else:
```

### Comparing `pastastore-1.1.0/pastastore/plotting.py` & `pastastore-1.2.0/pastastore/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,17 +583,20 @@
             mask = df["kind"].isin(kind)
             stresses = df[mask]
         else:
             stresses = df
 
         mask0 = (stresses["x"] != 0.0) | (stresses["y"] != 0.0)
 
-        c = stresses.loc[mask0, "kind"]
-        kind_to_color = {k: f"C{i}" for i, k in enumerate(c.unique())}
-        c = c.apply(lambda k: kind_to_color[k])
+        if "c" in kwargs:
+            c = kwargs.pop("c", None)
+        else:
+            c = stresses.loc[mask0, "kind"]
+            kind_to_color = {k: f"C{i}" for i, k in enumerate(c.unique())}
+            c = c.apply(lambda k: kind_to_color[k])
 
         r = self._plotmap_dataframe(stresses.loc[mask0], c=c, figsize=figsize, **kwargs)
         if "ax" in kwargs:
             ax = kwargs["ax"]
         else:
             ax = r
         if labels:
```

### Comparing `pastastore-1.1.0/pastastore/store.py` & `pastastore-1.2.0/pastastore/store.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.1.0/pastastore/util.py` & `pastastore-1.2.0/pastastore/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 def delete_pystore_connector(
     conn=None,
     path: Optional[str] = None,
     name: Optional[str] = None,
     libraries: Optional[List[str]] = None,
-) -> None:
+) -> None:  # pragma: no cover
     """Delete libraries from pystore.
 
     Parameters
     ----------
     conn : PystoreConnector, optional
         PystoreConnector object
     path : str, optional
@@ -61,15 +61,15 @@
 
 
 def delete_arctic_connector(
     conn=None,
     connstr: Optional[str] = None,
     name: Optional[str] = None,
     libraries: Optional[List[str]] = None,
-) -> None:
+) -> None:  # pragma: no cover
     """Delete libraries from arctic database.
 
     Parameters
     ----------
     conn : pastastore.ArcticConnector
         ArcticConnector object
     connstr : str, optional
@@ -106,14 +106,75 @@
         arc.delete_library(lib)
         if libraries is not None:
             print()
             print(f" - deleted: {lib}")
     print("Done!")
 
 
+def delete_arcticdb_connector(
+    conn=None,
+    uri: Optional[str] = None,
+    name: Optional[str] = None,
+    libraries: Optional[List[str]] = None,
+) -> None:
+    """Delete libraries from arcticDB database.
+
+    Parameters
+    ----------
+    conn : pastastore.ArcticDBConnector
+        ArcticDBConnector object
+    uri : str, optional
+        uri connection string to the database
+    name : str, optional
+        name of the database
+    libraries : Optional[List[str]], optional
+        list of library names to delete, by default None which deletes
+        all libraries
+    """
+    import shutil
+
+    import arcticdb
+
+    if conn is not None:
+        name = conn.name
+        uri = conn.uri
+    elif name is None or uri is None:
+        raise ValueError("Provide 'name' and 'uri' OR 'conn'!")
+
+    arc = arcticdb.Arctic(uri)
+
+    print(f"Deleting ArcticDBConnector database: '{name}' ... ", end="")
+    # get library names
+    if libraries is None:
+        libs = []
+        for ilib in arc.list_libraries():
+            if ilib.split(".")[0] == name:
+                # TODO: remove replace when arcticdb is able to delete
+                libs.append(ilib.replace(".", "/"))
+    elif name is not None:
+        # TODO: replace / with . when arcticdb is able to delete
+        libs = [name + "/" + ilib for ilib in libraries]
+    else:
+        raise ValueError("Provide 'name' and 'uri' OR 'conn'!")
+
+    for lib in libs:
+        # arc.delete_library(lib)  # TODO: not working at the moment.
+        shutil.rmtree(os.path.join(conn.uri.split("//")[-1], lib))
+
+        if libraries is not None:
+            print()
+            print(f" - deleted: {lib}")
+
+    remaining = [ilib for ilib in arc.list_libraries() if ilib.split(".") == name]
+    if len(remaining) == 0:
+        shutil.rmtree(os.path.join(conn.uri.split("//")[-1], name))
+
+    print("Done!")
+
+
 def delete_dict_connector(conn, libraries: Optional[List[str]] = None) -> None:
     print(f"Deleting DictConnector: '{conn.name}' ... ", end="")
     if libraries is None:
         del conn
         print(" Done!")
     else:
         for lib in libraries:
@@ -163,14 +224,16 @@
     """
     if pstore.conn.conn_type == "pystore":
         delete_pystore_connector(conn=pstore.conn, libraries=libraries)
     elif pstore.conn.conn_type == "dict":
         delete_dict_connector(pstore)
     elif pstore.conn.conn_type == "arctic":
         delete_arctic_connector(conn=pstore.conn, libraries=libraries)
+    elif pstore.conn.conn_type == "arcticdb":
+        delete_arcticdb_connector(conn=pstore.conn, libraries=libraries)
     elif pstore.conn.conn_type == "pas":
         delete_pas_connector(conn=pstore.conn, libraries=libraries)
     else:
         raise TypeError(
             "Unrecognized pastastore Connector type: " f"{pstore.conn.conn_type}"
         )
```

### Comparing `pastastore-1.1.0/pastastore/yaml_interface.py` & `pastastore-1.2.0/pastastore/yaml_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import logging
 import os
 from copy import deepcopy
 from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
@@ -29,16 +30,20 @@
             _convert_dict_dtypes_for_yaml(v)
         elif isinstance(v, list) and k == "stress":
             for iv in v:
                 if isinstance(iv, dict):
                     _convert_dict_dtypes_for_yaml(iv)
         elif isinstance(v, pd.Timestamp):
             d[k] = v.strftime("%Y-%m-%d %H:%M:%S")
+        elif isinstance(v, datetime.datetime):
+            d[k] = pd.to_datetime(v).strftime("%Y-%m-%d %H:%M:%S")
         elif isinstance(v, pd.Timedelta):
             d[k] = v.to_timedelta64().__str__()
+        elif isinstance(v, datetime.timedelta):
+            d[k] = pd.to_timedelta(v).to_timedelta64().__str__()
         elif isinstance(v, np.int64):
             d[k] = int(v)
         elif isinstance(v, np.float64):
             d[k] = float(v)
         elif isinstance(v, pd.DataFrame):
             d[k] = v.reset_index().to_dict(orient="records")
 
@@ -469,14 +474,122 @@
                 "  | no 'up' provided, set to 'False', "
                 "(i.e. pumping rate is positive for extraction)."
             )
             d["up"] = False
 
         return d
 
+    def construct_mldict(self, mlyml: dict, mlnam: str) -> dict:
+        # get oseries + metadata
+        if isinstance(mlyml["oseries"], dict):
+            onam = str(mlyml["oseries"]["name"])
+            _ = mlyml.pop("oseries")
+        else:
+            onam = str(mlyml.pop("oseries"))
+
+        logger.info(f"Building model '{mlnam}' for oseries '{onam}'")
+        o, ometa = self.pstore.get_oseries(onam, return_metadata=True)
+
+        # create model to obtain default model settings
+        ml = ps.Model(o, name=mlnam, metadata=ometa)
+        mldict = ml.to_dict(series=True)
+
+        # update with stored model settings
+        if "settings" in mlyml:
+            mldict["settings"].update(mlyml["settings"])
+
+        # stressmodels
+        for smnam, smyml in mlyml["stressmodels"].items():
+            # set name if not provided
+            if smyml is not None:
+                name = smyml.get("name", smnam)
+            else:
+                name = smnam
+            logger.info(f"| parsing stressmodel: '{name}'")
+
+            # check whether smtyp is defined
+            classkey = "stressmodel" if PASTAS_LEQ_022 else "class"
+            if smyml is not None:
+                if PASTAS_LEQ_022:
+                    if "class" in smyml:
+                        smyml["stressmodel"] = smyml.pop("class")
+                if classkey in smyml:
+                    smtyp = True
+                else:
+                    smtyp = False
+            else:
+                smtyp = False
+
+            # check if RechargeModel based on name if smtyp not defined
+            if (
+                smnam.lower() in ["rch", "rech", "recharge", "rechargemodel"]
+            ) and not smtyp:
+                logger.info("| assuming RechargeModel based on stressmodel name.")
+                # check if stressmodel dictionary is empty, create (nearly
+                # empty) dict so defaults are used
+                if smyml is None:
+                    mlyml["stressmodels"][smnam] = {"name": "recharge"}
+                    smyml = mlyml["stressmodels"][smnam]
+                if "name" not in smyml:
+                    smyml["name"] = smnam
+                smtyp = smyml.get(classkey, "RechargeModel")
+            else:
+                # if no info is provided, raise error,
+                # cannot make any assumptions for non-RechargeModels
+                if smyml is None:
+                    raise ValueError(
+                        "Insufficient information " f"for stressmodel '{name}'!"
+                    )
+                # get stressmodel type, with default StressModel
+                if classkey in smyml:
+                    smtyp = smyml[classkey]
+                else:
+                    logger.info(
+                        "| no stressmodel class type provided, " "using 'StressModel'"
+                    )
+                    smtyp = "StressModel"
+
+            # parse dictionary based on smtyp
+            if smtyp in ["RechargeModel", "TarsoModel"]:
+                # parse RechargeModel
+                sm = self._parse_rechargemodel_dict(smyml, onam=onam)
+
+                # turn off constant for TarsoModel
+                if smtyp == "TarsoModel":
+                    mldict["constant"] = False
+            elif smtyp == "StressModel":
+                # parse StressModel
+                sm = self._parse_stressmodel_dict(smyml, onam=onam)
+            elif smtyp == "WellModel":
+                # parse WellModel
+                sm = self._parse_wellmodel_dict(smyml, onam=onam)
+            else:
+                raise NotImplementedError(
+                    "PastaStore.yaml interface does " f"not (yet) support '{smtyp}'!"
+                )
+
+            # add to list
+            smyml.update(sm)
+
+        # update model dict w/ default settings with loaded data
+        mldict.update(mlyml)
+
+        # add name to dictionary if not already present
+        if "name" not in mldict:
+            mldict["name"] = mlnam
+
+        # convert warmup and time_offset to panads.Timedelta
+        if "warmup" in mldict["settings"]:
+            mldict["settings"]["warmup"] = pd.Timedelta(mldict["settings"]["warmup"])
+        if "time_offset" in mldict["settings"]:
+            mldict["settings"]["time_offset"] = pd.Timedelta(
+                mldict["settings"]["time_offset"]
+            )
+        return mldict
+
     def load(self, fyaml: str) -> List[ps.Model]:
         """Load Pastas YAML file.
 
         Note: currently supports RechargeModel, StressModel and WellModel.
 
         Parameters
         ----------
@@ -500,123 +613,15 @@
             yml = yaml.load(f, Loader=yaml.CFullLoader)
 
         models = []
 
         for mlnam in yml.keys():
             mlyml = yml[mlnam]
 
-            # get oseries + metadata
-            if isinstance(mlyml["oseries"], dict):
-                onam = str(mlyml["oseries"]["name"])
-                _ = mlyml.pop("oseries")
-            else:
-                onam = str(mlyml.pop("oseries"))
-
-            logger.info(f"Building model '{mlnam}' for oseries '{onam}'")
-            o, ometa = self.pstore.get_oseries(onam, return_metadata=True)
-
-            # create model to obtain default model settings
-            ml = ps.Model(o, name=mlnam, metadata=ometa)
-            mldict = ml.to_dict(series=True)
-
-            # update with stored model settings
-            if "settings" in mlyml:
-                mldict["settings"].update(mlyml["settings"])
-
-            # stressmodels
-            for smnam, smyml in mlyml["stressmodels"].items():
-                # set name if not provided
-                if smyml is not None:
-                    name = smyml.get("name", smnam)
-                else:
-                    name = smnam
-                logger.info(f"| parsing stressmodel: '{name}'")
-
-                # check whether smtyp is defined
-                classkey = "stressmodel" if PASTAS_LEQ_022 else "class"
-                if smyml is not None:
-                    if PASTAS_LEQ_022:
-                        if "class" in smyml:
-                            smyml["stressmodel"] = smyml.pop("class")
-                    if classkey in smyml:
-                        smtyp = True
-                    else:
-                        smtyp = False
-                else:
-                    smtyp = False
-
-                # check if RechargeModel based on name if smtyp not defined
-                if (
-                    smnam.lower() in ["rch", "rech", "recharge", "rechargemodel"]
-                ) and not smtyp:
-                    logger.info("| assuming RechargeModel based on stressmodel name.")
-                    # check if stressmodel dictionary is empty, create (nearly
-                    # empty) dict so defaults are used
-                    if smyml is None:
-                        mlyml["stressmodels"][smnam] = {"name": "recharge"}
-                        smyml = mlyml["stressmodels"][smnam]
-                    if "name" not in smyml:
-                        smyml["name"] = smnam
-                    smtyp = smyml.get(classkey, "RechargeModel")
-                else:
-                    # if no info is provided, raise error,
-                    # cannot make any assumptions for non-RechargeModels
-                    if smyml is None:
-                        raise ValueError(
-                            "Insufficient information " f"for stressmodel '{name}'!"
-                        )
-                    # get stressmodel type, with default StressModel
-                    if classkey in smyml:
-                        smtyp = smyml[classkey]
-                    else:
-                        logger.info(
-                            "| no stressmodel class type provided, "
-                            "using 'StressModel'"
-                        )
-                        smtyp = "StressModel"
-
-                # parse dictionary based on smtyp
-                if smtyp in ["RechargeModel", "TarsoModel"]:
-                    # parse RechargeModel
-                    sm = self._parse_rechargemodel_dict(smyml, onam=onam)
-
-                    # turn off constant for TarsoModel
-                    if smtyp == "TarsoModel":
-                        mldict["constant"] = False
-                elif smtyp == "StressModel":
-                    # parse StressModel
-                    sm = self._parse_stressmodel_dict(smyml, onam=onam)
-                elif smtyp == "WellModel":
-                    # parse WellModel
-                    sm = self._parse_wellmodel_dict(smyml, onam=onam)
-                else:
-                    raise NotImplementedError(
-                        "PastaStore.yaml interface does "
-                        f"not (yet) support '{smtyp}'!"
-                    )
-
-                # add to list
-                smyml.update(sm)
-
-            # update model dict w/ default settings with loaded data
-            mldict.update(mlyml)
-
-            # add name to dictionary if not already present
-            if "name" not in mldict:
-                mldict["name"] = mlnam
-
-            # convert warmup and time_offset to panads.Timedelta
-            if "warmup" in mldict["settings"]:
-                mldict["settings"]["warmup"] = pd.Timedelta(
-                    mldict["settings"]["warmup"]
-                )
-            if "time_offset" in mldict["settings"]:
-                mldict["settings"]["time_offset"] = pd.Timedelta(
-                    mldict["settings"]["time_offset"]
-                )
+            mldict = self.construct_mldict(mlyml, mlnam)
 
             # load model
             ml = ps.io.base._load_model(mldict)
             models.append(ml)
 
         return models
```

### Comparing `pastastore-1.1.0/pastastore.egg-info/PKG-INFO` & `pastastore-1.2.0/pastastore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastastore
-Version: 1.1.0
+Version: 1.2.0
 Summary: Tools for managing Pastas time series models.
 Author: D.A. Brakenhoff
 Maintainer-email: "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 D.A. Brakenhoff
         
@@ -49,14 +49,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: optional
 Provides-Extra: test
 Provides-Extra: pystore
 Provides-Extra: arctic
+Provides-Extra: arcticdb
 Provides-Extra: docs
 License-File: LICENSE
 
 ![pastastore](https://github.com/pastas/pastastore/workflows/pastastore/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/pastastore/badge/?version=latest)](https://pastastore.readthedocs.io/en/latest/?badge=latest)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/81b1e0294f5247cfa4eca657a8eebc61)](https://www.codacy.com/gh/pastas/pastastore?utm_source=github.com&utm_medium=referral&utm_content=pastas/pastastore&utm_campaign=Badge_Grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/81b1e0294f5247cfa4eca657a8eebc61)](https://www.codacy.com/gh/pastas/pastastore/dashboard?utm_source=github.com&utm_medium=referral&utm_content=pastas/pastastore&utm_campaign=Badge_Coverage)
@@ -113,14 +114,15 @@
 
 Now the user can add time series, models or analyze or visualize existing
 objects in the database. Some examples showing the functionality of the
 PastaStore object are shown below:
 
 ```python
 import pandas as pd
+import pastas as ps
 
 # load oseries from CSV and add to database
 oseries = pd.read_csv("oseries.csv")
 pstore.add_oseries(oseries, "my_oseries", metadata={"x": 100_000, "y": 400_000})
 
 # read oseries from database
 oseries = pstore.get_oseries("my_oseries")
@@ -132,15 +134,14 @@
 ax = pstore.maps.oseries()
 pstore.maps.add_background_map(ax)  # add a background map
 
 # plot my_oseries time series
 ax2 = pstore.plot.oseries(names=["my_oseries"])
 
 # create a model with pastas
-import pastas as ps
 ml = ps.Model(oseries, name="my_model")
 
 # add model to database
 pstore.add_model(ml)
 
 # load model from database
 ml2 = pstore.get_models("my_model")
```

### Comparing `pastastore-1.1.0/pastastore.egg-info/SOURCES.txt` & `pastastore-1.2.0/pastastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastastore-1.1.0/pyproject.toml` & `pastastore-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -43,28 +43,31 @@
 repository = "https://github.com/pastas/pastastore"
 documentation = "https://pastastore.readthedocs.io/en/latest/"
 
 [project.optional-dependencies]
 lint = ["black", "flake8", "isort"]
 optional = ["contextily", "pyproj", "adjustText"]
 test = [
-    "pastastore[lint,optional]",
+    "pastastore[arcticdb,lint,optional]",
     "hydropandas",
     "coverage",
     "codecov",
     "pytest",
     "pytest-cov",
     "pytest-dependency",
     "pytest-benchmark",
     "codacy-coverage",
 ]
 pystore = ["fsspec>=0.3.3", "python-snappy", "dask[dataframe]"]
 arctic = [
     "arctic", # will not work as releases not uploaded to PyPI
 ]
+arcticdb = [
+    "arcticdb",
+]
 docs = [
     "pastastore[optional]",
     "sphinx_rtd_theme",
     "Ipython",
     "ipykernel",
     "nbsphinx",
     "nbsphinx_link",
```

### Comparing `pastastore-1.1.0/readme.md` & `pastastore-1.2.0/readme.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
 Now the user can add time series, models or analyze or visualize existing
 objects in the database. Some examples showing the functionality of the
 PastaStore object are shown below:
 
 ```python
 import pandas as pd
+import pastas as ps
 
 # load oseries from CSV and add to database
 oseries = pd.read_csv("oseries.csv")
 pstore.add_oseries(oseries, "my_oseries", metadata={"x": 100_000, "y": 400_000})
 
 # read oseries from database
 oseries = pstore.get_oseries("my_oseries")
@@ -74,15 +75,14 @@
 ax = pstore.maps.oseries()
 pstore.maps.add_background_map(ax)  # add a background map
 
 # plot my_oseries time series
 ax2 = pstore.plot.oseries(names=["my_oseries"])
 
 # create a model with pastas
-import pastas as ps
 ml = ps.Model(oseries, name="my_model")
 
 # add model to database
 pstore.add_model(ml)
 
 # load model from database
 ml2 = pstore.get_models("my_model")
```

### Comparing `pastastore-1.1.0/tests/test_002_connectors.py` & `pastastore-1.2.0/tests/test_002_connectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     import pastastore as pst
 
 ps.set_log_level("ERROR")
 
 
 def test_get_library(conn):
     olib = conn._get_library("oseries")
-    return
 
 
 def test_add_get_series(request, conn):
     o1 = pd.Series(
         index=pd.date_range("2000", periods=10, freq="D"),
         data=1.0,
         dtype=np.float64,
@@ -31,15 +30,14 @@
     if conn.conn_type == "pas":
         o2 = o2.squeeze()
     try:
         assert isinstance(o2, pd.Series)
         assert (o1 == o2).all()
     finally:
         conn.del_oseries("test_series")
-    return
 
 
 def test_add_get_series_wnans(request, conn):
     o1 = pd.Series(
         index=pd.date_range("2000", periods=10, freq="D"),
         data=1.0,
         dtype=np.float64,
@@ -52,15 +50,14 @@
     if conn.conn_type == "pas":
         o2 = o2.squeeze()
     try:
         assert isinstance(o2, pd.Series)
         assert o1.equals(o2)
     finally:
         conn.del_oseries("test_series_nans")
-    return
 
 
 def test_add_get_dataframe(request, conn):
     o1 = pd.DataFrame(
         data=1.0,
         columns=["test_df"],
         index=pd.date_range("2000", periods=10, freq="D"),
@@ -70,30 +67,28 @@
     o2 = conn.get_oseries("test_df")
     try:
         assert isinstance(o2, pd.DataFrame)
         # little hack as PasConnector has dtype int after load...
         assert o1.equals(o2.astype(float))
     finally:
         conn.del_oseries("test_df")
-    return
 
 
 def test_add_pastas_timeseries(request, conn):
     o1 = pd.DataFrame(
         data=1.0,
         columns=["test_df"],
         index=pd.date_range("2000", periods=10, freq="D"),
     )
     o1.index.name = "test_idx"
     ts = ps.timeseries.TimeSeries(o1, metadata={"x": 100000.0, "y": 400000.0})
     try:
         conn.add_oseries(ts, "test_pastas_ts", metadata=None)
     except DeprecationWarning:
         pass
-    return
 
 
 def test_update_series(request, conn):
     o1 = pd.DataFrame(
         data=1.0,
         columns=["test_df"],
         index=pd.date_range("2000", periods=10, freq="D"),
@@ -109,15 +104,14 @@
     conn.update_oseries(o2, "test_df", metadata={"x": 200000.0, "y": 400000})
     o3 = conn.get_oseries("test_df")
     try:
         assert (o3.iloc[-2:] == 2.0).all().all()
         assert o3.index.size == 11
     finally:
         conn.del_oseries("test_df")
-    return
 
 
 def test_upsert_oseries(request, conn):
     o1 = pd.DataFrame(
         data=1.0,
         columns=["test_df"],
         index=pd.date_range("2000", periods=10, freq="D"),
@@ -133,15 +127,14 @@
     conn.upsert_oseries(o2, "test_df", metadata={"x": 200000.0, "y": 400000})
     o3 = conn.get_oseries("test_df")
     try:
         assert (o3.iloc[-10:] == 2.0).all().all()
         assert o3.index.size == 14
     finally:
         conn.del_oseries("test_df")
-    return
 
 
 def test_upsert_stress(request, conn):
     s1 = pd.DataFrame(
         data=1.0,
         columns=["test_df"],
         index=pd.date_range("2000", periods=10, freq="D"),
@@ -163,15 +156,14 @@
     s3 = conn.get_stresses("test_df")
     try:
         assert (s3.iloc[-10:] == 2.0).all().all()
         assert s3.index.size == 14
         assert conn.stresses.loc["test_df", "kind"] == "not useless"
     finally:
         conn.del_stress("test_df")
-    return
 
 
 def test_update_metadata(request, conn):
     o1 = pd.DataFrame(
         data=1.1,
         columns=["test_df"],
         index=pd.date_range("2000", periods=10, freq="D"),
@@ -183,123 +175,109 @@
     m = conn._get_metadata("oseries", "test_df")
     try:
         assert isinstance(m, dict)
         assert m["x"] == 200000.0
         assert m["y"] == 400000.0
     finally:
         conn.del_oseries("test_df")
-    return
 
 
 @pytest.mark.dependency()
 def test_add_oseries(conn):
     o = pd.read_csv("./tests/data/obs.csv", index_col=0, parse_dates=True)
     conn.add_oseries(
         o,
         "oseries1",
         metadata={"name": "oseries1", "x": 100000, "y": 400000},
         overwrite=True,
     )
-    return
 
 
 @pytest.mark.dependency()
 def test_add_stress(conn):
     s = pd.read_csv("./tests/data/rain.csv", index_col=0, parse_dates=True)
     conn.add_stress(
         s,
         "prec",
         kind="prec",
         metadata={"kind": "prec", "x": 100001, "y": 400001},
     )
-    return
 
 
 @pytest.mark.dependency()
 def test_get_oseries(request, conn):
     depends(request, [f"test_add_oseries[{conn.type}]"])
     o = conn.get_oseries("oseries1")
-    return
 
 
 @pytest.mark.dependency()
 def test_get_oseries_and_metadata(request, conn):
     depends(request, [f"test_add_oseries[{conn.type}]"])
     o, m = conn.get_oseries("oseries1", return_metadata=True)
-    return
 
 
 @pytest.mark.dependency()
 def test_get_stress(request, conn):
     depends(request, [f"test_add_stress[{conn.type}]"])
     s = conn.get_stresses("prec")
     s.name = "prec"
-    return
 
 
 @pytest.mark.dependency()
 def test_get_stress_and_metadata(request, conn):
     depends(request, [f"test_add_stress[{conn.type}]"])
     s, m = conn.get_stresses("prec", return_metadata=True)
     s.name = "prec"
-    return
 
 
 @pytest.mark.dependency()
 def test_oseries_prop(request, conn):
     depends(request, [f"test_add_oseries[{conn.type}]"])
     conn.oseries
-    return
 
 
 @pytest.mark.dependency()
 def test_stresses_prop(request, conn):
     depends(request, [f"test_add_stress[{conn.type}]"])
     conn.stresses
-    return
 
 
 def test_repr(conn):
     conn.__repr__()
-    return
 
 
 @pytest.mark.dependency()
 def test_del_oseries(request, conn):
     depends(request, [f"test_add_oseries[{conn.type}]"])
     conn.del_oseries("oseries1")
-    return
 
 
 @pytest.mark.dependency()
 def test_del_stress(request, conn):
     depends(request, [f"test_add_stress[{conn.type}]"])
     conn.del_stress("prec")
-    return
 
 
 @pytest.mark.dependency()
 def test_empty_library(request, conn):
     s1 = pd.Series(
         index=pd.date_range("2000", periods=10, freq="D"),
         data=1.0,
         dtype=np.float64,
     )
     s1.name = "test_series"
     conn.add_oseries(s1, "test_series", metadata=None)
     conn.empty_library("stresses", prompt=False, progressbar=False)
-    return
 
 
 @pytest.mark.dependency()
 def test_delete(request, conn):
     # no need to delete dictconnector (in memory)
     if conn.conn_type == "arctic":
         pst.util.delete_arctic_connector(conn, libraries=["oseries"])
         pst.util.delete_arctic_connector(conn)
     elif conn.conn_type == "pystore":
         pst.util.delete_pystore_connector(conn, libraries=["oseries"])
         pst.util.delete_pystore_connector(conn)
     elif conn.conn_type == "pas":
         pst.util.delete_pas_connector(conn, libraries=["oseries"])
         pst.util.delete_pas_connector(conn)
-    return
```

### Comparing `pastastore-1.1.0/tests/test_003_pastastore.py` & `pastastore-1.2.0/tests/test_003_pastastore.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,42 +12,37 @@
     warnings.simplefilter(action="ignore", category=FutureWarning)
     import pastastore as pst
 
 
 @pytest.mark.dependency()
 def test_iter_oseries(pstore):
     _ = list(pstore.iter_oseries())
-    return
 
 
 @pytest.mark.dependency()
 def test_iter_stresses(pstore):
     _ = list(pstore.iter_stresses())
-    return
 
 
 @pytest.mark.dependency()
 def test_get_tmintmax(pstore):
     _ = pstore.get_tmin_tmax("oseries")
     _ = pstore.get_tmin_tmax("stresses")
-    return
 
 
 @pytest.mark.dependency()
 def test_search(pstore):
     results = pstore.search("oseries", "OSER", case_sensitive=False)
     assert len(results) == 3
     assert len(set(results) - {"oseries1", "oseries2", "oseries3"}) == 0
-    return
 
 
 @pytest.mark.dependency()
 def test_create_model(pstore):
     ml = pstore.create_model("oseries1")
-    return
 
 
 @pytest.mark.dependency()
 def test_properties(pstore):
     pstore.add_oseries(pd.Series(dtype=np.float64), "deleteme", validate=False)
     pstore.add_stress(
         pd.Series(dtype=np.float64), "deleteme", kind="useless", validate=False
@@ -60,23 +55,20 @@
     try:
         assert pstore.n_oseries == pstore.conn.n_oseries
         assert pstore.n_stresses == pstore.conn.n_stresses
     finally:
         pstore.del_oseries("deleteme")
         pstore.del_stress("deleteme")
 
-    return
-
 
 @pytest.mark.dependency()
 def test_store_model(request, pstore):
     depends(request, [f"test_create_model[{pstore.type}]"])
     ml = pstore.create_model("oseries1")
     pstore.conn.add_model(ml)
-    return
 
 
 @pytest.mark.dependency()
 def test_model_accessor(request, pstore):
     depends(request, [f"test_store_model[{pstore.type}]"])
     # repr
     pstore.models.__repr__()
@@ -88,15 +80,14 @@
     mnames = [ml.name for ml in pstore.models]
     try:
         assert len(mnames) == 2
         assert mnames[0] in ["oseries1", "oseries1_2"]
         assert mnames[1] in ["oseries1", "oseries1_2"]
     finally:
         pstore.del_models("oseries1_2")
-    return
 
 
 @pytest.mark.dependency()
 def test_oseries_model_accessor(request, pstore):
     depends(request, [f"test_store_model[{pstore.type}]"])
     # repr
     pstore.oseries_models.__repr__()
@@ -110,15 +101,14 @@
     ml_list2 = pstore.oseries_models["oseries1"]
     assert len(ml_list2) == 2
 
     # delete model
     pstore.del_models("oseries1_2")
     ml_list3 = pstore.oseries_models["oseries1"]
     assert len(ml_list3) == 1
-    return
 
 
 @pytest.mark.dependency()
 def test_store_model_missing_series(request, pstore):
     depends(
         request,
         [
@@ -132,80 +122,73 @@
     pstore.del_models("oseries1")
     pstore.del_oseries("oseries1")
     try:
         pstore.add_model(ml)
     except LookupError:
         pstore.add_oseries(o, "oseries1", metadata=meta)
         pstore.add_model(ml)
-        return
 
 
 @pytest.mark.dependency()
 def test_get_model(request, pstore):
     depends(
         request,
         [
             f"test_create_model[{pstore.type}]",
             f"test_store_model[{pstore.type}]",
             f"test_store_model_missing_series[{pstore.type}]",
         ],
     )
     ml = pstore.conn.get_models("oseries1")
-    return
 
 
 @pytest.mark.dependency()
 def test_del_model(request, pstore):
     depends(
         request,
         [
             f"test_create_model[{pstore.type}]",
             f"test_store_model[{pstore.type}]",
             f"test_store_model_missing_series[{pstore.type}]",
             f"test_get_model[{pstore.type}]",
         ],
     )
     pstore.conn.del_models("oseries1")
-    return
 
 
 @pytest.mark.dependency()
 def test_create_models(pstore):
     mls = pstore.create_models_bulk(
         ["oseries1", "oseries2"], store=True, progressbar=False
     )
     _ = pstore.conn.models
-    return
 
 
 @pytest.mark.dependency()
 def test_get_parameters(request, pstore):
     depends(request, [f"test_create_models[{pstore.type}]"])
     p = pstore.get_parameters(progressbar=False, param_value="initial")
     assert p.index.size == 2
     assert p.isna().sum().sum() == 0
-    return
 
 
 @pytest.mark.dependency()
 def test_iter_models(request, pstore):
     depends(request, [f"test_create_models[{pstore.type}]"])
     _ = list(pstore.iter_models())
-    return
 
 
 @pytest.mark.dependency()
 def test_solve_models_and_get_stats(request, pstore):
     depends(request, [f"test_create_models[{pstore.type}]"])
     mls = pstore.solve_models(
         ignore_solve_errors=False, progressbar=False, store_result=True
     )
     stats = pstore.get_statistics(["evp", "aic"], progressbar=False)
     assert stats.index.size == 2
-    return
 
 
 @pytest.mark.dependency()
 def test_save_and_load_model(request, pstore):
     ml = pstore.create_model("oseries2")
     sm = ps.StressModel(
         pstore.get_stresses("well1"), ps.Gamma(), name="well1", settings="well"
@@ -214,15 +197,14 @@
     ml.solve(tmin="1993-1-1")
     evp_ml = ml.stats.evp()
     pstore.add_model(ml, overwrite=True)
     ml2 = pstore.get_models(ml.name)
     evp_ml2 = ml2.stats.evp()
     assert allclose(evp_ml, evp_ml2)
     assert pst.util.compare_models(ml, ml2)
-    return
 
 
 def test_update_ts_settings(request, pstore):
     pstore.set_check_model_series_values(False)
 
     o = pstore.get_oseries("oseries2")
     ml = ps.Model(o.loc[:"2013"], name="ml_oseries2")
@@ -248,58 +230,53 @@
         assert ml2.stressmodels["recharge"].prec.settings["tmax"] == tmax
         assert ml2.stressmodels["recharge"].evap.settings["tmax"] == tmax
         assert ml2.stressmodels["prec"].stress[0].settings["tmax"] == p2.index[-1]
     except AssertionError:
         pstore.del_models("ml_oseries2")
         pstore.set_check_model_series_values(True)
         raise
-    return
 
 
 # @pytest.mark.dependency()
 # def test_model_results(request, pstore):
 #     depends(request, [f"test_create_models[{pstore.type}]",
 #                       f"test_solve_models[{pstore.type}]"])
 #     pstore.model_results(["oseries1", "oseries2"], progressbar=False)
-#     return
 
 
 def test_oseries_distances(pstore):
     _ = pstore.get_nearest_oseries()
-    return
 
 
 def test_repr(pstore):
     pstore.__repr__()
-    return
 
 
 def test_copy_dbase(pstore):
     conn2 = pst.DictConnector("destination")
     pst.util.copy_database(pstore.conn, conn2, overwrite=False, progressbar=True)
-    return
 
 
 def test_to_from_zip(pstore):
     zipname = f"test_{pstore.type}.zip"
+    if pstore.type == "arcticdb":
+        pytest.xfail("model datetime objects not supported")
     pstore.to_zip(zipname, progressbar=False, overwrite=True)
     conn = pst.DictConnector("test")
     try:
         store = pst.PastaStore.from_zip(zipname, conn)
         assert not store.oseries.empty
     finally:
         os.remove(zipname)
-    return
 
 
 def test_example_pastastore():
     from pastastore.datasets import example_pastastore
 
     _ = example_pastastore()
-    return
 
 
 def test_validate_names():
     from pastastore.util import validate_names
 
     validate_names(s="(test)") == "test"
     validate_names(d={"(test)": 2})["test"]
```

### Comparing `pastastore-1.1.0/tests/test_004_yaml.py` & `pastastore-1.2.0/tests/test_004_yaml.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,14 @@
           evap: evap2                 # name of evaporation stress, obtained from pastastore
           recharge: Linear            # pastas recharge type
           rfunc: Exponential          # response function
     """
     with tempyaml(yamlstr) as f:
         ml = pstore.yaml.load(f)[0]
     pstore.add_model(ml)
-    return
 
 
 @pytest.mark.dependency()
 def test_load_yaml_stressmodel(pstore):
     yamlstr = """
     my_second_model:                  # model name
       oseries: oseries2               # head time series name, obtained from pastastore
@@ -49,15 +48,14 @@
           class: StressModel          # type of pastas StressModel
           stress: prec2               # name of precipitation stress, obtained from pastastore
           rfunc: Gamma                # response function
     """
     with tempyaml(yamlstr) as f:
         ml = pstore.yaml.load(f)[0]
     pstore.add_model(ml)
-    return
 
 
 @pytest.mark.dependency()
 def test_load_yaml_wellmodel(pstore):
     yamlstr = """
     my_third_model:                   # model name
       oseries: oseries1               # head time series name, obtained from pastastore
@@ -67,15 +65,14 @@
           stress: well1               # name of well stress, obtained from pastastore
           distances: [100]
 
     """
     with tempyaml(yamlstr) as f:
         ml = pstore.yaml.load(f)[0]
     pstore.add_model(ml)
-    return
 
 
 @pytest.mark.dependency()
 def test_write_load_compare_yaml(request, pstore):
     depends(
         request,
         [
@@ -87,15 +84,14 @@
     pstore.yaml.export_models(modelnames=["my_first_model"])
     ml1 = pstore.models["my_first_model"]
     ml2 = pstore.yaml.load("my_first_model.yaml")[0]
     assert (
         pst.util.compare_models(ml1, ml2, detailed_comparison=True).iloc[1:, -1].all()
     )
     os.remove("my_first_model.yaml")
-    return
 
 
 @pytest.mark.dependency()
 def test_write_yaml_per_oseries(request, pstore):
     depends(
         request,
         [
@@ -103,15 +99,14 @@
             f"test_load_yaml_stressmodel[{pstore.type}]",
             f"test_load_yaml_wellmodel[{pstore.type}]",
         ],
     )
     pstore.yaml.export_stored_models_per_oseries()
     os.remove("oseries1.yaml")
     os.remove("oseries2.yaml")
-    return
 
 
 @pytest.mark.dependency()
 def test_write_yaml_minimal(request, pstore):
     depends(
         request,
         [
@@ -119,15 +114,14 @@
             f"test_load_yaml_stressmodel[{pstore.type}]",
             f"test_load_yaml_wellmodel[{pstore.type}]",
         ],
     )
     ml = pstore.models["my_first_model"]
     pstore.yaml.export_model(ml, minimal_yaml=True)
     os.remove("my_first_model.yaml")
-    return
 
 
 @pytest.mark.dependency()
 def test_write_yaml_minimal_nearest(request, pstore):
     depends(
         request,
         [
@@ -135,8 +129,7 @@
             f"test_load_yaml_stressmodel[{pstore.type}]",
             f"test_load_yaml_wellmodel[{pstore.type}]",
         ],
     )
     ml = pstore.models["my_third_model"]
     pstore.yaml.export_model(ml, minimal_yaml=True, use_nearest=True)
     os.remove("my_third_model.yaml")
-    return
```

### Comparing `pastastore-1.1.0/tests/test_005_maps_plots.py` & `pastastore-1.2.0/tests/test_005_maps_plots.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.1.0/tests/test_006_benchmark.py` & `pastastore-1.2.0/tests/test_006_benchmark.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,89 +17,98 @@
     conn.add_oseries(s, "oseries1", metadata=metadata, overwrite=True)
 
 
 # @pytest.mark.benchmark(group="write_series")
 # def test_benchmark_write_series_dict(benchmark):
 #     conn = pst.DictConnector("test")
 #     _ = benchmark(series_write, conn=conn)
-#     return
 
 
 @pytest.mark.benchmark(group="write_series")
 def test_benchmark_write_series_pas(benchmark):
     conn = pst.PasConnector("test", "./tests/data/pas")
     _ = benchmark(series_write, conn=conn)
-    return
 
 
 @pytest.mark.benchmark(group="write_series")
 @requires_pkg("pystore")
 def test_benchmark_write_series_pystore(benchmark):
     path = "./tests/data/pystore"
     conn = pst.PystoreConnector("test", path)
     _ = benchmark(series_write, conn=conn)
-    return
 
 
 @pytest.mark.benchmark(group="write_series")
 @requires_pkg("arctic")
 def test_benchmark_write_series_arctic(benchmark):
     connstr = "mongodb://localhost:27017/"
     conn = pst.ArcticConnector("test", connstr)
     _ = benchmark(series_write, conn=conn)
-    return
+
+
+@pytest.mark.benchmark(group="write_series")
+@requires_pkg("arcticdb")
+def test_benchmark_write_series_arcticdb(benchmark):
+    uri = "lmdb://./arctic_db/"
+    conn = pst.ArcticDBConnector("test", uri)
+    _ = benchmark(series_write, conn=conn)
 
 
 # %% read
 
 
 def series_read(conn):
     _ = conn.get_oseries("oseries1")
 
 
 # @pytest.mark.benchmark(group="read_series")
 # def test_benchmark_write_series_dict(benchmark):
 #     conn = pst.DictConnector("test")
 #     _ = benchmark(series_read, conn=conn)
-#     return
+#
 
 
 @pytest.mark.benchmark(group="read_series")
 def test_benchmark_read_series_pas(benchmark):
     conn = pst.PasConnector("test", "./tests/data/pas")
     _ = benchmark(series_read, conn=conn)
-    return
 
 
 @pytest.mark.benchmark(group="read_series")
 @requires_pkg("pystore")
 def test_benchmark_read_series_pystore(benchmark):
     path = "./tests/data/pystore"
     conn = pst.PystoreConnector("test", path)
     _ = benchmark(series_read, conn=conn)
-    return
 
 
 @pytest.mark.benchmark(group="read_series")
 @requires_pkg("arctic")
 def test_benchmark_read_series_arctic(benchmark):
     connstr = "mongodb://localhost:27017/"
     conn = pst.ArcticConnector("test", connstr)
     _ = benchmark(series_read, conn=conn)
-    return
+
+
+@pytest.mark.benchmark(group="read_series")
+@requires_pkg("arcticdb")
+def test_benchmark_read_series_arcticdb(benchmark):
+    uri = "lmdb://./arctic_db/"
+    conn = pst.ArcticDBConnector("test", uri)
+    _ = benchmark(series_read, conn=conn)
 
 
 # %% write model
 
 
 def build_model(conn):
     store = pst.PastaStore(conn, "test")
 
     # oseries nb1
-    if "oseries_nb1" not in store.oseries.index:
+    if "oseries_nb1" not in store.oseries_names:
         o = pd.read_csv("./tests/data/head_nb1.csv", index_col=0, parse_dates=True)
         store.add_oseries(o, "oseries_nb1", metadata={"x": 100300, "y": 400400})
 
     # prec nb1
     if "prec_nb1" not in store.stresses.index:
         s = pd.read_csv("./tests/data/rain_nb1.csv", index_col=0, parse_dates=True)
         store.add_stress(
@@ -123,43 +132,48 @@
 
 
 # @pytest.mark.benchmark(group="write_model")
 # def test_benchmark_write_model_dict(benchmark):
 #     conn = pst.DictConnector("test")
 #     ml = build_model(conn)
 #     _ = benchmark(write_model, conn=conn, ml=ml)
-#     return
 
 
 @pytest.mark.benchmark(group="write_model")
 def test_benchmark_write_model_pas(benchmark):
     conn = pst.PasConnector("test", "./tests/data/pas")
     ml = build_model(conn)
     _ = benchmark(write_model, conn=conn, ml=ml)
-    return
 
 
 @pytest.mark.benchmark(group="write_model")
 @requires_pkg("pystore")
 def test_benchmark_write_model_pystore(benchmark):
     path = "./tests/data/pystore"
     conn = pst.PystoreConnector("test", path)
     ml = build_model(conn)
     _ = benchmark(write_model, conn=conn, ml=ml)
-    return
 
 
 @pytest.mark.benchmark(group="write_model")
 @requires_pkg("arctic")
 def test_benchmark_write_model_arctic(benchmark):
     connstr = "mongodb://localhost:27017/"
     conn = pst.ArcticConnector("test", connstr)
     ml = build_model(conn)
     _ = benchmark(write_model, conn=conn, ml=ml)
-    return
+
+
+@pytest.mark.benchmark(group="write_model")
+@requires_pkg("arcticdb")
+def test_benchmark_write_model_arcticdb(benchmark):
+    uri = "lmdb://./arctic_db/"
+    conn = pst.ArcticDBConnector("test", uri)
+    ml = build_model(conn)
+    _ = benchmark(write_model, conn=conn, ml=ml)
 
 
 # %%
 
 
 def write_model_nocheckts(conn, ml):
     conn.set_check_model_series_values(False)
@@ -167,71 +181,85 @@
 
 
 @pytest.mark.benchmark(group="write_model")
 def test_benchmark_write_model_nocheckts_pas(benchmark):
     conn = pst.PasConnector("test", "./tests/data/pas")
     ml = build_model(conn)
     _ = benchmark(write_model_nocheckts, conn=conn, ml=ml)
-    return
 
 
 @pytest.mark.benchmark(group="write_model")
 @requires_pkg("pystore")
 def test_benchmark_write_model_nocheckts_pystore(benchmark):
     path = "./tests/data/pystore"
     conn = pst.PystoreConnector("test", path)
     ml = build_model(conn)
     _ = benchmark(write_model_nocheckts, conn=conn, ml=ml)
-    return
 
 
 @pytest.mark.benchmark(group="write_model")
 @requires_pkg("arctic")
 def test_benchmark_write_model_nocheckts_arctic(benchmark):
     connstr = "mongodb://localhost:27017/"
     conn = pst.ArcticConnector("test", connstr)
     ml = build_model(conn)
     _ = benchmark(write_model_nocheckts, conn=conn, ml=ml)
-    return
+
+
+@pytest.mark.benchmark(group="write_model")
+@requires_pkg("arcticdb")
+def test_benchmark_write_model_nocheckts_arcticdb(benchmark):
+    uri = "lmdb://./arctic_db/"
+    conn = pst.ArcticDBConnector("test", uri)
+    ml = build_model(conn)
+    _ = benchmark(write_model_nocheckts, conn=conn, ml=ml)
 
 
 # %% read model
 
 
 def read_model(conn):
     ml = conn.get_models("oseries_nb1")
     return ml
 
 
 # @pytest.mark.benchmark(group="read_model")
 # def test_benchmark_read_model_dict(benchmark):
 #     conn = pst.DictConnector("test")
 #     _ = benchmark(read_model, conn=conn, ml=ml)
-#     return
 
 
 @pytest.mark.benchmark(group="read_model")
 def test_benchmark_read_model_pas(benchmark):
     conn = pst.PasConnector("test", "./tests/data/pas")
     _ = benchmark(read_model, conn=conn)
     pst.util.delete_pas_connector(conn)
-    return
 
 
 @pytest.mark.benchmark(group="read_model")
 @requires_pkg("pystore")
 def test_benchmark_read_model_pystore(benchmark):
     path = "./tests/data/pystore"
     conn = pst.PystoreConnector("test", path)
     _ = benchmark(read_model, conn=conn)
     pst.util.delete_pystore_connector(conn=conn)
-    return
 
 
 @pytest.mark.benchmark(group="read_model")
 @requires_pkg("arctic")
 def test_benchmark_read_model_arctic(benchmark):
     connstr = "mongodb://localhost:27017/"
     conn = pst.ArcticConnector("test", connstr)
     _ = benchmark(read_model, conn=conn)
     pst.util.delete_arctic_connector(conn=conn)
-    return
+
+
+@pytest.mark.benchmark(group="read_model")
+@requires_pkg("arcticdb")
+def test_benchmark_read_model_arcticdb(benchmark):
+    uri = "lmdb://./arctic_db/"
+    conn = pst.ArcticDBConnector("test", uri)
+    _ = benchmark(read_model, conn=conn)
+    pst.util.delete_arcticdb_connector(conn=conn)
+    import shutil
+
+    shutil.rmtree("./arctic_db/")
```

