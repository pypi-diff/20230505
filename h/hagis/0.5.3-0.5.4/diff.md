# Comparing `tmp/hagis-0.5.3.tar.gz` & `tmp/hagis-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.5.3.tar", last modified: Fri May  5 01:07:03 2023, max compression
+gzip compressed data, was "hagis-0.5.4.tar", last modified: Fri May  5 18:39:03 2023, max compression
```

## Comparing `hagis-0.5.3.tar` & `hagis-0.5.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 01:07:03.282823 hagis-0.5.3/
--rw-rw-rw-   0        0        0      923 2023-05-05 01:07:03.275681 hagis-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 01:07:03.275681 hagis-0.5.3/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-05 01:07:03.000000 hagis-0.5.3/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-05 01:07:03.000000 hagis-0.5.3/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 01:07:03.000000 hagis-0.5.3/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 01:07:03.000000 hagis-0.5.3/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21659 2023-05-05 01:04:04.000000 hagis-0.5.3/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-05 01:06:02.000000 hagis-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 01:07:03.284484 hagis-0.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 18:39:03.245037 hagis-0.5.4/
+-rw-rw-rw-   0        0        0      923 2023-05-05 18:39:03.243035 hagis-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 18:39:03.241032 hagis-0.5.4/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-05 18:39:03.000000 hagis-0.5.4/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-05 18:39:03.000000 hagis-0.5.4/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 18:39:03.000000 hagis-0.5.4/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 18:39:03.000000 hagis-0.5.4/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21959 2023-05-05 18:26:46.000000 hagis-0.5.4/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-05 14:38:55.000000 hagis-0.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 18:39:03.245037 hagis-0.5.4/setup.cfg
```

### Comparing `hagis-0.5.3/PKG-INFO` & `hagis-0.5.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.3
+Version: 0.5.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.3/hagis.egg-info/PKG-INFO` & `hagis-0.5.4/hagis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.3
+Version: 0.5.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.3/hagis.py` & `hagis-0.5.4/hagis.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,15 +314,15 @@
         obj = self._call("query", where=where_clause, outFields=fields, **kwargs)
         date_fields = [f.name for f in obj.fields if f.type == "esriFieldTypeDate"] if hasattr(obj, "fields") else []
 
         for feature in obj.features:
             if date_fields:
                 for key, value in feature.attributes.__dict__.items():
                     if key in date_fields and value:
-                        feature.attributes.__dict__[key] = datetime.fromtimestamp(value / 1000)
+                        feature.attributes.__dict__[key] = datetime.utcfromtimestamp(value / 1000)
             if hasattr(feature, "geometry") and feature.geometry and hasattr(obj, "spatialReference"):
                 feature.geometry.spatialReference = obj.spatialReference.__dict__
 
         return (obj.features, obj.exceededTransferLimit if hasattr(obj, "exceededTransferLimit") else False)
 
     def _get_oids(self, where_clause: str) -> List[int]:
         obj = self._call("query", where=where_clause, returnIdsOnly="true")
@@ -364,55 +364,57 @@
 
             with futures.ThreadPoolExecutor(max_workers) as executor:
                 for rows in executor.map(get_more_rows, remaining_batches):
                     for row in rows:
                         yield self._map(row)
 
     def _to_sql(self, predicate: Callable[[T], bool]) -> str:
-
         class LambdaFinder(ast.NodeVisitor):
             def __init__(self, expression: Any) -> None:
                 super().__init__()
 
-                # Capture closure variables.
-                closure = expression.__closure__
-                if closure:
-                    self.freevars = dict(zip(expression.__code__.co_freevars, [x.cell_contents for x in closure]))
-                else:
-                    self.freevars = {}
+                self.freevars: Dict[str, Any] = {}
 
                 # Check globals.
                 for name in expression.__code__.co_names:
                     if name in expression.__globals__:
-                        if name not in self.freevars:
-                            self.freevars[name] = expression.__globals__[name]
+                        self.freevars[name] = expression.__globals__[name]
+
+                # Capture closure variables.
+                closure = expression.__closure__
+                if closure:
+                    for name, value in zip(expression.__code__.co_freevars, [x.cell_contents for x in closure]):
+                        self.freevars[name] = value
 
                 line = getsource(expression).strip()
                 self.visit(ast.parse(f"{line}\n    pass" if line.endswith(":") else line))
 
             def visit_Lambda(self, node: ast.Lambda) -> Any:  # pylint: disable-all
                 self.expression = node
 
             @staticmethod
             def find(expression: Any):  # pylint: disable-all
                 visitor = LambdaFinder(expression)
                 return visitor.expression, visitor.freevars
 
         class LambdaVisitor(ast.NodeVisitor):
-
-            def __init__(self, expression: ast.expr, freevars: Dict[str, Any], fields: Dict[str, str]):
+            def __init__(self, expression: ast.expr, freevars: Dict[str, Any], fields: Dict[str, str]) -> None:
                 super().__init__()
                 self._expressions: List[Union[LambdaVisitor, str]] = []
                 self._freevars = freevars
                 self._fields = fields
                 self.visit(expression)
 
             def visit_Attribute(self, node: Attribute) -> Any:
-                field_name = self._fields[node.attr]
-                self._expressions.append(field_name)
+                attr = node.attr
+                value: Any = node.value
+                if value.id in self._freevars:
+                    self._expressions.append(self._get_sql_value(getattr(self._freevars[value.id], attr)))
+                else:
+                    self._expressions.append(self._fields[attr])
 
             def visit_BoolOp(self, node: BoolOp) -> Any:
                 self._expressions.append("(")
                 expressions: List[Union[LambdaVisitor, str]] = []
                 for value in node.values:
                     expressions.append(LambdaVisitor(value, self._freevars, self._fields))
                     expressions.append(self._convert_op(node.op))
@@ -439,21 +441,20 @@
                     self._expressions.append(f"{field_name} LIKE '%{self._get_value(node.left)}%'")
                 else:
                     self._expressions.append(LambdaVisitor(node.left, self._freevars, self._fields))
                     self._expressions.append(self._convert_op(node.ops[0]))
                     self._expressions.append(LambdaVisitor(node.comparators[0], self._freevars, self._fields))
 
             def visit_Constant(self, node: Constant) -> Any:
-                self._expressions.append(self._get_sql_value(node))
+                self._expressions.append(self._get_sql_value(node.value))
 
             def visit_Name(self, node: Name) -> Any:
-                self._expressions.append(self._get_sql_value(node))
+                self._expressions.append(self._get_sql_value(self._freevars[node.id]))
 
-            def _get_sql_value(self, node: Any) -> str:
-                value = self._get_value(node)
+            def _get_sql_value(self, value: Any) -> str:
                 if value is None:
                     return "NULL"
                 if isinstance(value, str):
                     return f"'{value}'"
                 if isinstance(value, datetime):
                     return f"timestamp '{value:%Y-%m-%d %H:%M:%S}'"
                 return str(value)
@@ -486,15 +487,18 @@
 
             def to_sql(self) -> str:
                 text = ""
                 for e in self._expressions:
                     text += e.to_sql() if isinstance(e, LambdaVisitor) else f" {e}"
                 return text
 
+        # Find the lambda expression and any free variables encapsulated in it.
         expression, freevars = LambdaFinder.find(predicate)
+
+        # Generate a where clause.
         where_clause = LambdaVisitor(expression, freevars, self._fields).to_sql().strip()
 
         return where_clause
 
 
 class Point:  # pylint: disable=too-few-public-methods
     """ Point class.
```

### Comparing `hagis-0.5.3/pyproject.toml` & `hagis-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.5.3"
+version = "0.5.4"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

