# Comparing `tmp/muffin_rest-4.8.8.tar.gz` & `tmp/muffin_rest-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-4.8.8.tar", max compression
+gzip compressed data, was "muffin_rest-4.9.0.tar", max compression
```

## Comparing `muffin_rest-4.8.8.tar` & `muffin_rest-4.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1082 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/LICENSE
--rw-r--r--   0        0        0     2616 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/README.rst
--rw-r--r--   0        0        0     1242 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/errors.py
--rw-r--r--   0        0        0     5187 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/filters.py
--rw-r--r--   0        0        0    10377 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/handler.py
--rw-r--r--   0        0        0     4842 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8808 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/options.py
--rw-r--r--   0        0        0     5372 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2418 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     1111 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     2266 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0        0 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2515 2023-05-05 06:07:27.747536 muffin_rest-4.8.8/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6397 2023-05-05 06:07:27.751536 muffin_rest-4.8.8/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-05-05 06:07:27.751536 muffin_rest-4.8.8/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-05-05 06:07:27.751536 muffin_rest-4.8.8/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-05-05 06:07:27.751536 muffin_rest-4.8.8/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     4058 2023-05-05 06:07:27.751536 muffin_rest-4.8.8/muffin_rest/swagger.html
--rw-r--r--   0        0        0      455 2023-05-05 06:07:27.751536 muffin_rest-4.8.8/muffin_rest/types.py
--rw-r--r--   0        0        0     2113 2023-05-05 06:07:27.751536 muffin_rest-4.8.8/muffin_rest/utils.py
--rw-r--r--   0        0        0     2670 2023-05-05 06:07:27.751536 muffin_rest-4.8.8/pyproject.toml
--rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 muffin_rest-4.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-05 06:47:12.394818 muffin_rest-4.9.0/LICENSE
+-rw-r--r--   0        0        0     2616 2023-05-05 06:47:12.394818 muffin_rest-4.9.0/README.rst
+-rw-r--r--   0        0        0     1242 2023-05-05 06:47:12.394818 muffin_rest-4.9.0/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-05-05 06:47:12.394818 muffin_rest-4.9.0/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5212 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10372 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4842 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8808 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/options.py
+-rw-r--r--   0        0        0     5372 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2418 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     1111 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1076 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1780 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2813 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6397 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2460 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     4058 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      455 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/types.py
+-rw-r--r--   0        0        0     2081 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2670 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 muffin_rest-4.9.0/PKG-INFO
```

### Comparing `muffin_rest-4.8.8/LICENSE` & `muffin_rest-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/README.rst` & `muffin_rest-4.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/__init__.py` & `muffin_rest-4.9.0/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/api.py` & `muffin_rest-4.9.0/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/errors.py` & `muffin_rest-4.9.0/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/filters.py` & `muffin_rest-4.9.0/muffin_rest/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Support API filters."""
 from __future__ import annotations
 
 import operator
-from typing import TYPE_CHECKING, Any, Callable, Dict, Mapping, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Dict, Mapping, Optional, Tuple  # py38
 
 import marshmallow as ma
 from asgi_tools._compat import json_loads  # type: ignore[]
 
 from .utils import Mutate, Mutator
 
 if TYPE_CHECKING:
@@ -116,39 +116,36 @@
 
     """Build filters for handlers."""
 
     MUTATE_CLASS = Filter
     mutations: Mapping[str, Filter]
 
     async def apply(
-        self,
-        request: Request,
-        collection: TVCollection,
-        **options,
-    ) -> TVCollection:
+        self, request: Request, collection: TVCollection, **options
+    ) -> Tuple[TVCollection, Dict[str, Any]]:
         """Filter the given collection."""
         raw_data = request.url.query.get(FILTERS_PARAM)
+        filters = {}
         if raw_data is not None:
             try:
                 data = json_loads(raw_data)
                 assert isinstance(data, dict)
                 mutations = self.mutations
                 for name in data:
                     if name in mutations:
-                        _, collection = await mutations[name].apply(
-                            collection,
-                            data,
-                            **options,
+                        ops, collection = await mutations[name].apply(
+                            collection, data, **options
                         )
+                        filters[name] = ops
 
             except (ValueError, TypeError, AssertionError):
                 api = self.handler._api
                 api.logger.warning("Invalid filters data: %s", request.url)
 
-        return collection
+        return collection, filters
 
     def convert(self, obj, **meta):
         """Convert params to filters."""
         if isinstance(obj, self.MUTATE_CLASS):
             return obj
 
         field = meta.pop("field", None) or obj
```

### Comparing `muffin_rest-4.8.8/muffin_rest/handler.py` & `muffin_rest-4.9.0/muffin_rest/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     auth: Any
     collection: Any
     resource: Any
 
     meta: RESTOptions
     meta_class: Type[RESTOptions] = RESTOptions
     _api: Optional[API] = None
+    filters: Dict[str, Any] = {}
+    sorting: Dict[str, Any] = {}
 
     class Meta:
         """Tune the handler."""
 
         # Resource filters
         filters: Sequence[Union[str, Tuple[str, str], Filter]] = ()
 
@@ -101,19 +103,15 @@
         for _, method in inspect.getmembers(cls, lambda m: hasattr(m, "__route__")):
             cpaths, cparams = method.__route__
             router.bind(cls, *cpaths, __meth__=method.__name__, **cparams)
 
         return cls
 
     async def __call__(
-        self,
-        request: Request,
-        *,
-        __meth__: Optional[str] = None,
-        **options,
+        self, request: Request, *, __meth__: Optional[str] = None, **options
     ) -> Any:
         """Dispatch the given request by HTTP method."""
         method = getattr(self, __meth__ or request.method.lower())
         self.auth = await self.authorize(request)
         self.collection = await self.prepare_collection(request)
         resource = await self.prepare_resource(request)
         if resource or request.method != "GET":
@@ -122,26 +120,22 @@
             except ValidationError as exc:
                 raise APIError.BAD_REQUEST("Invalid data", errors=exc.messages) from exc
 
         meta = self.meta
 
         # Filter collection
         if meta.filters:
-            self.collection = await meta.filters.apply(
-                request,
-                self.collection,
-                **options,
+            self.collection, self.filters = await meta.filters.apply(
+                request, self.collection, **options
             )
 
         # Sort collection
         if meta.sorting:
-            self.collection = await meta.sorting.apply(
-                request,
-                self.collection,
-                **options,
+            self.collection, self.sorting = await meta.sorting.apply(
+                request, self.collection, **options
             )
 
         # Paginate the collection
         headers = {}
         if meta.limit:
             limit, offset = self.paginate_prepare_params(request)
             if limit and offset >= 0:
```

### Comparing `muffin_rest-4.8.8/muffin_rest/mongo/__init__.py` & `muffin_rest-4.9.0/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/mongo/filters.py` & `muffin_rest-4.9.0/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/mongo/schema.py` & `muffin_rest-4.9.0/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/mongo/sorting.py` & `muffin_rest-4.9.0/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/mongo/utils.py` & `muffin_rest-4.9.0/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/openapi.py` & `muffin_rest-4.9.0/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/options.py` & `muffin_rest-4.9.0/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/peewee/__init__.py` & `muffin_rest-4.9.0/muffin_rest/peewee/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/peewee/filters.py` & `muffin_rest-4.9.0/muffin_rest/peewee/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/peewee/openapi.py` & `muffin_rest-4.9.0/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/peewee/options.py` & `muffin_rest-4.9.0/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/peewee/schemas.py` & `muffin_rest-4.9.0/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/peewee/sorting.py` & `muffin_rest-4.9.0/muffin_rest/peewee/sorting.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Type, Union, cast
 
 from peewee import Field
 
-from muffin_rest.sorting import SORT_PARAM, Sort, Sorting, to_sort
+from muffin_rest.sorting import Sort, Sorting
 
 if TYPE_CHECKING:
-    from muffin import Request
-
     from .types import TVCollection
 
 
 class PWSort(Sort):
     """Sorter for Peewee."""
 
     async def apply(
@@ -25,30 +23,17 @@
 
 
 class PWSorting(Sorting):
     """Sort Peewee ORM Queries."""
 
     MUTATE_CLASS: Type[PWSort] = PWSort
 
-    async def apply(
-        self, request: Request, collection: TVCollection, **_
-    ) -> TVCollection:
-        """Sort the given collection. Reset sorting."""
-        data = request.url.query.get(SORT_PARAM)
-        if data:
-            collection = collection.order_by()
-            for name, desc in to_sort(data.split(",")):
-                sort = self.mutations.get(name)
-                if sort:
-                    collection = await sort.apply(collection, desc=desc)
-
-        elif self.default:
-            return self.sort_default(collection)
-
-        return collection
+    def prepare(self, collection: TVCollection) -> TVCollection:
+        """Prepare collection for sorting."""
+        return collection.order_by()
 
     def convert(self, obj: Union[str, Field, PWSort], **meta):
         """Prepare sorters."""
         from . import PWRESTHandler
 
         if isinstance(obj, PWSort):
             return obj
```

### Comparing `muffin_rest-4.8.8/muffin_rest/redoc.html` & `muffin_rest-4.9.0/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/sorting.py` & `muffin_rest-4.9.0/muffin_rest/sorting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implement sorting."""
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
+    Dict,
     Generator,
     Iterable,
     List,
     Mapping,
     Sequence,
     Tuple,
     Type,
@@ -43,26 +44,33 @@
     def __init__(self, handler: Type[RESTBase], params: Iterable):
         """Initialize the sorting."""
         self.default: List[Sort] = []
         super(Sorting, self).__init__(handler, params)
 
     async def apply(
         self, request: Request, collection: TVCollection, **_
-    ) -> TVCollection:
+    ) -> Tuple[TVCollection, Dict[str, Any]]:
         """Sort the given collection."""
         data = request.url.query.get(SORT_PARAM)
+        sorting = {}
         if data:
+            collection = self.prepare(collection)
             for name, desc in to_sort(data.split(",")):
                 sort = self.mutations.get(name)
                 if sort:
                     collection = await sort.apply(collection, desc=desc)
+                    sorting[sort.name] = desc
 
         elif self.default:
-            return self.sort_default(collection)
+            return self.sort_default(collection), sorting
 
+        return collection, sorting
+
+    def prepare(self, collection: TVCollection) -> TVCollection:
+        """Prepare the collection."""
         return collection
 
     def convert(self, obj, **meta) -> Sort:
         """Prepare sorters."""
         sort = cast(Sort, super(Sorting, self).convert(obj, **meta))
         if sort.meta.get("default"):
             self.default.append(sort)
```

### Comparing `muffin_rest-4.8.8/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-4.9.0/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-4.9.0/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-4.9.0/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/swagger.html` & `muffin_rest-4.9.0/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.8/muffin_rest/utils.py` & `muffin_rest-4.9.0/muffin_rest/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """REST Utils."""
 from __future__ import annotations
 
 import abc
-from typing import TYPE_CHECKING, Any, Iterable, Mapping, Type
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Mapping, Tuple, Type
 
 if TYPE_CHECKING:
     from muffin import Request
 
     from muffin_rest.types import TVCollection
 
 
 class Mutate(abc.ABC):
     """Mutate collections."""
 
-    __slots__ = ("name", "field", "meta")
-
     def __init__(self, name: str, *, field=None, **meta):
         """Initialize a name."""
         self.name = name
         self.field: Any = name if field is None else field
         self.meta = meta
 
     def __str__(self):
@@ -68,14 +66,11 @@
         if isinstance(obj, self.MUTATE_CLASS):
             return obj
 
         return self.MUTATE_CLASS(obj, **meta)
 
     @abc.abstractmethod
     async def apply(
-        self,
-        request: Request,
-        collection: TVCollection,
-        **options,
-    ) -> TVCollection:
+        self, request: Request, collection: TVCollection, **options
+    ) -> Tuple[TVCollection, Dict[str, Any]]:
         """Mutate a collection."""
         raise NotImplementedError
```

### Comparing `muffin_rest-4.8.8/pyproject.toml` & `muffin_rest-4.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "4.8.8"
+version = "4.9.0"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-4.8.8/PKG-INFO` & `muffin_rest-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 4.8.8
+Version: 4.9.0
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

