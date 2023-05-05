# Comparing `tmp/quivr-0.1.1.tar.gz` & `tmp/quivr-0.2.0.tar.gz`

## Comparing `quivr-0.1.1.tar` & `quivr-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/__init__.py~
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/__version__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/__version__.py~
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/concat.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/concat.py~
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/coordinates.py~
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/defragment.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/defragment.py~
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/errors.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/errors.py~
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/indexing.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/indexing.py~
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/matrix.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/matrix.py~
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/models.py~
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/quiver.py~
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/schemagraph.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/schemagraph.py~
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/streaming.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/streaming.py~
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/struct_demo.py~
--rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/tables.py
--rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/tables.py~
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 quivr-0.1.1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.1.1/LICENSE
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 quivr-0.1.1/README.md
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 quivr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 quivr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/__init__.py~
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/__version__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/__version__.py~
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/concat.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/concat.py~
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/coordinates.py~
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/defragment.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/defragment.py~
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/errors.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/errors.py~
+-rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/fields.py
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/fields.py~
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/indexing.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/indexing.py~
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/matrix.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/matrix.py~
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/models.py~
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/quiver.py~
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/schemagraph.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/schemagraph.py~
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/streaming.py~
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/struct_demo.py~
+-rw-r--r--   0        0        0    17362 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/tables.py
+-rw-r--r--   0        0        0    13287 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/tables.py~
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 quivr-0.2.0/quivr/tables2.py~
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 quivr-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 quivr-0.2.0/README.md
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 quivr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 quivr-0.2.0/PKG-INFO
```

### Comparing `quivr-0.1.1/quivr/concat.py` & `quivr-0.2.0/quivr/concat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Iterator, TypeVar
 
 import pyarrow as pa
 
 from .defragment import defragment
-from .tables import TableBase
+from .tables import Table
 
-Table = TypeVar("Table", bound=TableBase)
+T = TypeVar("T", bound=Table)
 
 
-def concatenate(values: Iterator[Table], defrag: bool = True) -> Table:
+def concatenate(values: Iterator[T], defrag: bool = True) -> T:
     """Concatenate a collection of Tables into a single Table.
 
     All input Tables must have the same schema (typically, this will
     be from being the same class).
 
     By default, results are compacted to be contiguous in memory,
     which involves a copy. In a tight loop, this can be very
@@ -25,11 +25,11 @@
     first = True
     for v in values:
         batches += v.table.to_batches()
         if first:
             cls = v.__class__
             first = False
     table = pa.Table.from_batches(batches)
-    result = cls(table=table)
+    result = cls(pa_table=table)
     if defrag:
         result = defragment(result)
     return result
```

### Comparing `quivr-0.1.1/quivr/coordinates.py~` & `quivr-0.2.0/quivr/coordinates.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.1/quivr/indexing.py` & `quivr-0.2.0/quivr/indexing.py~`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Generic, Optional, TypeVar
 
 import mmh3
 import pyarrow as pa
 import pyarrow.compute as pc
 
-from .tables import TableBase
+from quiver.tables import TableBase
 
 T = TypeVar("T", bound=TableBase)
 
 
 class StringIndex(Generic[T]):
     """StringIndex is a simple index that maps a string column to a
     list of row indices. It can be used for fast lookups of sub-slices
```

### Comparing `quivr-0.1.1/quivr/indexing.py~` & `quivr-0.2.0/quivr/indexing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Generic, Optional, TypeVar
 
 import mmh3
 import pyarrow as pa
 import pyarrow.compute as pc
 
-from quiver.tables import TableBase
+from .tables import Table
 
-T = TypeVar("T", bound=TableBase)
+T = TypeVar("T", bound=Table)
 
 
 class StringIndex(Generic[T]):
     """StringIndex is a simple index that maps a string column to a
     list of row indices. It can be used for fast lookups of sub-slices
     of a Table based on string values.
```

### Comparing `quivr-0.1.1/quivr/matrix.py` & `quivr-0.2.0/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.1.1/quivr/matrix.py~` & `quivr-0.2.0/quivr/matrix.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.1/quivr/models.py~` & `quivr-0.2.0/quivr/models.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.1/quivr/quiver.py~` & `quivr-0.2.0/quivr/quiver.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.1/quivr/struct_demo.py~` & `quivr-0.2.0/quivr/struct_demo.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.1/quivr/tables.py` & `quivr-0.2.0/quivr/tables.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,48 @@
-"""Table base classes."""
-
 import functools
-import pickle
-from typing import Any, Optional, Self, Union
+from typing import Generic, TypeVar, TypeAlias, Union, Optional, Self, ClassVar, Any
 from io import IOBase
 import os
 
+
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.csv
 import pyarrow.feather
 import pyarrow.parquet
 
+from .fields import Field, SubTableField, MetadataDict
+from .schemagraph import _walk_schema
 from .errors import TableFragmentedError
-from .schemagraph import _walk_schema, compute_depth
-
-_METADATA_MODEL_KEY = b"__quivr_model_pickle"
-_METADATA_NAME_KEY = b"__quivr_model_name"
-_METADATA_UNPICKLE_KWARGS_KEY = b"__quivr_model_unpickle_kwargs"
-
-
-class TableMetaclass(type):
-    """TableMetaclass is a metaclass which attaches accessors
-    to Tables based on their schema class-level attribute.
-
-    Each field in the class's schema becomes an attribute on the class.
-
-    """
-
-    def __new__(cls, name, bases, attrs):
-        # Invoked when a class is created. We use this to generate
-        # accessors for the class's schema's fields.
-        if "schema" not in attrs:
-            raise TypeError(f"Table {name} requires a schema attribute")
-        if not isinstance(attrs["schema"], pa.Schema):
-            raise TypeError(f"Table {name} schema attribute must be a pyarrow.Schema")
-        accessors = dict(cls.generate_accessors(attrs["schema"]))
-        attrs.update(accessors)
-
-        # Compute the depth of the schema, which is used when flattening.
-        attrs["_schema_depth"] = compute_depth(attrs["schema"])
-
-        return super().__new__(cls, name, bases, attrs)
-
-    def generate_accessors(schema: pa.Schema):
-        """Generate all the property accessors for the schema's fields.
-
-        Each field is accessed by name. When getting the field, its
-        underlying value is unloaded out of the Arrow array. If the
-        field has a model attached to it, the model is instantiated
-        with the data. Otherwise, the data is returned as-is.
-
-        """
-
-        def getter(_self, field: pa.Field):
-            return _self.column(field.name)
-
-        def setter(_self, value: Any):
-            raise NotImplementedError("Tables are immutable")
-
-        def deleter(_self):
-            raise NotImplementedError("Tables are immutable")
-
-        for idx, field in enumerate(schema):
-            g = functools.partial(getter, field=field)
-            prop = property(fget=g, fset=setter, fdel=deleter)
-            yield (field.name, prop)
 
 
-class TableBase(metaclass=TableMetaclass):
+class Table:
+    schema: ClassVar[pa.Schema]
     table: pa.Table
-    schema: pa.Schema = pa.schema([])
-    _schema_depth: int
 
-    def __init__(self, table: pa.Table):
-        self.table = []
-        if not isinstance(table, pa.Table):
-            raise TypeError(f"Data must be a pyarrow.Table for {self.__class__.__name__}")
-        if table.schema != self.schema:
-            raise TypeError(f"Data schema must match schema for {self.__class__.__name__}")
-        self.table = table
+    def __init_subclass__(cls, **kwargs):
+        fields = []
+        for name, field in cls.__dict__.items():
+            if isinstance(field, Field):
+                fields.append(field.pyarrow_field())
+
+        # Generate a pyarrow schema
+        schema = pa.schema(fields)
+        cls.schema = schema
+        super().__init_subclass__(**kwargs)
+
+    def __init__(self, pa_table: pa.Table):
+        self.table = pa_table
 
     @classmethod
     def from_data(cls, data: Optional[Any] = None, **kwargs) -> Self:
-        """Create an instance of the TableBase and populate it with data.
+        """
+        Create an instance of the Table and populate it with data.
 
         This is a convenience method which tries to infer the right
         underlying constructors to use based on the type of data. It
         can also accept keyword-style arguments to pass data in. If
         you know the data's structure well in advance, the more
         precise constructors (from_arrays, from_pylist, etc) should be
         preferred.
@@ -127,107 +80,114 @@
                 return cls.from_rows(data)
             if isinstance(data[0], dict):
                 return cls.from_rows(data)
             elif isinstance(data[0], list):
                 return cls.from_lists(data)
         if isinstance(data, pd.DataFrame):
             return cls.from_pandas(data)
-        if isinstance(data, np.ndarray):
-            return cls.from_numpy(data)
-        raise TypeError(f"Unsupported data type: {type(data)}")
+        raise TypeError(f"Unsupported type: {type(data)}")
 
     @classmethod
-    def from_kwargs(cls, **kwargs) -> Self:
-        """Create a TableBase object from keyword arguments.
+    def from_pydict(cls, data: dict[str, list], *args, **kwargs) -> Self:
+        table = pa.Table.from_pydict(data, schema=cls.schema)
+        return cls(table, *args, **kwargs)
 
-        Each keyword argument corresponds to a column in the table.
+    @classmethod
+    def as_field(cls, nullable: bool = True, metadata: Optional[MetadataDict] = None) -> SubTableField:
+        return SubTableField(cls, nullable=nullable, metadata=metadata)
 
-        Each keyword value can be a list, numpy array, pyarrow array,
-        or TableBase instance.
+    @classmethod
+    def from_kwargs(cls, **kwargs) -> Self:
+        """Create a Table instance from keyword arguments.
 
-        """
+        Each keyword argument corresponds to a field in the Table.
 
+        The keys should correspond to the field names, and the values
+        can be a list, numpy array, pyarrow array, or Table instance.
+        """
         arrays = []
         for column_name in cls.schema.names:
             if column_name not in kwargs:
                 raise ValueError(f"Missing column {column_name}")
             value = kwargs[column_name]
-            if isinstance(value, TableBase):
+            if isinstance(value, Table):
                 arrays.append(value.to_structarray())
             elif isinstance(value, pa.Array):
                 arrays.append(value)
             elif isinstance(value, np.ndarray):
                 arrays.append(pa.array(value))
             elif isinstance(value, list):
                 arrays.append(pa.array(value))
             else:
                 raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
         return cls.from_arrays(arrays)
 
     @classmethod
     def from_arrays(cls, arrays: list[pa.array]) -> Self:
-        """Create a TableBase object from a list of arrays.
+        """Create a Table object from a list of arrays.
 
         Args:
             arrays: A list of pyarrow.Array objects.
 
         Returns:
-            A TableBase object.
+            A Table object.
 
         """
         table = pa.Table.from_arrays(arrays, schema=cls.schema)
-        return cls(table=table)
+        return cls(pa_table=table)
 
     @classmethod
-    def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]]):
+    def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]]) -> Self:
         table = pa.Table.from_pydict(d, schema=cls.schema)
-        return cls(table=table)
+        return cls(pa_table=table)
 
     @classmethod
-    def from_rows(cls, l: list[dict]):
+    def from_rows(cls, l: list[dict]) -> Self:
         """
-        Create a TableBase object from a list of dictionaries.
+        Create a Table object from a list of dictionaries.
 
         Args:
             l: A list of values. Each value corresponds to a row in the table.
 
         Returns:
-            A TableBase object.
+            A Table object.
 
         Examples:
             >>> import quivr
-            >>> class Inner(quivr.TableBase):
-            ...     schema = pyarrow.schema([pyarrow.field("a", pyarrow.string())])
+            >>> class Inner(quivr.Table):
+            ...     a = quivr.StringField()
             ...
             >>> class Outer(quivr.TableBase):
-            ...     schema = pyarrow.schema([pyarrow.field("z", pyarrow.string()), Inner.as_field("i")])
+            ...     z = quivr.StringField()
+            ...     i = Inner.as_field()
             ...
             >>> data = [{"z": "v1", "i": {"a": "v1_in"}}, {"z": "v2", "i": {"a": "v2_in"}}]
             >>> Outer.from_pylist(data)
             Outer(size=2)
         """
         table = pa.Table.from_pylist(l, schema=cls.schema)
-        return cls(table=table)
+        return cls(pa_table=table)
 
     @classmethod
     def from_lists(cls, l: list[list]) -> Self:
-        """Create a TableBase object from a list of lists.
+        """Create a Table object from a list of lists.
 
-        Each inner list corresponds to a column in the table. They
-        should be specified in the same order as the columns in the
-        schema.
+        Each inner list corresponds to a field in the Table. They
+        should be specified in the same order as the fields in the
+        class.
 
         Args:
             l: A list of lists. Each inner list corresponds to a column in the table.
 
         Returns:
             A TableBase object.
+
         """
         table = pa.Table.from_arrays(list(map(pa.array, l)), schema=cls.schema)
-        return cls(table=table)
+        return cls(pa_table=table)
 
     @classmethod
     def from_dataframe(cls, df: pd.DataFrame):
         """Load a DataFrame into the Table.
 
         If the DataFrame is missing any of the Table's columns, an
         error is raised. If the DataFrame has extra columns, they are
@@ -236,15 +196,15 @@
         This function cannot load "flattened" dataframes. This only
         matters for nested Tables which contain other Table
         definitions as fields. For that use case, either load an
         unflattened DataFrame, or use from_flat_dataframe.
         """
 
         table = pa.Table.from_pandas(df, schema=cls.schema)
-        return cls(table=table)
+        return cls(pa_table=table)
 
     @classmethod
     def _unflatten_table(cls, table: pa.Table):
         """Unflatten a Table.
 
         This is used when loading a flattened DataFrame into a nested
         Table. It takes a Table with a flat schema, and returns a
@@ -254,15 +214,15 @@
         struct_fields = []
 
         for field in cls.schema:
             if pa.types.is_struct(field.type):
                 struct_fields.append(field)
 
         if len(struct_fields) == 0:
-            return cls(table=pa.from_dataframe(df, schema=cls.schema))
+            return cls(pa_table=pa.from_dataframe(df, schema=cls.schema))
 
         # Walk the schema, and build a StructArray for each embedded
         # type.
 
         def struct_array_for(field: pa.Field, ancestors: list[pa.Field]):
             prefix = ".".join([f.name for f in ancestors if f.name] + [field.name])
 
@@ -292,15 +252,15 @@
         """
         struct_fields = []
         for field in cls.schema:
             if pa.types.is_struct(field.type):
                 struct_fields.append(field)
 
         if len(struct_fields) == 0:
-            return cls(table=pa.from_dataframe(df, schema=cls.schema))
+            return cls(pa_table=pa.from_dataframe(df, schema=cls.schema))
 
         root = pa.field("", pa.struct(cls.schema))
 
         # Walk the schema, and build a StructArray for each embedded
         # type. These are stored in a dictionary, keyed by their
         # dot-separated path. For example, if the schema is:
         #
@@ -360,24 +320,24 @@
 
         table_arrays = []
         for subfield in cls.schema:
             # Pull out the fields of that root-level struct array.
             table_arrays.append(sa.field(subfield.name))
 
         table = pa.Table.from_arrays(table_arrays, schema=cls.schema)
-        return cls(table=table)
+        return cls(pa_table=table)
 
     def flattened_table(self) -> pa.Table:
         """Completely flatten the Table's underlying Arrow table,
         taking into account any nested structure, and return the data
         table itself.
-
         """
+
         table = self.table
-        for i in range(self._schema_depth - 1):
+        while any(isinstance(field.type, pa.StructType) for field in table.schema):
             table = table.flatten()
         return table
 
     def select(self, column_name: str, value: Any) -> Self:
         """Select from the table by exact match, returning a new
         Table which only contains rows for which the value in
         column_name equals value.
@@ -446,93 +406,67 @@
 
         """
         table = self.table
         if flatten:
             table = self.flattened_table()
         return table.to_pandas()
 
-    @classmethod
-    def as_field(cls, name: str, nullable: bool = True, metadata: Optional[dict] = None):
-        metadata = metadata or {}
-        metadata[_METADATA_NAME_KEY] = cls.__name__
-        metadata[_METADATA_MODEL_KEY] = pickle.dumps(cls)
-        field = pa.field(name, pa.struct(cls.schema), nullable=nullable, metadata=metadata)
-        return field
-
-    def column(self, field_name: str):
-        field = self.schema.field(field_name)
-        if field.metadata is not None and _METADATA_MODEL_KEY in field.metadata:
-            # If the field has type information attached to it in
-            # metadata, pull it out. The metadata store the model (as
-            # a class object), and may optionally have some keyword
-            # arguments to be used when instantiating the model from
-            # the data.
-            model = pickle.loads(field.metadata[_METADATA_MODEL_KEY])
-            if _METADATA_UNPICKLE_KWARGS_KEY in field.metadata:
-                init_kwargs = pickle.loads(field.metadata[_METADATA_UNPICKLE_KWARGS_KEY])
-            else:
-                init_kwargs = {}
-            table = _sub_table(self.table, field_name)
-            return model(table=table, **init_kwargs)
+    def column(self, field_name: str) -> pa.ChunkedArray:
+        """Returns the column with the given name as a raw pyarrow ChunkedArray."""
         return self.table.column(field_name)
 
     def __repr__(self):
         return f"{self.__class__.__name__}(size={len(self.table)})"
 
     def __len__(self):
         return len(self.table)
 
     def __getitem__(self, idx):
+        # TODO: This comes out a little funky. You get chunked arrays
+        # instead of arrays. Is there a way to flatten them safely?
+        
         if isinstance(idx, int):
             return self.__class__(self.table[idx : idx + 1])
         return self.__class__(self.table[idx])
 
     def __iter__(self):
         for i in range(len(self)):
             yield self[i : i + 1]
 
-    def __eq__(self, other):
-        if not isinstance(other, TableBase):
-            return NotImplemented
-        return self.table.equals(other.table)
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, Table):
+            return self.table.equals(other.table)
+        if isinstance(other, pa.Table):
+            return self.table.equals(other)
+        return False
 
     def take(self, row_indices: Union[list[int], pa.IntegerArray]) -> Self:
         """Return a new Table with only the rows at the given indices."""
         return self.__class__(self.table.take(row_indices))
 
     def to_parquet(self, path: str, **kwargs):
         """Write the table to a Parquet file."""
         pyarrow.parquet.write_table(self.table, path, **kwargs)
 
     @classmethod
     def from_parquet(cls, path: str, **kwargs):
         """Read a table from a Parquet file."""
-        return cls(table=pyarrow.parquet.read_table(path, **kwargs))
+        return cls(pa_table=pyarrow.parquet.read_table(path, **kwargs))
 
     def to_feather(self, path: str, **kwargs):
         """Write the table to a Feather file."""
         pyarrow.feather.write_feather(self.table, path, **kwargs)
 
     @classmethod
     def from_feather(cls, path: str, **kwargs):
         """Read a table from a Feather file."""
-        return cls(table=pyarrow.feather.read_table(path, **kwargs))
+        return cls(pa_table=pyarrow.feather.read_table(path, **kwargs))
 
     def to_csv(self, path: str):
         """Write the table to a CSV file. Any nested structure is flattened."""
         pyarrow.csv.write_csv(self.flattened_table(), path)
 
     @classmethod
     def from_csv(cls, input_file: Union[str, os.PathLike, IOBase]):
         """Read a table from a CSV file."""
         flat_table = pyarrow.csv.read_csv(input_file)
-        return cls(table=cls._unflatten_table(flat_table))
-
-
-def _sub_table(tab: pa.Table, field_name: str):
-    """Given a table which contains a StructArray under given field
-    name, construct a table from the sub-object.
-
-    """
-    column = tab.column(field_name)
-    schema = pa.schema(column.type)
-    return pa.Table.from_arrays(column.flatten(), schema=schema)
+        return cls(pa_table=cls._unflatten_table(flat_table))
```

### Comparing `quivr-0.1.1/quivr/tables.py~` & `quivr-0.2.0/quivr/tables.py~`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,133 @@
-import functools
-import pickle
-from typing import Any, Optional, Self, Union
+from typing import Generic, TypeVar, TypeAlias, Union, Optional, Self, ClassVar, Any
 
+import pyarrow as pa
 import numpy as np
 import pandas as pd
-import pyarrow as pa
-import pyarrow.compute as pc
-import pyarrow.feather
-import pyarrow.parquet
 
+from .fields import Field, SubTableField, MetadataDict
+from .schemagraph import _walk_schema
 from .errors import TableFragmentedError
-from .schemagraph import _walk_schema, compute_depth
 
-_METADATA_MODEL_KEY = b"__quiver_model_pickle"
-_METADATA_NAME_KEY = b"__quiver_model_name"
-_METADATA_UNPICKLE_KWARGS_KEY = b"__quiver_model_unpickle_kwargs"
+class Table:
+    schema: ClassVar[pa.Schema]
+    table: pa.Table
 
+    def __init_subclass__(cls, **kwargs):
+        fields = []
+        for name, field in cls.__dict__.items():
+            if isinstance(field, Field):
+                fields.append(field.pyarrow_field())
+
+        # Generate a pyarrow schema
+        schema = pa.schema(fields)
+        cls.schema = schema
+        super().__init_subclass__(**kwargs)
 
-class TableMetaclass(type):
-    """TableMetaclass is a metaclass which attaches accessors
-    to Tables based on their schema class-level attribute.
+    def __init__(self, pa_table: pa.Table):
+        self.table = pa_table
 
-    Each field in the class's schema becomes an attribute on the class.
+    @classmethod
+    def from_pydict(cls, data: dict[str, list], *args, **kwargs) -> Self:
+        table = pa.Table.from_pydict(data, schema=cls.schema)
+        return cls(table, *args, **kwargs)
 
-    """
+    @classmethod
+    def as_field(cls, nullable: bool = True, metadata: Optional[MetadataDict] = None) -> SubTableField:
+        return SubTableField(cls, nullable=nullable, metadata=metadata)
 
-    def __new__(cls, name, bases, attrs):
-        # Invoked when a class is created. We use this to generate
-        # accessors for the class's schema's fields.
-        if "schema" not in attrs:
-            raise TypeError(f"Table {name} requires a schema attribute")
-        if not isinstance(attrs["schema"], pa.Schema):
-            raise TypeError(f"Table {name} schema attribute must be a pyarrow.Schema")
-        accessors = dict(cls.generate_accessors(attrs["schema"]))
-        attrs.update(accessors)
+    @classmethod
+    def from_kwargs(cls, **kwargs) -> Self:
+        """Create a Table instance from keyword arguments.
 
-        # Compute the depth of the schema, which is used when flattening.
-        attrs["_schema_depth"] = compute_depth(attrs["schema"])
+        Each keyword argument corresponds to a field in the Table.
+        
+        The keys should correspond to the field names, and the values
+        can be a list, numpy array, pyarrow array, or Table instance.
+        """
+        arrays = []
+        for column_name in cls.schema.names:
+            if column_name not in kwargs:
+                raise ValueError(f"Missing column {column_name}")
+            value = kwargs[column_name]
+            if isinstance(value, Table):
+                arrays.append(value.to_structarray())
+            elif isinstance(value, pa.Array):
+                arrays.append(value)
+            elif isinstance(value, np.ndarray):
+                arrays.append(pa.array(value))
+            elif isinstance(value, list):
+                arrays.append(pa.array(value))
+            else:
+                raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
+        return cls.from_arrays(arrays)
 
-        return super().__new__(cls, name, bases, attrs)
+    @classmethod
+    def from_arrays(cls, arrays: list[pa.array]) -> Self:
+        """Create a Table object from a list of arrays.
 
-    def generate_accessors(schema: pa.Schema):
-        """Generate all the property accessors for the schema's fields.
+        Args:
+            arrays: A list of pyarrow.Array objects.
 
-        Each field is accessed by name. When getting the field, its
-        underlying value is unloaded out of the Arrow array. If the
-        field has a model attached to it, the model is instantiated
-        with the data. Otherwise, the data is returned as-is.
+        Returns:
+            A Table object.
 
         """
+        table = pa.Table.from_arrays(arrays, schema=cls.schema)
+        return cls(pa_table=table)
+    
+    @classmethod
+    def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]]) -> Self:
+        table = pa.Table.from_pydict(d, schema=cls.schema)
+        return cls(pa_table=table)
 
-        def getter(_self, field: pa.Field):
-            return _self.column(field.name)
+    @classmethod
+    def from_rows(cls, l: list[dict]) -> Self:
+        """
+        Create a Table object from a list of dictionaries.
 
-        def setter(_self, value: Any):
-            raise NotImplementedError("Tables are immutable")
+        Args:
+            l: A list of values. Each value corresponds to a row in the table.
 
-        def deleter(_self):
-            raise NotImplementedError("Tables are immutable")
+        Returns:
+            A Table object.
 
-        for idx, field in enumerate(schema):
-            g = functools.partial(getter, field=field)
-            prop = property(fget=g, fset=setter, fdel=deleter)
-            yield (field.name, prop)
+        Examples:
+            >>> import quivr
+            >>> class Inner(quivr.Table):
+            ...     a = quivr.StringField()
+            ...
+            >>> class Outer(quivr.TableBase):
+            ...     z = quivr.StringField()
+            ...     i = Inner.as_field()
+            ...
+            >>> data = [{"z": "v1", "i": {"a": "v1_in"}}, {"z": "v2", "i": {"a": "v2_in"}}]
+            >>> Outer.from_pylist(data)
+            Outer(size=2)
+        """
+        table = pa.Table.from_pylist(l, schema=cls.schema)
+        return cls(pa_table=table)
 
+    @classmethod
+    def from_lists(cls, l: list[list]) -> Self:
+        """Create a Table object from a list of lists.
 
-class TableBase(metaclass=TableMetaclass):
-    table: pa.Table
-    schema: pa.Schema = pa.schema([])
-    _schema_depth: int
+        Each inner list corresponds to a field in the Table. They
+        should be specified in the same order as the fields in the
+        class.
 
-    def __init__(self, table: pa.Table):
-        if not isinstance(table, pa.Table):
-            raise TypeError(f"Data must be a pyarrow.Table for {self.__class__.__name__}")
-        if table.schema != self.schema:
-            raise TypeError(f"Data schema must match schema for {self.__class__.__name__}")
-        self.table = table
+        Args:
+            l: A list of lists. Each inner list corresponds to a column in the table.
 
-    @classmethod
-    def from_arrays(cls, arrays: list[pa.array]):
-        table = pa.Table.from_arrays(arrays, schema=cls.schema)
-        return cls(table=table)
+        Returns:
+            A TableBase object.
 
-    @classmethod
-    def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]]):
-        table = pa.Table.from_pydict(d, schema=cls.schema)
-        return cls(table=table)
+        """
+        table = pa.Table.from_arrays(list(map(pa.array, l)), schema=cls.schema)
+        return cls(pa_table=table)
 
     @classmethod
     def from_dataframe(cls, df: pd.DataFrame):
         """Load a DataFrame into the Table.
 
         If the DataFrame is missing any of the Table's columns, an
         error is raised. If the DataFrame has extra columns, they are
@@ -98,117 +136,15 @@
         This function cannot load "flattened" dataframes. This only
         matters for nested Tables which contain other Table
         definitions as fields. For that use case, either load an
         unflattened DataFrame, or use from_flat_dataframe.
         """
 
         table = pa.Table.from_pandas(df, schema=cls.schema)
-        return cls(table=table)
-
-    @classmethod
-    def from_flat_dataframe(cls, df: pd.DataFrame):
-        """Load a flattened DataFrame into the Table.
-
-        known bug: Doesn't correctly interpret fixed-length lists.
-        """
-        struct_fields = []
-        for field in cls.schema:
-            if pa.types.is_struct(field.type):
-                struct_fields.append(field)
-
-        if len(struct_fields) == 0:
-            return cls(table=pa.from_dataframe(df, schema=cls.schema))
-
-        root = pa.field("", pa.struct(cls.schema))
-
-        # Walk the schema, and build a StructArray for each embedded
-        # type. These are stored in a dictionary, keyed by their
-        # dot-separated path. For example, if the schema is:
-        #
-        #   pa.field("foo", pa.struct([
-        #       pa.field("bar", pa.struct([
-        #           pa.field("baz", pa.int64())
-        #       ]))
-        #   ]))
-        #
-        # Then the struct array for the inner struct will be stored in
-        # the dictionary at the key "foo.bar".
-
-        struct_arrays: dict[str, pa.StructArray] = {}
-
-        def visitor(field: pa.Field, ancestors: list[pa.Field]):
-            # Modify the dataframe in place, trimming out the columns we
-            # have already processed in depth-first order.
-            nonlocal df
-            if len(ancestors) == 0:
-                # Root - gets special behavior.
-                df_key = ""
-            else:
-                lineage = [f.name for f in ancestors if f.name] + [field.name]
-                df_key = ".".join(lineage)
-
-            # Pull out just the columns relevant to this field
-            field_columns = df.columns[df.columns.str.startswith(df_key)]
-            field_df = df[field_columns]
-
-            # Replace column names like "foo.bar.baz" with "baz", the
-            # last component.
-            if len(ancestors) == 0:
-                # If we're at the root, use the original column names.
-                names = field_df.columns
-            else:
-                names = field_df.columns.str.slice(len(df_key) + 1)
-            field_df.columns = names
-
-            # Build a StructArray of all of the subfields.
-            arrays = []
-            for subfield in field.type:
-                sa_key = df_key + "." + subfield.name if df_key else subfield.name
-                if sa_key in struct_arrays:
-                    # We've already built this array, so just use it.
-                    arrays.append(struct_arrays[sa_key])
-                else:
-                    arrays.append(field_df[subfield.name])
-            sa = pa.StructArray.from_arrays(arrays, fields=list(field.type))
-            struct_arrays[df_key] = sa
-
-            # Clean the fields out
-            df = df.drop(field_columns, axis="columns")
-
-        _walk_schema(root, visitor, None)
-        # Now build a table back up. Grab the root-level struct array.
-        sa = struct_arrays[""]
-
-        table_arrays = []
-        for subfield in cls.schema:
-            # Pull out the fields of that root-level struct array.
-            table_arrays.append(sa.field(subfield.name))
-
-        table = pa.Table.from_arrays(table_arrays, schema=cls.schema)
-        return cls(table=table)
-
-    def flattened_table(self) -> pa.Table:
-        """Completely flatten the Table's underlying Arrow table,
-        taking into account any nested structure, and return the data
-        table itself.
-
-        """
-        table = self.table
-        for i in range(self._schema_depth - 1):
-            table = table.flatten()
-        return table
-
-    def select(self, column_name: str, value: Any) -> Self:
-        """Select from the table by exact match, returning a new
-        Table which only contains rows for which the value in
-        column_name equals value.
-
-        """
-        table = self.table.filter(pc.field(column_name) == value)
-        return self.__class__(table)
+        return cls(pa_table=table)
 
     def sort_by(self, by: Union[str, list[tuple[str, str]]]) -> Self:
         """Sorts the Table by the given column name (or multiple
         columns). This operation requires a copy, and returns a new
         Table using the copied data.
 
         by should be a column name to sort by, or a list of (column,
@@ -266,38 +202,33 @@
 
         """
         table = self.table
         if flatten:
             table = self.flattened_table()
         return table.to_pandas()
 
-    @classmethod
-    def as_field(cls, name: str, nullable: bool = True, metadata: Optional[dict] = None):
-        metadata = metadata or {}
-        metadata[_METADATA_NAME_KEY] = cls.__name__
-        metadata[_METADATA_MODEL_KEY] = pickle.dumps(cls)
-        field = pa.field(name, pa.struct(cls.schema), nullable=nullable, metadata=metadata)
-        return field
-
-    def column(self, field_name: str):
-        field = self.schema.field(field_name)
-        if field.metadata is not None and _METADATA_MODEL_KEY in field.metadata:
-            # If the field has type information attached to it in
-            # metadata, pull it out. The metadata store the model (as
-            # a class object), and may optionally have some keyword
-            # arguments to be used when instantiating the model from
-            # the data.
-            model = pickle.loads(field.metadata[_METADATA_MODEL_KEY])
-            if _METADATA_UNPICKLE_KWARGS_KEY in field.metadata:
-                init_kwargs = pickle.loads(field.metadata[_METADATA_UNPICKLE_KWARGS_KEY])
-            else:
-                init_kwargs = {}
-            table = _sub_table(self.table, field_name)
-            return model(table=table, **init_kwargs)
-        return self.table.column(field_name)
+    def flattened_table(self) -> pa.Table:
+        """Completely flatten the Table's underlying Arrow table,
+        taking into account any nested structure, and return the data
+        table itself.
+        """
+
+        table = self.table
+        while any(isinstance(field.type, pa.StructType) for field in table.schema):
+            table = table.flatten()
+        return table
+
+    def select(self, column_name: str, value: Any) -> Self:
+        """Select from the table by exact match, returning a new
+        Table which only contains rows for which the value in
+        column_name equals value.
+
+        """
+        table = self.table.filter(pc.field(column_name) == value)
+        return self.__class__(table)
 
     def __repr__(self):
         return f"{self.__class__.__name__}(size={len(self.table)})"
 
     def __len__(self):
         return len(self.table)
 
@@ -306,38 +237,130 @@
             return self.__class__(self.table[idx : idx + 1])
         return self.__class__(self.table[idx])
 
     def __iter__(self):
         for i in range(len(self)):
             yield self[i : i + 1]
 
-    def take(self, row_indices: Union[list[int], pa.IntegerArray]) -> Self:
-        """Return a new Table with only the rows at the given indices."""
-        return self.__class__(self.table.take(row_indices))
-
-    def to_parquet(self, path: str, **kwargs):
-        """Write the table to a Parquet file."""
-        pyarrow.parquet.write_table(self.table, path, **kwargs)
-
     @classmethod
-    def from_parquet(cls, path: str, **kwargs):
-        """Read a table from a Parquet file."""
-        return cls(table=pyarrow.parquet.read_table(path, **kwargs))
-
-    def to_feather(self, path: str, **kwargs):
-        """Write the table to a Feather file."""
-        pyarrow.feather.write_feather(self.table, path, **kwargs)
+    def _unflatten_table(cls, table: pa.Table):
+        """Unflatten a Table.
+
+        This is used when loading a flattened DataFrame into a nested
+        Table. It takes a Table with a flat schema, and returns a
+        Table with a nested schema.
+
+        """
+        struct_fields = []
+
+        for field in cls.schema:
+            if pa.types.is_struct(field.type):
+                struct_fields.append(field)
+
+        if len(struct_fields) == 0:
+            return cls(pa_table=pa.from_dataframe(df, schema=cls.schema))
+
+        # Walk the schema, and build a StructArray for each embedded
+        # type.
+
+        def struct_array_for(field: pa.Field, ancestors: list[pa.Field]):
+            prefix = ".".join([f.name for f in ancestors if f.name] + [field.name])
+
+            child_arrays = []
+            for subfield in field.type:
+                if pa.types.is_struct(subfield.type):
+                    child_arrays.append(struct_array_for(subfield, ancestors + [field]))
+                else:
+                    path = prefix + "." + subfield.name
+                    child_arrays.append(table.column(path).combine_chunks())
+            return pa.StructArray.from_arrays(child_arrays, fields=list(field.type))
+
+        child_arrays = []
+        for field in cls.schema:
+            if pa.types.is_struct(field.type):
+                child_arrays.append(struct_array_for(field, []))
+            else:
+                child_arrays.append(table.column(field.name).combine_chunks())
+
+        return pa.Table.from_arrays(child_arrays, schema=cls.schema)
 
     @classmethod
-    def from_feather(cls, path: str, **kwargs):
-        """Read a table from a Feather file."""
-        return cls(table=pyarrow.feather.read_feather(path, **kwargs))
+    def from_flat_dataframe(cls, df: pd.DataFrame):
+        """Load a flattened DataFrame into the Table.
 
+        known bug: Doesn't correctly interpret fixed-length lists.
+        """
+        struct_fields = []
+        for field in cls.schema:
+            if pa.types.is_struct(field.type):
+                struct_fields.append(field)
+
+        if len(struct_fields) == 0:
+            return cls(pa_table=pa.from_dataframe(df, schema=cls.schema))
 
-def _sub_table(tab: pa.Table, field_name: str):
-    """Given a table which contains a StructArray under given field
-    name, construct a table from the sub-object.
-
-    """
-    column = tab.column(field_name)
-    schema = pa.schema(column.type)
-    return pa.Table.from_arrays(column.flatten(), schema=schema)
+        root = pa.field("", pa.struct(cls.schema))
+
+        # Walk the schema, and build a StructArray for each embedded
+        # type. These are stored in a dictionary, keyed by their
+        # dot-separated path. For example, if the schema is:
+        #
+        #   pa.field("foo", pa.struct([
+        #       pa.field("bar", pa.struct([
+        #           pa.field("baz", pa.int64())
+        #       ]))
+        #   ]))
+        #
+        # Then the struct array for the inner struct will be stored in
+        # the dictionary at the key "foo.bar".
+
+        struct_arrays: dict[str, pa.StructArray] = {}
+
+        def visitor(field: pa.Field, ancestors: list[pa.Field]):
+            # Modify the dataframe in place, trimming out the columns we
+            # have already processed in depth-first order.
+            nonlocal df
+            if len(ancestors) == 0:
+                # Root - gets special behavior.
+                df_key = ""
+            else:
+                lineage = [f.name for f in ancestors if f.name] + [field.name]
+                df_key = ".".join(lineage)
+
+            # Pull out just the columns relevant to this field
+            field_columns = df.columns[df.columns.str.startswith(df_key)]
+            field_df = df[field_columns]
+
+            # Replace column names like "foo.bar.baz" with "baz", the
+            # last component.
+            if len(ancestors) == 0:
+                # If we're at the root, use the original column names.
+                names = field_df.columns
+            else:
+                names = field_df.columns.str.slice(len(df_key) + 1)
+            field_df.columns = names
+
+            # Build a StructArray of all of the subfields.
+            arrays = []
+            for subfield in field.type:
+                sa_key = df_key + "." + subfield.name if df_key else subfield.name
+                if sa_key in struct_arrays:
+                    # We've already built this array, so just use it.
+                    arrays.append(struct_arrays[sa_key])
+                else:
+                    arrays.append(field_df[subfield.name])
+            sa = pa.StructArray.from_arrays(arrays, fields=list(field.type))
+            struct_arrays[df_key] = sa
+
+            # Clean the fields out
+            df = df.drop(field_columns, axis="columns")
+
+        _walk_schema(root, visitor, None)
+        # Now build a table back up. Grab the root-level struct array.
+        sa = struct_arrays[""]
+
+        table_arrays = []
+        for subfield in cls.schema:
+            # Pull out the fields of that root-level struct array.
+            table_arrays.append(sa.field(subfield.name))
+
+        table = pa.Table.from_arrays(table_arrays, schema=cls.schema)
+        return cls(pa_table=table)
```

### Comparing `quivr-0.1.1/LICENSE` & `quivr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.1.1/README.md` & `quivr-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -40,33 +40,30 @@
 ## Installation
 
 Check out this repo, and `pip install` it.
 
 ## Usage
 
 Your main entrypoint to Quivr is through defining classes which
-represent your tables. You write a `pyarrow.Schema` as the `schema`
-class attribute of your class, and Quivr will take care of the rest.
+represent your tables. You write a subclass of quivr.Table, annotating
+it with Fields that describe the data you're working with, and quivr
+will handle the rest.
 
 ```python
-from quivr import TableBase
+from quivr import Table, Float64Field
 import pyarrow as pa
 
 
 class Coordinates(TableBase):
-    schema = pa.schema(
-        [
-            pa.field("x", pa.float64()),
-            pa.field("y", pa.float64()),
-            pa.field("z", pa.float64()),
-            pa.field("vx", pa.float64()),
-            pa.field("vy", pa.float64()),
-            pa.field("vz", pa.float64()),
-        ]
-    )
+	x = Float64Field()
+	y = Float64Field()
+	z = Float64Field()
+	vx = Float64Field()
+	vy = Float64Field()
+	vz = Float64Field()
 ```
 
 Then, you can construct tables from data:
 
 ```python
 
 coords = Coordinates.from_data(
@@ -94,41 +91,50 @@
 ### Embedded definitions and nullable fields
 
 You can embed one table's definition within another, and you can make fields nullable:
 
 ```python
 
 class AsteroidOrbit(TableBase):
-    schema = pa.schema(
-        [
-            pa.field("designation", pa.string()),
-            pa.field("mass", pa.float64(), nullable=True),
-            pa.field("radius", pa.float64(), nullable=True),
-            Coordinates.as_field("coords"),
-        ]
-    )
+	designation = StringField()
+	mass = Float64Field(nullable=True)
+	radius = Float64Field(nullable=True)
+	coords = Coordinates.as_field()
 
 # You can construct embedded fields from Arrow StructArrays, which you can get from
 # other Quivr tables using the to_structarray() method with zero copy.
 orbits = AsteroidOrbit.from_data(
     designation=np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
     mass=np.array([9.393e20, 2.06e21, 2.59e20, None]),
     radius=np.array([4.6e6, 2.7e6, 2.6e6, None]),
     coords=coords.to_structarray(),
 )
 ```
 
 ### Computing
 
-You can use the columns of the data to do computations:
+#### Using Numpy
+When you reference columns, you'll get numpy arrays which you can use to do computations:
+
+```python
+import numpy as np
+
+print(np.quantile(orbits.mass + 10, 0.5)
+```
+
+
+#### Using pyarrow.compute
+
+You can also use access columns of the data as Arrow Arrays to do
+computations using the Pyarrow compute kernels:
 
 ```python
 import pyarrow.compute as pc
 
-median_mass = pc.quantile(orbits.mass, q=0.5)
+median_mass = pc.quantile(pc.add(orbits.column(mass, as_numpy=False), 10), q=0.5)
 # median_mass is a pyarrow.Scalar, which you can get the value of with .as_py()
 print(median_mass.as_py())
 ```
 
 There is a very extensive set of functions available in the
 `pyarrow.compute` package, which you can see
 [here](https://arrow.apache.org/docs/python/compute.html). These
@@ -141,57 +147,42 @@
 behavior of your tables by adding or overriding methods. For example, if you want to add a
 method to compute the total mass of the asteroids in the table, you
 can do so like this:
 
 ```python
 
 class AsteroidOrbit(TableBase):
-    schema = pa.schema(
-        [
-            pa.field("designation", pa.string()),
-            pa.field("mass", pa.float64(), nullable=True),
-            pa.field("radius", pa.float64(), nullable=True),
-            Coordinates.as_field("coords"),
-        ]
-    )
+	designation = StringField()
+	mass = Float64Field(nullable=True)
+	radius = Float64Field(nullable=True)
+	coords = Coordinates.as_field()
 
     def total_mass(self):
         return pc.sum(self.mass)
 
 ```
 
 You can also use this to add "meta-fields" which are combinations of other fields. For example:
 
 ```python
 class CoordinateCovariance(TableBase):
-    schema = pa.schema(
-        [
-            # The covariance matrix of the coordinates as a 6x6 matrix (3 positions, 3 velocities)
-            pa.field("matrix_values", pa.list_(pa.float64(), 36)),
-        ]
-    )
+	matrix_values = ListField(pa.float64(), 36)
 
     @property
     def matrix(self):
         # This is a numpy array of shape (n, 6, 6)
         return self.matrix_values.to_numpy().reshape(-1, 6, 6)
 
 
 class AsteroidOrbit(TableBase):
-    schema = pa.schema(
-        [
-            pa.field("designation", pa.string()),
-            pa.field("mass", pa.float64(), nullable=True),
-            pa.field("radius", pa.float64(), nullable=True),
-            Coordinates.as_field("coords"),
-            CoordinateCovariance.as_field("covariance"),
-        ]
-    )
-
-
+	designation = StringField()
+	mass = Float64Field(nullable=True)
+	radius = Float64Field(nullable=True)
+	coords = Coordinates.as_field()
+	covariance = CoordinateCovariance.as_field()
 
 orbits = load_orbits() # Analogous to the example above
 
 # Compute the determinant of the covariance matrix for each asteroid
 determinants = np.linalg.det(orbits.covariance.matrix)
 ```
```

### Comparing `quivr-0.1.1/pyproject.toml` & `quivr-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.1.1/PKG-INFO` & `quivr-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.1.1
+Version: 0.2.0
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: mmh3
 Requires-Dist: numpy
@@ -54,33 +54,30 @@
 ## Installation
 
 Check out this repo, and `pip install` it.
 
 ## Usage
 
 Your main entrypoint to Quivr is through defining classes which
-represent your tables. You write a `pyarrow.Schema` as the `schema`
-class attribute of your class, and Quivr will take care of the rest.
+represent your tables. You write a subclass of quivr.Table, annotating
+it with Fields that describe the data you're working with, and quivr
+will handle the rest.
 
 ```python
-from quivr import TableBase
+from quivr import Table, Float64Field
 import pyarrow as pa
 
 
 class Coordinates(TableBase):
-    schema = pa.schema(
-        [
-            pa.field("x", pa.float64()),
-            pa.field("y", pa.float64()),
-            pa.field("z", pa.float64()),
-            pa.field("vx", pa.float64()),
-            pa.field("vy", pa.float64()),
-            pa.field("vz", pa.float64()),
-        ]
-    )
+	x = Float64Field()
+	y = Float64Field()
+	z = Float64Field()
+	vx = Float64Field()
+	vy = Float64Field()
+	vz = Float64Field()
 ```
 
 Then, you can construct tables from data:
 
 ```python
 
 coords = Coordinates.from_data(
@@ -108,41 +105,50 @@
 ### Embedded definitions and nullable fields
 
 You can embed one table's definition within another, and you can make fields nullable:
 
 ```python
 
 class AsteroidOrbit(TableBase):
-    schema = pa.schema(
-        [
-            pa.field("designation", pa.string()),
-            pa.field("mass", pa.float64(), nullable=True),
-            pa.field("radius", pa.float64(), nullable=True),
-            Coordinates.as_field("coords"),
-        ]
-    )
+	designation = StringField()
+	mass = Float64Field(nullable=True)
+	radius = Float64Field(nullable=True)
+	coords = Coordinates.as_field()
 
 # You can construct embedded fields from Arrow StructArrays, which you can get from
 # other Quivr tables using the to_structarray() method with zero copy.
 orbits = AsteroidOrbit.from_data(
     designation=np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
     mass=np.array([9.393e20, 2.06e21, 2.59e20, None]),
     radius=np.array([4.6e6, 2.7e6, 2.6e6, None]),
     coords=coords.to_structarray(),
 )
 ```
 
 ### Computing
 
-You can use the columns of the data to do computations:
+#### Using Numpy
+When you reference columns, you'll get numpy arrays which you can use to do computations:
+
+```python
+import numpy as np
+
+print(np.quantile(orbits.mass + 10, 0.5)
+```
+
+
+#### Using pyarrow.compute
+
+You can also use access columns of the data as Arrow Arrays to do
+computations using the Pyarrow compute kernels:
 
 ```python
 import pyarrow.compute as pc
 
-median_mass = pc.quantile(orbits.mass, q=0.5)
+median_mass = pc.quantile(pc.add(orbits.column(mass, as_numpy=False), 10), q=0.5)
 # median_mass is a pyarrow.Scalar, which you can get the value of with .as_py()
 print(median_mass.as_py())
 ```
 
 There is a very extensive set of functions available in the
 `pyarrow.compute` package, which you can see
 [here](https://arrow.apache.org/docs/python/compute.html). These
@@ -155,57 +161,42 @@
 behavior of your tables by adding or overriding methods. For example, if you want to add a
 method to compute the total mass of the asteroids in the table, you
 can do so like this:
 
 ```python
 
 class AsteroidOrbit(TableBase):
-    schema = pa.schema(
-        [
-            pa.field("designation", pa.string()),
-            pa.field("mass", pa.float64(), nullable=True),
-            pa.field("radius", pa.float64(), nullable=True),
-            Coordinates.as_field("coords"),
-        ]
-    )
+	designation = StringField()
+	mass = Float64Field(nullable=True)
+	radius = Float64Field(nullable=True)
+	coords = Coordinates.as_field()
 
     def total_mass(self):
         return pc.sum(self.mass)
 
 ```
 
 You can also use this to add "meta-fields" which are combinations of other fields. For example:
 
 ```python
 class CoordinateCovariance(TableBase):
-    schema = pa.schema(
-        [
-            # The covariance matrix of the coordinates as a 6x6 matrix (3 positions, 3 velocities)
-            pa.field("matrix_values", pa.list_(pa.float64(), 36)),
-        ]
-    )
+	matrix_values = ListField(pa.float64(), 36)
 
     @property
     def matrix(self):
         # This is a numpy array of shape (n, 6, 6)
         return self.matrix_values.to_numpy().reshape(-1, 6, 6)
 
 
 class AsteroidOrbit(TableBase):
-    schema = pa.schema(
-        [
-            pa.field("designation", pa.string()),
-            pa.field("mass", pa.float64(), nullable=True),
-            pa.field("radius", pa.float64(), nullable=True),
-            Coordinates.as_field("coords"),
-            CoordinateCovariance.as_field("covariance"),
-        ]
-    )
-
-
+	designation = StringField()
+	mass = Float64Field(nullable=True)
+	radius = Float64Field(nullable=True)
+	coords = Coordinates.as_field()
+	covariance = CoordinateCovariance.as_field()
 
 orbits = load_orbits() # Analogous to the example above
 
 # Compute the determinant of the covariance matrix for each asteroid
 determinants = np.linalg.det(orbits.covariance.matrix)
 ```
```

