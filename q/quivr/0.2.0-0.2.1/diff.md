# Comparing `tmp/quivr-0.2.0.tar.gz` & `tmp/quivr-0.2.1.tar.gz`

## Comparing `quivr-0.2.0.tar` & `quivr-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,16 @@
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/__init__.py~
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/__version__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/__version__.py~
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/concat.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/concat.py~
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/coordinates.py~
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/defragment.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/defragment.py~
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/errors.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/errors.py~
--rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/fields.py
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/fields.py~
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/indexing.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/indexing.py~
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/matrix.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/matrix.py~
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/models.py~
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/quiver.py~
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/schemagraph.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/schemagraph.py~
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/streaming.py~
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/struct_demo.py~
--rw-r--r--   0        0        0    17362 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/tables.py
--rw-r--r--   0        0        0    13287 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/tables.py~
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/tables2.py~
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 quivr-0.2.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.2.0/LICENSE
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 quivr-0.2.0/README.md
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 quivr-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 quivr-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/__version__.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/concat.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/defragment.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/errors.py
+-rw-r--r--   0        0        0    22772 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/fields.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/indexing.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/py.typed
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/schemagraph.py
+-rw-r--r--   0        0        0    17108 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/tables.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 quivr-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 quivr-0.2.1/README.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 quivr-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 quivr-0.2.1/PKG-INFO
```

### Comparing `quivr-0.2.0/quivr/__init__.py` & `quivr-0.2.1/quivr/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 from .concat import concatenate
-from .indexing import StringIndex
-from .matrix import MatrixArray, MatrixExtensionType
-from .tables import Table
 from .fields import (
+    BinaryField,
+    Date32Field,
+    Date64Field,
+    Decimal128Field,
+    Decimal256Field,
+    DictionaryField,
+    DurationField,
     Field,
-    SubTableField,
-    Int8Field,
-    Int16Field,
-    Int32Field,
-    Int64Field,
-    UInt8Field,
-    UInt16Field,
-    UInt32Field,
-    UInt64Field,
     Float16Field,
     Float32Field,
     Float64Field,
-    StringField,
+    Int16Field,
+    Int32Field,
+    Int64Field,
     LargeBinaryField,
+    LargeListField,
     LargeStringField,
-    Date32Field,
-    Date64Field,
-    TimestampField,
-    Time32Field,
-    Time64Field,
-    DurationField,
-    MonthDayNanoIntervalField,
-    BinaryField,
-    Decimal128Field,
-    Decimal256Field,
-    NullField,
     ListField,
-    LargeListField,
     MapField,
-    DictionaryField,
+    MonthDayNanoIntervalField,
+    NullField,
+    RunEndEncodedField,
+    StringField,
     StructField,
-    RunEndEncodedField
+    Time32Field,
+    Time64Field,
+    TimestampField,
+    UInt8Field,
+    UInt16Field,
+    UInt32Field,
+    UInt64Field,
 )
+from .indexing import StringIndex
+from .matrix import MatrixArray, MatrixExtensionType
 
 __all__ = [
     "TableBase",
     "MatrixArray",
     "MatrixExtensionType",
     "concatenate",
     "StringIndex",
     "Field",
-    "SubTableField"
-    "Int8Field",
+    "SubTableField" "Int8Field",
     "Int16Field",
     "Int32Field",
     "Int64Field",
     "UInt8Field",
     "UInt16Field",
     "UInt32Field",
     "UInt64Field",
@@ -72,9 +68,9 @@
     "Decimal256Field",
     "NullField",
     "ListField",
     "LargeListField",
     "MapField",
     "DictionaryField",
     "StructField",
-    "RunEndEncodedField"
+    "RunEndEncodedField",
 ]
```

### Comparing `quivr-0.2.0/quivr/concat.py` & `quivr-0.2.1/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.0/quivr/fields.py` & `quivr-0.2.1/quivr/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Optional, Union, TypeAlias, TYPE_CHECKING, TypeVar, Generic
+from typing import TYPE_CHECKING, Generic, Optional, TypeAlias, TypeVar, Union
 
 import pyarrow as pa
 
 if TYPE_CHECKING:
-    from .table import Table
+    from .tables import Table
 
 Byteslike: TypeAlias = Union[bytes, bytearray, memoryview, str]
 MetadataDict: TypeAlias = dict[Byteslike, Byteslike]
 
 
 class Field:
     """
@@ -18,14 +18,18 @@
         self.dtype = dtype
         self.nullable = nullable
         self.metadata = metadata
 
     def __get__(self, obj: "Table", objtype: type):
         return obj.table.column(self.name)
 
+    def __set__(self, obj: "Table", value):
+        idx = obj.table.schema.get_field_index(self.name)
+        obj.table = obj.table.set_column(idx, self.pyarrow_field(), [value])
+
     def __set_name__(self, owner: type, name: str):
         self.name = name
 
     def pyarrow_field(self):
         return pa.field(self.name, self.dtype, self.nullable, self.metadata)
```

### Comparing `quivr-0.2.0/quivr/indexing.py` & `quivr-0.2.1/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.0/quivr/matrix.py` & `quivr-0.2.1/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.0/quivr/schemagraph.py` & `quivr-0.2.1/quivr/schemagraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,7 @@
 
     for subfield in field.type:
         if pa.types.is_struct(subfield.type):
             _walk_schema(subfield, visitor, ancestors)
 
     ancestors.pop()
     visitor(field, ancestors)
-
```

### Comparing `quivr-0.2.0/quivr/tables.py` & `quivr-0.2.1/quivr/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-import functools
-from typing import Generic, TypeVar, TypeAlias, Union, Optional, Self, ClassVar, Any
-from io import IOBase
 import os
-
+from io import IOBase
+from typing import Any, ClassVar, Optional, Self, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.csv
 import pyarrow.feather
 import pyarrow.parquet
 
-from .fields import Field, SubTableField, MetadataDict
-from .schemagraph import _walk_schema
 from .errors import TableFragmentedError
+from .fields import Field, MetadataDict, SubTableField
+from .schemagraph import _walk_schema
 
 
 class Table:
     schema: ClassVar[pa.Schema]
     table: pa.Table
 
     def __init_subclass__(cls, **kwargs):
@@ -68,35 +66,30 @@
             >>> MyTable.from_data(a=np.array(["a", "b"]), b=np.array([1, 2]))
             MyTable(size=2)
         """
         if data is None:
             return cls.from_kwargs(**kwargs)
 
         if isinstance(data, pa.Table):
-            return cls(table=data)
+            return cls(pa_table=data)
         if isinstance(data, dict):
             return cls.from_pydict(data)
         if isinstance(data, list):
             if len(data) == 0:
                 return cls.from_rows(data)
             if isinstance(data[0], dict):
                 return cls.from_rows(data)
             elif isinstance(data[0], list):
                 return cls.from_lists(data)
         if isinstance(data, pd.DataFrame):
-            return cls.from_pandas(data)
+            return cls.from_dataframe(data)
         raise TypeError(f"Unsupported type: {type(data)}")
 
     @classmethod
-    def from_pydict(cls, data: dict[str, list], *args, **kwargs) -> Self:
-        table = pa.Table.from_pydict(data, schema=cls.schema)
-        return cls(table, *args, **kwargs)
-
-    @classmethod
-    def as_field(cls, nullable: bool = True, metadata: Optional[MetadataDict] = None) -> SubTableField:
+    def as_field(cls, nullable: bool = True, metadata: Optional[MetadataDict] = None) -> SubTableField[Self]:
         return SubTableField(cls, nullable=nullable, metadata=metadata)
 
     @classmethod
     def from_kwargs(cls, **kwargs) -> Self:
         """Create a Table instance from keyword arguments.
 
         Each keyword argument corresponds to a field in the Table.
@@ -137,20 +130,20 @@
 
     @classmethod
     def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]]) -> Self:
         table = pa.Table.from_pydict(d, schema=cls.schema)
         return cls(pa_table=table)
 
     @classmethod
-    def from_rows(cls, l: list[dict]) -> Self:
+    def from_rows(cls, rows: list[dict]) -> Self:
         """
         Create a Table object from a list of dictionaries.
 
         Args:
-            l: A list of values. Each value corresponds to a row in the table.
+            rows: A list of values. Each value corresponds to a row in the table.
 
         Returns:
             A Table object.
 
         Examples:
             >>> import quivr
             >>> class Inner(quivr.Table):
@@ -160,33 +153,33 @@
             ...     z = quivr.StringField()
             ...     i = Inner.as_field()
             ...
             >>> data = [{"z": "v1", "i": {"a": "v1_in"}}, {"z": "v2", "i": {"a": "v2_in"}}]
             >>> Outer.from_pylist(data)
             Outer(size=2)
         """
-        table = pa.Table.from_pylist(l, schema=cls.schema)
+        table = pa.Table.from_pylist(rows, schema=cls.schema)
         return cls(pa_table=table)
 
     @classmethod
-    def from_lists(cls, l: list[list]) -> Self:
+    def from_lists(cls, lists: list[list]) -> Self:
         """Create a Table object from a list of lists.
 
         Each inner list corresponds to a field in the Table. They
         should be specified in the same order as the fields in the
         class.
 
         Args:
-            l: A list of lists. Each inner list corresponds to a column in the table.
+            lists: A list of lists. Each inner list corresponds to a column in the table.
 
         Returns:
             A TableBase object.
 
         """
-        table = pa.Table.from_arrays(list(map(pa.array, l)), schema=cls.schema)
+        table = pa.Table.from_arrays(list(map(pa.array, lists)), schema=cls.schema)
         return cls(pa_table=table)
 
     @classmethod
     def from_dataframe(cls, df: pd.DataFrame):
         """Load a DataFrame into the Table.
 
         If the DataFrame is missing any of the Table's columns, an
@@ -214,15 +207,15 @@
         struct_fields = []
 
         for field in cls.schema:
             if pa.types.is_struct(field.type):
                 struct_fields.append(field)
 
         if len(struct_fields) == 0:
-            return cls(pa_table=pa.from_dataframe(df, schema=cls.schema))
+            return cls(pa_table=table)
 
         # Walk the schema, and build a StructArray for each embedded
         # type.
 
         def struct_array_for(field: pa.Field, ancestors: list[pa.Field]):
             prefix = ".".join([f.name for f in ancestors if f.name] + [field.name])
 
@@ -419,15 +412,15 @@
 
     def __len__(self):
         return len(self.table)
 
     def __getitem__(self, idx):
         # TODO: This comes out a little funky. You get chunked arrays
         # instead of arrays. Is there a way to flatten them safely?
-        
+
         if isinstance(idx, int):
             return self.__class__(self.table[idx : idx + 1])
         return self.__class__(self.table[idx])
 
     def __iter__(self):
         for i in range(len(self)):
             yield self[i : i + 1]
```

### Comparing `quivr-0.2.0/LICENSE` & `quivr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.2.0/README.md` & `quivr-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.2.0/pyproject.toml` & `quivr-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
 [tool.hatch.envs.default.scripts]
 check = [
   "lint",
   "typecheck",
   "test",
 ]
+fix = [
+  "ruff ./quivr ./test --fix"
+]
 lint = [
   "ruff ./quivr ./test",
   "black --check ./quivr ./test",
   "isort --check-only ./quivr ./test"
 ]
 format = [
   "black ./quivr ./test",
```

### Comparing `quivr-0.2.0/PKG-INFO` & `quivr-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.2.0
+Version: 0.2.1
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

