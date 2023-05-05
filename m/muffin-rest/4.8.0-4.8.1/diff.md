# Comparing `tmp/muffin_rest-4.8.0.tar.gz` & `tmp/muffin_rest-4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-4.8.0.tar", max compression
+gzip compressed data, was "muffin_rest-4.8.1.tar", max compression
```

## Comparing `muffin_rest-4.8.0.tar` & `muffin_rest-4.8.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1082 2023-03-23 10:24:47.941083 muffin_rest-4.8.0/LICENSE
--rw-r--r--   0        0        0     2616 2023-03-23 10:24:47.941083 muffin_rest-4.8.0/README.rst
--rw-r--r--   0        0        0     1242 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/errors.py
--rw-r--r--   0        0        0     5051 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/filters.py
--rw-r--r--   0        0        0    10377 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/handler.py
--rw-r--r--   0        0        0     4842 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8808 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/options.py
--rw-r--r--   0        0        0     5372 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     3058 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     1111 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1644 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0        0 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2526 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6397 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3038 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     4058 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/swagger.html
--rw-r--r--   0        0        0      455 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/types.py
--rw-r--r--   0        0        0     2070 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/muffin_rest/utils.py
--rw-r--r--   0        0        0     2707 2023-03-23 10:24:47.945083 muffin_rest-4.8.0/pyproject.toml
--rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 muffin_rest-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/LICENSE
+-rw-r--r--   0        0        0     2616 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/README.rst
+-rw-r--r--   0        0        0     1242 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5051 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10377 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4842 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8808 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/options.py
+-rw-r--r--   0        0        0     5372 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     3055 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     1111 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1076 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     2270 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0        0 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2515 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6397 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3038 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     4058 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      455 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/types.py
+-rw-r--r--   0        0        0     2070 2023-05-04 11:10:45.082423 muffin_rest-4.8.1/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2707 2023-05-04 11:10:45.086423 muffin_rest-4.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 muffin_rest-4.8.1/PKG-INFO
```

### Comparing `muffin_rest-4.8.0/LICENSE` & `muffin_rest-4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/README.rst` & `muffin_rest-4.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/__init__.py` & `muffin_rest-4.8.1/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/api.py` & `muffin_rest-4.8.1/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/errors.py` & `muffin_rest-4.8.1/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/filters.py` & `muffin_rest-4.8.1/muffin_rest/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/handler.py` & `muffin_rest-4.8.1/muffin_rest/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/mongo/__init__.py` & `muffin_rest-4.8.1/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/mongo/filters.py` & `muffin_rest-4.8.1/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/mongo/schema.py` & `muffin_rest-4.8.1/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/mongo/sorting.py` & `muffin_rest-4.8.1/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/mongo/utils.py` & `muffin_rest-4.8.1/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/openapi.py` & `muffin_rest-4.8.1/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/options.py` & `muffin_rest-4.8.1/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/peewee/__init__.py` & `muffin_rest-4.8.1/muffin_rest/peewee/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/peewee/filters.py` & `muffin_rest-4.8.1/muffin_rest/peewee/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Support filters for Peewee ORM."""
 from __future__ import annotations
 
 import operator
-from typing import TYPE_CHECKING, Any, Callable, Optional, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Optional, Tuple, Type, Union, cast
 
 from peewee import Field, ModelSelect
 
 from muffin_rest.filters import Filter, Filters
 
 if TYPE_CHECKING:
     import marshmallow as ma
@@ -45,18 +45,15 @@
         self.schema_field = schema_field or self.schema_field_cls(
             attribute=field and field.name or name,
         )
         if operator:
             self.default_operator = operator
 
     async def filter(
-        self,
-        collection: ModelSelect,
-        *ops: Tuple[Callable, Any],
-        **kwargs,
+        self, collection: ModelSelect, *ops: Tuple[Callable, Any], **kwargs
     ) -> ModelSelect:
         """Apply the filters to Peewee QuerySet.."""
         if self.field and ops:
             return self.query(collection, self.field, *ops, **kwargs)
         return collection
 
     def query(self, qs: ModelSelect, column: Field, *ops: Tuple, **_) -> ModelSelect:
@@ -66,15 +63,15 @@
 
         return qs
 
 
 class PWFilters(Filters):
     """Bind Peewee filter class."""
 
-    MUTATE_CLASS = PWFilter
+    MUTATE_CLASS: Type[PWFilter] = PWFilter
 
     def convert(self, obj: Union[str, Field, PWFilter], **meta):
         """Convert params to filters."""
         from . import PWRESTHandler
 
         handler = cast(PWRESTHandler, self.handler)
         model_meta = handler.meta.model._meta  # type: ignore[]
```

### Comparing `muffin_rest-4.8.0/muffin_rest/peewee/openapi.py` & `muffin_rest-4.8.1/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/peewee/options.py` & `muffin_rest-4.8.1/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/peewee/schemas.py` & `muffin_rest-4.8.1/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/peewee/sorting.py` & `muffin_rest-4.8.1/muffin_rest/sqlalchemy/sorting.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,63 @@
-"""Support sorting for Peewee ORM."""
-
+"""Support sorting for SQLAlchemy ORM."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Union, cast
 
-from peewee import Field
+from sqlalchemy import Column
 
 from muffin_rest.sorting import Sort, Sorting
 
 if TYPE_CHECKING:
     from .types import TVCollection
 
 
-class PWSort(Sort):
+class SASort(Sort):
     """Sorter for Peewee."""
 
     async def apply(
-        self,
-        collection: TVCollection,
-        *,
-        desc: bool = False,
-        **_,
+        self, collection: TVCollection, *, desc: bool = False, **_,
     ) -> TVCollection:
         """Sort the collection."""
-        return collection.order_by_extend(self.field if not desc else self.field.desc())
+        field = self.field
+        if desc and isinstance(field, Column):
+            field = field.desc()
+
+        return collection.order_by(field)
 
 
-class PWSorting(Sorting):
+class SASorting(Sorting):
     """Sort Peewee ORM Queries."""
 
-    MUTATE_CLASS = PWSort
+    MUTATE_CLASS = SASort
 
-    def convert(self, obj: Union[str, Field, PWSort], **meta):
+    def convert(self, obj: Union[str, Column, SASort], **meta):
         """Prepare sorters."""
-        from . import PWRESTHandler
+        from . import SARESTHandler
 
-        if isinstance(obj, PWSort):
+        if isinstance(obj, SASort):
             return obj
 
-        handler = cast(PWRESTHandler, self.handler)
-        model_meta = handler.meta.model._meta  # type: ignore[]
+        handler = cast(SARESTHandler, self.handler)
 
-        if isinstance(obj, Field):
+        if isinstance(obj, Column):
             name, field = obj.name, obj
 
         else:
             name = obj
-            field = meta.get("field", model_meta.fields.get(name))
+            field = meta.get("field", handler.meta.table.c.get(name))
 
-        if field:
+        if field is not None:
             sort = self.MUTATE_CLASS(name, field=field, **meta)
             if sort.meta.get("default"):
                 self.default.append(sort)
 
             return sort
 
     def sort_default(self, collection: TVCollection) -> TVCollection:
         """Sort collection by default."""
-        sorting = [
-            sort.field.desc() if sort.meta["default"] == "desc" else sort.field
-            for sort in self.default
-        ]
-        return collection.order_by(*sorting)
+        return collection.order_by(
+            *[
+                sort.field.desc() if sort.meta["default"] == "desc" else sort.field
+                for sort in self.default
+            ],
+        )
```

### Comparing `muffin_rest-4.8.0/muffin_rest/redoc.html` & `muffin_rest-4.8.1/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/sorting.py` & `muffin_rest-4.8.1/muffin_rest/sorting.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,25 +42,23 @@
 
     def __init__(self, handler: Type[RESTBase], params: Iterable):
         """Initialize the sorting."""
         self.default: List[Sort] = []
         super(Sorting, self).__init__(handler, params)
 
     async def apply(
-        self,
-        request: Request,
-        collection: TVCollection,
-        **_,
+        self, request: Request, collection: TVCollection, **_
     ) -> TVCollection:
         """Sort the given collection."""
         data = request.url.query.get(SORT_PARAM)
         if data:
             for name, desc in to_sort(data.split(",")):
-                if name in self.mutations:
-                    collection = await self.mutations[name].apply(collection, desc=desc)
+                sort = self.mutations.get(name)
+                if sort:
+                    collection = await sort.apply(collection, desc=desc)
 
         elif self.default:
             return self.sort_default(collection)
 
         return collection
 
     def convert(self, obj, **meta) -> Sort:
```

### Comparing `muffin_rest-4.8.0/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-4.8.1/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-4.8.1/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/swagger.html` & `muffin_rest-4.8.1/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/muffin_rest/utils.py` & `muffin_rest-4.8.1/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.8.0/pyproject.toml` & `muffin_rest-4.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "4.8.0"
+version = "4.8.1"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-4.8.0/PKG-INFO` & `muffin_rest-4.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 4.8.0
+Version: 4.8.1
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

