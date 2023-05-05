# Comparing `tmp/pydiverse-pipedag-0.2.3.tar.gz` & `tmp/pydiverse-pipedag-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse-pipedag-0.2.3.tar", max compression
+gzip compressed data, was "pydiverse-pipedag-0.2.4.tar", max compression
```

## Comparing `pydiverse-pipedag-0.2.3.tar` & `pydiverse-pipedag-0.2.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1517 2022-08-30 10:19:17.882077 pydiverse-pipedag-0.2.3/LICENSE
--rw-r--r--   0        0        0     7028 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.3/docs/package/README.md
--rw-r--r--   0        0        0     2822 2023-04-17 10:30:00.401257 pydiverse-pipedag-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       13 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      204 2022-12-07 13:24:39.752944 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      749 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       61 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     5323 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0    10555 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/lock.py
--rw-r--r--   0        0        0      177 2022-08-30 10:19:17.886078 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    19418 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0     7232 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0    65364 2023-04-17 10:28:16.433476 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/sql.py
--rw-r--r--   0        0        0       45 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     1274 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
--rw-r--r--   0        0        0    40372 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
--rw-r--r--   0        0        0      342 2022-12-15 12:57:17.081298 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0     6241 2023-02-07 12:13:02.783303 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    24901 2023-04-17 10:28:16.433476 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      164 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0     9075 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     2512 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     5714 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     6308 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      285 2022-12-14 22:29:15.934795 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      648 2022-12-15 12:19:12.124658 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     6516 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1380 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0      124 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     8463 2023-04-17 10:28:16.433476 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0     4246 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0     7739 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2039 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    16598 2023-03-31 15:18:57.066051 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0       37 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/__init__.py
--rw-r--r--   0        0        0     1104 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/cache.py
--rw-r--r--   0        0        0     3647 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/json.py
--rw-r--r--   0        0        0      228 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0    14721 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/config.py
--rw-r--r--   0        0        0     2061 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1435 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      880 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1707 2022-12-15 13:01:08.984954 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     8982 2023-02-08 18:46:59.148930 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0      818 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     9052 2023-04-17 10:30:13.052195 pydiverse-pipedag-0.2.3/setup.py
--rw-r--r--   0        0        0     8954 2023-04-17 10:30:13.052739 pydiverse-pipedag-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1517 2022-08-30 10:19:17.882077 pydiverse-pipedag-0.2.4/LICENSE
+-rw-r--r--   0        0        0     7028 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.4/docs/package/README.md
+-rw-r--r--   0        0        0     3466 2023-05-05 12:50:21.019475 pydiverse-pipedag-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       13 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      204 2022-12-07 13:24:39.752944 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      749 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       61 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     5277 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0    10555 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/lock.py
+-rw-r--r--   0        0        0      177 2022-08-30 10:19:17.886078 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    19418 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0     7232 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0    79713 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/sql.py
+-rw-r--r--   0        0        0       45 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     1274 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
+-rw-r--r--   0        0        0    40345 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
+-rw-r--r--   0        0        0      342 2022-12-15 12:57:17.081298 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0     6241 2023-02-07 12:13:02.783303 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    25109 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      164 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0     9075 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     2512 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     5714 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     6308 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      285 2022-12-14 22:29:15.934795 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      648 2022-12-15 12:19:12.124658 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     6516 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1380 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0      124 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     8463 2023-04-17 10:28:16.433476 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0     4332 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0     7739 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2039 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    16598 2023-03-31 15:18:57.066051 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0       37 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/__init__.py
+-rw-r--r--   0        0        0     1104 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/cache.py
+-rw-r--r--   0        0        0     4231 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/json.py
+-rw-r--r--   0        0        0      228 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0    14721 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/config.py
+-rw-r--r--   0        0        0     2061 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1435 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      880 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1707 2022-12-15 13:01:08.984954 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     8982 2023-02-08 18:46:59.148930 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0      818 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     9297 2023-05-05 12:51:14.349947 pydiverse-pipedag-0.2.4/setup.py
+-rw-r--r--   0        0        0     9432 2023-05-05 12:51:14.350385 pydiverse-pipedag-0.2.4/PKG-INFO
```

### Comparing `pydiverse-pipedag-0.2.3/LICENSE` & `pydiverse-pipedag-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/docs/package/README.md` & `pydiverse-pipedag-0.2.4/docs/package/README.md`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/pyproject.toml` & `pydiverse-pipedag-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.2.3"
+version = "0.2.4"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
@@ -17,17 +17,17 @@
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "Programming Language :: SQL",
   "Topic :: Database",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-pandas = "^1.4.3"
-SQLAlchemy = "^1.4.39"
+python = ">=3.9, <3.11"  # currently, optional dependency tidypolars does not support python 3.11
+pandas = ">=1.4.3"
+SQLAlchemy = ">=1.4.39"
 typing-extensions = "<5, >=4.1.0"
 networkx = ">=2.8"
 attrs = ">=22.1.0"
 structlog = ">=22.1.0"
 tomli = ">=2.0.1"
 pynng = ">=0.7.1"
 msgpack = ">=1.0.4"
@@ -42,31 +42,42 @@
 sphinx-rtd-theme = { version = ">=1.0.0", optional = true }
 sphinxcontrib-apidoc = { version=">=0.3.0", optional = true }
 
 pyodbc = { version = ">=4.0.35", optional = true }
 pytsql = { version = ">=1.1.4", optional = true }
 ibm-db = { version = ">=3.1.4", optional = true }
 ibm-db-sa = { version = ">=0.3.8", optional = true }
+pydiverse-transform = { version = ">=0.1.1", optional = true }
+ibis = { version = ">=3.2.0", optional = true }
+ibis-framework = {extras = ["mssql", "postgres"], version = "^5.1.0", optional = true }
+tidypolars = { version = ">=0.2.19", optional = true }
+connectorx = { version=">=0.3.1", optional = true }
+pyarrow = { version=">=11.0.0", optional = true }
+polars = { version=">=0.16.18,<0.17", optional = true }
 prefect = { version = ">=1.3,<2", optional = true }
 # for prefect 2 (radical change of paradigmns especially in task graph display => not ideal for rather linear pipeline)
 # prefect = { version = "prefect>=2.0,<3", optional = true }
 
 [tool.poetry.extras]
 filelock = ["filelock"]
 zookeeper = ["kazoo"]
 docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-apidoc"]
 mssql = ["pyodbc", "pytsql"]
 ibm_db2 = ["ibm-db", "ibm-db-sa"]
+pdtransform = ["pydiverse-transform"]
+ibis = ["ibis", "ibis-framework"]
+polars = ["tidypolars", "polars", "connectorx", "pyarrow"]
 prefect = ["prefect", "docker-compose"]
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.2.0"
 pytest-mock = ">=3.10.0"
 pytest-timeout = ">=2.1.0"
-black = ">=22.6.0"
+black = "^23.3.0"
+isort = "^5.10.1"
 ruff = ">=0.0.189"
 pre-commit = ">=2.20.0"
 kazoo = ">=2.8.0"
 psycopg2 = ">=2.9.3"
 pydot = ">=1.4.2"
 setuptools = ">=65.6.3"
```

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/_typing.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/blob.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/blob.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import pickle
 import shutil
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from pydiverse.pipedag.context import ConfigContext
-from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.util import Disposable, normalize_name
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core import Stage
     from pydiverse.pipedag.materialize import Blob
 
 __all__ = [
@@ -132,15 +131,15 @@
     def copy_blob_to_transaction(self, blob: Blob):
         try:
             shutil.copy2(
                 self.get_blob_path(blob.stage.name, blob.name),
                 self.get_blob_path(blob.stage.transaction_name, blob.name),
             )
         except FileNotFoundError:
-            raise CacheError(
+            raise RuntimeError(
                 f"Can't copy blob '{blob.name}' (stage: '{blob.stage.name}')"
                 " to working transaction because no such blob exists."
             ) from None
 
     def delete_blob_from_transaction(self, blob: Blob):
         try:
             os.remove(self.get_blob_path(blob.stage.transaction_name, blob.name))
```

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/lock.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/lock.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/sql.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/sql.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 import re
 import textwrap
 import threading
 import time
 import traceback
 import warnings
 from collections.abc import Iterable
+from contextlib import contextmanager
 from typing import Any
 
 import pandas as pd
 import sqlalchemy as sa
 import sqlalchemy.exc
 import sqlalchemy.sql.elements
+from sqlalchemy.dialects.mssql import DATETIME2
 
 from pydiverse.pipedag import Stage, Table
 from pydiverse.pipedag.backend.table.base import BaseTableStore, TableHook
 from pydiverse.pipedag.backend.table.util import engine_dispatch
 from pydiverse.pipedag.backend.table.util.sql_ddl import (
     AddIndex,
     AddPrimaryKey,
@@ -120,18 +122,26 @@
         self.pytsql_isolate_top_level_statements = pytsql_isolate_top_level_statements
         self.print_materialize = print_materialize
         self.print_sql = print_sql
         self.no_db_locking = no_db_locking
         self.metadata_schema = self.get_schema(self.METADATA_SCHEMA)
 
         self._init_database(engine_url, create_database_if_not_exists)
+        self.engine_url_obj = sa.engine.make_url(engine_url)
+        self.engine_url_no_pw = repr(self.engine_url_obj)
         self.engine = self._connect(engine_url, self.schema_prefix, self.schema_suffix)
+        self.engines_other = dict()  # i.e. for IBIS connection
 
         # Set up metadata tables and schema
-        from sqlalchemy import BigInteger, Boolean, Column, DateTime, String
+        from sqlalchemy import CLOB, BigInteger, Boolean, Column, DateTime, String
+
+        if self.engine.dialect.name == "ibm_db_sa":
+            clob_type = CLOB  # VARCHAR(MAX) does not exist
+        else:
+            clob_type = String  # VARCHAR(MAX)s
 
         self.sql_metadata = sa.MetaData()
 
         # Stage Table is unique for stage
         # (we currently cannot version changes of this metadata table when using
         # stage_commit_tequnique=read_views)
         self.stage_table = sa.Table(
@@ -162,15 +172,15 @@
             Column("name", String(128)),
             Column("stage", String(64)),
             Column("version", String(64)),
             Column("timestamp", DateTime),
             Column("run_id", String(32)),
             Column("input_hash", String(32)),
             Column("cache_fn_hash", String(32)),
-            Column("output_json", String(2048)),  # 2k might be too small => TBD
+            Column("output_json", clob_type),
             Column("in_transaction_schema", Boolean),
             schema=self.metadata_schema.get(),
         )
 
         # Lazy Cache Table is unique for stage * in_transaction_schema
         self.lazy_cache_table = sa.Table(
             "lazy_tables",
@@ -194,14 +204,21 @@
             Column("stage", String(64)),
             Column("query_hash", String(32)),
             Column("task_hash", String(32)),
             Column("in_transaction_schema", Boolean),
             schema=self.metadata_schema.get(),
         )
 
+        self.logger.info(
+            "Initialized SQL Table Store",
+            engine_url=self.engine_url_no_pw,
+            schema_prefix=self.schema_prefix,
+            schema_suffix=self.schema_suffix,
+        )
+
     @staticmethod
     def _init_database(engine_url: str, create_database_if_not_exists: bool):
         if not create_database_if_not_exists:
             return
 
         engine = sa.create_engine(engine_url)
         if engine.dialect.name in ["mssql", "ibm_db_sa"]:
@@ -214,44 +231,46 @@
         #            if the database does not exist
         url = sa.engine.make_url(engine_url)
 
         if engine.dialect.name == "postgresql":
             try:
                 with engine.connect() as conn:
                     # try whether connection with database in connect string works
-                    conn.execute("SELECT 1")
+                    conn.execute(sa.text("SELECT 1"))
             except sa.exc.DBAPIError:
                 postgres_db_url = url.set(database="postgres")
                 tmp_engine = sa.create_engine(postgres_db_url)
                 try:
                     with tmp_engine.connect() as conn:
-                        conn.execute("COMMIT")
+                        conn.execute(sa.text("COMMIT"))
                         conn.execute(CreateDatabase(url.database))
                 except sa.exc.DBAPIError:
                     # This happens if multiple instances try to create the database
                     # at the same time.
                     with engine.connect() as conn:
                         # Verify database actually exists
-                        conn.execute("SELECT 1")
+                        conn.execute(sa.text("SELECT 1"))
         else:
             raise NotImplementedError(
                 "create_database_if_not_exists is only implemented for postgres, yet"
             )
         engine.dispose()
 
     @staticmethod
     def _connect(engine_url, schema_prefix, schema_suffix):
         engine = sa.create_engine(engine_url)
+
         # if engine.dialect.name == "ibm_db_sa":
         #     engine.dispose()
         #     # switch to READ STABILITY isolation level to avoid unnecessary deadlock
         #     # victims in case of background operations when reflecting columns
         #     engine = sa.create_engine(
         #         engine_url, execution_options={"isolation_level": "RS"}
         #     )
+        # sqlalchemy 2 has create_engine().execution_options()
 
         if engine.dialect.name == "mssql":
             engine.dispose()
             # this is needed to allow for CREATE DATABASE statements
             # (we don't rely on database transactions anyways)
             engine = sa.create_engine(engine_url, connect_args={"autocommit": True})
 
@@ -267,41 +286,70 @@
                 raise AttributeError(
                     "Config Error: There must be exactly dot in both schema_prefix and"
                     " schema_suffix together for SQL Server / mssql database:"
                     f' schema_prefix="{schema_prefix}", schema_suffix="{schema_suffix}"'
                 )
         return engine
 
+    @contextmanager
+    def engine_connect(self):
+        if self.engine.dialect.name == "ibm_db_sa":
+            conn = self.engine.connect()
+        else:
+            # sqlalchemy 2.0 uses this (except for dialect ibm_db_sa)
+            conn = self.engine.connect().execution_options(isolation_level="AUTOCOMMIT")
+        try:
+            yield conn
+        finally:
+            try:
+                # sqlalchemy 2.0 + ibm_db_sa needs this
+                conn.commit()
+            except AttributeError:
+                # sqlalchemy 1.x does not have this function and does not need it
+                pass
+
     def get_schema(self, name):
         return Schema(name, self.schema_prefix, self.schema_suffix)
 
     def _execute(self, query, conn: sa.engine.Connection):
         if self.print_sql:
             if isinstance(query, str):
                 query_str = query
             else:
                 query_str = str(
                     query.compile(self.engine, compile_kwargs={"literal_binds": True})
                 )
             pretty_query_str = self.format_sql_string(query_str)
             self.logger.info(f"Executing sql:\n{pretty_query_str}")
 
-        return conn.execute(query)
+        if isinstance(query, str):
+            return conn.execute(sa.text(query))
+        else:
+            return conn.execute(query)
 
     def execute(self, query, *, conn: sa.engine.Connection = None):
         if conn is None:
-            with self.engine.connect() as conn:
-                return self.execute(query, conn=conn)
+            with self.engine_connect() as conn:
+                if isinstance(query, str):
+                    return self.execute(sa.text(query), conn=conn)
+                else:
+                    return self.execute(query, conn=conn)
 
         if isinstance(query, sa.schema.DDLElement):
             # Some custom DDL statements contain multiple statements.
             # They are all seperated using a special seperator.
             query_str = str(
                 query.compile(self.engine, compile_kwargs={"literal_binds": True})
             )
+            try:
+                # sqlalchemy 2.0 + ibm_db_sa needs this
+                conn.commit()
+            except AttributeError:
+                # sqlalchemy 1.x does not have this function and does not need it
+                pass
             with conn.begin():
                 for part in split_ddl_statement(query_str):
                     self._execute(part, conn)
             return
 
         return self._execute(query, conn)
 
@@ -406,14 +454,15 @@
                 # deadlock victim
                 try:
                     self.execute(
                         ChangeColumnNullable(
                             table_name, schema, key_columns, nullable=False
                         )
                     )
+                    break
                 except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
                     if retry_iteration == 3:
                         raise
                     time.sleep(retry_iteration * retry_iteration * 1.1)
         self.execute(AddPrimaryKey(table_name, schema, key_columns, name))
 
     # @add_index.dialect("ibm_db_sa")
@@ -495,15 +544,15 @@
             if statement == "":
                 # allow GO at end of script
                 continue
 
             if re.match(r"\bUSE\b", statement):
                 last_use_statement = statement
 
-            with self.engine.connect() as conn:
+            with self.engine_connect() as conn:
                 if last_use_statement is not None:
                     self.execute(last_use_statement, conn=conn)
                 self.execute(statement, conn=conn)
 
     def _execute_raw_sql_mssql_pytsql(self, raw_sql: RawSql):
         """Use pytsql for executing T-SQL scripts containing many GO statements."""
         # noinspection PyUnresolvedReferences,PyPackageRequirements
@@ -523,43 +572,43 @@
             isolate_top_level_statements=self.pytsql_isolate_top_level_statements,
         )
 
     def setup(self):
         super().setup()
         if not self.avoid_drop_create_schema:
             self.execute(CreateSchema(self.metadata_schema, if_not_exists=True))
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             try:
                 version = conn.execute(
                     sa.select(self.version_table.c.version)
                 ).scalar_one_or_none()
             except sa.exc.ProgrammingError:
                 # table metadata_version does not yet exist
                 version = None
-            if version is None:
-                with conn.begin():
-                    self.sql_metadata.create_all(conn)
-                    version = conn.execute(
-                        sa.select(self.version_table.c.version)
-                    ).scalar_one_or_none()
-                    assert version is None  # detect race condition
-                    conn.execute(
-                        self.version_table.insert().values(
-                            version=self.metadata_version,
-                        )
+        if version is None:
+            with self.engine_connect() as conn, conn.begin():
+                self.sql_metadata.create_all(conn)
+                version = conn.execute(
+                    sa.select(self.version_table.c.version)
+                ).scalar_one_or_none()
+                assert version is None  # detect race condition
+                conn.execute(
+                    self.version_table.insert().values(
+                        version=self.metadata_version,
                     )
-            elif version != self.metadata_version:
-                # disable caching due to incompatible metadata table schemas
-                # (in future versions, consider automatic metadata schema upgrade)
-                self.disable_caching = True
-                self.logger.warning(
-                    "Disabled caching due to metadata version mismatch",
-                    version=version,
-                    expected_version=self.metadata_version,
                 )
+        elif version != self.metadata_version:
+            # disable caching due to incompatible metadata table schemas
+            # (in future versions, consider automatic metadata schema upgrade)
+            self.disable_caching = True
+            self.logger.warning(
+                "Disabled caching due to metadata version mismatch",
+                version=version,
+                expected_version=self.metadata_version,
+            )
 
     def dispose(self):
         self.engine.dispose()
         super().dispose()
 
     def init_stage(self, stage: Stage):
         stage_commit_technique = ConfigContext.get().stage_commit_technique
@@ -571,18 +620,20 @@
 
     @engine_dispatch
     def drop_all_dialect_specific(self, schema: Schema):
         pass
 
     @drop_all_dialect_specific.dialect("ibm_db_sa")
     def _drop_all_dialect_specific_ibm_db_sa(self, schema: Schema):
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             alias_names = conn.execute(
-                "SELECT NAME FROM SYSIBM.SYSTABLES WHERE CREATOR ="
-                f" '{ibm_db_sa_fix_name(schema.get())}' and TYPE='A'"
+                sa.text(
+                    "SELECT NAME FROM SYSIBM.SYSTABLES WHERE CREATOR ="
+                    f" '{ibm_db_sa_fix_name(schema.get())}' and TYPE='A'"
+                )
             ).all()
         alias_names = [row[0] for row in alias_names]
         for alias in alias_names:
             self.execute(DropAlias(alias, schema))
 
     @engine_dispatch
     def _init_stage_schema_swap(self, stage: Stage):
@@ -591,15 +642,15 @@
 
         cs_base = CreateSchema(schema, if_not_exists=True)
         ds_trans = DropSchema(
             transaction_schema, if_exists=True, cascade=True, engine=self.engine
         )
         cs_trans = CreateSchema(transaction_schema, if_not_exists=False)
 
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             if self.avoid_drop_create_schema:
                 # empty tansaction_schema by deleting all tables and views
                 # Attention: similar code in sql_ddl.py:visit_drop_schema_ibm_db_sa
                 # for drop.cascade=True
                 inspector = sa.inspect(self.engine)
                 for table in inspector.get_table_names(schema=transaction_schema.get()):
                     self.execute(DropTable(table, schema=transaction_schema))
@@ -636,15 +687,15 @@
 
         # TODO: detect whether tmp_schema exists and rename it as base or
         #       transaction schema if one is missing
         database, trans_schema_only = transaction_schema.get().split(".")
 
         # don't drop/create databases, just replace the schema underneath
         # (files will keep name on renaming)
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             if not self.avoid_drop_create_schema:
                 self.execute(cs_base, conn=conn)
                 self.execute(cs_trans, conn=conn)
             self.execute(f"USE [{database}]", conn=conn)
             # clear tables in schema
             self.execute(
                 f"""
@@ -693,15 +744,15 @@
                         table.delete()
                         .where(table.c.stage == stage.name)
                         .where(table.c.in_transaction_schema)
                     )
 
     def _init_stage_read_views(self, stage: Stage):
         try:
-            with self.engine.connect() as conn:
+            with self.engine_connect() as conn:
                 metadata_rows = (
                     conn.execute(
                         self.stage_table.select().where(
                             self.stage_table.c.stage == stage.name
                         )
                     )
                     .mappings()
@@ -734,15 +785,19 @@
         tmp_schema = self.get_schema(stage.name + "__swap")
 
         # potentially this disposal must be optional since it does not allow
         # for multithreaded stage execution
         # dispose open connections which may prevent schema swapping
         self.engine.dispose()
 
-        with self.engine.connect() as conn, conn.begin():
+        # We might want to also append ', conn.begin()' to the with statement,
+        # but this collides with the inner conn.begin() used to execute
+        # statement parts as one transaction. This is solvable via complex code,
+        # but we typically don't want to rely on database transactions anyways.
+        with self.engine_connect() as conn:
             # TODO: for mssql try to find schema does not exist and then move
             #       the forgotten tmp schema there
             assert not self.avoid_drop_create_schema, (
                 "The option avoid_drop_create_schema is currently not supported in "
                 "combination with dialect mssql"
             )
             self.execute(
@@ -757,15 +812,15 @@
 
             self._commit_stage_update_metadata(stage, conn=conn)
 
     def _commit_stage_read_views(self, stage: Stage):
         dest_schema = self.get_schema(stage.name)
         src_schema = self.get_schema(stage.transaction_name)
 
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             # Delete all read views in visible (destination) schema
             views = self.get_view_names(dest_schema.get())
             for view in views:
                 self.execute(DropView(view, schema=dest_schema), conn=conn)
             self.drop_all_dialect_specific(schema=dest_schema)
 
             # Create views for all tables in transaction schema
@@ -845,15 +900,15 @@
                 )
 
     def copy_table_to_transaction(self, table: Table):
         stage = table.stage
         schema_name = self.get_schema(stage.name).get()
         has_table = sa.inspect(self.engine).has_table(table.name, schema=schema_name)
         if not has_table:
-            raise CacheError(
+            raise RuntimeError(
                 f"Can't copy table '{table.name}' (schema: '{stage.name}')"
                 " to transaction because no such table exists."
             )
 
         try:
             self.execute(
                 CopyTable(
@@ -865,20 +920,18 @@
             )
         except Exception as _e:
             msg = (
                 f"Failed to copy table '{table.name}' (schema: '{stage.name}')"
                 " to transaction."
             )
             self.logger.error(
-                msg
-                + " This error is treated as cache-lookup-failure and thus we can"
-                " continue.",
+                msg,
                 exception=traceback.format_exc(),
             )
-            raise CacheError(msg) from _e
+            raise RuntimeError(msg) from _e
         self.add_indexes(table, self.get_schema(stage.transaction_name))
 
     def deferred_copy_lazy_table_to_transaction(
         self, src_name: str, src_stage: Stage, table: Table
     ):
         stage = table.stage
         src_schema = self.get_schema(src_stage)
@@ -960,15 +1013,15 @@
         if not has_table:
             msg = (
                 f"Can't copy lazy table '{metadata.name}' (schema:"
                 f" '{metadata.stage}') to transaction because no such table"
                 " exists."
             )
             self.logger.error(msg)
-            raise CacheError(msg)
+            raise RuntimeError(msg)
 
         try:
             self.execute(
                 CreateAlias(
                     metadata.name,
                     self.get_schema(metadata.stage),
                     metadata.name,
@@ -985,15 +1038,15 @@
             )
         except Exception as _e:
             msg = (
                 f"Failed to copy lazy table {metadata.name} (schema:"
                 f" '{metadata.stage}') to transaction."
             )
             self.logger.error(msg, exception=traceback.format_exc())
-            raise CacheError(msg) from _e
+            raise RuntimeError(msg) from _e
 
     @engine_dispatch
     def get_view_names(self, schema: str, *, include_everything=False) -> list[str]:
         """
         List all views that are present in a schema.
 
         It may also include other database objects like stored procedures, functions,
@@ -1018,15 +1071,15 @@
             return self.get_view_names.original(
                 self, schema, include_everything=include_everything
             )
         return list(self._get_mssql_sql_modules(schema).keys())
 
     # noinspection SqlDialectInspection
     def _get_mssql_sql_modules(self, schema: str):
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             database, schema_only = schema.split(".")
             self.execute(f"USE {database}", conn=conn)
             # include stored procedures in view names because they can also be recreated
             # based on sys.sql_modules.description
             sql = (
                 "select obj.name, obj.type from sys.sql_modules as mod "
                 "left join sys.objects as obj on mod.object_id=obj.object_id "
@@ -1034,15 +1087,15 @@
                 f"where schem.name='{schema_only}'"
             )
             rows = self.execute(sql, conn=conn).fetchall()
         return {row[0]: row[1] for row in rows}
 
     # noinspection SqlDialectInspection
     def _get_mssql_sql_synonyms(self, schema: str):
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             database, schema_only = schema.split(".")
             self.execute(f"USE {database}", conn=conn)
             # include stored procedures in view names because they can also be recreated
             # based on sys.sql_modules.description
             sql = (
                 "select syn.name, syn.type from sys.synonyms as syn "
                 "left join sys.schemas as schem on schem.schema_id=syn.schema_id "
@@ -1081,20 +1134,18 @@
                 )
             except Exception as _e:
                 msg = (
                     f"Failed to copy raw sql generated table {table_name} (schema:"
                     f" '{src_schema}') to transaction."
                 )
                 self.logger.error(
-                    msg
-                    + " This error is treated as cache-lookup-failure and thus we can"
-                    " continue.",
+                    msg,
                     exception=traceback.format_exc(),
                 )
-                raise CacheError(msg) from _e
+                raise RuntimeError(msg) from _e
 
         views_to_copy = new_tables & set(views)
         for view_name in views_to_copy:
             self._copy_view_to_transaction(view_name, src_schema, dest_schema)
 
     @engine_dispatch
     def _copy_view_to_transaction(
@@ -1106,15 +1157,15 @@
     @_copy_view_to_transaction.dialect("mssql")
     def _copy_view_to_transaction_mssql(
         self, view_name: str, src_schema: Schema, dest_schema: Schema
     ):
         src_database, src_schema_only = src_schema.get().split(".")
         dest_database, dest_schema_only = dest_schema.get().split(".")
 
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             self.execute(f"USE {src_database}", conn=conn)
             view_sql = self.execute(
                 f"""
                 SELECT definition
                 FROM sys.sql_modules
                 WHERE [object_id] = OBJECT_ID('[{src_schema_only}].[{view_name}]');
                 """,
@@ -1148,15 +1199,15 @@
                 self.get_schema(table.stage.transaction_name),
                 if_exists=True,
             )
         )
 
     def store_task_metadata(self, metadata: TaskMetadata, stage: Stage):
         if not self.disable_caching:
-            with self.engine.connect() as conn:
+            with self.engine_connect() as conn:
                 conn.execute(
                     self.tasks_table.insert().values(
                         name=metadata.name,
                         stage=metadata.stage,
                         version=metadata.version,
                         timestamp=metadata.timestamp,
                         run_id=metadata.run_id,
@@ -1174,15 +1225,15 @@
             raise CacheError(
                 "Caching is disabled, so we also don't even try to retrieve task"
                 f" cache: {task}"
             )
 
         ignore_fresh_input = RunContext.get().ignore_fresh_input
         try:
-            with self.engine.connect() as conn:
+            with self.engine_connect() as conn:
                 result = (
                     conn.execute(
                         self.tasks_table.select()
                         .where(self.tasks_table.c.name == task.name)
                         .where(self.tasks_table.c.stage == task.stage.name)
                         .where(self.tasks_table.c.version == task.version)
                         .where(self.tasks_table.c.input_hash == input_hash)
@@ -1193,15 +1244,15 @@
                         )
                         .where(self.tasks_table.c.in_transaction_schema.in_([False]))
                     )
                     .mappings()
                     .one_or_none()
                 )
         except sa.exc.MultipleResultsFound:
-            raise CacheError("Multiple results found task metadata") from None
+            raise RuntimeError("Multiple results found task metadata") from None
 
         if result is None:
             raise CacheError(f"Couldn't retrieve task from cache: {task}")
 
         return TaskMetadata(
             name=result.name,
             stage=result.stage,
@@ -1211,15 +1262,15 @@
             input_hash=result.input_hash,
             cache_fn_hash=result.cache_fn_hash,
             output_json=result.output_json,
         )
 
     def store_lazy_table_metadata(self, metadata: LazyTableMetadata):
         if not self.disable_caching:
-            with self.engine.connect() as conn:
+            with self.engine_connect() as conn:
                 conn.execute(
                     self.lazy_cache_table.insert().values(
                         name=metadata.name,
                         stage=metadata.stage,
                         query_hash=metadata.query_hash,
                         task_hash=metadata.task_hash,
                         in_transaction_schema=True,
@@ -1233,30 +1284,30 @@
         if self.disable_caching:
             raise CacheError(
                 "Caching is disabled, so we also don't even try to retrieve lazy table"
                 " cache"
             )
 
         try:
-            with self.engine.connect() as conn:
+            with self.engine_connect() as conn:
                 result = (
                     conn.execute(
                         self.lazy_cache_table.select()
                         .where(self.lazy_cache_table.c.stage == stage.name)
                         .where(self.lazy_cache_table.c.query_hash == query_hash)
                         .where(self.lazy_cache_table.c.task_hash == task_hash)
                         .where(
                             self.lazy_cache_table.c.in_transaction_schema.in_([False])
                         )
                     )
                     .mappings()
                     .one_or_none()
                 )
         except sa.exc.MultipleResultsFound:
-            raise CacheError(
+            raise RuntimeError(
                 "Multiple results found for lazy table cache key"
             ) from None
 
         if result is None:
             raise CacheError("No result found for lazy table cache key")
 
         return LazyTableMetadata(
@@ -1264,15 +1315,15 @@
             stage=result.stage,
             query_hash=result.query_hash,
             task_hash=result.task_hash,
         )
 
     def store_raw_sql_metadata(self, metadata: RawSqlMetadata):
         if not self.disable_caching:
-            with self.engine.connect() as conn:
+            with self.engine_connect() as conn:
                 conn.execute(
                     self.raw_sql_cache_table.insert().values(
                         prev_tables=json.dumps(metadata.prev_tables),
                         tables=json.dumps(metadata.tables),
                         stage=metadata.stage,
                         query_hash=metadata.query_hash,
                         task_hash=metadata.task_hash,
@@ -1287,15 +1338,15 @@
         if self.disable_caching:
             raise CacheError(
                 "Caching is disabled, so we also don't even try to retrieve raw sql"
                 " cache"
             )
 
         try:
-            with self.engine.connect() as conn:
+            with self.engine_connect() as conn:
                 result = (
                     conn.execute(
                         self.raw_sql_cache_table.select()
                         .where(self.raw_sql_cache_table.c.stage == stage.name)
                         .where(self.raw_sql_cache_table.c.query_hash == query_hash)
                         .where(self.raw_sql_cache_table.c.task_hash == task_hash)
                         .where(
@@ -1304,15 +1355,15 @@
                             )
                         )
                     )
                     .mappings()
                     .one_or_none()
                 )
         except sa.exc.MultipleResultsFound:
-            raise CacheError("Multiple results found for raw sql cache key") from None
+            raise RuntimeError("Multiple results found for raw sql cache key") from None
 
         if result is None:
             raise CacheError("No result found for raw sql cache key")
 
         return RawSqlMetadata(
             prev_tables=json.loads(result.prev_tables),
             tables=json.loads(result.tables),
@@ -1323,20 +1374,20 @@
 
     @engine_dispatch
     def resolve_aliases(self, table_name, schema):
         return table_name, schema
 
     @resolve_aliases.dialect("ibm_db_sa")
     def resolve_aliases_ibm_db_sa(self, table_name, schema):
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             return _resolve_alias_ibm_db_sa(conn, table_name, schema)
 
     @resolve_aliases.dialect("mssql")
     def resolve_aliases_mssql(self, table_name, schema):
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             return _resolve_alias_mssql(conn, table_name, schema)
 
     def list_tables(self, stage: Stage, *, include_everything=False):
         """
         List all tables that were generated in a stage.
 
         It may also include other objects database objects like views, stored
@@ -1364,17 +1415,17 @@
         # We only need to look in tasks_table since the output_json column is updated
         # after evaluating lazy output objects for cache validity. This is the same
         # information we use for producing input_hash of downstream tasks.
         if self.disable_caching:
             raise NotImplementedError(
                 "computing stage hash with disabled caching is currently not supported"
             )
-        with self.engine.connect() as conn:
+        with self.engine_connect() as conn:
             result = conn.execute(
-                sa.select([self.tasks_table.c.output_json])
+                sa.select(self.tasks_table.c.output_json)
                 .where(self.tasks_table.c.stage == stage.name)
                 .where(self.tasks_table.c.in_transaction_schema.in_([False]))
                 .order_by(self.tasks_table.c.output_json)
             ).all()
             result = [row[0] for row in result]
         return compute_cache_key(*result)
 
@@ -1436,59 +1487,61 @@
             try:
                 tbl = sa.Table(
                     table_name,
                     sa.MetaData(),
                     schema=schema,
                     autoload_with=store.engine,
                 )
+                break
             except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
                 if retry_iteration == 3:
                     raise
                 time.sleep(retry_iteration * retry_iteration * 1.2)
         return tbl
 
     @classmethod
     def lazy_query_str(cls, store, obj) -> str:
         if isinstance(obj, sa.sql.selectable.FromClause):
-            query = sa.select([sa.text("*")]).select_from(obj)
+            query = sa.select(sa.text("*")).select_from(obj)
         else:
             query = obj
         query_str = str(
             query.compile(store.engine, compile_kwargs={"literal_binds": True})
         )
         # hacky way to canonicalize query (despite __tmp/__even/__odd suffixes
         # and alias resolution)
+        query_str = re.sub(r'["\[\]]', "", query_str)
         query_str = re.sub(
-            r"(__tmp|__even|__odd)(?=[ \t\n.;]|$)", "", query_str.lower()
+            r'(__tmp|__even|__odd)(?=[ \t\n.;"]|$)', "", query_str.lower()
         )
-        query_str = re.sub(r'["\[\]]', "", query_str)
         return query_str
 
 
 def _resolve_alias_ibm_db_sa(conn, table_name: str, schema: str, *, _iteration=0):
     # TODO: consider speeding this up by caching information for complete schemas
     #  instead of running at least two queries per source table; Ultimately problem can
     #  also be fixed by upstream contribution to ibm_db_sa
 
     # we need to resolve aliases since pandas.read_sql_table does not work for them
     # and sa.Table does not auto-reflect columns
     table_name = ibm_db_sa_fix_name(table_name)
     schema = ibm_db_sa_fix_name(schema)
     tbl = sa.Table("SYSTABLES", sa.MetaData(), schema="SYSIBM", autoload_with=conn)
     query = (
-        sa.select([tbl.c.base_name, tbl.c.base_schema])
+        sa_select([tbl.c.base_name, tbl.c.base_schema])
         .select_from(tbl)
         .where(
             (tbl.c.creator == schema) & (tbl.c.name == table_name) & (tbl.c.TYPE == "A")
         )
     )
     for retry_iteration in range(4):
         # retry operation since it might have been terminated as a deadlock victim
         try:
             row = conn.execute(query).mappings().one_or_none()
+            break
         except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
             if retry_iteration == 3:
                 raise
             time.sleep(retry_iteration * retry_iteration)
     if row is not None:
         assert _iteration < 3, f"Unexpected recursion looking up {schema}.{table_name}"
         table_name, schema = _resolve_alias_ibm_db_sa(
@@ -1501,23 +1554,23 @@
     # TODO: consider speeding this up by caching information for complete schemas
     #  instead of running at least two queries per source table; Ultimately problem can
     #  also be fixed by upstream contribution to ibm_db_sa
 
     # we need to resolve aliases since pandas.read_sql_table does not work for them
     # and sa.Table does not auto-reflect columns
     database, schema_only = schema.split(".")
-    conn.execute(f"USE [{database}]")
+    conn.execute(sa.text(f"USE [{database}]"))
     # include stored procedures in view names because they can also be recreated
     # based on sys.sql_modules.description
     sql = (
         "select syn.base_object_name from sys.synonyms as syn left join sys.schemas as"
         f" schem on schem.schema_id=syn.schema_id where schem.name='{schema_only}' and"
         f" syn.name='{table_name}' and syn.type='SN'"
     )
-    row = conn.execute(sql).mappings().one_or_none()
+    row = conn.execute(sa.text(sql)).mappings().one_or_none()
     if row is not None:
         parts = row["base_object_name"].split(".")
         assert len(parts) == 3, (
             "Unexpected number of '.' delimited parts when looking up synonym for "
             f"{schema}.{table_name}: {row['base_object_name']}"
         )
         assert _iteration < 3, f"Unexpected recursion looking up {schema}.{table_name}"
@@ -1529,16 +1582,47 @@
         table_name = parts[2]
         table_name, schema = _resolve_alias_mssql(
             conn, table_name, schema, _iteration=_iteration + 1
         )
     return table_name, schema
 
 
+def adj_pandas_types(df: pd.DataFrame):
+    df = df.copy()
+    for col in df.dtypes.loc[lambda x: x == int].index:
+        df[col] = df[col].astype(pd.Int64Dtype())
+    for col in df.dtypes.loc[lambda x: x == bool].index:
+        df[col] = df[col].astype(pd.BooleanDtype())
+    for col in df.dtypes.loc[lambda x: x == object].index:
+        df[col] = df[col].astype(pd.StringDtype())
+    return df
+
+
 @SQLTableStore.register_table(pd)
 class PandasTableHook(TableHook[SQLTableStore]):
+    """
+    Materalize pandas->sql and retrieve sql->pandas.
+
+    We like to limit the use of types, so operations can be implemented reliably
+    without the use of pandas dtype=object where every row can have different type:
+      - string/varchar/clob: pd.StringDType
+      - date: datetime64[ns] (we cap year in 1900..2199 and save original year
+            in separate column)
+      - datetime: datetime64[ns] (we cap year in 1900..2199 and save original year
+            in separate column)
+      - int: pd.Int64DType
+      - boolean: pd.BooleanDType
+
+    Dialect specific aspects:
+      * ibm_db_sa:
+        - DB2 does not support boolean type -> integer
+        - We limit string columns to 256 characters since larger columns have
+          trouble with adding indexes/primary keys
+    """
+
     @classmethod
     def can_materialize(cls, type_) -> bool:
         return issubclass(type_, pd.DataFrame)
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return type_ == pd.DataFrame
@@ -1547,56 +1631,257 @@
     def materialize(
         cls,
         store,
         table: Table[pd.DataFrame],
         stage_name,
         task_info: TaskInfo,
     ):
+        # we might try to avoid this copy for speedup / saving RAM
+        df = table.obj.copy()
         schema = store.get_schema(stage_name)
         if store.print_materialize:
             store.logger.info(
                 f"Writing table '{schema.get()}.{table.name}':\n{table.obj}"
             )
         dtype_map = {}
         table_name = table.name
+        str_type = sa.String()
         if store.engine.dialect.name == "ibm_db_sa":
             # Default string target is CLOB which can't be used for indexing.
             # We could use VARCHAR(32000), but if we change this to VARCHAR(256)
             # for indexed columns, DB2 hangs.
-            dtype_map = {
-                col: sa.VARCHAR(256)
-                for col in table.obj.dtypes.loc[lambda x: x == object].index
-            }
+            str_type = sa.VARCHAR(256)
             table_name = ibm_db_sa_fix_name(table_name)
-        table.obj.to_sql(
+        # force dtype=object to string (we require dates to be stored in datetime64[ns])
+        for col in df.dtypes.loc[lambda x: x == object].index:
+            if table.type_map is None or col not in table.type_map:
+                df[col] = df[col].astype(str)
+                dtype_map[col] = str_type
+        for col in df.dtypes.loc[
+            lambda x: (x != object) & x.isin([pd.Int32Dtype, pd.UInt16Dtype])
+        ].index:
+            dtype_map[col] = sa.INTEGER()
+        for col in df.dtypes.loc[
+            lambda x: (x != object)
+            & x.isin([pd.Int16Dtype, pd.Int8Dtype, pd.UInt8Dtype])
+        ].index:
+            dtype_map[col] = sa.SMALLINT()
+        if table.type_map is not None:
+            dtype_map.update(table.type_map)
+        # Todo: do better abstraction of dialect specific code
+        if store.engine.dialect.name == "mssql":
+            for col, _type in dtype_map.items():
+                if _type == sa.DateTime:
+                    dtype_map[col] = DATETIME2()
+        df.to_sql(
             table_name,
             store.engine,
             schema=schema.get(),
             index=False,
             dtype=dtype_map,
+            chunksize=100_000,
         )
         store.add_indexes(table, schema)
 
+    @staticmethod
+    def _pandas_type(sql_type):
+        if isinstance(sql_type, sa.SmallInteger):
+            return pd.Int16Dtype()
+        elif isinstance(sql_type, sa.BigInteger):
+            return pd.Int64Dtype()
+        elif isinstance(sql_type, sa.Integer):
+            return pd.Int32Dtype()
+        elif isinstance(sql_type, sa.Boolean):
+            return pd.BooleanDtype()
+        elif isinstance(sql_type, sa.String):
+            return pd.StringDtype()
+        elif isinstance(sql_type, sa.Date):
+            return "datetime64[ns]"
+        elif isinstance(sql_type, sa.DateTime):
+            return "datetime64[ns]"
+
+    @staticmethod
+    def _fix_cols(cols: dict[str, Any], dialect_name):
+        cols = cols.copy()
+        year_cols = []
+        min_date = "1900-01-01"
+        max_date = "2199-12-31"
+        for name, col in list(cols.items()):
+            if isinstance(col.type, sa.Date) or isinstance(col.type, sa.DateTime):
+                if name + "_year" not in cols:
+                    cols[name + "_year"] = sa.cast(
+                        sa.func.extract("year", cols[name]), sa.Integer
+                    ).label(name + "_year")
+                    year_cols.append(name + "_year")
+                # Todo: do better abstraction of dialect specific code
+                if dialect_name == "mssql":
+                    cap_min = sa.func.iif(cols[name] < min_date, min_date, cols[name])
+                    cols[name] = sa.func.iif(
+                        cap_min > max_date, max_date, cap_min
+                    ).label(name)
+                else:
+                    cols[name] = sa.func.least(
+                        max_date, sa.func.greatest(min_date, cols[name])
+                    ).label(name)
+        return cols, year_cols
+
     @classmethod
     def retrieve(cls, store, table, stage_name, as_type):
         schema = store.get_schema(stage_name).get()
         with store.engine.connect() as conn:
             table_name = table.name
             table_name, schema = store.resolve_aliases(table_name, schema)
-            df = pd.read_sql_table(table_name, conn, schema=schema)
+            for retry_iteration in range(4):
+                # retry operation since it might have been terminated as a
+                # deadlock victim
+                try:
+                    sql_table = sa.Table(
+                        table_name,
+                        sa.MetaData(),
+                        schema=schema,
+                        autoload_with=store.engine,
+                    ).alias("tbl")
+                    dtype_map = {c.name: cls._pandas_type(c.type) for c in sql_table.c}
+                    cols, year_cols = cls._fix_cols(
+                        {c.name: c for c in sql_table.c}, store.engine.dialect.name
+                    )
+                    dtype_map.update({col: pd.Int16Dtype() for col in year_cols})
+                    query = sa_select(cols.values()).select_from(sql_table)
+                    try:
+                        # works only from pandas 2.0.0 on
+                        df = pd.read_sql(
+                            query,
+                            con=conn,
+                            dtype=dtype_map,
+                        )
+                    except TypeError:
+                        df = pd.read_sql(query, con=conn)
+                        for col, _type in dtype_map.items():
+                            df[col] = df[col].astype(_type)
+                    break
+                except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
+                    if retry_iteration == 3:
+                        raise
+                    time.sleep(retry_iteration * retry_iteration * 1.3)
             return df
 
     @classmethod
     def auto_table(cls, obj: pd.DataFrame):
         if name := obj.attrs.get("name"):
             return Table(obj, name)
         return super().auto_table(obj)
 
 
 try:
+    # optional dependency to polars
+    import connectorx
+    import polars
+except ImportError as e:
+    warnings.warn(str(e), ImportWarning)
+    polars = None
+    connectorx = None
+
+
+@SQLTableStore.register_table(polars, connectorx)
+class PolarsTableHook(TableHook[SQLTableStore]):
+    @classmethod
+    def can_materialize(cls, type_) -> bool:
+        # attention: tidypolars.Tibble is subclass of polars DataFrame
+        return type_ == polars.dataframe.DataFrame
+
+    @classmethod
+    def can_retrieve(cls, type_) -> bool:
+        return type_ == polars.dataframe.DataFrame
+
+    @classmethod
+    def materialize(
+        cls,
+        store,
+        table: Table[polars.dataframe.DataFrame],
+        stage_name,
+        task_info: TaskInfo,
+    ):
+        schema = store.get_schema(stage_name)
+        if store.print_materialize:
+            store.logger.info(
+                f"Writing table '{schema.get()}.{table.name}':\n{table.obj}"
+            )
+        table_name = table.name
+        # TODO:
+        # dtype_map = {}
+        # if store.engine.dialect.name == "ibm_db_sa":
+        #     # Default string target is CLOB which can't be used for indexing.
+        #     # We could use VARCHAR(32000), but if we change this to VARCHAR(256)
+        #     # for indexed columns, DB2 hangs.
+        #     dtype_map = {
+        #         col: sa.VARCHAR(256)
+        #         for col in table.obj.dtypes.loc[lambda x: x == object].index
+        #     }
+        #     table_name = ibm_db_sa_fix_name(table_name)
+        table.obj.to_pandas(use_pyarrow_extension_array=True).to_sql(
+            name=table_name, con=store.engine, schema=schema.get(), index=False
+        )
+        store.add_indexes(table, schema)
+
+    @classmethod
+    def retrieve(cls, store, table, stage_name, as_type):
+        schema = store.get_schema(stage_name).get()
+        table_name = table.name
+        table_name, schema = store.resolve_aliases(table_name, schema)
+        conn = str(store.engine_url_obj)
+        df = polars.read_database(f'SELECT * FROM {schema}."{table_name}"', conn)
+        return df
+
+    @classmethod
+    def auto_table(cls, obj: polars.dataframe.DataFrame):
+        return super().auto_table(obj)
+
+
+try:
+    # optional dependency to polars
+    import tidypolars
+except ImportError as e:
+    warnings.warn(str(e), ImportWarning)
+    tidypolars = None
+
+
+@SQLTableStore.register_table(tidypolars, polars, connectorx)
+class TidyPolarsTableHook(TableHook[SQLTableStore]):
+    @classmethod
+    def can_materialize(cls, type_) -> bool:
+        return issubclass(type_, tidypolars.Tibble)
+
+    @classmethod
+    def can_retrieve(cls, type_) -> bool:
+        return type_ == tidypolars.Tibble
+
+    @classmethod
+    def materialize(
+        cls,
+        store,
+        table: Table[tidypolars.Tibble],
+        stage_name,
+        task_info: TaskInfo,
+    ):
+        table = copy.deepcopy(table)
+        table.obj = table.obj.to_polars()
+        PolarsTableHook.materialize(store, table, stage_name, task_info)
+
+    @classmethod
+    def retrieve(cls, store, table, stage_name, as_type):
+        df = PolarsTableHook.retrieve(store, table, stage_name, as_type)
+        return tidypolars.from_polars(df)
+
+    @classmethod
+    def auto_table(cls, obj: tidypolars.Tibble):
+        return super().auto_table(obj)
+
+
+try:
+    # optional dependency to pydiverse-transform
     import pydiverse.transform as pdt
 except ImportError as e:
     warnings.warn(str(e), ImportWarning)
     pdt = None
 
 
 # noinspection PyUnresolvedReferences, PyProtectedMember
@@ -1655,7 +1940,111 @@
         from pydiverse.transform.core.verbs import build_query
 
         query = obj >> build_query()
 
         if query is not None:
             return str(query)
         return super().lazy_query_str(store, obj)
+
+
+try:
+    # optional dependency to ibis
+    import ibis
+    import ibis.expr.types as ibis_types
+except ImportError as e:
+    warnings.warn(str(e), ImportWarning)
+    ibis = None
+    ibis_types = None
+
+
+@SQLTableStore.register_table(ibis)
+class IbisTableHook(TableHook[SQLTableStore]):
+    @staticmethod
+    def get_con(store):
+        # TODO: move this function to a better ibis specific place
+        con = store.engines_other.get("ibis")
+        if con is None:
+            url = store.engine_url_obj
+            dialect = store.engine.dialect.name
+            if dialect == "postgresql":
+                con = ibis.postgres.connect(
+                    host=url.host,
+                    user=url.username,
+                    password=url.password,
+                    port=url.port,
+                    database=url.database,
+                )
+            elif dialect == "mssql":
+                con = ibis.mssql.connect(
+                    host=url.host,
+                    user=url.username,
+                    password=url.password,
+                    port=url.port,
+                    database=url.database,
+                )
+            else:
+                raise RuntimeError(
+                    f"initializing ibis for {dialect} is not supported, yet "
+                    "-- supported: postgresql, mssql"
+                )
+            store.engines_other["ibis"] = con
+        return con
+
+    @classmethod
+    def can_materialize(cls, type_) -> bool:
+        # Operations on a table like mutate() or join() don't change the type
+        return issubclass(type_, ibis_types.Table)
+
+    @classmethod
+    def can_retrieve(cls, type_) -> bool:
+        return issubclass(type_, ibis_types.Table)
+
+    @classmethod
+    def materialize(
+        cls, store, table: Table[ibis_types.Table], stage_name, task_info: TaskInfo
+    ):
+        t = table.obj
+        table.obj = sa.text(cls.lazy_query_str(store, t))
+        return SQLAlchemyTableHook.materialize(store, table, stage_name, task_info)
+
+    @classmethod
+    def retrieve(cls, store, table, stage_name, as_type):
+        con = cls.get_con(store)
+        table_name = table.name
+        schema = store.get_schema(stage_name).get()
+        table_name, schema = store.resolve_aliases(table_name, schema)
+        for retry_iteration in range(4):
+            # retry operation since it might have been terminated as a deadlock victim
+            try:
+                tbl = con.table(
+                    table_name,
+                    schema=schema,
+                )
+                break
+            except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
+                if retry_iteration == 3:
+                    raise
+                time.sleep(retry_iteration * retry_iteration * 1.2)
+        return tbl
+
+    @classmethod
+    def auto_table(cls, obj: ibis_types.Table):
+        if obj.has_name():
+            return Table(obj, obj.get_name())
+        else:
+            return super().auto_table(obj)
+
+    @classmethod
+    def lazy_query_str(cls, store, obj: ibis_types.Table) -> str:
+        return str(ibis.to_sql(obj, cls.get_con(store).name))
+
+
+def sa_select(*args, **kwargs):
+    """Run sa.select in 'old' way compatible with sqlalchemy>=2.0."""
+    try:
+        return sa.select(*args, **kwargs)
+    except sa.exc.ArgumentError:
+        if len(args) == 1 and isinstance(args[0], Iterable) and len(kwargs) == 0:
+            # for sqlalchemy 2.0, we need to unpack columns
+            return sa.select(*args[0])
+        else:
+            raise
```

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/sql_ddl.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/backend/table/util/sql_ddl.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,19 +394,18 @@
         for table in inspector.get_table_names(schema=drop.schema.get()):
             add_statements.append(DropTable(table, schema=drop.schema))
         for view in inspector.get_view_names(schema=drop.schema.get()):
             add_statements.append(DropView(view, schema=drop.schema))
         # see SQLTableStore.drop_all_dialect_specific()
         with drop.engine.connect() as conn:
             alias_names = conn.execute(
-                (
+                sa.text(
                     "SELECT NAME FROM SYSIBM.SYSTABLES WHERE CREATOR ="
                     f" '{ibm_db_sa_fix_name(drop.schema.get())}' and TYPE='A'"
                 ),
-                conn=drop.engine,
             ).all()
         alias_names = [row[0] for row in alias_names]
         for alias in alias_names:
             add_statements.append(DropAlias(alias, drop.schema))
         statements += [compiler.process(stmt) for stmt in add_statements]
 
     # Compile DROP SCHEMA statement
```

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/context.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/context.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/run_context.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/context/run_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -750,14 +750,22 @@
 
 
 # msgpack hooks
 # Only used to transmit Table and Blob type metadata
 
 
 def _msg_default(obj):
-    return msgpack.ExtType(0, pickle.dumps(obj))
+    # some table implementations are not picklable
+    if hasattr(obj, "obj"):
+        save = obj.obj
+        obj.obj = None
+        ret = pickle.dumps(obj)
+        obj.obj = save
+    else:
+        ret = pickle.dumps(obj)
+    return msgpack.ExtType(0, ret)
 
 
 def _msg_ext_hook(code, data):
     if code == 0:
         return pickle.loads(data)
     return msgpack.ExtType(code, data)
```

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/flow.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/flow.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/result.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/result.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/stage.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/stage.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/task.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/core/task.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/base.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/container.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Generic
+from typing import TYPE_CHECKING, Any, Generic
 
 from pydiverse.pipedag._typing import T
 from pydiverse.pipedag.util import normalize_name
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core.stage import Stage
 
@@ -26,22 +26,24 @@
     def __init__(
         self,
         obj: T | None = None,
         name: str | None = None,
         stage: Stage | None = None,
         primary_key: str | list[str] | None = None,
         indexes: list[list[str]] | None = None,
+        type_map: dict[str, Any] | None = None,
     ):
         self._name = None
 
         self.obj = obj
         self.name = name
         self.stage = stage
         self.primary_key = primary_key
         self.indexes = indexes
+        self.type_map = type_map
 
         # cache_key will be overridden shortly before handing over to downstream tasks
         # that use it to compute their input_hash for cache_invalidation due to input
         # change
         self.cache_key = None
 
     def __str__(self):
```

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/core.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/core.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/store.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/store.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/cache.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/json.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/materialize/util/json.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 PipeDAG objects get serialized as JSON objects with a special `_pipedag_type_`
 key to identify them when decoding. The associated value encodes the
 type of the object.
 """
 
 from __future__ import annotations
 
+import datetime as dt
 from pathlib import Path
 
 from pydiverse.pipedag import Stage
 from pydiverse.pipedag.context import RunContext
 from pydiverse.pipedag.materialize.container import Blob, RawSql, Table
 from pydiverse.pipedag.util.config import PipedagConfig
 
 PIPEDAG_TYPE = "_pipedag_type_"
 PIPEDAG_TYPE_TABLE = "table"
 PIPEDAG_TYPE_RAWSQL = "raw_sql"
 PIPEDAG_TYPE_BLOB = "blob"
 PIPEDAG_TYPE_STAGE = "stage"
 PIPEDAG_TYPE_PIPEDAG_CONFIG = "pipedag_config"
 PIPEDAG_TYPE_PATH = "path"
+PIPEDAG_TYPE_DATE = "date"
+PIPEDAG_TYPE_DATETIME = "datetime"
 
 
 def json_default(o):
     """Encode `Table`, `RawSql`, 'Stage', and `Blob` objects"""
     if isinstance(o, Table):
         return {
             PIPEDAG_TYPE: PIPEDAG_TYPE_TABLE,
@@ -59,14 +62,24 @@
             "config_dict": o.config_dict,
         }
     if isinstance(o, Path):
         return {
             PIPEDAG_TYPE: PIPEDAG_TYPE_PATH,
             "path": str(o),
         }
+    if isinstance(o, dt.date):
+        return {
+            PIPEDAG_TYPE: PIPEDAG_TYPE_DATE,
+            "date": o.isoformat(),
+        }
+    if isinstance(o, dt.datetime):
+        return {
+            PIPEDAG_TYPE: PIPEDAG_TYPE_DATETIME,
+            "datetime": o.isoformat(),
+        }
 
     raise TypeError(f"Object of type {type(o).__name__} is not JSON serializable")
 
 
 def json_object_hook(d: dict):
     """Decode json with `Table` and `Blob` objects"""
     pipedag_type = d.get(PIPEDAG_TYPE)
@@ -102,13 +115,17 @@
         elif pipedag_type == PIPEDAG_TYPE_PIPEDAG_CONFIG:
             # PipedagConfig objects are allowed as input to @materialize tasks,
             # but it is not allowed as output since this might cause trouble
             # for cache-invalidation
             raise TypeError("PipedagConfig can't be deserialized.")
         elif pipedag_type == PIPEDAG_TYPE_PATH:
             return Path(d["path"])
+        elif pipedag_type == PIPEDAG_TYPE_DATE:
+            return dt.date.fromisoformat(d["date"])
+        elif pipedag_type == PIPEDAG_TYPE_DATETIME:
+            return dt.datetime.fromisoformat(d["datetime"])
         else:
             raise ValueError(
                 f"Invalid value for '{PIPEDAG_TYPE}' key: {repr(pipedag_type)}"
             )
 
     return d
```

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/config.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/config.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/disposable.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/import_.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/ipc.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/naming.py` & `pydiverse-pipedag-0.2.4/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.3/setup.py` & `pydiverse-pipedag-0.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,49 +19,55 @@
  'pydiverse.pipedag.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0',
- 'SQLAlchemy>=1.4.39,<2.0.0',
+ 'SQLAlchemy>=1.4.39',
  'attrs>=22.1.0',
  'msgpack>=1.0.4',
  'networkx>=2.8',
  'packaging>=21.3',
- 'pandas>=1.4.3,<2.0.0',
+ 'pandas>=1.4.3',
  'pynng>=0.7.1',
  'python-box>=6.1.0',
  'structlog>=22.1.0',
  'tomli>=2.0.1',
  'typing-extensions>=4.1.0,<5']
 
 extras_require = \
 {'docs': ['Sphinx>=5.1.1',
           'sphinx-rtd-theme>=1.0.0',
           'sphinxcontrib-apidoc>=0.3.0'],
  'filelock': ['filelock>=3.7.1'],
+ 'ibis': ['ibis>=3.2.0', 'ibis-framework[mssql,postgres]>=5.1.0,<6.0.0'],
  'ibm_db2': ['ibm-db>=3.1.4', 'ibm-db-sa>=0.3.8'],
  'mssql': ['pyodbc>=4.0.35', 'pytsql>=1.1.4'],
+ 'pdtransform': ['pydiverse-transform>=0.1.1'],
+ 'polars': ['tidypolars>=0.2.19',
+            'connectorx>=0.3.1',
+            'pyarrow>=11.0.0',
+            'polars>=0.16.18,<0.17'],
  'prefect': ['prefect>=1.3,<2'],
  'zookeeper': ['kazoo>=2.8.0']}
 
 setup_kwargs = {
     'name': 'pydiverse-pipedag',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.',
     'long_description': '# pydiverse.pipedag\n\n[![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml)\n\nA pipeline orchestration library executing tasks within one python session. It takes care of SQL table\n(de)materialization, caching and cache invalidation. Blob storage is supported as well for example\nfor storing model files.\n\nThis is an early stage version 0.x which lacks documentation. Please contact\nhttps://github.com/orgs/pydiverse/teams/code-owners if you like to become an early adopter\nor to contribute early stage usage examples.\n\n## Usage\n\npydiverse.pipedag can either be installed via pypi with `pip install pydiverse-pipedag` or via conda-forge\nwith `conda install pydiverse-pipedag -c conda-forge`.\n\n## Example\n\nA flow can look like this (i.e. put this in a file named `run_pipeline.py`):\n\n```python\nfrom pydiverse.pipedag import materialize, Table, Flow, Stage\nimport sqlalchemy as sa\nimport pandas as pd\n\nfrom pydiverse.pipedag.context import StageLockContext, RunContext\nfrom pydiverse.pipedag.util import setup_structlog\n\n\n@materialize(lazy=True)\ndef lazy_task_1():\n    return sa.select([sa.literal(1).label("x"), sa.literal(2).label("y")])\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_2(input1: sa.Table, input2: sa.Table):\n    query = sa.select([(input1.c.x * 5).label("x5"), input2.c.a]).select_from(\n        input1.outerjoin(input2, input2.c.x == input1.c.x)\n    )\n    return Table(query, name="task_2_out", primary_key=["a"])\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_3(input: sa.Table, my_stage: Stage):\n    return sa.text(f"SELECT * FROM {my_stage.transaction_name}.{input.name}")\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_4(input: sa.Table, prev_stage: Stage):\n    return sa.text(f"SELECT * FROM {prev_stage.name}.{input.name}")\n\n\n@materialize(nout=2, version="1.0.0")\ndef eager_inputs():\n    dfA = pd.DataFrame(\n        {\n            "a": [0, 1, 2, 4],\n            "b": [9, 8, 7, 6],\n        }\n    )\n    dfB = pd.DataFrame(\n        {\n            "a": [2, 1, 0, 1],\n            "x": [1, 1, 2, 2],\n        }\n    )\n    return Table(dfA, "dfA"), Table(dfB, "dfB_%%")\n\n\n@materialize(version="1.0.0", input_type=pd.DataFrame)\ndef eager_task(tbl1: pd.DataFrame, tbl2: pd.DataFrame):\n    return tbl1.merge(tbl2, on="x")\n\n\ndef main():\n    with Flow() as f:\n        with Stage("stage_1"):\n            lazy_1 = lazy_task_1()\n            a, b = eager_inputs()\n\n        with Stage("stage_2") as stage2:\n            lazy_2 = lazy_task_2(lazy_1, b)\n            lazy_3 = lazy_task_3(lazy_2, stage2)\n            eager = eager_task(lazy_1, b)\n\n        with Stage("stage_3"):\n            lazy_4 = lazy_task_4(lazy_2, stage2)\n        _ = lazy_3, lazy_4, eager  # unused terminal output tables\n\n    # Run flow\n    result = f.run()\n    assert result.successful\n\n    # Run in a different way for testing\n    with StageLockContext():\n        result = f.run()\n        assert result.successful\n        assert result.get(lazy_1, as_type=pd.DataFrame)["x"][0] == 1\n\n\nif __name__ == "__main__":\n    # initialize logging\n    setup_structlog()\n    main()\n```\n\nCreate a file called `pipedag.yaml` in the same directory:\n\n```yaml\nname: pipedag_tests\ntable_store_connections:\n  postgres:\n    # Postgres: this can be used after running `docker-compose up`\n    url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"\n\ninstances:\n  __any__:\n    # listen-interface for pipedag context server which synchronizes some task state during DAG execution\n    network_interface: "127.0.0.1"\n    # classes to be materialized to table store even without pipedag Table wrapper (we have loose coupling between\n    # pipedag and pydiverse.transform, so consider adding \'pydiverse.transform.Table\' in your config)\n    auto_table: ["pandas.DataFrame", "sqlalchemy.sql.elements.TextClause", "sqlalchemy.sql.selectable.Selectable"]\n    fail_fast: true\n\n    instance_id: pipedag_default\n    table_store:\n      class: "pydiverse.pipedag.backend.table.SQLTableStore"\n\n      # Postgres: this can be used after running `docker-compose up`\n      table_store_connection: postgres\n      create_database_if_not_exists: True\n\n      # print select statements before being encapsualted in materialize expressions and tables before writing to\n      # database\n      print_materialize: true\n      # print final sql statements\n      print_sql: true\n\n    blob_store:\n      class: "pydiverse.pipedag.backend.blob.FileBlobStore"\n      base_path: "/tmp/pipedag/blobs"\n\n    lock_manager:\n      class: "pydiverse.pipedag.backend.lock.ZooKeeperLockManager"\n      hosts: "localhost:2181"\n\n    orchestration:\n      class: "pydiverse.pipedag.engine.SequentialEngine"\n```\n\nIf you don\'t have a postgres, Microsoft SQL Server, or IBM DB2 database at hand, you can\nstart a postgres database with the following `docker-compose.yaml` file:\n\n```yaml\nversion: "3.9"\nservices:\n  postgres:\n    image: postgres\n    environment:\n      POSTGRES_USER: sa\n      POSTGRES_PASSWORD: Pydiverse23\n      POSTGRES_PORT: 6543\n    ports:\n      - 6543:5432\n  zoo:\n    image: zookeeper\n    environment:\n      ZOO_4LW_COMMANDS_WHITELIST: ruok\n      ZOO_MAX_CLIENT_CNXNS: 100\n    ports:\n      - 2181:2181\n```\n\nRun `docker-compose up` in the directory of your `docker-compose.yaml` and then execute\nthe flow script as follows with a shell like `bash` and a python environment that\nincludes `pydiverse-pipedag`, `pandas`, and `sqlalchemy`:\n\n```bash\nexport POSTGRES_USERNAME=sa\nexport POSTGRES_PASSWORD=Pydiverse23\npython run_pipeline.py\n```\n\nFinally, you may connect to your localhost postgres database `pipedag_default` and\nlook at tables in schemas `stage_1`..`stage_3`.\n\nIf you don\'t have a SQL UI at hand, you may use `psql` command line tool inside the docker container.\nCheck out the `NAMES` column in `docker ps` output. If the name of your postgres container is\n`example_postgres_1`, then you can look at output tables like this:\n\n```bash\ndocker exec example_postgres_1 psql --username=sa --dbname=pipedag_default -c \'select * from stage_1.dfa;\'\n```\n\nOr more interactively:\n\n```bash\ndocker exec -t -i example_postgres_1 bash\npsql --username=sa --dbname=pipedag_default\n\\dt stage_*.*\nselect * from stage_2.task_2_out;\n```\n\n## Troubleshooting\n\n### Installing mssql odbc driver for linux\n\nInstalling with\ninstructions [here](https://docs.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16#suse18)\nworked.\nBut `odbcinst -j` revealed that it installed the configuration in `/etc/unixODBC/*`. But conda installed pyodbc brings\nits own `odbcinst` executable and that shows odbc config files are expected in `/etc/*`. Symlinks were enough to fix the\nproblem. Try `python -c \'import pyodbc;print(pyodbc.drivers())\'` and see whether you get more than an empty list.\nFurthermore, make sure you use 127.0.0.1 instead of localhost. It seems that /etc/hosts is ignored.\n',
     'author': 'QuantCo, Inc.',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.9,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pydiverse-pipedag-0.2.3/PKG-INFO` & `pydiverse-pipedag-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.2.3
+Version: 0.2.4
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Provides-Extra: docs
 Provides-Extra: filelock
+Provides-Extra: ibis
 Provides-Extra: ibm_db2
 Provides-Extra: mssql
+Provides-Extra: pdtransform
+Provides-Extra: polars
 Provides-Extra: prefect
 Provides-Extra: zookeeper
 Requires-Dist: PyYAML (>=6.0)
-Requires-Dist: SQLAlchemy (>=1.4.39,<2.0.0)
+Requires-Dist: SQLAlchemy (>=1.4.39)
 Requires-Dist: Sphinx (>=5.1.1); extra == "docs"
 Requires-Dist: attrs (>=22.1.0)
+Requires-Dist: connectorx (>=0.3.1); extra == "polars"
 Requires-Dist: filelock (>=3.7.1); extra == "filelock"
+Requires-Dist: ibis (>=3.2.0); extra == "ibis"
+Requires-Dist: ibis-framework[mssql,postgres] (>=5.1.0,<6.0.0); extra == "ibis"
 Requires-Dist: ibm-db (>=3.1.4); extra == "ibm_db2"
 Requires-Dist: ibm-db-sa (>=0.3.8); extra == "ibm_db2"
 Requires-Dist: kazoo (>=2.8.0); extra == "zookeeper"
 Requires-Dist: msgpack (>=1.0.4)
 Requires-Dist: networkx (>=2.8)
 Requires-Dist: packaging (>=21.3)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: pandas (>=1.4.3)
+Requires-Dist: polars (>=0.16.18,<0.17); extra == "polars"
 Requires-Dist: prefect (>=1.3,<2); extra == "prefect"
+Requires-Dist: pyarrow (>=11.0.0); extra == "polars"
+Requires-Dist: pydiverse-transform (>=0.1.1); extra == "pdtransform"
 Requires-Dist: pynng (>=0.7.1)
 Requires-Dist: pyodbc (>=4.0.35); extra == "mssql"
 Requires-Dist: python-box (>=6.1.0)
 Requires-Dist: pytsql (>=1.1.4); extra == "mssql"
 Requires-Dist: sphinx-rtd-theme (>=1.0.0); extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc (>=0.3.0); extra == "docs"
 Requires-Dist: structlog (>=22.1.0)
+Requires-Dist: tidypolars (>=0.2.19); extra == "polars"
 Requires-Dist: tomli (>=2.0.1)
 Requires-Dist: typing-extensions (>=4.1.0,<5)
 Description-Content-Type: text/markdown
 
 # pydiverse.pipedag
 
 [![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml)
```

