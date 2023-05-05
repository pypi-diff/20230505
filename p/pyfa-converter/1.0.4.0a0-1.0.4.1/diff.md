# Comparing `tmp/pyfa_converter-1.0.4.0a0.tar.gz` & `tmp/pyfa_converter-1.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfa_converter-1.0.4.0a0.tar", max compression
+gzip compressed data, was "pyfa_converter-1.0.4.1.tar", max compression
```

## Comparing `pyfa_converter-1.0.4.0a0.tar` & `pyfa_converter-1.0.4.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1063 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/LICENSE.md
--rw-r--r--   0        0        0     2432 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/README.md
--rw-r--r--   0        0        0      247 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/__init__.py
--rw-r--r--   0        0        0     1144 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/depends.py
--rw-r--r--   0        0        0     4034 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/main.py
--rw-r--r--   0        0        0        0 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/utils/__init__.py
--rw-r--r--   0        0        0     5603 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/utils/deprecation.py
--rw-r--r--   0        0        0      444 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/utils/deprecation_message.py
--rw-r--r--   0        0        0      881 2022-12-19 06:26:32.997966 pyfa_converter-1.0.4.0a0/pyproject.toml
--rw-r--r--   0        0        0     3240 1970-01-01 00:00:00.000000 pyfa_converter-1.0.4.0a0/setup.py
--rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 pyfa_converter-1.0.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-05 06:38:55.303976 pyfa_converter-1.0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     2326 2023-05-05 06:38:55.303976 pyfa_converter-1.0.4.1/README.md
+-rw-r--r--   0        0        0      247 2023-05-05 06:38:55.303976 pyfa_converter-1.0.4.1/pyfa_converter/__init__.py
+-rw-r--r--   0        0        0     1144 2023-05-05 06:38:55.303976 pyfa_converter-1.0.4.1/pyfa_converter/depends.py
+-rw-r--r--   0        0        0     4218 2023-05-05 06:38:55.303976 pyfa_converter-1.0.4.1/pyfa_converter/main.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:38:55.303976 pyfa_converter-1.0.4.1/pyfa_converter/utils/__init__.py
+-rw-r--r--   0        0        0     5603 2023-05-05 06:38:55.303976 pyfa_converter-1.0.4.1/pyfa_converter/utils/deprecation.py
+-rw-r--r--   0        0        0      444 2023-05-05 06:38:55.307976 pyfa_converter-1.0.4.1/pyfa_converter/utils/deprecation_message.py
+-rw-r--r--   0        0        0      880 2023-05-05 06:39:11.052428 pyfa_converter-1.0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 pyfa_converter-1.0.4.1/PKG-INFO
```

### Comparing `pyfa_converter-1.0.4.0a0/LICENSE.md` & `pyfa_converter-1.0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfa_converter-1.0.4.0a0/README.md` & `pyfa_converter-1.0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,15 @@
     date: Optional[datetime] = Field(
         None, description="Example: 2021-12-14T09:56:31.056Z"
     )
 
 
 @app.post("/form-data-body")
 async def example_foo_body_handler(
-    data: PostContractBodySchema = FormDepends(PostContractBodySchema),
-    # data1: PostContractBodySchema = PyFaDepends( # OR
-    #         model= PostContractBodySchema, _type=Form
-    #     ),
+    data1: PostContractBodySchema = PyFaDepends(model=PostContractBodySchema, _type=Form),
     document: UploadFile = File(...),
 ):
     return {"title": data.title, "date": data.date, "file_name": document.filename}
 ```
 
 ---
```

### Comparing `pyfa_converter-1.0.4.0a0/pyfa_converter/depends.py` & `pyfa_converter-1.0.4.1/pyfa_converter/depends.py`

 * *Files identical despite different names*

### Comparing `pyfa_converter-1.0.4.0a0/pyfa_converter/main.py` & `pyfa_converter-1.0.4.1/pyfa_converter/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,18 @@
             return cls.__fill_params(param=_type, model_field=field, default=...)
         return cls.__fill_params(param=_type, model_field=field, default=field.default)
 
     @classmethod
     def __fill_params(
         cls, param: Callable[..., FieldInfo], model_field: ModelField, default: Any
     ) -> FieldInfo:
+        default_value = default if isinstance(default, bool) else default or None
+        
         return param(
-            default=default or None,
+            default=default_value,
             alias=model_field.field_info.alias or None,
             title=model_field.field_info.title or None,
             description=model_field.field_info.description or None,
             gt=model_field.field_info.gt or None,
             ge=model_field.field_info.ge or None,
             lt=model_field.field_info.lt or None,
             le=model_field.field_info.le or None,
@@ -85,21 +87,23 @@
                 field: The field to convert.
 
             Returns:
                 Either the result of `Query`, if the field is not a sub-model, or
                 the result of `Depends on` if it is.
 
             """
-            if issubclass(field.type_, BaseModel):
+            field_type = type(field.type_) if not isinstance(field.type_, type) else field.type_
+
+            if issubclass(field_type, BaseModel):
                 # This is a sub-model.
-                assert hasattr(field.type_, _type_var_name), (
+                assert hasattr(field_type, _type_var_name), (
                     f"Sub-model class for {field.name} field must be decorated with"
                     f" `as_form` too."
                 )
-                attr = getattr(field.type_, _type_var_name)
+                attr = getattr(field_type, _type_var_name)
                 return Depends(attr)  # noqa
             else:
                 return cls.param_maker(field=field, _type=_type)
 
         new_params = PydanticConverterUtils.override_signature_parameters(
             model=model_cls, param_maker=make_form_parameter
         )
```

### Comparing `pyfa_converter-1.0.4.0a0/pyfa_converter/utils/deprecation.py` & `pyfa_converter-1.0.4.1/pyfa_converter/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyfa_converter-1.0.4.0a0/pyproject.toml` & `pyfa_converter-1.0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfa-converter"
-version = "1.0.4.0a"
+version = "1.0.4.1"
 description = "Pydantic to fastapi model converter."
 authors = ["dotX12 <dev@shitposting.team>"]
 license = "MIT License"
 homepage = "https://github.com/dotX12/pyfa-converter"
 repository = "https://github.com/dotX12/pyfa-converter"
 readme = "README.md"
```

### Comparing `pyfa_converter-1.0.4.0a0/setup.py` & `pyfa_converter-1.0.4.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,91 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyfa-converter
+Version: 1.0.4.1
+Summary: Pydantic to fastapi model converter.
+Home-page: https://github.com/dotX12/pyfa-converter
+License: MIT
+Author: dotX12
+Author-email: dev@shitposting.team
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi (>=0.65)
+Requires-Dist: pydantic (>=1.6)
+Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
+Project-URL: Repository, https://github.com/dotX12/pyfa-converter
+Description-Content-Type: text/markdown
 
-packages = \
-['pyfa_converter', 'pyfa_converter.utils']
+# pyfa-converter
+Allows you to convert pydantic models for fastapi param models - query, form, header, cookie, body, etc.
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['fastapi>=0.65', 'pydantic>=1.6', 'python-multipart>=0.0.5,<0.0.6']
-
-setup_kwargs = {
-    'name': 'pyfa-converter',
-    'version': '1.0.4.0a0',
-    'description': 'Pydantic to fastapi model converter.',
-    'long_description': '# pyfa-converter\nAllows you to convert pydantic models for fastapi param models - query, form, header, cookie, body, etc.\n\n\n\n### How to install?\n`pip install pyfa_converter`\n\n### How to simplify your life?\n```python3\nfrom datetime import datetime\nfrom typing import Optional\n\nfrom fastapi import FastAPI, UploadFile, File, Form\nfrom pydantic import BaseModel, Field\n\nfrom pyfa_converter import FormDepends, PyFaDepends\n\napp = FastAPI()\n\n\nclass PostContractBodySchema(BaseModel):\n    title: str = Field(..., description="Description title")\n    date: Optional[datetime] = Field(\n        None, description="Example: 2021-12-14T09:56:31.056Z"\n    )\n\n\n@app.post("/form-data-body")\nasync def example_foo_body_handler(\n    data: PostContractBodySchema = FormDepends(PostContractBodySchema),\n    # data1: PostContractBodySchema = PyFaDepends( # OR\n    #         model= PostContractBodySchema, _type=Form\n    #     ),\n    document: UploadFile = File(...),\n):\n    return {"title": data.title, "date": data.date, "file_name": document.filename}\n```\n\n---\n\n### What do I need to do?\n```python3\nfrom pyfa_converter import PyFaDepends, FormDepends, QueryDepends\nfrom fastapi import Header, Form\n...\n\nasync def foo(data: MyCustomModel = PyFaDepends(MyCustomModel, _type=Header)): ...\nasync def foo(data: MyCustomModel = PyFaDepends(MyCustomModel, _type=Form)): ...\n\nasync def foo(data: MyCustomModel = FormDepends(MyCustomModel)): ...\nasync def foo(data: MyCustomModel = QueryDepends(MyCustomModel)): ...\n```\n\n---\n\nIf you want to accept a file on an endpoint, then the content-type for that endpoint changes from application/json to www-form-data.\n\nFastAPI does not know how to override the pydantic schema so that parameters are passed as form.\nEven if you do\n\n`foo: CustomPydanticModel = Depends()`\nall model attributes will be passed as query, but we want them to become body, that\'s what this library exists for.\n\n### Usually you use something along the lines of:\n![image](https://user-images.githubusercontent.com/64792903/161484700-642e3d0e-242f-49f6-82e8-45c5e912a2c2.png)\n\nBut, if we accept a lot of fields, then the function becomes very large (the number of attributes for the endpoint increases and it does not look very good).\n\nThanks to this library, it is possible to force the conversion of Field fields into fields of FastAPI Form with full preservation of all attributes (alias, gt, te, description, title, example and more...)\n\n\n',
-    'author': 'dotX12',
-    'author_email': 'dev@shitposting.team',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dotX12/pyfa-converter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8',
-}
+
+### How to install?
+`pip install pyfa_converter`
+
+### How to simplify your life?
+```python3
+from datetime import datetime
+from typing import Optional
+
+from fastapi import FastAPI, UploadFile, File, Form
+from pydantic import BaseModel, Field
+
+from pyfa_converter import FormDepends, PyFaDepends
+
+app = FastAPI()
+
+
+class PostContractBodySchema(BaseModel):
+    title: str = Field(..., description="Description title")
+    date: Optional[datetime] = Field(
+        None, description="Example: 2021-12-14T09:56:31.056Z"
+    )
+
+
+@app.post("/form-data-body")
+async def example_foo_body_handler(
+    data1: PostContractBodySchema = PyFaDepends(model=PostContractBodySchema, _type=Form),
+    document: UploadFile = File(...),
+):
+    return {"title": data.title, "date": data.date, "file_name": document.filename}
+```
+
+---
+
+### What do I need to do?
+```python3
+from pyfa_converter import PyFaDepends, FormDepends, QueryDepends
+from fastapi import Header, Form
+...
+
+async def foo(data: MyCustomModel = PyFaDepends(MyCustomModel, _type=Header)): ...
+async def foo(data: MyCustomModel = PyFaDepends(MyCustomModel, _type=Form)): ...
+
+async def foo(data: MyCustomModel = FormDepends(MyCustomModel)): ...
+async def foo(data: MyCustomModel = QueryDepends(MyCustomModel)): ...
+```
+
+---
+
+If you want to accept a file on an endpoint, then the content-type for that endpoint changes from application/json to www-form-data.
+
+FastAPI does not know how to override the pydantic schema so that parameters are passed as form.
+Even if you do
+
+`foo: CustomPydanticModel = Depends()`
+all model attributes will be passed as query, but we want them to become body, that's what this library exists for.
+
+### Usually you use something along the lines of:
+![image](https://user-images.githubusercontent.com/64792903/161484700-642e3d0e-242f-49f6-82e8-45c5e912a2c2.png)
+
+But, if we accept a lot of fields, then the function becomes very large (the number of attributes for the endpoint increases and it does not look very good).
+
+Thanks to this library, it is possible to force the conversion of Field fields into fields of FastAPI Form with full preservation of all attributes (alias, gt, te, description, title, example and more...)
+
 
 
-setup(**setup_kwargs)
```

