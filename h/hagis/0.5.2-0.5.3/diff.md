# Comparing `tmp/hagis-0.5.2.tar.gz` & `tmp/hagis-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.5.2.tar", last modified: Thu May  4 17:45:11 2023, max compression
+gzip compressed data, was "hagis-0.5.3.tar", last modified: Fri May  5 01:07:03 2023, max compression
```

## Comparing `hagis-0.5.2.tar` & `hagis-0.5.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:45:11.918082 hagis-0.5.2/
--rw-rw-rw-   0        0        0      923 2023-05-04 17:45:11.916170 hagis-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 17:45:11.912626 hagis-0.5.2/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-04 17:45:11.000000 hagis-0.5.2/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-04 17:45:11.000000 hagis-0.5.2/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:45:11.000000 hagis-0.5.2/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-04 17:45:11.000000 hagis-0.5.2/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21207 2023-05-04 17:43:31.000000 hagis-0.5.2/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-04 17:44:08.000000 hagis-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 17:45:11.919524 hagis-0.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 01:07:03.282823 hagis-0.5.3/
+-rw-rw-rw-   0        0        0      923 2023-05-05 01:07:03.275681 hagis-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 01:07:03.275681 hagis-0.5.3/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-05 01:07:03.000000 hagis-0.5.3/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-05 01:07:03.000000 hagis-0.5.3/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 01:07:03.000000 hagis-0.5.3/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 01:07:03.000000 hagis-0.5.3/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21659 2023-05-05 01:04:04.000000 hagis-0.5.3/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-05 01:06:02.000000 hagis-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 01:07:03.284484 hagis-0.5.3/setup.cfg
```

### Comparing `hagis-0.5.2/PKG-INFO` & `hagis-0.5.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.2
+Version: 0.5.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.2/hagis.egg-info/PKG-INFO` & `hagis-0.5.3/hagis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.2
+Version: 0.5.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.2/hagis.py` & `hagis-0.5.3/hagis.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,19 +368,28 @@
                         yield self._map(row)
 
     def _to_sql(self, predicate: Callable[[T], bool]) -> str:
 
         class LambdaFinder(ast.NodeVisitor):
             def __init__(self, expression: Any) -> None:
                 super().__init__()
+
+                # Capture closure variables.
                 closure = expression.__closure__
                 if closure:
                     self.freevars = dict(zip(expression.__code__.co_freevars, [x.cell_contents for x in closure]))
                 else:
                     self.freevars = {}
+
+                # Check globals.
+                for name in expression.__code__.co_names:
+                    if name in expression.__globals__:
+                        if name not in self.freevars:
+                            self.freevars[name] = expression.__globals__[name]
+
                 line = getsource(expression).strip()
                 self.visit(ast.parse(f"{line}\n    pass" if line.endswith(":") else line))
 
             def visit_Lambda(self, node: ast.Lambda) -> Any:  # pylint: disable-all
                 self.expression = node
 
             @staticmethod
@@ -441,14 +450,16 @@
 
             def _get_sql_value(self, node: Any) -> str:
                 value = self._get_value(node)
                 if value is None:
                     return "NULL"
                 if isinstance(value, str):
                     return f"'{value}'"
+                if isinstance(value, datetime):
+                    return f"timestamp '{value:%Y-%m-%d %H:%M:%S}'"
                 return str(value)
 
             def _get_value(self, node: Any) -> Any:
                 return self._freevars[node.id] if isinstance(node, Name) else node.value
 
             def _convert_op(self, op: Any) -> str:
                 if isinstance(op, ast.And):
@@ -476,15 +487,14 @@
             def to_sql(self) -> str:
                 text = ""
                 for e in self._expressions:
                     text += e.to_sql() if isinstance(e, LambdaVisitor) else f" {e}"
                 return text
 
         expression, freevars = LambdaFinder.find(predicate)
-
         where_clause = LambdaVisitor(expression, freevars, self._fields).to_sql().strip()
 
         return where_clause
 
 
 class Point:  # pylint: disable=too-few-public-methods
     """ Point class.
```

### Comparing `hagis-0.5.2/pyproject.toml` & `hagis-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

