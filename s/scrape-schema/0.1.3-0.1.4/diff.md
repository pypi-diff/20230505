# Comparing `tmp/scrape_schema-0.1.3.tar.gz` & `tmp/scrape_schema-0.1.4.tar.gz`

## Comparing `scrape_schema-0.1.3.tar` & `scrape_schema-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/__init__.py
--rw-r--r--   0        0        0    22015 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/callbacks/parsel.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/parsel.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/LICENSE
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/README.md
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/__init__.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/_base_configs.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/_logger.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/_type_caster.py
+-rw-r--r--   0        0        0    20804 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/callbacks/parsel.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/mock.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/parsel.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/README.md
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 scrape_schema-0.1.4/PKG-INFO
```

### Comparing `scrape_schema-0.1.3/scrape_schema/base.py` & `scrape_schema-0.1.4/scrape_schema/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import logging
 import sys
 import warnings
 from abc import ABC, abstractmethod
 from typing import (
     Any,
     ByteString,
     Callable,
-    ClassVar,
     Dict,
     Iterable,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
@@ -28,157 +26,68 @@
     from typing_extensions import TypeAlias, get_args, get_origin, get_type_hints
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
+from scrape_schema._base_configs import BaseFieldConfig, BaseSchemaConfig
+from scrape_schema._logger import logger
+from scrape_schema._type_caster import TypeCaster
 from scrape_schema.exceptions import MarkupNotFoundError, ParseFailAttemptsError
 
-NoneType = type(None)
-
-logger = logging.getLogger("scrape_schema")
-logger.setLevel(logging.DEBUG)
-_formatter = logging.Formatter("%(asctime)s [%(levelname)s] %(message)s")
-_stdout_handler = logging.StreamHandler()
-_stdout_handler.setFormatter(_formatter)
-logger.addHandler(_stdout_handler)
-
 T = TypeVar("T")
 MARKUP_TYPE: TypeAlias = Any
 
 
 def extract_fields(markup: MARKUP_TYPE, **fields: "BaseField") -> Dict[str, Any]:
     return {key: field.extract(markup) for key, field in fields.items()}
 
 
 class ABCField(ABC):
     @abstractmethod
     def _parse(self, markup: MARKUP_TYPE) -> Any:
         ...
 
     @abstractmethod
-    def _filter(self, value: T) -> bool:
+    def _filter(
+        self,
+        value: T,
+        *,
+        schema_instance: Optional["BaseSchema"] = None,
+        name: Optional[str] = None,
+    ) -> bool:
         ...
 
     @abstractmethod
-    def _factory(self, value: T) -> T:
+    def _factory(
+        self,
+        value: T,
+        *,
+        schema_instance: Optional["BaseSchema"] = None,
+        name: Optional[str] = None,
+    ) -> T:
         ...
 
     @abstractmethod
-    def _callback(self, value: T) -> T:
+    def _callback(
+        self,
+        value: T,
+        *,
+        schema_instance: Optional["BaseSchema"] = None,
+        name: Optional[str] = None,
+    ) -> T:
         ...
 
     @abstractmethod
     def _typing(self, instance: "BaseSchema", name: str, value: T) -> T:
         ...
 
 
-class TypeCaster:
-    @staticmethod
-    def _is_iterable_and_not_string_type(value_type: Type) -> bool:
-        return issubclass(value_type, Iterable) and not issubclass(
-            value_type, (ByteString, str)
-        )
-
-    @staticmethod
-    def _is_iterable_and_not_string_value(value: T) -> bool:
-        return isinstance(value, Iterable) and not (
-            isinstance(value, (ByteString, str))
-        )
-
-    def _typing_to_builtin(self, type_hint: Type) -> Type:
-        origin = get_origin(type_hint)
-        args = get_args(type_hint)
-
-        if origin is not None and args:
-            # Recursively convert the nested generic types
-            converted_args = tuple(self._typing_to_builtin(arg) for arg in args)
-            return origin[converted_args]
-        else:
-            return type_hint
-
-    def _cast_type(self, type_hint: Type, value: Any) -> Any:
-        if sys.version_info >= (3, 9):
-            type_hint = self._typing_to_builtin(type_hint)
-
-        origin = get_origin(type_hint)
-        args = get_args(type_hint)
-        logger.info(
-            "`%s` Cast type start. `value=%s`, type_annotation=%s, `origin=%s`, `args=%s`",
-            self.__class__.__name__,
-            value,
-            type_hint,
-            origin,
-            args,
-        )
-        # None
-        if value is None and type_hint is not bool:
-            return value
-
-        if origin is not None and args:
-            # list
-            if origin is list:
-                logger.debug(
-                    "List cast %s -> arg=%s, value=%s",
-                    self.__class__.__name__,
-                    args[0],
-                    value,
-                )
-                return [self._cast_type(type_hint=args[0], value=v) for v in value]
-            # dict
-            elif origin is dict:
-                key_type, value_type = args
-                logger.debug(
-                    "Dict cast %s -> key=%s, value=%s  `%s`",
-                    self.__class__.__name__,
-                    key_type.__name__,
-                    value_type.__name__,
-                    value,
-                )
-                return {
-                    self._cast_type(type_hint=key_type, value=k): self._cast_type(
-                        type_hint=value_type, value=v
-                    )
-                    for k, v in value.items()
-                }
-            # Optional
-            elif origin is Union:
-                if value is None and NoneType in args:
-                    logger.debug(
-                        "Optional cast %s -> %s", self.__class__.__name__, value
-                    )
-                    return None
-                # in python3.8 raise TypeError: issubclass() arg 1 must be a class
-                # example _cast_type(Optional[List[int]], [])
-                non_none_args = [arg for arg in args if arg is not NoneType]
-                if len(non_none_args) == 1:
-                    return self._cast_type(type_hint=non_none_args[0], value=value)
-        # bool cast
-        elif type_hint is bool:
-            logger.debug("Cast %s `%s()` -> bool", self.__class__.__name__, value)
-            return bool(value)
-        else:
-            # direct cast
-            logger.debug(
-                "Cast `%s` := `%s(%s)`", self.__class__.__name__, type_hint, value
-            )
-            return type_hint(value)
-
-
-class BaseFieldConfig:
-    """BaseField configuration class:
-
-    * parser: Optional[Type[Any]] - parser backend object. If value None - work with python str
-    """
-
-    parser: ClassVar[Optional[Type[Any]]] = None
-
-
-class BaseField(ABCField, TypeCaster):
+class BaseField(ABCField):
     class Config(BaseFieldConfig):
         pass
 
     def __init__(
         self,
         *,
         default: Optional[Any] = None,
@@ -195,24 +104,37 @@
         :param factory: function for evaluate result value. If passed - **ignore auto-typing feature**
         :param kwargs: any params for create fields
         """
         self.factory = factory
         self.callback = callback
         self.filter_ = filter_
         self.default = default
+        self._type_caster = TypeCaster()
 
     @abstractmethod
     def _parse(self, markup: MARKUP_TYPE) -> Any:
         """first parser entrypoint
 
         :param markup: parser class object or string. this value can be config in Config class
         :return: first parsed value
         """
         ...
 
+    @staticmethod
+    def _is_iterable_and_not_string_type(value_type: Type) -> bool:
+        return issubclass(value_type, Iterable) and not issubclass(
+            value_type, (ByteString, str)
+        )
+
+    @staticmethod
+    def _is_iterable_and_not_string_value(value: T) -> bool:
+        return isinstance(value, Iterable) and not (
+            isinstance(value, (ByteString, str))
+        )
+
     def extract(self, markup: MARKUP_TYPE, *, type_: Optional[Type] = None) -> Any:
         """parse markup without BaseSchema Instance
 
         :param markup: string target
         :param type_: optional type for type-casting
         """
         logger.info(
@@ -222,16 +144,15 @@
             repr(self.factory),
             repr(self.callback),
             repr(self.filter_),
             self.default,
         )
         if self.Config.parser and not isinstance(markup, self.Config.parser):
             raise TypeError(
-                f"Markup in `{self.__class__.__name__}` "
-                f"should be `{self.Config.parser.__name__}`,"
+                f"markup argument excepted {self.Config.parser.__name__} "
                 f"not {type(markup).__name__}"
             )
         value = self._parse(markup)
         if not value:
             logger.debug(
                 "%s.extract value not found, set default `%s` value",
                 self.__class__.__name__,
@@ -245,150 +166,200 @@
         if self.callback:
             logger.debug("%s.extract `callback(%s)`", self.__class__.__name__, value)
             value = self._callback(value)
         if self.factory:
             logger.debug("%s.extract `factory(%s)`", self.__class__.__name__, value)
             value = self._factory(value)
         elif type_:
-            value = self._cast_type(type_, value)
+            value = self._type_caster.cast(type_, value)
         logger.info(
             "%s.extract return `%s[%s]`",
             self.__class__.__name__,
             value,
             type(value).__name__,
         )
         return value
 
     def __call__(self, instance: "BaseSchema", name: str, markup: MARKUP_TYPE) -> Any:
+        """parser entrypoint inside a BaseSchema object"""
         logger.info(
             "%s.%s[%s]: Field attrs: factory=%s, callback=%s, filter_=%s, default=%s",
-            instance.__class__.__name__,
+            instance.__schema_name__,
             name,
             self.Config.parser or "str",
             repr(self.factory),
             repr(self.callback),
             repr(self.filter_),
             self.default,
         )
         value = self._parse(markup)
         if not value:
             logger.debug(
-                "%s.%s: value not found, set default `%s` value",
-                instance.__class__.__name__,
+                "%s.%s: value is %s, set default `%s`",
+                instance.__schema_name__,
                 name,
+                value,
                 self.default,
             )
             value = self.default
         else:
             logger.debug(
-                "%s.%s := %s raw value(s)", instance.__class__.__name__, name, value
-            )
-
-        if self._is_iterable_and_not_string_value(value):
-            value = self._filter(value)
-            if self.filter_:
-                logger.debug(
-                    "%s.%s := filter_(%s)", instance.__class__.__name__, name, value
-                )
-
-        value = self._callback(value)
-        if self.callback:
-            logger.debug(
-                "%s.%s := callback(%s)", instance.__class__.__name__, name, value
+                "%s.%s := %s raw value(s)", instance.__schema_name__, name, value
             )
 
-        if self.factory:
-            value = self._factory(value)
-            logger.debug(
-                "%s.%s := factory(%s)", instance.__class__.__name__, name, value
-            )
+        value = self._filter(value, schema_instance=instance, name=name)
+        value = self._callback(value, schema_instance=instance, name=name)
+        if self.factory or self.Config.hooks.get_factory(name):
+            value = self._factory(value, schema_instance=instance, name=name)
         else:
             value = self._typing(instance, name, value)
         logger.info("%s.%s = `%s` Done", instance.__class__.__name__, name, value)
         return value
 
-    def _filter(self, value: T) -> Any:
+    def _filter(
+        self,
+        value: T,
+        *,
+        schema_instance: Optional["BaseSchema"] = None,
+        name: Optional[str] = None,
+    ) -> Any:
         """filter parsed value by filter_ function, if it passed
 
         :param value: list or dict value. dict filter by values
         :return: filtered value
         """
-        if self.filter_:
+        if schema_instance and name:
+            if schema_instance.Config.hooks_priority:
+                hook = self.Config.hooks.get_filter(
+                    f"{schema_instance.__schema_name__}.{name}"
+                )
+                filter_ = hook or self.filter_
+            else:
+                hook = self.Config.hooks.get_filter(
+                    f"{schema_instance.__schema_name__}.{name}"
+                )
+                filter_ = self.filter_ or hook
+        else:
+            filter_ = self.filter_
+
+        if filter_ and self._is_iterable_and_not_string_value(value):
+            logger.debug(
+                "%s.%s := filter_(%s)",
+                schema_instance.__schema_name__
+                if schema_instance
+                else self.__class__.__name__,
+                name or "extract",
+                value,
+            )
             if isinstance(value, list):
-                return list(filter(self.filter_, value))
+                return list(filter(filter_, value))
             elif isinstance(value, dict):
-                return {k: v for k, v in value.items() if self.filter_(v)}
+                return {k: v for k, v in value.items() if filter_(v)}
         return value
 
-    def _factory(self, value: T) -> Any:
+    def _factory(
+        self,
+        value: T,
+        *,
+        schema_instance: Optional["BaseSchema"] = None,
+        name: Optional[str] = None,
+    ) -> Any:
         """factory result value entrypoint
 
         :param value: parsed value
         :return:
         """
-        return self.factory(value) if self.factory else value
+        if schema_instance and name:
+            if schema_instance.Config.hooks_priority:
+                hook = self.Config.hooks.get_factory(
+                    f"{schema_instance.__schema_name__}.{name}"
+                )
+                factory = hook or self.factory
+            else:
+                hook = self.Config.hooks.get_factory(
+                    f"{schema_instance.__schema_name__}.{name}"
+                )
+                factory = self.factory or hook
+        else:
+            factory = self.factory
+        if factory:
+            logger.debug(
+                "%s.%s := factory(%s)",
+                schema_instance.__schema_name__
+                if schema_instance
+                else self.__class__.__name__,
+                name or "extract",
+                value,
+            )
+        return factory(value) if factory else value
 
-    def _callback(self, value: T) -> Any:
+    def _callback(
+        self,
+        value: T,
+        *,
+        schema_instance: Optional["BaseSchema"] = None,
+        name: Optional[str] = None,
+    ) -> Any:
         """eval value by callback function
 
         :param value:
         :return:
         """
-        if not self.callback:
+        if schema_instance and name:
+            if schema_instance.Config.hooks_priority:
+                hook = self.Config.hooks.get_callback(
+                    f"{schema_instance.__schema_name__}.{name}"
+                )
+                callback = hook or self.callback
+            else:
+                hook = self.Config.hooks.get_callback(
+                    f"{schema_instance.__schema_name__}.{name}"
+                )
+                callback = self.callback or hook
+        else:
+            callback = self.callback
+
+        if not callback:
             return value
+        logger.debug(
+            "%s.%s := callback(%s)",
+            schema_instance.__schema_name__
+            if schema_instance
+            else self.__class__.__name__,
+            name or "extract",
+            value,
+        )
         if not self._is_iterable_and_not_string_value(value):
-            return self.callback(value)
+            return callback(value)
         if isinstance(value, list):
-            return [self.callback(i) for i in value]
+            return [callback(i) for i in value]
         elif isinstance(value, dict):
-            return {k: self.callback(v) for k, v in value}
-        return self.callback(value)
+            return {k: callback(v) for k, v in value}
+        return callback(value)
 
     def _typing(self, instance: "BaseSchema", name: str, value: T) -> Any:
         """auto type-cast method
 
         :param instance: BaseSchema instance
         :param name: field name
         :param value: field value
         :return: typed value
         """
         if instance.Config.type_cast:
             if type_annotation := instance.__schema_annotations__.get(name):
-                value = self._cast_type(type_annotation, value)
+                value = self._type_caster.cast(type_annotation, value)
         return value
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}(default={self.default}, callback={self.callback}, "
             f"filter_={self.filter_}, factory={self.factory})"
         )
 
 
-class BaseSchemaConfig:
-    """Schema configuration for BaseSchema
-
-    parsers_config: dict[Type[Any], dict[str, Any]] parser classes for usage backend
-
-    type_cast: bool usage type casting feature. default True
-
-    fails_attempt: int - fields parse success counter checker. default -1 disable
-
-    fails_attempt < 0   - disable checker (default)
-
-    fails_attempt == 0  - if _first_ field return `default` value - throw `ParseFailAttemptsError`
-
-    fails_attempt = n, fails_attempt > 0 - print *n* warnings messages if field return `default` value.
-    if `n` msgs - throw `ParseFailAttemptsError`
-    """
-
-    parsers_config: ClassVar[Dict[Type[Any], Dict[str, Any]]] = {}
-    type_cast: ClassVar[bool] = True
-    fails_attempt: ClassVar[int] = -1
-
-
 class SchemaMetaClass(type):
     @staticmethod
     def _is_type_field(attr: Type) -> bool:
         return get_origin(attr) is Annotated and all(
             isinstance(arg, BaseField) for arg in get_args(attr)[1:]
         )
 
@@ -417,29 +388,29 @@
         setattr(cls_schema, "__schema_fields__", __schema_fields__)
         setattr(cls_schema, "__schema_annotations__", __schema_annotations__)
 
         return cls_schema
 
 
 class BaseSchema(metaclass=SchemaMetaClass):
-    __schema_fields__: Dict[str, Tuple[BaseField, ...]] = {}
-    __schema_annotations__: Dict[str, Type] = {}
+    __schema_fields__: Dict[str, Tuple[BaseField, ...]]
+    __schema_annotations__: Dict[str, Type]
 
     class Config(BaseSchemaConfig):
         pass
 
     def _get_parser(self, field_parser_class: Type) -> Optional[Dict[str, Any]]:
         return self.Config.parsers_config.get(field_parser_class, None)
 
     def _check_parser_config(self, field: BaseField, field_parser: Type) -> bool:
         if self._get_parser(field_parser) is None:
             try:
                 raise MarkupNotFoundError(
                     f"{field.__class__.__name__} required "
-                    f"{field_parser.__class__.__name__} configuration"
+                    f"{type(field_parser).__name__} configuration"
                 )
             except MarkupNotFoundError as e:
                 logger.exception(e)
                 raise e
         return True
 
     @staticmethod
@@ -541,29 +512,27 @@
         """
         :param str markup: text target
         """
         _parsers: Dict[Type[Any], Any] = {}
         _fails_counter = 0
         logger.info(
             "Start parse `%s`. Fields count: %i",
-            self.__class__.__name__,
+            self.__schema_name__,
             len(self.__schema_fields__.keys()),
         )
 
         for name, fields in self.__schema_fields__.items():
             field, value = self._parse_field_value(
                 cached_parsers=_parsers, name=name, _fields=fields, markup=markup
             )
             _fails_counter = self._calculate_attempt_parse_errors(
                 fails_counter=_fails_counter, field=field, attr_name=name, value=value
             )
             setattr(self, name, value)
-        logger.debug(
-            "%s done! Fields fails: %i", self.__class__.__name__, _fails_counter
-        )
+        logger.debug("%s done! Fields fails: %i", self.__schema_name__, _fails_counter)
 
     def __init__(self, markup: str, *, parse_markup: bool = True, **kwargs):
         """
         :param markup: markup string target
         :param parse_markup: parse field markups. Default True
         :param kwargs: any kwargs attrs
         """
@@ -648,8 +617,12 @@
             if isinstance(v, BaseSchema)
             else f"{k}:{type(v).__name__}={repr(v)}"
             for k, v in self.__dict__.items()
             if not k.startswith("_") and k != "Config"
         ]
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({", ".join(self.__repr_args__())})'
+        return f'{self.__schema_name__}({", ".join(self.__repr_args__())})'
+
+    @property
+    def __schema_name__(self) -> str:
+        return self.__class__.__name__
```

### Comparing `scrape_schema-0.1.3/scrape_schema/callbacks/parsel.py` & `scrape_schema-0.1.4/scrape_schema/callbacks/parsel.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,31 @@
 
 from parsel import Selector, SelectorList
 from parsel.selector import _NOT_SET, LXML_SUPPORTS_HUGE_TREE, _SelectorType
 
 
 def get_text(
     default: Optional[str] = None,
+    strip: bool = False,
+    deep: bool = False,
+    sep: str = "",
 ) -> Callable[[Union[SelectorList[_SelectorType], Any]], Union[Optional[str], Any]]:
     def wrapper(
         element: Union[SelectorList[_SelectorType], Any]
     ) -> Union[Optional[str], Any]:
         if isinstance(element, (SelectorList, Selector)):
-            return element.css("::text").get(default=default)
+            if deep:
+                text = sep.join(element.css("::text").getall())
+            else:
+                # TODO
+                text = element.css("::text").get(default=default)  # type: ignore
+
+            if text:
+                return text.strip() if strip else text
+            return text
         return element
 
     return wrapper
 
 
 def replace_text(
     __old: str, __new: str, __count: int = -1, *, default: Optional[str] = None
```

### Comparing `scrape_schema-0.1.3/scrape_schema/callbacks/slax.py` & `scrape_schema-0.1.4/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.3/scrape_schema/callbacks/soup.py` & `scrape_schema-0.1.4/scrape_schema/callbacks/soup.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     :param soup_config: any BeautifulSoup kwargs config
     """
     if isinstance(element, str):
         element = element_to_dict(element)
 
     def wrapper(markup: str) -> str:
         soup = BeautifulSoup(markup, features=features, **soup_config)
-        return str(soup.find_all(**element))
+        return str(soup.find(**element))
 
     return wrapper
 
 
 def crop_by_selector(
     selector: str,
     namespaces: Optional[Dict[str, Any]] = None,
```

### Comparing `scrape_schema-0.1.3/scrape_schema/fields/nested.py` & `scrape_schema-0.1.4/scrape_schema/fields/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.3/scrape_schema/fields/parsel.py` & `scrape_schema-0.1.4/scrape_schema/fields/parsel.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.3/scrape_schema/fields/regex.py` & `scrape_schema-0.1.4/scrape_schema/fields/regex.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.3/scrape_schema/fields/slax.py` & `scrape_schema-0.1.4/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.3/scrape_schema/fields/soup.py` & `scrape_schema-0.1.4/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.3/.gitignore` & `scrape_schema-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.3/LICENSE` & `scrape_schema-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.3/README.md` & `scrape_schema-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Documentation Status](https://readthedocs.org/projects/scrape-schema/badge/?version=latest)](https://scrape-schema.readthedocs.io/en/latest/?badge=latest)
 ![CI](https://github.com/vypivshiy/scrape_schema/actions/workflows/ci.yml/badge.svg)
+![License](https://img.shields.io/github/license/vypivshiy/scrape-schema)
+![Version](https://img.shields.io/pypi/v/scrape-schema)
+![Python-versions](https://img.shields.io/pypi/pyversions/scrape_schema)
+[![codecov](https://codecov.io/gh/vypivshiy/scrape-schema/branch/master/graph/badge.svg?token=jqSNuE7g5l)](https://codecov.io/gh/vypivshiy/scrape-schema)
 # Scrape-schema
 This library is designed to write structured, readable, 
 reusable parsers for unstructured text data (like html, stdout or any text) and
 is inspired by dataclasses
 
 # Motivation
 Simplifying parsers support, where it is difficult to use 
@@ -25,16 +29,15 @@
 *If you usage schema-structures and they are separated from the logic of getting the text
 (stdout output, HTTP requests, etc)
 ____
 # Build-in libraries parsers support:
 - [x] re
 - [x] bs4
 - [x] selectolax(Modest)
-- [ ] parsel
-- [ ] lxml
+- [x] parsel
 - [ ] selenium
 - [ ] playwright
 ____
 # Install
 
 zero dependencies: regex, nested fields (and typing_extension if python < 3.11)
 ```shell
```

### Comparing `scrape_schema-0.1.3/pyproject.toml` & `scrape_schema-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,16 @@
 serve = "mkdocs serve --dev-addr localhost:8000"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "selectolax",
   "bs4",
-  "parsel"
+  "parsel",
+  "pytest-cov"
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=scrape_schema --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
```

### Comparing `scrape_schema-0.1.3/PKG-INFO` & `scrape_schema-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
@@ -54,14 +54,18 @@
 Provides-Extra: selectolax
 Requires-Dist: selectolax; extra == 'selectolax'
 Description-Content-Type: text/markdown
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Documentation Status](https://readthedocs.org/projects/scrape-schema/badge/?version=latest)](https://scrape-schema.readthedocs.io/en/latest/?badge=latest)
 ![CI](https://github.com/vypivshiy/scrape_schema/actions/workflows/ci.yml/badge.svg)
+![License](https://img.shields.io/github/license/vypivshiy/scrape-schema)
+![Version](https://img.shields.io/pypi/v/scrape-schema)
+![Python-versions](https://img.shields.io/pypi/pyversions/scrape_schema)
+[![codecov](https://codecov.io/gh/vypivshiy/scrape-schema/branch/master/graph/badge.svg?token=jqSNuE7g5l)](https://codecov.io/gh/vypivshiy/scrape-schema)
 # Scrape-schema
 This library is designed to write structured, readable, 
 reusable parsers for unstructured text data (like html, stdout or any text) and
 is inspired by dataclasses
 
 # Motivation
 Simplifying parsers support, where it is difficult to use 
@@ -82,16 +86,15 @@
 *If you usage schema-structures and they are separated from the logic of getting the text
 (stdout output, HTTP requests, etc)
 ____
 # Build-in libraries parsers support:
 - [x] re
 - [x] bs4
 - [x] selectolax(Modest)
-- [ ] parsel
-- [ ] lxml
+- [x] parsel
 - [ ] selenium
 - [ ] playwright
 ____
 # Install
 
 zero dependencies: regex, nested fields (and typing_extension if python < 3.11)
 ```shell
```

