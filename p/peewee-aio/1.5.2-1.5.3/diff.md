# Comparing `tmp/peewee_aio-1.5.2.tar.gz` & `tmp/peewee_aio-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_aio-1.5.2.tar", max compression
+gzip compressed data, was "peewee_aio-1.5.3.tar", max compression
```

## Comparing `peewee_aio-1.5.2.tar` & `peewee_aio-1.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4681 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/README.md
--rw-r--r--   0        0        0      132 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/databases.py
--rw-r--r--   0        0        0    17336 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/fields.py
--rw-r--r--   0        0        0    15756 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/manager.py
--rw-r--r--   0        0        0    17678 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/model.py
--rw-r--r--   0        0        0        0 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/py.typed
--rw-r--r--   0        0        0      268 2023-04-13 07:34:45.659423 peewee_aio-1.5.2/peewee_aio/types.py
--rw-r--r--   0        0        0     2585 2023-04-13 07:34:45.663423 peewee_aio-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 peewee_aio-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     4681 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/README.md
+-rw-r--r--   0        0        0      132 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/__init__.py
+-rw-r--r--   0        0        0     1210 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/databases.py
+-rw-r--r--   0        0        0    17336 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/fields.py
+-rw-r--r--   0        0        0    15580 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/manager.py
+-rw-r--r--   0        0        0    16604 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/model.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/py.typed
+-rw-r--r--   0        0        0      268 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/peewee_aio/types.py
+-rw-r--r--   0        0        0     2585 2023-05-05 06:28:33.153162 peewee_aio-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 peewee_aio-1.5.3/PKG-INFO
```

### Comparing `peewee_aio-1.5.2/README.md` & `peewee_aio-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.2/peewee_aio/databases.py` & `peewee_aio-1.5.3/peewee_aio/databases.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.2/peewee_aio/fields.py` & `peewee_aio-1.5.3/peewee_aio/fields.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.2/peewee_aio/manager.py` & `peewee_aio-1.5.3/peewee_aio/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,15 @@
 
 class Manager(Database):
     """Manage database and models."""
 
     pw_database: PWDatabase
     models: "WeakSet[Type[PWModel]]"
 
-    def __init__(
-        self,
-        url: str,
-        **backend_options,
-    ):
+    def __init__(self, url: str, **backend_options):
         """Initialize dialect and database."""
         backend_options.setdefault("convert_params", True)
         super().__init__(url, logger=logger, **backend_options)
 
         self.models = WeakSet()
         self.pw_database = get_db(self)
 
@@ -258,34 +254,26 @@
         models_cls = models_cls or tuple(self.models)
         for model_cls in reversed(sort_models(models_cls)):
             schema: SchemaManager = model_cls._schema
             ctx = schema._drop_table(**opts)  # type: ignore[]
             await self.execute(ctx)
 
     async def get_or_none(
-        self,
-        model_cls: Type[TVModel],
-        *args: Node,
-        **kwargs,
+        self, model_cls: Type[TVModel], *args: Node, **kwargs
     ) -> Optional[TVModel]:
         query: ModelSelect = model_cls.select()
         if kwargs:
             query = query.filter(**kwargs)
 
         if args:
             query = query.where(*args)  # type: ignore[]
 
         return await self.fetchone(query)
 
-    async def get(
-        self,
-        model_cls: Type[TVModel],
-        *args: Node,
-        **kwargs,
-    ) -> TVModel:
+    async def get(self, model_cls: Type[TVModel], *args: Node, **kwargs) -> TVModel:
         res = await self.get_or_none(model_cls, *args, **kwargs)
         if res is None:
             raise model_cls.DoesNotExist  # type: ignore[]
         return res
 
     async def get_by_id(self, model_cls: Type[TVModel], pk) -> TVModel:
         return await self.get(model_cls, model_cls._meta.primary_key == pk)  # type: ignore[]
@@ -300,18 +288,15 @@
 
     async def delete_by_id(self, model_cls: Type[PWModel], pk):
         return await self.execute(
             model_cls.delete().where(model_cls._meta.primary_key == pk),  # type: ignore[]
         )
 
     async def get_or_create(
-        self,
-        model_cls: Type[TVModel],
-        defaults: Optional[Dict] = None,
-        **kwargs,
+        self, model_cls: Type[TVModel], defaults: Optional[Dict] = None, **kwargs
     ) -> Tuple[TVModel, bool]:
         async with self.transaction():
             try:
                 return (await self.get(model_cls, **kwargs), False)
             except model_cls.DoesNotExist:  # type: ignore[]
                 return (
                     await self.create(model_cls, **dict(defaults or {}, **kwargs)),
@@ -381,19 +366,15 @@
             if pk is not None and (meta.auto_increment or pk_value is None):
                 inst._pk = pk  # type: ignore[]
 
         inst._dirty.clear()  # type: ignore[]
         return inst
 
     async def delete_instance(
-        self,
-        inst: PWModel,
-        *,
-        recursive: bool = False,
-        delete_nullable: bool = False,
+        self, inst: PWModel, *, recursive: bool = False, delete_nullable: bool = False
     ):
         if recursive:
             for query, fk in reversed(list(inst.dependencies(delete_nullable))):
                 if fk.null and not delete_nullable:
                     await self.execute(fk.model.update(**{fk.name: None}).where(query))
 
                 else:
@@ -457,18 +438,15 @@
 
     __slots__ = "query", "processor"
 
     def __init__(self, query: BaseQuery):
         self.query = query
         self.processor: Optional[Callable] = None
 
-    def __call__(
-        self,
-        res: Union[Mapping, Sequence[Mapping]],
-    ) -> Union[Any, Sequence[Any]]:
+    def __call__(self, res: Union[Mapping, Sequence[Mapping]]) -> Union[Any, Sequence[Any]]:
         """Process rows."""
         if not res:  # None or empty sequence
             return res
 
         if isinstance(res, Sequence):
             processor = self.get_processor(res[0])
             return [processor(r) for r in res]
```

### Comparing `peewee_aio-1.5.2/peewee_aio/model.py` & `peewee_aio-1.5.3/peewee_aio/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -131,19 +131,15 @@
         return await cls._manager.create_tables(cls, safe=safe, **kwargs)
 
     @classmethod
     async def drop_table(cls, *, safe=True, **kwargs):
         return await cls._manager.drop_tables(cls, safe=safe, **kwargs)
 
     @classmethod
-    async def get_or_none(
-        cls: Type[TVAIOModel],
-        *args: Node,
-        **kwargs,
-    ) -> Optional[TVAIOModel]:
+    async def get_or_none(cls: Type[TVAIOModel], *args: Node, **kwargs) -> Optional[TVAIOModel]:
         return await cls._manager.get_or_none(cls, *args, **kwargs)
 
     @classmethod
     async def get(cls: Type[TVAIOModel], *args: Node, **kwargs) -> TVAIOModel:
         return await cls._manager.get(cls, *args, **kwargs)
 
     @classmethod
@@ -156,17 +152,15 @@
 
     @classmethod
     async def delete_by_id(cls, pk):
         return await cls._manager.delete_by_id(cls, pk)
 
     @classmethod
     async def get_or_create(
-        cls: Type[TVAIOModel],
-        defaults: Optional[Dict[str, Any]] = None,
-        **kwargs,
+        cls: Type[TVAIOModel], defaults: Optional[Dict[str, Any]] = None, **kwargs
     ) -> Tuple[TVAIOModel, bool]:
         async with cls._manager.transaction():
             try:
                 return (await cls.get(**kwargs), False)
             except cls.DoesNotExist:
                 return (await cls.create(**dict(defaults or {}, **kwargs)), True)
 
@@ -249,56 +243,43 @@
         return n
 
     # Queryset methods
     # ----------------
 
     @classmethod
     def select(
-        cls: Type[TVAIOModel],
-        *select: Union[Type[Model], ColumnBase, Table, ModelAlias],
+        cls: Type[TVAIOModel], *select: Union[Type[Model], ColumnBase, Table, ModelAlias]
     ) -> AIOModelSelect[TVAIOModel]:
         return AIOModelSelect(
             cls,
             select or cls._meta.sorted_fields,
             is_default=not select,
         )
 
     @classmethod
-    def update(
-        cls: Type[TVAIOModel],
-        __data=None,
-        **update,
-    ) -> AIOModelUpdate[TVAIOModel]:
+    def update(cls: Type[TVAIOModel], __data=None, **update) -> AIOModelUpdate[TVAIOModel]:
         return AIOModelUpdate(cls, cls._normalize_data(__data, update))  # type: ignore[]
 
     @classmethod
-    def insert(
-        cls: Type[TVAIOModel],
-        __data=None,
-        **insert,
-    ) -> AIOModelInsert[TVAIOModel]:
+    def insert(cls: Type[TVAIOModel], __data=None, **insert) -> AIOModelInsert[TVAIOModel]:
         return AIOModelInsert(cls, cls._normalize_data(__data, insert))  # type: ignore[]
 
     @classmethod
     def insert_many(
-        cls: Type[TVAIOModel],
-        rows: Iterable,
-        fields=None,
+        cls: Type[TVAIOModel], rows: Iterable, fields=None
     ) -> AIOModelInsert[TVAIOModel]:
         if not rows:
             raise AIOModelInsert.DefaultValuesException("Error: no rows to insert.")
 
         rows = [row.__data__ if isinstance(row, Model) else row for row in rows]
         return AIOModelInsert(cls, insert=rows, columns=fields)
 
     @classmethod
     def insert_from(
-        cls: Type[TVAIOModel],
-        query: ModelSelect,
-        fields,
+        cls: Type[TVAIOModel], query: ModelSelect, fields
     ) -> AIOModelInsert[TVAIOModel]:
         columns = [getattr(cls, field) if isinstance(field, str) else field for field in fields]
         return AIOModelInsert(cls, insert=query, columns=columns)
 
     @classmethod
     def raw(cls: Type[TVAIOModel], sql, *params) -> AIOModelRaw[TVAIOModel]:
         return AIOModelRaw(cls, sql, params)
@@ -392,21 +373,18 @@
         return self.manager.run(self).__aiter__()  # type: ignore[return-value]
 
     @overload
     def __getitem__(self, value: int) -> Coroutine[Any, Any, TVAIOModel]:
         ...
 
     @overload
-    def __getitem__(self, value: slice) -> AIOModelSelect[TVAIOModel]:
+    def __getitem__(self, value: slice) -> Self:
         ...
 
-    def __getitem__(
-        self,
-        value,
-    ) -> Union[AIOModelSelect[TVAIOModel], Coroutine[Any, Any, TVAIOModel]]:
+    def __getitem__(self, value) -> Union[Self, Coroutine[Any, Any, TVAIOModel]]:
         limit, offset = 1, value
         if isinstance(value, slice):
             limit, offset = value.stop - value.start, value.start
 
         query = self.limit(limit).offset(offset)
         if limit == 1:
             return query.get()
@@ -455,69 +433,67 @@
             )
         return res
 
     if TYPE_CHECKING:
         _limit: Optional[int]
         _offset: Optional[int]
 
-        with_cte: Callable[..., AIOModelSelect[TVAIOModel]]
-        where: Callable[..., AIOModelSelect[TVAIOModel]]
-        filter: Callable[..., AIOModelSelect[TVAIOModel]]
-        orwhere: Callable[..., AIOModelSelect[TVAIOModel]]
-        order_by: Callable[..., AIOModelSelect[TVAIOModel]]
-        order_by_extend: Callable[..., AIOModelSelect[TVAIOModel]]
-        limit: Callable[[Union[int, None]], AIOModelSelect[TVAIOModel]]
-        offset: Callable[[int], AIOModelSelect[TVAIOModel]]
-        paginate: Callable[..., AIOModelSelect[TVAIOModel]]
-
-        columns: Callable[..., AIOModelSelect[TVAIOModel]]
-        select_extend: Callable[..., AIOModelSelect[TVAIOModel]]
-        from_: Callable[..., AIOModelSelect[TVAIOModel]]
-        join: Callable[..., AIOModelSelect[TVAIOModel]]
-        join_from: Callable[..., AIOModelSelect[TVAIOModel]]
-        group_by: Callable[..., AIOModelSelect[TVAIOModel]]
-        having: Callable[..., AIOModelSelect[TVAIOModel]]
-        distinct: Callable[..., AIOModelSelect[TVAIOModel]]
-        window: Callable[..., AIOModelSelect[TVAIOModel]]
-        for_update: Callable[..., AIOModelSelect[TVAIOModel]]
-        lateral: Callable[..., AIOModelSelect[TVAIOModel]]
+        with_cte: Callable[..., Self]
+        where: Callable[..., Self]
+        filter: Callable[..., Self]
+        orwhere: Callable[..., Self]
+        order_by: Callable[..., Self]
+        order_by_extend: Callable[..., Self]
+        limit: Callable[[Union[int, None]], Self]
+        offset: Callable[[int], Self]
+        paginate: Callable[..., Self]
+
+        columns: Callable[..., Self]
+        select_extend: Callable[..., Self]
+        from_: Callable[..., Self]
+        join: Callable[..., Self]
+        join_from: Callable[..., Self]
+        group_by: Callable[..., Self]
+        having: Callable[..., Self]
+        distinct: Callable[..., Self]
+        window: Callable[..., Self]
+        for_update: Callable[..., Self]
+        lateral: Callable[..., Self]
+        objects: Callable[..., Self]
 
         def __await__(self) -> Generator[Any, None, List[TVAIOModel]]:
             return self.manager.run(self).__await__()
 
 
-class AIOModelCompoundSelectQuery(
-    BaseModelSelect[TVAIOModel],
-    ModelCompoundSelectQuery,
-):
+class AIOModelCompoundSelectQuery(BaseModelSelect[TVAIOModel], ModelCompoundSelectQuery):
     if TYPE_CHECKING:
         _limit: Optional[int]
         _offset: Optional[int]
 
-        with_cte: Callable[..., AIOModelSelect[TVAIOModel]]
-        where: Callable[..., AIOModelSelect[TVAIOModel]]
-        filter: Callable[..., AIOModelSelect[TVAIOModel]]
-        orwhere: Callable[..., AIOModelSelect[TVAIOModel]]
-        order_by: Callable[..., AIOModelSelect[TVAIOModel]]
-        order_by_extend: Callable[..., AIOModelSelect[TVAIOModel]]
-        limit: Callable[[Union[int, None]], AIOModelSelect[TVAIOModel]]
-        offset: Callable[[int], AIOModelSelect[TVAIOModel]]
-        paginate: Callable[..., AIOModelSelect[TVAIOModel]]
-
-        columns: Callable[..., AIOModelSelect[TVAIOModel]]
-        select_extend: Callable[..., AIOModelSelect[TVAIOModel]]
-        from_: Callable[..., AIOModelSelect[TVAIOModel]]
-        join: Callable[..., AIOModelSelect[TVAIOModel]]
-        join_from: Callable[..., AIOModelSelect[TVAIOModel]]
-        group_by: Callable[..., AIOModelSelect[TVAIOModel]]
-        having: Callable[..., AIOModelSelect[TVAIOModel]]
-        distinct: Callable[..., AIOModelSelect[TVAIOModel]]
-        window: Callable[..., AIOModelSelect[TVAIOModel]]
-        for_update: Callable[..., AIOModelSelect[TVAIOModel]]
-        lateral: Callable[..., AIOModelSelect[TVAIOModel]]
+        with_cte: Callable[..., Self]
+        where: Callable[..., Self]
+        filter: Callable[..., Self]
+        orwhere: Callable[..., Self]
+        order_by: Callable[..., Self]
+        order_by_extend: Callable[..., Self]
+        limit: Callable[[Union[int, None]], Self]
+        offset: Callable[[int], Self]
+        paginate: Callable[..., Self]
+
+        columns: Callable[..., Self]
+        select_extend: Callable[..., Self]
+        from_: Callable[..., Self]
+        join: Callable[..., Self]
+        join_from: Callable[..., Self]
+        group_by: Callable[..., Self]
+        having: Callable[..., Self]
+        distinct: Callable[..., Self]
+        window: Callable[..., Self]
+        for_update: Callable[..., Self]
+        lateral: Callable[..., Self]
 
 
 class AIOModelUpdate(AIOQuery[TVAIOModel], ModelUpdate):
     if TYPE_CHECKING:
         where: Callable[..., AIOModelUpdate[TVAIOModel]]
         orwhere: Callable[..., AIOModelUpdate[TVAIOModel]]
         from_: Callable[..., AIOModelUpdate[TVAIOModel]]
```

### Comparing `peewee_aio-1.5.2/pyproject.toml` & `peewee_aio-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-aio"
-version = "1.5.2"
+version = "1.5.3"
 description = "Async support for Peewee ORM"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/klen/peewee-aio"
 repository = "https://github.com/klen/peewee-aio"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["peewee", "asyncio", "trio", "orm"]
```

### Comparing `peewee_aio-1.5.2/PKG-INFO` & `peewee_aio-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-aio
-Version: 1.5.2
+Version: 1.5.3
 Summary: Async support for Peewee ORM
 Home-page: https://github.com/klen/peewee-aio
 License: MIT
 Keywords: peewee,asyncio,trio,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

