# Comparing `tmp/lancedb-0.1.1.tar.gz` & `tmp/lancedb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.1.1.tar", last modified: Thu Apr 27 00:01:10 2023, max compression
+gzip compressed data, was "lancedb-0.1.2.tar", last modified: Fri May  5 18:28:58 2023, max compression
```

## Comparing `lancedb-0.1.1.tar` & `lancedb-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-27 00:01:10.529805 lancedb-0.1.1/
--rw-r--r--   0 changshe   (501) staff       (20)      996 2023-04-27 00:01:10.529662 lancedb-0.1.1/PKG-INFO
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-27 00:01:10.528124 lancedb-0.1.1/lancedb/
--rw-r--r--   0 changshe   (501) staff       (20)      922 2023-03-18 17:14:30.000000 lancedb-0.1.1/lancedb/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)      889 2023-03-22 23:02:41.000000 lancedb-0.1.1/lancedb/common.py
--rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-03-24 06:56:52.000000 lancedb-0.1.1/lancedb/context.py
--rw-r--r--   0 changshe   (501) staff       (20)     3058 2023-04-20 04:26:50.000000 lancedb-0.1.1/lancedb/db.py
--rw-r--r--   0 changshe   (501) staff       (20)     3721 2023-04-25 01:36:57.000000 lancedb-0.1.1/lancedb/embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     3970 2023-04-26 23:53:57.000000 lancedb-0.1.1/lancedb/query.py
--rw-r--r--   0 changshe   (501) staff       (20)     7884 2023-04-26 23:53:57.000000 lancedb-0.1.1/lancedb/table.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-27 00:01:10.528675 lancedb-0.1.1/lancedb.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)      996 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      386 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)      150 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)        8 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1325 2023-04-26 23:55:01.000000 lancedb-0.1.1/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-04-27 00:01:10.529843 lancedb-0.1.1/setup.cfg
--rw-r--r--   0 changshe   (501) staff       (20)      660 2023-03-23 18:53:47.000000 lancedb-0.1.1/setup.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-27 00:01:10.529463 lancedb-0.1.1/tests/
--rw-r--r--   0 changshe   (501) staff       (20)     2796 2023-04-20 04:26:50.000000 lancedb-0.1.1/tests/test_db.py
--rw-r--r--   0 changshe   (501) staff       (20)     1527 2023-03-31 02:15:49.000000 lancedb-0.1.1/tests/test_embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     2457 2023-04-26 23:53:57.000000 lancedb-0.1.1/tests/test_query.py
--rw-r--r--   0 changshe   (501) staff       (20)     3763 2023-04-20 04:26:50.000000 lancedb-0.1.1/tests/test_table.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-05 18:28:58.093741 lancedb-0.1.2/
+-rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-05-05 18:28:58.093630 lancedb-0.1.2/PKG-INFO
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-05 18:28:58.092912 lancedb-0.1.2/lancedb/
+-rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.2/lancedb/__init__.py
+-rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.2/lancedb/common.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.2/lancedb/context.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3377 2023-05-05 18:26:36.000000 lancedb-0.1.2/lancedb/db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.2/lancedb/embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3970 2023-05-05 01:55:15.000000 lancedb-0.1.2/lancedb/query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     7884 2023-05-05 18:26:36.000000 lancedb-0.1.2/lancedb/table.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1376 2023-05-05 01:55:15.000000 lancedb-0.1.2/lancedb/util.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-05-05 18:28:58.093464 lancedb-0.1.2/lancedb.egg-info/
+-rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)      320 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        1 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 changshe   (501) staff       (20)      150 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/requires.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        8 2023-05-05 18:28:58.000000 lancedb-0.1.2/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 changshe   (501) staff       (20)     1332 2023-05-05 18:25:41.000000 lancedb-0.1.2/pyproject.toml
+-rw-r--r--   0 changshe   (501) staff       (20)       38 2023-05-05 18:28:58.093779 lancedb-0.1.2/setup.cfg
+-rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.2/setup.py
```

### Comparing `lancedb-0.1.1/PKG-INFO` & `lancedb-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.1
+Version: 0.1.2
 Summary: lancedb
-Author-email: Lance Devs <dev@eto.ai>
+Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lancedb-0.1.1/lancedb/__init__.py` & `lancedb-0.1.2/lancedb/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from .db import LanceDBConnection, URI
+from .db import URI, LanceDBConnection
 
 
 def connect(uri: URI) -> LanceDBConnection:
     """Connect to a LanceDB instance at the given URI
 
     Parameters
     ----------
```

### Comparing `lancedb-0.1.1/lancedb/common.py` & `lancedb-0.1.2/lancedb/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from pathlib import Path
-from typing import Union, List
+from typing import List, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 
 VEC = Union[list, np.ndarray, pa.Array, pa.ChunkedArray]
 URI = Union[str, Path]
```

### Comparing `lancedb-0.1.1/lancedb/context.py` & `lancedb-0.1.2/lancedb/context.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.1/lancedb/db.py` & `lancedb-0.1.2/lancedb/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,44 +10,52 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 from pathlib import Path
+
 import pyarrow as pa
 
-from .common import URI, DATA
+from .common import DATA, URI
 from .table import LanceTable
+from .util import get_uri_scheme
 
 
 class LanceDBConnection:
     """
     A connection to a LanceDB database.
     """
 
     def __init__(self, uri: URI):
-        if isinstance(uri, str):
-            uri = Path(uri)
-        uri = uri.expanduser().absolute()
-        Path(uri).mkdir(parents=True, exist_ok=True)
+        is_local = isinstance(uri, Path) or get_uri_scheme(uri) == "file"
+        if is_local:
+            if isinstance(uri, str):
+                uri = Path(uri)
+            uri = uri.expanduser().absolute()
+            Path(uri).mkdir(parents=True, exist_ok=True)
         self._uri = str(uri)
 
     @property
     def uri(self) -> str:
         return self._uri
 
     def table_names(self) -> list[str]:
         """Get the names of all tables in the database.
 
         Returns
         -------
         A list of table names.
         """
-        return [p.stem for p in Path(self.uri).glob("*.lance")]
+        if get_uri_scheme(self.uri) == "file":
+            return [p.stem for p in Path(self.uri).glob("*.lance")]
+        raise NotImplementedError(
+            "List table_names is only supported for local filesystem for now"
+        )
 
     def __len__(self) -> int:
         return len(self.table_names())
 
     def __contains__(self, name: str) -> bool:
         return name in self.table_names()
```

### Comparing `lancedb-0.1.1/lancedb/embeddings.py` & `lancedb-0.1.2/lancedb/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import math
 import sys
-
-from retry import retry
 from typing import Callable, Union
 
-from lance.vector import vec_to_table
 import numpy as np
 import pandas as pd
 import pyarrow as pa
+from lance.vector import vec_to_table
+from retry import retry
 
 
 def with_embeddings(
     func: Callable,
     data: Union[pa.Table, pd.DataFrame],
     column: str = "text",
     wrap_api: bool = True,
@@ -64,15 +63,17 @@
 
             def embed_func(c):
                 return self.func(c.tolist())
 
         if len(self.rate_limiter_kwargs) > 0:
             v = int(sys.version_info.minor)
             if v >= 11:
-                print("WARNING: rate limit only support up to 3.10, proceeding without rate limiter")
+                print(
+                    "WARNING: rate limit only support up to 3.10, proceeding without rate limiter"
+                )
             else:
                 import ratelimiter
 
                 max_calls = self.rate_limiter_kwargs["max_calls"]
                 limiter = ratelimiter.RateLimiter(
                     max_calls, period=self.rate_limiter_kwargs["period"]
                 )
```

### Comparing `lancedb-0.1.1/lancedb/query.py` & `lancedb-0.1.2/lancedb/query.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.1/lancedb/table.py` & `lancedb-0.1.2/lancedb/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 import os
 from functools import cached_property
 
 import lance
 import numpy as np
 import pandas as pd
-from lance import LanceDataset
 import pyarrow as pa
+from lance import LanceDataset
 from lance.vector import vec_to_table
 
+from .common import DATA, VEC, VECTOR_COLUMN_NAME
 from .query import LanceQueryBuilder
-from .common import DATA, VECTOR_COLUMN_NAME, VEC
 
 
 def _sanitize_data(data, schema):
     if isinstance(data, list):
         data = pa.Table.from_pylist(data)
         data = _sanitize_schema(data, schema=schema)
     if isinstance(data, dict):
```

### Comparing `lancedb-0.1.1/lancedb.egg-info/PKG-INFO` & `lancedb-0.1.2/lancedb.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.1
+Version: 0.1.2
 Summary: lancedb
-Author-email: Lance Devs <dev@eto.ai>
+Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lancedb-0.1.1/pyproject.toml` & `lancedb-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "lancedb"
-version = "0.1.1"
-dependencies = ["pylance>=0.4.4", "ratelimiter", "retry", "tqdm"]
+version = "0.1.2"
+dependencies = ["pylance>=0.4.6", "ratelimiter", "retry", "tqdm"]
 description = "lancedb"
 authors = [
-    { name = "Lance Devs", email = "dev@eto.ai" },
+    { name = "LanceDB Devs", email = "dev@lancedb.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "data-format",
     "data-science",
```

### Comparing `lancedb-0.1.1/setup.py` & `lancedb-0.1.2/setup.py`

 * *Files identical despite different names*

