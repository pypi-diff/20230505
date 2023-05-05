# Comparing `tmp/py-strongly-typed-1.1.5.tar.gz` & `tmp/py-strongly-typed-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-strongly-typed-1.1.5.tar", last modified: Fri May  5 03:15:13 2023, max compression
+gzip compressed data, was "py-strongly-typed-2.0.0.tar", last modified: Fri May  5 05:30:47 2023, max compression
```

## Comparing `py-strongly-typed-1.1.5.tar` & `py-strongly-typed-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:13.787212 py-strongly-typed-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-05 03:15:13.787212 py-strongly-typed-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:13.783212 py-strongly-typed-1.1.5/py_strongly_typed/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/py_strongly_typed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/py_strongly_typed/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/py_strongly_typed/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/py_strongly_typed/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/py_strongly_typed/typed_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:13.787212 py-strongly-typed-1.1.5/py_strongly_typed/use_cases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/py_strongly_typed/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/py_strongly_typed/use_cases/validate_annotations_use_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:13.787212 py-strongly-typed-1.1.5/py_strongly_typed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-05 03:15:13.000000 py-strongly-typed-1.1.5/py_strongly_typed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-05 03:15:13.000000 py-strongly-typed-1.1.5/py_strongly_typed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:15:13.000000 py-strongly-typed-1.1.5/py_strongly_typed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 03:15:13.000000 py-strongly-typed-1.1.5/py_strongly_typed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 03:15:13.000000 py-strongly-typed-1.1.5/py_strongly_typed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-05 03:15:13.787212 py-strongly-typed-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-05 03:14:58.000000 py-strongly-typed-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:47.623604 py-strongly-typed-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-05 05:30:47.623604 py-strongly-typed-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:47.623604 py-strongly-typed-2.0.0/py_strongly_typed/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/py_strongly_typed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/py_strongly_typed/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/py_strongly_typed/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/py_strongly_typed/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/py_strongly_typed/typed_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:47.623604 py-strongly-typed-2.0.0/py_strongly_typed/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/py_strongly_typed/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/py_strongly_typed/use_cases/validate_annotations_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/py_strongly_typed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:47.623604 py-strongly-typed-2.0.0/py_strongly_typed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-05 05:30:47.000000 py-strongly-typed-2.0.0/py_strongly_typed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-05 05:30:47.000000 py-strongly-typed-2.0.0/py_strongly_typed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:30:47.000000 py-strongly-typed-2.0.0/py_strongly_typed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 05:30:47.000000 py-strongly-typed-2.0.0/py_strongly_typed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 05:30:47.000000 py-strongly-typed-2.0.0/py_strongly_typed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-05 05:30:47.623604 py-strongly-typed-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-05 05:30:36.000000 py-strongly-typed-2.0.0/setup.py
```

### Comparing `py-strongly-typed-1.1.5/LICENSE` & `py-strongly-typed-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-strongly-typed-1.1.5/PKG-INFO` & `py-strongly-typed-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-strongly-typed
-Version: 1.1.5
+Version: 2.0.0
 Summary: Python type enforcer
 Author: Christian Silva
 Author-email: chrislcontrol@hotmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/chrislcontrol/py-strongly-typed
 Project-URL: Tracker, https://github.com/chrislcontrol/py-strongly-typed/issues
 Requires-Python: >=3.5
@@ -136,43 +136,33 @@
 
   - ***typing_validator*** *[Type[IValidateAnnotationsUseCase]]* ***[default=ValidateAnnotationsUseCase]***: 
   `You can provide an custom class that validates typing.`
 
   - ***type_all_methods*** *[bool]* ***[default=True]***:
   `Defines if all methods of the class will be type validated or only __init__.`
 
-  - ***ignore_float_and_integer_difference*** *[bool]* ***[default=True]***: 
-  `If True, providing an integer on a float expected or inverse will be ignored.`
-
 
 - **@typed_function decorator**
 
   - ***typing_validator*** *[Type[IValidateAnnotationsUseCase]]*: `You can provide an custom class that validates
   typing.`
 
-  - ***ignore_float_and_integer_difference*** *[bool]*: `If True, providing an integer on a float expected or inverse 
-  will be ignored.`
-
 
 - **IValidateAnnotationsUseCase**
   - ***func*** *[Callable]*: Function that will has be called after typing validation.
-  - ***ignore_float_and_integer_difference*** *[bool]*: `If True, providing an integer on a float expected or inverse 
-  will be ignored.`
 
 
 Behavior
 ===========
    * When an invalid value type is provided, WrongType exception will be raised.
    * When function or method is defined with any argument missing annotation, 
 MissingAnnotation will be raised.
 
 Limitations
 ===========
-   * Generics (example: List[str]) are not supported yet.
-   * Typing using or operator will validate only first one. Example: providing str or int, 
+   * Typing using `or` operator will validate only first one. Example: providing str or int, 
 only str will be considered. To provide more than one expected type, use `|` operator or `Union`.
-   * `*args` and `**kwargs` are not supported due to be impossible to provide typing annotations for them 
-without Generics.
+   * `*args` and `**kwargs` are not supported yet.
 
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `py-strongly-typed-1.1.5/README.md` & `py-strongly-typed-2.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -122,43 +122,33 @@
 
   - ***typing_validator*** *[Type[IValidateAnnotationsUseCase]]* ***[default=ValidateAnnotationsUseCase]***: 
   `You can provide an custom class that validates typing.`
 
   - ***type_all_methods*** *[bool]* ***[default=True]***:
   `Defines if all methods of the class will be type validated or only __init__.`
 
-  - ***ignore_float_and_integer_difference*** *[bool]* ***[default=True]***: 
-  `If True, providing an integer on a float expected or inverse will be ignored.`
-
 
 - **@typed_function decorator**
 
   - ***typing_validator*** *[Type[IValidateAnnotationsUseCase]]*: `You can provide an custom class that validates
   typing.`
 
-  - ***ignore_float_and_integer_difference*** *[bool]*: `If True, providing an integer on a float expected or inverse 
-  will be ignored.`
-
 
 - **IValidateAnnotationsUseCase**
   - ***func*** *[Callable]*: Function that will has be called after typing validation.
-  - ***ignore_float_and_integer_difference*** *[bool]*: `If True, providing an integer on a float expected or inverse 
-  will be ignored.`
 
 
 Behavior
 ===========
    * When an invalid value type is provided, WrongType exception will be raised.
    * When function or method is defined with any argument missing annotation, 
 MissingAnnotation will be raised.
 
 Limitations
 ===========
-   * Generics (example: List[str]) are not supported yet.
-   * Typing using or operator will validate only first one. Example: providing str or int, 
+   * Typing using `or` operator will validate only first one. Example: providing str or int, 
 only str will be considered. To provide more than one expected type, use `|` operator or `Union`.
-   * `*args` and `**kwargs` are not supported due to be impossible to provide typing annotations for them 
-without Generics.
+   * `*args` and `**kwargs` are not supported yet.
 
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `py-strongly-typed-1.1.5/py_strongly_typed/typed_class.py` & `py-strongly-typed-2.0.0/py_strongly_typed/typed_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 from py_strongly_typed.use_cases.validate_annotations_use_case import ValidateAnnotationsUseCase
 from py_strongly_typed.decorators import typed_function
 
 
 class TypedClass:
     typing_validator: Type[IValidateAnnotationsUseCase] = ValidateAnnotationsUseCase
     type_all_methods: bool = True
-    ignore_float_and_integer_difference: bool = True
 
     def __getattribute__(self, name):
         attr = object.__getattribute__(self, name)
         if not callable(attr) or self.type_all_methods is False:
             return attr
 
-        return typed_function(attr, ignore_float_and_integer_difference=self.ignore_float_and_integer_difference)
+        return typed_function(attr)
 
     def __new__(cls, *args, **kwargs):
-        core = cls.typing_validator(func=cls.__init__,
-                                    ignore_float_and_integer_difference=cls.ignore_float_and_integer_difference)
+        core = cls.typing_validator(func=cls.__init__)
         core.execute(*args, **kwargs)
 
         return super().__new__(cls)
 
 
 class TypedInit(TypedClass):
     type_all_methods = False
```

### Comparing `py-strongly-typed-1.1.5/py_strongly_typed.egg-info/PKG-INFO` & `py-strongly-typed-2.0.0/py_strongly_typed.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-strongly-typed
-Version: 1.1.5
+Version: 2.0.0
 Summary: Python type enforcer
 Author: Christian Silva
 Author-email: chrislcontrol@hotmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/chrislcontrol/py-strongly-typed
 Project-URL: Tracker, https://github.com/chrislcontrol/py-strongly-typed/issues
 Requires-Python: >=3.5
@@ -136,43 +136,33 @@
 
   - ***typing_validator*** *[Type[IValidateAnnotationsUseCase]]* ***[default=ValidateAnnotationsUseCase]***: 
   `You can provide an custom class that validates typing.`
 
   - ***type_all_methods*** *[bool]* ***[default=True]***:
   `Defines if all methods of the class will be type validated or only __init__.`
 
-  - ***ignore_float_and_integer_difference*** *[bool]* ***[default=True]***: 
-  `If True, providing an integer on a float expected or inverse will be ignored.`
-
 
 - **@typed_function decorator**
 
   - ***typing_validator*** *[Type[IValidateAnnotationsUseCase]]*: `You can provide an custom class that validates
   typing.`
 
-  - ***ignore_float_and_integer_difference*** *[bool]*: `If True, providing an integer on a float expected or inverse 
-  will be ignored.`
-
 
 - **IValidateAnnotationsUseCase**
   - ***func*** *[Callable]*: Function that will has be called after typing validation.
-  - ***ignore_float_and_integer_difference*** *[bool]*: `If True, providing an integer on a float expected or inverse 
-  will be ignored.`
 
 
 Behavior
 ===========
    * When an invalid value type is provided, WrongType exception will be raised.
    * When function or method is defined with any argument missing annotation, 
 MissingAnnotation will be raised.
 
 Limitations
 ===========
-   * Generics (example: List[str]) are not supported yet.
-   * Typing using or operator will validate only first one. Example: providing str or int, 
+   * Typing using `or` operator will validate only first one. Example: providing str or int, 
 only str will be considered. To provide more than one expected type, use `|` operator or `Union`.
-   * `*args` and `**kwargs` are not supported due to be impossible to provide typing annotations for them 
-without Generics.
+   * `*args` and `**kwargs` are not supported yet.
 
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `py-strongly-typed-1.1.5/setup.py` & `py-strongly-typed-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description=long_description(),
     packages=find_packages(exclude=["*tests*"]),
     author='Christian Silva',
     author_email='chrislcontrol@hotmail.com',
     long_description_content_type='text/markdown',
     license='MIT License',
     python_requires=">=3.5",
-    version='1.1.5',
+    version='2.0.0',
     project_urls={
         "GitHub": "https://github.com/chrislcontrol/py-strongly-typed",
         "Tracker": "https://github.com/chrislcontrol/py-strongly-typed/issues",
     },
     install_requires=[
         'wheel'
     ],
```

