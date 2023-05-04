# Comparing `tmp/vsexprtools-1.4.3.tar.gz` & `tmp/vsexprtools-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsexprtools-1.4.3.tar", last modified: Sun Mar 26 17:38:40 2023, max compression
+gzip compressed data, was "vsexprtools-1.4.4.tar", last modified: Thu May  4 22:00:22 2023, max compression
```

## Comparing `vsexprtools-1.4.3.tar` & `vsexprtools-1.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:40.257139 vsexprtools-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-26 17:38:40.257139 vsexprtools-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-26 17:38:40.257139 vsexprtools-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:40.253139 vsexprtools-1.4.3/vsexprtools/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/exprop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/polyfills.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-03-26 17:38:13.000000 vsexprtools-1.4.3/vsexprtools/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:40.257139 vsexprtools-1.4.3/vsexprtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-26 17:38:40.000000 vsexprtools-1.4.3/vsexprtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-26 17:38:40.000000 vsexprtools-1.4.3/vsexprtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:38:40.000000 vsexprtools-1.4.3/vsexprtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-26 17:38:40.000000 vsexprtools-1.4.3/vsexprtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-26 17:38:40.000000 vsexprtools-1.4.3/vsexprtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/vsexprtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/exprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/polyfills.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-04 21:59:58.000000 vsexprtools-1.4.4/vsexprtools/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:22.552593 vsexprtools-1.4.4/vsexprtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 22:00:22.000000 vsexprtools-1.4.4/vsexprtools.egg-info/top_level.txt
```

### Comparing `vsexprtools-1.4.3/LICENSE` & `vsexprtools-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.3/PKG-INFO` & `vsexprtools-1.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsexprtools
-Version: 1.4.3
+Version: 1.4.4
 Summary: VapourSynth functions and helpers for writing RPN expressions.
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-exprtools
 Project-URL: Documentation, https://vsexprtools.encode.moe/en/latest/
```

### Comparing `vsexprtools-1.4.3/setup.cfg` & `vsexprtools-1.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.3/setup.py` & `vsexprtools-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.3/vsexprtools/exprop.py` & `vsexprtools-1.4.4/vsexprtools/exprop.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,67 +115,74 @@
         return norm_expr(
             clips, self, planes, format, opt, boundary, force_akarin, func, split_planes, **kwargs  # type: ignore
         )
 
 
 class ExprOpBase(str):
     value: str
+    n_op: int
+
+    def __new__(cls, value: str, n_op: int) -> ExprOpBase:
+        self = super().__new__(cls, value)
+        self.n_op = n_op
+
+        return self
 
     def combine(  # type: ignore
         self: ExprOp, *clips: vs.VideoNode | Iterable[vs.VideoNode | Iterable[vs.VideoNode]],
         suffix: StrArrOpt = None, prefix: StrArrOpt = None, expr_suffix: StrArrOpt = None,
         expr_prefix: StrArrOpt = None, planes: PlanesT = None, **expr_kwargs: Any
     ) -> vs.VideoNode:
         from .funcs import combine
 
         return combine(clips, self, suffix, prefix, expr_suffix, expr_prefix, planes, **expr_kwargs)
 
 
 class ExprOp(ExprOpBase, CustomEnum):
     # 1 Argument
-    EXP = "exp"
-    LOG = "log"
-    SQRT = "sqrt"
-    SIN = "sin"
-    COS = "cos"
-    ABS = "abs"
-    NOT = "not"
-    DUP = "dup"
-    DUPN = "dupN"
-    TRUNC = "trunc"
-    ROUND = "round"
-    FLOOR = "floor"
+    EXP = "exp", 1
+    LOG = "log", 1
+    SQRT = "sqrt", 1
+    SIN = "sin", 1
+    COS = "cos", 1
+    ABS = "abs", 1
+    NOT = "not", 1
+    DUP = "dup", 1
+    DUPN = "dupN", 1
+    TRUNC = "trunc", 1
+    ROUND = "round", 1
+    FLOOR = "floor", 1
 
     # 2 Arguments
-    MAX = "max"
-    MIN = "min"
-    ADD = "+"
-    SUB = "-"
-    MUL = "*"
-    DIV = "/"
-    POW = "pow"
-    GT = ">"
-    LT = "<"
-    EQ = "="
-    GTE = ">="
-    LTE = "<="
-    AND = "and"
-    OR = "or"
-    XOR = "xor"
-    SWAP = "swap"
-    SWAPN = "swapN"
-    MOD = "%"
+    MAX = "max", 2
+    MIN = "min", 2
+    ADD = "+", 2
+    SUB = "-", 2
+    MUL = "*", 2
+    DIV = "/", 2
+    POW = "pow", 2
+    GT = ">", 2
+    LT = "<", 2
+    EQ = "=", 2
+    GTE = ">=", 2
+    LTE = "<=", 2
+    AND = "and", 2
+    OR = "or", 2
+    XOR = "xor", 2
+    SWAP = "swap", 2
+    SWAPN = "swapN", 2
+    MOD = "%", 2
 
     # 3 Arguments
-    TERN = "?"
-    CLAMP = "clamp"
+    TERN = "?", 3
+    CLAMP = "clamp", 3
 
     # Special Operators
-    REL_PIX = '{char:s}[{x:d},{y:d}]'
-    ABS_PIX = '{x:d} {y:d} {char:s}[]'
+    REL_PIX = '{char:s}[{x:d},{y:d}]', 3
+    ABS_PIX = '{x:d} {y:d} {char:s}[]', 3
 
     @overload
     def __call__(  # type: ignore
         self, *clips: VideoNodeIterable, suffix: StrArrOpt = None,
         prefix: StrArrOpt = None, expr_suffix: StrArrOpt = None,
         expr_prefix: StrArrOpt = None, planes: PlanesT = None,
         **expr_kwargs: Any
@@ -190,15 +197,15 @@
         args = list[Any](flatten(pos_args))
 
         if isinstance(args[0], vs.VideoNode):
             return self.combine(*args, **kwargs)
 
         while True:
             try:
-                return ExprOpBase(self.format(*args, **kwargs))
+                return ExprOpBase(self.format(*args, **kwargs), 3)
             except KeyError as key:
                 try:
                     kwargs.update({str(key)[1:-1]: args.pop(0)})
                 except IndexError:
                     raise key
 
     def __str__(self) -> str:
@@ -217,15 +224,15 @@
     def clamp(
         cls, min: float | ExprToken = ExprToken.RangeMin, max: float | ExprToken = ExprToken.RangeMax, c: str = ''
     ) -> ExprList:
 
         if complexpr_available:
             return ExprList([c, min, max, ExprOp.CLAMP])
 
-        return ExprList([c, min, ExprOp.MAX, max, ExprOp.MAX])
+        return ExprList([c, min, ExprOp.MAX, max, ExprOp.MIN])
 
     @classmethod
     def matrix(
         cls, var: str, radius: int, mode: ConvMode = ConvMode.SQUARE, exclude: Iterable[tuple[int, int]] = []
     ) -> ExprList:
         exclude = list(exclude)
```

### Comparing `vsexprtools-1.4.3/vsexprtools/funcs.py` & `vsexprtools-1.4.4/vsexprtools/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,17 @@
 
     n_clips = len(clips)
 
     prefixes, suffixes = (_combine_norm__ix(x, n_clips) for x in (prefix, suffix))
 
     args = zip(prefixes, ExprVars(n_clips), suffixes)
 
-    operators = operator * max(n_clips - 1, 1)
+    has_op = (n_clips >= operator.n_op) or any(x is not None for x in (suffix, prefix, expr_suffix, expr_prefix))
+
+    operators = operator * max(n_clips - 1, int(has_op))
 
     return norm_expr(clips, [expr_prefix, args, operators, expr_suffix], planes, **kwargs)
 
 
 def norm_expr(
     clips: VideoNodeIterable, expr: str | StrArr | tuple[str | StrArr, ...], planes: PlanesT = None,
     format: HoldsVideoFormatT | VideoFormatT | None = None, opt: bool | None = None,
```

### Comparing `vsexprtools-1.4.3/vsexprtools/manager.py` & `vsexprtools-1.4.4/vsexprtools/manager.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.3/vsexprtools/operators.py` & `vsexprtools-1.4.4/vsexprtools/operators.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.3/vsexprtools/polyfills.py` & `vsexprtools-1.4.4/vsexprtools/polyfills.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.3/vsexprtools/util.py` & `vsexprtools-1.4.4/vsexprtools/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     func = func or bitdepth_aware_tokenize_expr
 
     if not expr or len(expr) < 4:
         return expr
 
     replaces = list[tuple[str, Callable[[vs.VideoNode, bool, ColorRange], float]]]()
 
-    for token in ExprToken:
+    for token in sorted(ExprToken, key=lambda x: len(x), reverse=True):
         if token.value in expr:
             replaces.append((token.value, token.get_value))
 
         if token.name in expr:
             replaces.append(
                 (f'{token.__class__.__name__}.{token.name}', token.get_value)
             )
```

### Comparing `vsexprtools-1.4.3/vsexprtools/variables.py` & `vsexprtools-1.4.4/vsexprtools/variables.py`

 * *Files identical despite different names*

### Comparing `vsexprtools-1.4.3/vsexprtools.egg-info/PKG-INFO` & `vsexprtools-1.4.4/vsexprtools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsexprtools
-Version: 1.4.3
+Version: 1.4.4
 Summary: VapourSynth functions and helpers for writing RPN expressions.
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-exprtools
 Project-URL: Documentation, https://vsexprtools.encode.moe/en/latest/
```

