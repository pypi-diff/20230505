# Comparing `tmp/stlog-0.0.8.tar.gz` & `tmp/stlog-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlog-0.0.8.tar", max compression
+gzip compressed data, was "stlog-0.1.0.tar", max compression
```

## Comparing `stlog-0.0.8.tar` & `stlog-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-04-21 15:06:41.936559 stlog-0.0.8/LICENSE
--rw-r--r--   0        0        0     8365 2023-04-21 15:06:41.936559 stlog-0.0.8/README.md
--rw-r--r--   0        0        0     1089 2023-04-21 15:07:02.157027 stlog-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      593 2023-04-21 15:07:01.813020 stlog-0.0.8/stlog/__init__.py
--rw-r--r--   0        0        0     2658 2023-04-21 15:06:41.940559 stlog-0.0.8/stlog/adapter.py
--rw-r--r--   0        0        0     7632 2023-04-21 15:06:41.940559 stlog-0.0.8/stlog/base.py
--rw-r--r--   0        0        0     2638 2023-04-21 15:06:41.940559 stlog-0.0.8/stlog/context.py
--rw-r--r--   0        0        0    12850 2023-04-21 15:06:41.940559 stlog-0.0.8/stlog/formatter.py
--rw-r--r--   0        0        0     2499 2023-04-21 15:06:41.944559 stlog-0.0.8/stlog/handler.py
--rw-r--r--   0        0        0     3284 2023-04-21 15:06:41.944559 stlog-0.0.8/stlog/kvformatter.py
--rw-r--r--   0        0        0     5109 2023-04-21 15:06:41.944559 stlog-0.0.8/stlog/output.py
--rw-r--r--   0        0        0     7070 2023-04-21 15:06:41.944559 stlog-0.0.8/stlog/setup.py
--rw-r--r--   0        0        0     8917 1970-01-01 00:00:00.000000 stlog-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-05 11:49:10.364241 stlog-0.1.0/LICENSE
+-rw-r--r--   0        0        0     8415 2023-05-05 11:49:10.364241 stlog-0.1.0/README.md
+-rw-r--r--   0        0        0     1089 2023-05-05 11:49:33.904414 stlog-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      593 2023-05-05 11:49:33.548411 stlog-0.1.0/stlog/__init__.py
+-rw-r--r--   0        0        0     2658 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/adapter.py
+-rw-r--r--   0        0        0     7771 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/base.py
+-rw-r--r--   0        0        0     2638 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/context.py
+-rw-r--r--   0        0        0    13298 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/formatter.py
+-rw-r--r--   0        0        0     2499 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/handler.py
+-rw-r--r--   0        0        0     5173 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/kvformatter.py
+-rw-r--r--   0        0        0     5109 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/output.py
+-rw-r--r--   0        0        0     7070 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/setup.py
+-rw-r--r--   0        0        0     8967 1970-01-01 00:00:00.000000 stlog-0.1.0/PKG-INFO
```

### Comparing `stlog-0.0.8/LICENSE` & `stlog-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stlog-0.0.8/README.md` & `stlog-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -246,8 +246,9 @@
 ```
 
 <!--quickstart-end-->
 
 ## Roadmap
 
 - [ ] add `file` outputs
-- [ ] add a full `logfmt` formatter
+- [x] add a full `logfmt` formatter
+- [ ] more configuration options through env vars
```

### Comparing `stlog-0.0.8/pyproject.toml` & `stlog-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stlog"
-version = "0.0.8"
+version = "0.1.0"
 description = ""
 authors = ["Fabien MARTY <fabien.marty@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "stlog"}]
 
 [tool.poetry.dependencies]
```

### Comparing `stlog-0.0.8/stlog/__init__.py` & `stlog-0.1.0/stlog/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     "base": False,
     "adapter": False,
     "handler": False,
     "context": False,
     "warn": False,
     "fatal": False,
 }
-VERSION = "0.0.8"
+VERSION = "0.1.0"
```

### Comparing `stlog-0.0.8/stlog/adapter.py` & `stlog-0.1.0/stlog/adapter.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.8/stlog/base.py` & `stlog-0.1.0/stlog/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,16 @@
         for key, value in to_check.items():
             if not isinstance(key, str):
                 raise StlogError("dict keys should be str, found %s" % type(key))
             check_json_types_or_raise(value)
 
 
 # Adapted from https://github.com/jteppinette/python-logfmter/blob/main/logfmter/formatter.py
+# FIXME: have a look at golang code to see if the encoding here is enough
+# https://github.com/go-logfmt/logfmt/blob/v0.6.0/encode.go#L236
 def logfmt_format_string(value: str) -> str:
     needs_dquote_escaping = '"' in value
     needs_newline_escaping = "\n" in value
     needs_quoting = " " in value or "=" in value
     if needs_dquote_escaping:
         value = value.replace('"', '\\"')
     if needs_newline_escaping:
```

### Comparing `stlog-0.0.8/stlog/context.py` & `stlog-0.1.0/stlog/context.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.8/stlog/formatter.py` & `stlog-0.1.0/stlog/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,19 @@
     """Abstract base class for `stlog` formatters.
 
     Attributes:
         fmt: the default format for the formatter.
         datefmt: the format to use for `{asctime}` placeholder.
         style: can be '%', '{' or '$' to select how the format string will be merged with its data
             (see https://docs.python.org/3/library/logging.html#logging.Formatter for details)
-        include_extras_keys_fnmatchs: fnmatch patterns list for including keys in `{extra}` placeholder.
-        exclude_extras_keys_fnmatchs: fnmatch patterns list for excluding keys in `{extra}` placeholder.
+        include_extras_keys_fnmatchs: fnmatch patterns list for including keys in `{extras}` placeholder.
+        exclude_extras_keys_fnmatchs: fnmatch patterns list for excluding keys in `{extras}` placeholder.
         extra_key_rename_fn: callable which takes a key name and return a renamed key to use
             (or None to ignore the key/value).
-        extra_key_max_length: maximum size of extra keys to be included in `{extra}` placeholder
+        extra_key_max_length: maximum size of extra keys to be included in `{extras}` placeholder
             (after this limit, the value will be truncated and ... will be added at the end, 0 means "no limit").
         converter: time converter function (use `time.gmtime` (default) for UTC date/times, use `time.time`
             for local date/times), if you change the default, please change also `datefmt` keyword.
         kv_formatter: key values special formatter for formatting `{extras}`
             placeholder.
         include_reserved_attrs_in_extras: automatical include some reserved
             logrecord attributes in "extras" (example: `["process", "thread"]`).
@@ -81,22 +81,45 @@
 
     fmt: str | None = None
     datefmt: str | None = DEFAULT_STLOG_DATE_FORMAT
     style: str = "{"
     include_extras_keys_fnmatchs: Sequence[str] | None = None
     exclude_extras_keys_fnmatchs: Sequence[str] | None = None
     extra_key_rename_fn: Callable[[str], str | None] | None = None
-    extra_key_max_length: int = 32
+    extra_key_max_length: int | None = None
     converter: Callable[[float | None], time.struct_time] = time.gmtime
     kv_formatter: KVFormatter | None = None
     include_reserved_attrs_in_extras: Sequence[str] = field(default_factory=list)
     _placeholders_in_fmt: list[str] | None = field(
         init=False, default=None, repr=False, compare=False
     )
 
+    def __post_init__(self):
+        super().__init__(  # explicit call because logging.Formatter is not a dataclass
+            fmt=self.fmt, datefmt=self.datefmt, style=self.style  # type: ignore
+        )
+        if self.extra_key_max_length is None:
+            self.extra_key_max_length = 32
+        self.include_extra_keys_patterns: list[re.Pattern] = [
+            re.compile(fnmatch.translate("*"))
+        ]  # all by default
+        self.exclude_extra_keys_patterns: list[re.Pattern] = []  # empty by default
+        if self.include_extras_keys_fnmatchs is not None:
+            self.include_extra_keys_patterns = [
+                re.compile(fnmatch.translate(x))
+                for x in self.include_extras_keys_fnmatchs
+            ]
+        if self.exclude_extras_keys_fnmatchs is not None:
+            self.exclude_extra_keys_patterns = [
+                re.compile(fnmatch.translate(x))
+                for x in self.exclude_extras_keys_fnmatchs
+            ]
+        if GLOBAL_LOGGING_CONFIG._unit_tests_mode:
+            self.converter = _unit_tests_converter
+
     @property
     def placeholders_in_fmt(self) -> list[str]:
         if self._placeholders_in_fmt is None:
             self._placeholders_in_fmt = parse_format(self.fmt, self.style)
         return self._placeholders_in_fmt
 
     def _make_extras_string(
@@ -112,35 +135,14 @@
             self.include_reserved_attrs_in_extras
         ):
             key = self._make_extra_key_name(k)
             if key:
                 kvs[key] = getattr(record, k)
         return self.kv_formatter.format(kvs)
 
-    def __post_init__(self):
-        super().__init__(  # explicit call because logging.Formatter is not a dataclass
-            fmt=self.fmt, datefmt=self.datefmt, style=self.style  # type: ignore
-        )
-        self.include_extra_keys_patterns: list[re.Pattern] = [
-            re.compile(fnmatch.translate("*"))
-        ]  # all by default
-        self.exclude_extra_keys_patterns: list[re.Pattern] = []  # empty by default
-        if self.include_extras_keys_fnmatchs is not None:
-            self.include_extra_keys_patterns = [
-                re.compile(fnmatch.translate(x))
-                for x in self.include_extras_keys_fnmatchs
-            ]
-        if self.exclude_extras_keys_fnmatchs is not None:
-            self.exclude_extra_keys_patterns = [
-                re.compile(fnmatch.translate(x))
-                for x in self.exclude_extras_keys_fnmatchs
-            ]
-        if GLOBAL_LOGGING_CONFIG._unit_tests_mode:
-            self.converter = _unit_tests_converter
-
     def _make_extra_key_name(self, extra_key: str) -> str | None:
         new_extra_key: str | None = extra_key
         if self.extra_key_rename_fn is not None:
             new_extra_key = (self.extra_key_rename_fn)(extra_key)
         if new_extra_key is None:
             return None
         for pattern in self.include_extra_keys_patterns:
@@ -148,15 +150,18 @@
                 break
         else:
             # not found
             return None
         for pattern in self.exclude_extra_keys_patterns:
             if re.match(pattern, new_extra_key):
                 return None
-        return _truncate_str(new_extra_key, self.extra_key_max_length)
+        return _truncate_str(
+            new_extra_key,
+            self.extra_key_max_length if self.extra_key_max_length is not None else 0,
+        )
 
     def format(self, record: logging.LogRecord) -> str:
         if GLOBAL_LOGGING_CONFIG._unit_tests_mode:
             # FIXME: it would be better as a Filter, wouldn't be?
             # fix some fields in record to get always the same values
             record.filename = "filename.py"
             record.pathname = "/path/filename.py"
@@ -168,29 +173,29 @@
 
 
 # Adapted from https://github.com/Mergifyio/daiquiri/blob/main/daiquiri/formatter.py
 @dataclass
 class HumanFormatter(Formatter):
     """Formatter for a "human" output.
 
-    Extra keywords are merged into a `{extra}` placeholder by a `stlog.kvformatter.KVFormatter`.
+    Extra keywords are merged into a `{extras}` placeholder by a `stlog.kvformatter.KVFormatter`.
 
     If you use this placeholder on your `fmt`, any keywords
     passed to a logging call will be formatted into a "extras" string and
     included in a logging message.
 
     Example::
 
         logger.info("my message", foo="bar", foo2=123)
 
     will cause an "extras" string of::
 
         {foo=bar foo2=123}
 
-    You can change the way the `{extra}` placeholder is formatted
+    You can change the way the `{extras}` placeholder is formatted
     by providing a KVFormatter object.
 
     """
 
     def __post_init__(self):
         if self.fmt is None:
             self.fmt = DEFAULT_STLOG_HUMAN_FORMAT
@@ -285,24 +290,26 @@
         return format_string(self.fmt, self.style, record_dict)
 
 
 @dataclass
 class JsonFormatter(Formatter):
     """Formatter for a JSON / parsing friendly output."""
 
-    extra_key_max_length: int = 0
     indent: int | None = None
     sort_keys: bool = True
-    include_extras_in_key: str | None = None
+    include_extras_in_key: str | None = ""
     exc_info_key: str | None = "exc_info"
     stack_info_key: str | None = "stack_info"
 
     def __post_init__(self):
+        if self.extra_key_max_length is None:
+            self.extra_key_max_length = 0
         if self.kv_formatter is None:
-            self.kv_formatter = JsonKVFormatter()
+            # note: no need to sort/indent here as it will be sorted/indented at this level
+            self.kv_formatter = JsonKVFormatter(sort_keys=False, indent=False)
         if self.fmt is None:
             self.fmt = DEFAULT_STLOG_JSON_FORMAT
         if self.extra_key_rename_fn is None:
             self.extra_key_rename_fn = json_formatter_default_extra_key_rename_fn
         super().__post_init__()
 
     def json_serialize(self, message_dict: dict[str, Any]) -> str:
@@ -319,22 +326,23 @@
             record.asctime = self.formatTime(record, self.datefmt)
         record_dict: dict[str, Any] = {
             k: json.dumps(getattr(record, k))
             for k in self.placeholders_in_fmt
             if k != "extras"
         }
         s = format_string(self.fmt, self.style, record_dict)
-        obj = json.loads(s)
-        extras_obj = json.loads(self._make_extras_string(record))
-        if self.include_extras_in_key:
-            obj[self.include_extras_in_key] = extras_obj
-        else:
-            for key, value in extras_obj.items():
-                if key not in obj:
-                    obj[key] = value
+        if self.include_extras_in_key is not None:
+            obj = json.loads(s)
+            extras_obj = json.loads(self._make_extras_string(record))
+            if self.include_extras_in_key == "":
+                for key, value in extras_obj.items():
+                    if key not in obj:
+                        obj[key] = value
+            else:
+                obj[self.include_extras_in_key] = extras_obj
         if self.exc_info_key:
             if record.exc_info:
                 obj[self.exc_info_key] = self.formatException(record.exc_info)
             elif record.exc_text:
                 obj[self.exc_info_key] = record.exc_text
         if self.stack_info_key and record.stack_info:
             obj[self.stack_info_key] = self.formatStack(record.stack_info)
```

### Comparing `stlog-0.0.8/stlog/handler.py` & `stlog-0.1.0/stlog/handler.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.8/stlog/output.py` & `stlog-0.1.0/stlog/output.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.8/stlog/setup.py` & `stlog-0.1.0/stlog/setup.py`

 * *Files identical despite different names*

### Comparing `stlog-0.0.8/PKG-INFO` & `stlog-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlog
-Version: 0.0.8
+Version: 0.1.0
 Summary: 
 License: MIT
 Author: Fabien MARTY
 Author-email: fabien.marty@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -263,9 +263,10 @@
 ```
 
 <!--quickstart-end-->
 
 ## Roadmap
 
 - [ ] add `file` outputs
-- [ ] add a full `logfmt` formatter
+- [x] add a full `logfmt` formatter
+- [ ] more configuration options through env vars
```

