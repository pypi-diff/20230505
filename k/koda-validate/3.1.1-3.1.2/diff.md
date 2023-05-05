# Comparing `tmp/koda_validate-3.1.1.tar.gz` & `tmp/koda_validate-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koda_validate-3.1.1.tar", max compression
+gzip compressed data, was "koda_validate-3.1.2.tar", max compression
```

## Comparing `koda_validate-3.1.1.tar` & `koda_validate-3.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1070 2022-10-24 05:53:28.522319 koda_validate-3.1.1/LICENSE
--rw-r--r--   0        0        0     1165 2023-01-28 17:57:33.106400 koda_validate-3.1.1/README.md
--rw-r--r--   0        0        0     4047 2023-01-26 16:37:28.349002 koda_validate-3.1.1/koda_validate/__init__.py
--rw-r--r--   0        0        0      530 2023-01-06 07:32:05.411107 koda_validate-3.1.1/koda_validate/_generics.py
--rw-r--r--   0        0        0     9711 2023-01-26 16:37:28.349310 koda_validate-3.1.1/koda_validate/_internal.py
--rw-r--r--   0        0        0     6660 2023-01-28 17:57:33.112881 koda_validate-3.1.1/koda_validate/base.py
--rw-r--r--   0        0        0      710 2023-01-26 16:37:28.349533 koda_validate-3.1.1/koda_validate/boolean.py
--rw-r--r--   0        0        0     1078 2023-01-26 16:37:28.349770 koda_validate-3.1.1/koda_validate/bytes.py
--rw-r--r--   0        0        0     1021 2023-01-26 16:37:28.349949 koda_validate-3.1.1/koda_validate/coerce.py
--rw-r--r--   0        0        0    10548 2023-01-26 16:37:28.350205 koda_validate-3.1.1/koda_validate/dataclasses.py
--rw-r--r--   0        0        0     1149 2023-01-26 16:37:28.350385 koda_validate-3.1.1/koda_validate/decimal.py
--rw-r--r--   0        0        0    37827 2023-01-26 16:37:28.350767 koda_validate-3.1.1/koda_validate/dictionary.py
--rw-r--r--   0        0        0     2745 2023-01-26 16:37:28.351067 koda_validate-3.1.1/koda_validate/errors.py
--rw-r--r--   0        0        0      717 2023-01-26 16:37:28.351232 koda_validate-3.1.1/koda_validate/float.py
--rw-r--r--   0        0        0     8800 2023-01-26 16:37:28.351549 koda_validate-3.1.1/koda_validate/generic.py
--rw-r--r--   0        0        0      703 2023-01-26 16:37:28.351720 koda_validate-3.1.1/koda_validate/integer.py
--rw-r--r--   0        0        0      870 2023-01-26 16:37:28.351954 koda_validate-3.1.1/koda_validate/is_type.py
--rw-r--r--   0        0        0     5238 2023-01-26 16:37:28.352358 koda_validate-3.1.1/koda_validate/list.py
--rw-r--r--   0        0        0     1882 2023-01-06 07:32:05.414848 koda_validate-3.1.1/koda_validate/maybe.py
--rw-r--r--   0        0        0    10428 2023-01-26 16:37:28.352593 koda_validate-3.1.1/koda_validate/namedtuple.py
--rw-r--r--   0        0        0     2252 2023-01-26 16:37:28.352892 koda_validate-3.1.1/koda_validate/none.py
--rw-r--r--   0        0        0        0 2022-07-11 17:15:27.213209 koda_validate-3.1.1/koda_validate/py.typed
--rw-r--r--   0        0        0      391 2023-01-06 07:32:05.415501 koda_validate-3.1.1/koda_validate/serialization/__init__.py
--rw-r--r--   0        0        0      207 2023-01-06 07:32:05.415715 koda_validate-3.1.1/koda_validate/serialization/base.py
--rw-r--r--   0        0        0     7040 2023-01-21 00:25:50.442897 koda_validate-3.1.1/koda_validate/serialization/errors.py
--rw-r--r--   0        0        0    18918 2023-01-06 07:32:05.416190 koda_validate-3.1.1/koda_validate/serialization/json_schema.py
--rw-r--r--   0        0        0     5670 2023-01-26 16:37:28.353257 koda_validate-3.1.1/koda_validate/set.py
--rw-r--r--   0        0        0    18017 2023-01-26 16:37:28.353660 koda_validate-3.1.1/koda_validate/signature.py
--rw-r--r--   0        0        0     1536 2023-01-26 16:37:28.354000 koda_validate-3.1.1/koda_validate/string.py
--rw-r--r--   0        0        0     1898 2023-01-26 16:37:28.354179 koda_validate-3.1.1/koda_validate/time.py
--rw-r--r--   0        0        0    19128 2023-01-28 17:57:33.113194 koda_validate-3.1.1/koda_validate/tuple.py
--rw-r--r--   0        0        0     9980 2023-01-26 16:37:28.354894 koda_validate-3.1.1/koda_validate/typeddict.py
--rw-r--r--   0        0        0     7653 2023-01-26 16:37:28.355281 koda_validate-3.1.1/koda_validate/typehints.py
--rw-r--r--   0        0        0     6796 2023-01-28 17:57:33.113403 koda_validate-3.1.1/koda_validate/union.py
--rw-r--r--   0        0        0     1055 2023-01-26 16:37:28.355587 koda_validate-3.1.1/koda_validate/uuid.py
--rw-r--r--   0        0        0     1457 2023-01-26 16:37:28.355783 koda_validate-3.1.1/koda_validate/valid.py
--rw-r--r--   0        0        0     2813 2023-01-28 17:57:33.114557 koda_validate-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     1886 1970-01-01 00:00:00.000000 koda_validate-3.1.1/setup.py
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 koda_validate-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-10-24 05:53:28.522319 koda_validate-3.1.2/LICENSE
+-rw-r--r--   0        0        0     1165 2023-01-28 17:57:33.106400 koda_validate-3.1.2/README.md
+-rw-r--r--   0        0        0     4047 2023-01-26 16:37:28.349002 koda_validate-3.1.2/koda_validate/__init__.py
+-rw-r--r--   0        0        0      530 2023-01-06 07:32:05.411107 koda_validate-3.1.2/koda_validate/_generics.py
+-rw-r--r--   0        0        0     9711 2023-01-26 16:37:28.349310 koda_validate-3.1.2/koda_validate/_internal.py
+-rw-r--r--   0        0        0     6660 2023-01-28 17:57:33.112881 koda_validate-3.1.2/koda_validate/base.py
+-rw-r--r--   0        0        0      710 2023-01-26 16:37:28.349533 koda_validate-3.1.2/koda_validate/boolean.py
+-rw-r--r--   0        0        0     1078 2023-01-26 16:37:28.349770 koda_validate-3.1.2/koda_validate/bytes.py
+-rw-r--r--   0        0        0     1021 2023-01-26 16:37:28.349949 koda_validate-3.1.2/koda_validate/coerce.py
+-rw-r--r--   0        0        0    10548 2023-01-26 16:37:28.350205 koda_validate-3.1.2/koda_validate/dataclasses.py
+-rw-r--r--   0        0        0     1149 2023-01-26 16:37:28.350385 koda_validate-3.1.2/koda_validate/decimal.py
+-rw-r--r--   0        0        0    37827 2023-01-26 16:37:28.350767 koda_validate-3.1.2/koda_validate/dictionary.py
+-rw-r--r--   0        0        0     2745 2023-01-26 16:37:28.351067 koda_validate-3.1.2/koda_validate/errors.py
+-rw-r--r--   0        0        0      717 2023-01-26 16:37:28.351232 koda_validate-3.1.2/koda_validate/float.py
+-rw-r--r--   0        0        0     8800 2023-01-26 16:37:28.351549 koda_validate-3.1.2/koda_validate/generic.py
+-rw-r--r--   0        0        0      703 2023-01-26 16:37:28.351720 koda_validate-3.1.2/koda_validate/integer.py
+-rw-r--r--   0        0        0      870 2023-01-26 16:37:28.351954 koda_validate-3.1.2/koda_validate/is_type.py
+-rw-r--r--   0        0        0     5238 2023-01-26 16:37:28.352358 koda_validate-3.1.2/koda_validate/list.py
+-rw-r--r--   0        0        0     1882 2023-01-06 07:32:05.414848 koda_validate-3.1.2/koda_validate/maybe.py
+-rw-r--r--   0        0        0    10428 2023-01-26 16:37:28.352593 koda_validate-3.1.2/koda_validate/namedtuple.py
+-rw-r--r--   0        0        0     2252 2023-01-26 16:37:28.352892 koda_validate-3.1.2/koda_validate/none.py
+-rw-r--r--   0        0        0        0 2022-07-11 17:15:27.213209 koda_validate-3.1.2/koda_validate/py.typed
+-rw-r--r--   0        0        0      391 2023-01-06 07:32:05.415501 koda_validate-3.1.2/koda_validate/serialization/__init__.py
+-rw-r--r--   0        0        0      207 2023-01-06 07:32:05.415715 koda_validate-3.1.2/koda_validate/serialization/base.py
+-rw-r--r--   0        0        0     7040 2023-01-21 00:25:50.442897 koda_validate-3.1.2/koda_validate/serialization/errors.py
+-rw-r--r--   0        0        0    18918 2023-01-06 07:32:05.416190 koda_validate-3.1.2/koda_validate/serialization/json_schema.py
+-rw-r--r--   0        0        0     5670 2023-01-26 16:37:28.353257 koda_validate-3.1.2/koda_validate/set.py
+-rw-r--r--   0        0        0    18981 2023-05-05 06:07:52.642895 koda_validate-3.1.2/koda_validate/signature.py
+-rw-r--r--   0        0        0     1536 2023-01-26 16:37:28.354000 koda_validate-3.1.2/koda_validate/string.py
+-rw-r--r--   0        0        0     1898 2023-01-26 16:37:28.354179 koda_validate-3.1.2/koda_validate/time.py
+-rw-r--r--   0        0        0    19128 2023-01-28 17:57:33.113194 koda_validate-3.1.2/koda_validate/tuple.py
+-rw-r--r--   0        0        0     9980 2023-01-26 16:37:28.354894 koda_validate-3.1.2/koda_validate/typeddict.py
+-rw-r--r--   0        0        0     7653 2023-01-26 16:37:28.355281 koda_validate-3.1.2/koda_validate/typehints.py
+-rw-r--r--   0        0        0     6796 2023-01-28 17:57:33.113403 koda_validate-3.1.2/koda_validate/union.py
+-rw-r--r--   0        0        0     1055 2023-01-26 16:37:28.355587 koda_validate-3.1.2/koda_validate/uuid.py
+-rw-r--r--   0        0        0     1457 2023-01-26 16:37:28.355783 koda_validate-3.1.2/koda_validate/valid.py
+-rw-r--r--   0        0        0     2813 2023-05-05 06:07:52.644602 koda_validate-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 koda_validate-3.1.2/setup.py
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 koda_validate-3.1.2/PKG-INFO
```

### Comparing `koda_validate-3.1.1/LICENSE` & `koda_validate-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/README.md` & `koda_validate-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/__init__.py` & `koda_validate-3.1.2/koda_validate/__init__.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/_generics.py` & `koda_validate-3.1.2/koda_validate/_generics.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/_internal.py` & `koda_validate-3.1.2/koda_validate/_internal.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/base.py` & `koda_validate-3.1.2/koda_validate/base.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/boolean.py` & `koda_validate-3.1.2/koda_validate/boolean.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/bytes.py` & `koda_validate-3.1.2/koda_validate/bytes.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/coerce.py` & `koda_validate-3.1.2/koda_validate/coerce.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/dataclasses.py` & `koda_validate-3.1.2/koda_validate/dataclasses.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/decimal.py` & `koda_validate-3.1.2/koda_validate/decimal.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/dictionary.py` & `koda_validate-3.1.2/koda_validate/dictionary.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/errors.py` & `koda_validate-3.1.2/koda_validate/errors.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/float.py` & `koda_validate-3.1.2/koda_validate/float.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/generic.py` & `koda_validate-3.1.2/koda_validate/generic.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/integer.py` & `koda_validate-3.1.2/koda_validate/integer.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/is_type.py` & `koda_validate-3.1.2/koda_validate/is_type.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/list.py` & `koda_validate-3.1.2/koda_validate/list.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/maybe.py` & `koda_validate-3.1.2/koda_validate/maybe.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/namedtuple.py` & `koda_validate-3.1.2/koda_validate/namedtuple.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/none.py` & `koda_validate-3.1.2/koda_validate/none.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/serialization/errors.py` & `koda_validate-3.1.2/koda_validate/serialization/errors.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/serialization/json_schema.py` & `koda_validate-3.1.2/koda_validate/serialization/json_schema.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/set.py` & `koda_validate-3.1.2/koda_validate/set.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/signature.py` & `koda_validate-3.1.2/koda_validate/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,36 +181,43 @@
     if inspect.iscoroutinefunction(func) or inspect.iscoroutinefunction(
         getattr(func, "__call__", None)
     ):
 
         async def inner_async(*args: Any, **kwargs: Any) -> Any:
             errs: Dict[str, Invalid] = {}
             var_args_errs: List[Tuple[Any, Invalid]] = []
+            # in case the values get mutated during validation
+            ok_args: List[Any] = list(args)
+            ok_kw_args: Dict[str, Any] = kwargs.copy()
             for i, arg in enumerate(args):
                 if len(positional_validators) >= i + 1:
                     arg_details = positional_validators[i]
                     if arg_details is None:
                         # not an annotated argument
                         continue
                     else:
                         key, arg_validator = arg_details
                         if not (
                             result := await arg_validator.validate_async(arg)
                         ).is_valid:
                             errs[key] = result
+                        else:
+                            ok_args[i] = result.val
 
                 else:
                     if var_args_key_and_validator:
                         var_args_key, var_args_validator = var_args_key_and_validator
                         if not (
                             var_args_result := await var_args_validator.validate_async(
                                 arg
                             )
                         ).is_valid:
                             var_args_errs.append((arg, var_args_result))
+                        else:
+                            ok_args[i] = var_args_result.val
 
             if var_args_errs and var_args_key_and_validator:
                 errs[var_args_key_and_validator[0]] = Invalid(
                     IndexErrs({i: err_ for i, (_, err_) in enumerate(var_args_errs)}),
                     tuple(a for a, _ in var_args_errs),
                     var_args_key_and_validator[1],
                 )
@@ -218,27 +225,28 @@
             for kw_key, kw_val in kwargs.items():
                 if kw_key in schema:
                     if schema_validator := schema[kw_key]:
                         if not (
                             kw_result := await schema_validator.validate_async(kw_val)
                         ).is_valid:
                             errs[kw_key] = kw_result
-                elif (
-                    kwargs_validator
-                    and kw_key not in ignored_extra_kwargs
-                    and not (
+                        else:
+                            ok_kw_args[kw_key] = kw_result.val
+                elif kwargs_validator and kw_key not in ignored_extra_kwargs:
+                    if not (
                         kwargs_result := await kwargs_validator.validate_async(kw_val)
-                    ).is_valid
-                ):
-                    errs[kw_key] = kwargs_result
+                    ).is_valid:
+                        errs[kw_key] = kwargs_result
+                    else:
+                        ok_kw_args[kw_key] = kwargs_result.val
 
             if errs:
                 raise InvalidArgsError(errs)
             elif return_validator:
-                result = await func(*args, **kwargs)
+                result = await func(*ok_args, **ok_kw_args)
                 if (ret_result := await return_validator.validate_async(result)).is_valid:
                     return result
                 else:
                     raise InvalidReturnError(ret_result)
             else:
                 return await func(*args, **kwargs)
 
@@ -246,60 +254,68 @@
 
     else:
 
         @functools.wraps(func)
         def inner(*args: Any, **kwargs: Any) -> Any:
             errs: Dict[str, Invalid] = {}
             var_args_errs: List[Tuple[Any, Invalid]] = []
+            # in case the values get mutated during validation
+            ok_args: List[Any] = list(args)
+            ok_kw_args: Dict[str, Any] = kwargs.copy()
             for i, arg in enumerate(args):
                 if len(positional_validators) >= i + 1:
                     arg_details = positional_validators[i]
                     if arg_details is None:
                         # not an annotated argument
                         continue
                     else:
                         key, arg_validator = arg_details
                         if not (result := arg_validator(arg)).is_valid:
                             errs[key] = result
+                        else:
+                            ok_args[i] = result.val
 
                 else:
                     if var_args_key_and_validator:
                         var_args_key, var_args_validator = var_args_key_and_validator
                         if not (var_args_result := var_args_validator(arg)).is_valid:
                             var_args_errs.append((arg, var_args_result))
+                        else:
+                            ok_args[i] = var_args_result.val
 
             if var_args_errs and var_args_key_and_validator:
                 errs[var_args_key_and_validator[0]] = Invalid(
                     IndexErrs({i: err_ for i, (_, err_) in enumerate(var_args_errs)}),
                     tuple(a for a, _ in var_args_errs),
                     var_args_key_and_validator[1],
                 )
 
             for kw_key, kw_val in kwargs.items():
                 if kw_key in schema:
                     if schema_validator := schema[kw_key]:
                         if not (kw_result := schema_validator(kw_val)).is_valid:
                             errs[kw_key] = kw_result
-                elif (
-                    kwargs_validator
-                    and kw_key not in ignored_extra_kwargs
-                    and not (kwargs_result := kwargs_validator(kw_val)).is_valid
-                ):
-                    errs[kw_key] = kwargs_result
+                        else:
+                            ok_kw_args[kw_key] = kw_result.val
+                elif kwargs_validator and kw_key not in ignored_extra_kwargs:
+                    if (kwargs_result := kwargs_validator(kw_val)).is_valid:
+                        ok_kw_args[kw_key] = kwargs_result.val
+                    else:
+                        errs[kw_key] = kwargs_result
 
             if errs:
                 raise InvalidArgsError(errs)
             elif return_validator:
-                result = func(*args, **kwargs)
+                result = func(*ok_args, **ok_kw_args)
                 if (ret_result := return_validator(result)).is_valid:
                     return result
                 else:
                     raise InvalidReturnError(ret_result)
             else:
-                return func(*args, **kwargs)
+                return func(*ok_args, **kwargs)
 
         return cast(_DecoratedFunc, inner)
 
 
 @overload
 def validate_signature(
     func: _DecoratedFunc,
@@ -441,14 +457,15 @@
                 )
                 ret += f"\n{next_}"
     elif isinstance(err_type, SetErrs):
         ret += f"{err_type.__class__.__name__}\n"
         ret += "\n".join(
             [
                 f"{_get_arg_fail_message(e, next_indent)} :: {_trunc_str(repr(e.value), 30)}"  # noqa: E501
+                # noqa: E501
                 for e in err_type.item_errs
             ]
         )
 
     return ret
```

### Comparing `koda_validate-3.1.1/koda_validate/string.py` & `koda_validate-3.1.2/koda_validate/string.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/time.py` & `koda_validate-3.1.2/koda_validate/time.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/tuple.py` & `koda_validate-3.1.2/koda_validate/tuple.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/typeddict.py` & `koda_validate-3.1.2/koda_validate/typeddict.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/typehints.py` & `koda_validate-3.1.2/koda_validate/typehints.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/union.py` & `koda_validate-3.1.2/koda_validate/union.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/uuid.py` & `koda_validate-3.1.2/koda_validate/uuid.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/koda_validate/valid.py` & `koda_validate-3.1.2/koda_validate/valid.py`

 * *Files identical despite different names*

### Comparing `koda_validate-3.1.1/pyproject.toml` & `koda_validate-3.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koda-validate"
-version = "3.1.1"
+version = "3.1.2"
 readme = "README.md"
 description = "Typesafe, composable validation"
 documentation = "https://koda-validate.readthedocs.io/en/stable/"
 authors = ["Keith Philpott"]
 license = "MIT"
 homepage = "https://github.com/keithasaurus/koda-validate"
 keywords = ["validation", "type hints", "asyncio", "serialization", "typesafe", "validate", "validators", "predicate", "processor"]
@@ -21,40 +21,40 @@
     'Operating System :: Unix',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Utilities',
     'Typing :: Typed'
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8.1"
 koda = "1.4.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "7.2.0"
-pyright = "1.1.285"
+pytest = "7.3.1"
+pyright = "1.1.306"
 pytest-cov = "4.0.0"
-isort = "5.10.1"
-flake8 = "5.0.4"
-pre-commit = "2.20.0"
-mypy = "0.991"
-pydantic = "1.10.2"
-pytest-asyncio = "0.20.2"
+isort = "5.12.0"
+flake8 = "6.0.0"
+pre-commit = "3.3.1"
+mypy = "1.1.1"
+pydantic = "1.10.7"
+pytest-asyncio = "0.21.0"
 voluptuous = "0.13.1"
 ssort = "0.11.6"
 jsonschema = "4.17.3"
-types-jsonschema = "4.17.0.2"
-sphinx = "5.3.0"
-furo = "2022.12.7"
-flask = {version = "2.2.2", extras = ["async"]}
-django = "4.1.4"
-django-stubs = "1.13.1"
+types-jsonschema = "4.17.0.7"
+sphinx = "6.2.1"
+furo = "2023.3.27"
+flask = {version = "2.3.2", extras = ["async"]}
+django = "4.2.1"
+django-stubs = "1.16.0"
 pytest-django = "4.5.2"
-sphinx-autodoc-typehints = "1.19.5"
+sphinx-autodoc-typehints = "1.23.0"
 darglint = "1.8.1"
-black = "22.12.0"
+black = "23.3.0"
 
 [tool.mypy]
 exclude = ["build", "bench"]
 allow_redefinition = false
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
```

### Comparing `koda_validate-3.1.1/setup.py` & `koda_validate-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['koda==1.4.0']
 
 setup_kwargs = {
     'name': 'koda-validate',
-    'version': '3.1.1',
+    'version': '3.1.2',
     'description': 'Typesafe, composable validation',
     'long_description': "# Koda Validate\n\nBuild typesafe validators automatically or explicitly -- or write your own. Combine them to\nbuild validators of arbitrary complexity. Koda Validate is async-friendly, pure Python, and\n1.5x - 12x faster than Pydantic.\n\nDocs: [https://koda-validate.readthedocs.io/en/stable/](https://koda-validate.readthedocs.io/en/stable/)\n\n```python\n\nfrom typing import TypedDict \nfrom koda_validate import (StringValidator, MaxLength, MinLength, \n                           ListValidator, TypedDictValidator)\nfrom koda_validate.signature import validate_signature\n\n# Explicit Validators\nstring_validator = StringValidator(MinLength(8), MaxLength(20))\n\nlist_string_validator = ListValidator(string_validator)\n\n\n# Derived Validators\nclass Person(TypedDict):\n    name: str\n    hobbies: list[str] \n\nperson_validator = TypedDictValidator(Person)\n\n\n# Runtime type checking\n@validate_signature\ndef add(a: int, b: int) -> int:\n    return a + b\n\n```\n\nThere's much, much more... Check out the [Docs](https://koda-validate.readthedocs.io/en/stable/).\n\n\n## Something's Missing Or Wrong \nOpen an [issue on GitHub](https://github.com/keithasaurus/koda-validate/issues) please!\n",
     'author': 'Keith Philpott',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/keithasaurus/koda-validate',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `koda_validate-3.1.1/PKG-INFO` & `koda_validate-3.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: koda-validate
-Version: 3.1.1
+Version: 3.1.2
 Summary: Typesafe, composable validation
 Home-page: https://github.com/keithasaurus/koda-validate
 License: MIT
 Keywords: validation,type hints,asyncio,serialization,typesafe,validate,validators,predicate,processor
 Author: Keith Philpott
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Hypothesis
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: koda (==1.4.0)
```

