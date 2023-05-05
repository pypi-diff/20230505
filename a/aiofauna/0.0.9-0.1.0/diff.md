# Comparing `tmp/aiofauna-0.0.9.tar.gz` & `tmp/aiofauna-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.0.9.tar", max compression
+gzip compressed data, was "aiofauna-0.1.0.tar", max compression
```

## Comparing `aiofauna-0.0.9.tar` & `aiofauna-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-04-10 13:14:14.629944 aiofauna-0.0.9/aiofauna/__init__.py
--rw-r--r--   0        0        0     7816 2023-04-09 15:50:09.852936 aiofauna-0.0.9/aiofauna/application.py
--rw-r--r--   0        0        0     4881 2023-04-09 00:48:46.949196 aiofauna-0.0.9/aiofauna/client.py
--rw-r--r--   0        0        0      493 2023-04-04 07:02:54.142000 aiofauna-0.0.9/aiofauna/deprecated.py
--rw-r--r--   0        0        0     8215 2023-04-10 13:14:13.610780 aiofauna-0.0.9/aiofauna/errors.py
--rw-r--r--   0        0        0     2198 2023-04-09 16:11:33.832628 aiofauna-0.0.9/aiofauna/helpers.py
--rw-r--r--   0        0        0     6724 2023-04-09 00:48:44.968530 aiofauna-0.0.9/aiofauna/json.py
--rw-r--r--   0        0        0     1303 2023-04-09 01:04:59.396687 aiofauna-0.0.9/aiofauna/meta.py
--rw-r--r--   0        0        0     5777 2023-04-09 14:32:34.125477 aiofauna-0.0.9/aiofauna/objects.py
--rw-r--r--   0        0        0    15914 2023-04-10 13:14:11.811186 aiofauna-0.0.9/aiofauna/odm.py
--rw-r--r--   0        0        0     2624 2023-04-04 08:57:42.050368 aiofauna-0.0.9/aiofauna/page.py
--rw-r--r--   0        0        0    41509 2023-04-02 02:01:30.987614 aiofauna-0.0.9/aiofauna/query.py
--rw-r--r--   0        0        0     1132 2023-04-10 13:24:00.328399 aiofauna-0.0.9/LICENSE
--rw-r--r--   0        0        0      589 2023-04-10 13:25:34.650690 aiofauna-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      804 2023-04-10 13:25:48.777899 aiofauna-0.0.9/setup.py
--rw-r--r--   0        0        0      708 2023-04-10 13:25:48.777899 aiofauna-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1113 2023-05-01 08:40:13.385351 aiofauna-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3069 2023-05-05 11:52:01.285112 aiofauna-0.1.0/README.md
+-rw-r--r--   0        0        0     4075 2023-05-02 01:57:27.857521 aiofauna-0.1.0/aiofauna/__init__.py
+-rw-r--r--   0        0        0    17190 2023-05-04 02:13:14.898858 aiofauna-0.1.0/aiofauna/api.py
+-rw-r--r--   0        0        0    15131 2023-05-02 01:57:28.093559 aiofauna-0.1.0/aiofauna/application.py
+-rw-r--r--   0        0        0     4337 2023-05-02 01:57:27.909530 aiofauna-0.1.0/aiofauna/asgi.py
+-rw-r--r--   0        0        0      220 2023-05-02 01:57:13.298647 aiofauna-0.1.0/aiofauna/cli.py
+-rw-r--r--   0        0        0     4014 2023-05-02 03:44:15.825940 aiofauna-0.1.0/aiofauna/client.py
+-rw-r--r--   0        0        0     3678 2023-05-02 03:44:16.169933 aiofauna-0.1.0/aiofauna/datastructures.py
+-rw-r--r--   0        0        0      529 2023-05-02 03:44:16.533925 aiofauna-0.1.0/aiofauna/deprecated.py
+-rw-r--r--   0        0        0     8161 2023-05-02 03:44:16.889918 aiofauna-0.1.0/aiofauna/errors.py
+-rw-r--r--   0        0        0     2978 2023-05-02 03:44:17.217911 aiofauna-0.1.0/aiofauna/helpers.py
+-rw-r--r--   0        0        0     6673 2023-05-02 03:44:17.525905 aiofauna-0.1.0/aiofauna/json.py
+-rw-r--r--   0        0        0     5861 2023-05-02 03:44:17.853898 aiofauna-0.1.0/aiofauna/objects.py
+-rw-r--r--   0        0        0    14824 2023-05-05 12:09:47.607251 aiofauna-0.1.0/aiofauna/odm.py
+-rw-r--r--   0        0        0     2760 2023-05-02 03:44:15.489947 aiofauna-0.1.0/aiofauna/page.py
+-rw-r--r--   0        0        0    41588 2023-05-02 03:44:15.141955 aiofauna-0.1.0/aiofauna/query.py
+-rw-r--r--   0        0        0      829 2023-05-05 11:52:16.905014 aiofauna-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3988 2023-05-05 12:11:56.329063 aiofauna-0.1.0/setup.py
+-rw-r--r--   0        0        0     4116 2023-05-05 12:11:56.329635 aiofauna-0.1.0/PKG-INFO
```

### Comparing `aiofauna-0.0.9/aiofauna/client.py` & `aiofauna-0.1.0/aiofauna/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import io
 
+import os
+
+from dotenv import load_dotenv
 
 from typing import Any, AsyncGenerator, Optional
 
 
 from aiohttp import ClientSession
 
 
-from aiofauna.errors import AioFaunaException
+from .errors import AioFaunaException
 
 
-from aiofauna.objects import Expr
+from .objects import Expr
 
 
-from aiofauna.json import FaunaJSONEncoder
+from .json import FaunaJSONEncoder
 
+load_dotenv()
 
 def to_json(obj: Expr) -> str:
     """
 
 
     `to_json`
 
@@ -71,58 +75,21 @@
 
         The `_Expr` object will be serialized with `FaunaJSONEncoder` from json module so the FaunaDB API can understand it.
 
 
         The response will be deserialized by the `FaunaModel` class from orm module.
     """
 
-    secret: str
-
-    def __init__(self, secret: Optional[str] = None) -> None:
+    def __init__(self, secret = None):
 
         if secret is None:
 
-            try:
-                import os
-
-                self.secret = os.environ["FAUNA_SECRET"]
-
-            except KeyError:
-
-                try:
-
-                    with open(".env", "r", encoding="utf-8") as file:
-
-                        txt = file.read()
-
-                        for key, val in dict(
-                            [i.split("=") for i in txt.split("\n")]
-                        ).items():
-
-                            if "FAUNA_SECRET" in key:
-
-                                self.secret = val
-
-                                break
-
-                except:  # pylint: disable=bare-except
-
-                    while secret is None:
-
-                        _secret = input("Please enter your FaunaDB secret: ")
-
-                        if _secret:
-
-                            self.secret = _secret
-
-                            break
-
-        else:
-
-            self.secret = secret
+           secret = os.getenv("FAUNA_SECRET")
+           
+        self.secret = secret
 
     async def query(self, expr: Expr) -> Any:
         """
 
 
         `AsyncFaunaClient.query`
 
@@ -151,15 +118,15 @@
 
             async with session.post(
                 "https://db.fauna.com",
                 data=to_json(expr),
                 headers={
                     "Authorization": f"Bearer {self.secret}",
                     "Content-type": "application/json",
-                    "Accept": "application/json",
+                    "Accept": "application/json"
                 },
             ) as response:
                 try:
 
                     data = await response.json()
 
                     return data["resource"]
```

### Comparing `aiofauna-0.0.9/aiofauna/errors.py` & `aiofauna-0.1.0/aiofauna/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Error types that methods in the FaunaDB client throw."""
 
 # pylint: disable=redefined-builtin
 
 from builtins import object
 
-from typing import Union
-
 from pydantic import ValidationError
 
 from aiohttp.web_exceptions import HTTPException
 
 
 class codes:
 
@@ -25,21 +23,18 @@
 
     internal_server_error = 500
 
     unavailable = 503
 
 
 def _get_or_raise(request_result, dct, key):
-
     if isinstance(dct, dict) and key in dct:
-
         return dct[key]
 
     else:
-
         raise UnexpectedError(
             "Response JSON does not contain expected key %s" % key, request_result
         )
 
 
 # region FaunaError
 
@@ -50,52 +45,43 @@
     Error returned by the FaunaDB server.
 
     For documentation of error types, see the `docs <https://fauna.com/documentation#errors>`__.
     """
 
     @staticmethod
     def raise_for_status_code(request_result):
-
         code = request_result.status_code
 
         # pylint: disable=no-member, too-many-return-statements
 
         if 200 <= code <= 299:
             pass
 
         elif code == codes.bad_request:
-
             raise BadRequest(request_result)
 
         elif code == codes.unauthorized:
-
             raise Unauthorized(request_result)
 
         elif code == codes.forbidden:
-
             raise PermissionDenied(request_result)
 
         elif code == codes.not_found:
-
             raise NotFound(request_result)
 
         elif code == codes.internal_server_error:
-
             raise InternalError(request_result)
 
         elif code == codes.unavailable:
-
             raise UnavailableError(request_result)
 
         else:
-
             raise UnexpectedError("Unexpected status code.", request_result)
 
     def __init__(self, description, request_result):
-
         super(FaunaError, self).__init__(description)
 
         self.request_result = request_result
 
         """:any:`RequestResult` for the request that caused this error."""
 
 
@@ -104,49 +90,44 @@
     """Error for when the server returns an unexpected kind of response."""
 
     pass
 
 
 class HttpError(FaunaError):
     def __init__(self, request_result):
-
         self.errors = HttpError._get_errors(request_result)
 
         """List of all :py:class:`ErrorData` objects sent by the server."""
 
         super(HttpError, self).__init__(self._get_description(), request_result)
 
     @staticmethod
     def _get_errors(request_result):
-
         response = request_result.response_content
 
         errors = _get_or_raise(request_result, response, "errors")
 
         return [ErrorData.from_dict(error, request_result) for error in errors]
 
     def __str__(self):
-
         return repr(self.errors[0])
 
     def _get_description(self):
-
         return self.errors[0].description if self.errors else "(empty `errors`)"
 
 
 class BadRequest(HttpError):
 
     """HTTP 400 error."""
 
     pass
 
 
 class Unauthorized(HttpError):
     def __init__(self, request_result):
-
         super(Unauthorized, self).__init__(request_result)
 
         self.errors[
             0
         ].description = "Unauthorized. Check that endpoint, schema, port and secret are correct during client’s instantiation"
 
 
@@ -185,48 +166,42 @@
     """
 
     Data for one error returned by the server.
     """
 
     @staticmethod
     def from_dict(dct, request_result):
-
         return ErrorData(
             _get_or_raise(request_result, dct, "code"),
             _get_or_raise(request_result, dct, "description"),
             dct.get("position"),
             ErrorData.get_failures(dct, request_result),
             ErrorData.get_cause(dct, request_result),
         )
 
     @staticmethod
     def get_failures(dct, request_result):
-
         if "failures" in dct:
-
             return [
                 Failure.from_dict(failure, request_result)
                 for failure in dct["failures"]
             ]
 
         return None
 
     @staticmethod
     def get_cause(dct, request_result):
-
         if "cause" in dct:
-
             return [
                 ErrorData.from_dict(cause, request_result) for cause in dct["cause"]
             ]
 
         return None
 
     def __init__(self, code, description, position, failures, cause=None):
-
         self.code = code
 
         """Error code. See all error codes `here <https://fauna.com/documentation#errors>`__."""
 
         self.description = description
 
         """Error description."""
@@ -244,38 +219,35 @@
 
     List of all :py:class:`Failure` objects returned by the server.
 
     None unless code == "validation failed".
     """
 
     def __repr__(self):
-
         return (
             "ErrorData(code=%s, description=%s, position=%s, failures=%s, cause=%s)"
             % (
                 repr(self.code),
                 repr(self.description),
                 repr(self.position),
                 repr(self.failures),
                 repr(self.cause),
             )
         )
 
     def __eq__(self, other):
-
         return (
             self.__class__ == other.__class__
             and self.description == other.description
             and self.position == other.position
             and self.failures == other.failures
             and self.cause == other.cause
         )
 
     def __ne__(self, other):
-
         # pylint: disable=unneeded-not
 
         return not self == other
 
 
 class Failure(object):
     """
@@ -283,53 +255,48 @@
     Part of the ``failures`` of an :py:class:`ErrorData`.
 
     See the ``Invalid Data`` section of the `docs <https://fauna.com/documentation#errors>`__.
     """
 
     @staticmethod
     def from_dict(dct, request_result):
-
         return Failure(
             _get_or_raise(request_result, dct, "code"),
             _get_or_raise(request_result, dct, "description"),
             _get_or_raise(request_result, dct, "field"),
         )
 
     def __init__(self, code, description, field):
-
         self.code = code
 
         """Failure code."""
 
         self.description = description
 
         """Failure description."""
 
         self.field = field
 
         """Field of the failure in the instance."""
 
     def __repr__(self):
-
         return "Failure(code=%s, description=%s, field=%s)" % (
             repr(self.code),
             repr(self.description),
             repr(self.field),
         )
 
     def __eq__(self, other):
-
         return (
             self.code == other.code
             and self.description == other.description
             and self.field == other.field
         )
 
     def __ne__(self, other):
-
         # pylint: disable=unneeded-not
 
         return not self == other
 
 
 AioFaunaException = (
     ValidationError,
@@ -370,7 +337,12 @@
     ProcessLookupError,
     TimeoutError,
     BlockingIOError,
     ChildProcessError,
     ConnectionError,
     BrokenPipeError,
 )
+
+
+"""
+(c) 2016 Fauna, Inc.
+"""
```

### Comparing `aiofauna-0.0.9/aiofauna/helpers.py` & `aiofauna-0.1.0/aiofauna/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """
 Flaskaesque helper functions for aiohttp.
 """
+import asyncio
 from functools import wraps
 from aiohttp import web
+from aiohttp.web_request import FileField
 from jinja2 import Environment, FileSystemLoader
 
+
 def jsonify(func):
     """
     Decorator to convert the result of an asynchronous function to a JSON response.
 
     Args:
         func (callable): The asynchronous function to be wrapped.
 
     Returns:
         callable: A wrapped version of the input function that returns a JSON response.
     """
+
     @wraps(func)
     async def wrapper(request):
         try:
             return web.json_response(await func(request))
         except Exception as e:
             return web.json_response(func(request))
+
     return wrapper
 
 
 def redirect(url):
     """
     Create an HTTP redirect response.
 
@@ -58,11 +63,36 @@
 
     Args
         template_name (str): The name of the template file.
         **kwargs: Keyword arguments representing context variables to be passed to the template.
 
     Returns:
         web.Response: An HTTP response with the rendered template as its body and content type set to "text/html".
-    """    
+    """
     env = Environment(loader=FileSystemLoader("templates"))
     template = env.get_template(template_name).render(**kwargs)
-    return web.Response(body=template.encode(), content_type="text/html")
+    return web.Response(body=template.encode(), content_type="text/html")
+
+
+def upload_files(func):
+    """
+    Decorator to handler file uploading in an asynchronous function.
+
+    Args:
+        func (callable): The asynchronous function to be wrapped.
+
+    Returns:
+        callable: A wrapped version of the input function that returns a JSON response.
+    """
+
+    @wraps(func)
+    async def wrapper(request: web.Request):
+        file_payload = await request.post()
+        files = {}
+        for key, value in file_payload.items():
+            if isinstance(value, FileField):
+                files[key] = value
+        if asyncio.iscoroutinefunction(func):
+            return await func(request, files)
+        return func(request, files)
+
+    return wrapper
```

### Comparing `aiofauna-0.0.9/aiofauna/json.py` & `aiofauna-0.1.0/aiofauna/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,93 +1,81 @@
 import asyncio
 from base64 import urlsafe_b64decode, urlsafe_b64encode
 from datetime import date, datetime
 from json import JSONEncoder, dumps, loads
-from typing import overload
 from typing_extensions import override
 from iso8601 import parse_date
-from pydantic import BaseModel # pylint: disable=no-name-in-module
-from aiofauna.objects import FaunaTime, Native, Query, Ref, SetRef
-from aiofauna.query import Expr
-from aiohttp.web import Request, Response
+from pydantic import BaseModel  # pylint: disable=no-name-in-module
+from .objects import FaunaTime, Native, Query, Ref, SetRef
+from .query import Expr
+from aiohttp.web import Request
+
 
 def parse_json(json_string):
     """
 
     Parses a JSON string into python values.
 
     Also parses :any:`Ref`, :any:`SetRef`, :any:`FaunaTime`, and :class:`date`.
     """
 
     return loads(json_string, object_hook=_parse_json_hook)
 
 
 def parse_json_or_none(json_string):
     try:
-
         return parse_json(json_string)
 
     except ValueError:
-
         pass
 
 
 def _parse_json_hook(dct):
-
     # pylint: disable=too-many-return-statements
     """
 
     Looks for FaunaDB types in a JSON object and converts to them if possible.
     """
 
     if "@ref" in dct:
-
         ref = dct["@ref"]
 
         if (not "collection" in ref) and (not "database" in ref):
-
             return Native.from_name(ref["id"])
 
         return Ref(ref["id"], ref.get("collection"), ref.get("database"))
 
     if "@obj" in dct:
-
         return dct["@obj"]
 
     if "@set" in dct:
-
         return SetRef(dct["@set"])
 
     if "@query" in dct:
-
         return Query(dct["@query"])
 
     if "@ts" in dct:
-
         return FaunaTime(dct["@ts"])
 
     if "@date" in dct:
-
         return parse_date(dct["@date"]).date()
 
     if "@bytes" in dct:
-
         return bytearray(urlsafe_b64decode(dct["@bytes"].encode()))
     return dct
 
 
 def to_json(dct, pretty=True, sort_keys=True):
     """
 
     Opposite of parse_json.
 
     Converts a :any`_Expr` into a request body, calling :any:`to_fauna_json`.
     """
     if pretty:
-
         return dumps(
             dct, cls=FaunaJSONEncoder, sort_keys=True, indent=4, separators=(", ", ": ")
         )
 
     return dumps(dct, cls=FaunaJSONEncoder, sort_keys=sort_keys, separators=(",", ":"))
 
 
@@ -103,15 +91,14 @@
     Attributes:
     ----------
     No public attributes.
     """
 
     @override
     def default(self, obj):
-        
         """
         Encodes the given object in Fauna-compatible JSON format.
 
         Parameters:
         ----------
         obj: any
             The object to be encoded.
@@ -132,26 +119,29 @@
             return {"@date": obj.isoformat()}
         elif isinstance(obj, (bytes, bytearray)):
             return {"@bytes": urlsafe_b64encode(obj).decode("utf-8")}
         elif isinstance(obj, BaseModel):
             return obj.dict()
         elif isinstance(obj, Request):
             # Swagger UI
-            if obj.content_type in ("application/json", "application/x-www-form-urlencoded"):
+            if obj.content_type in (
+                "application/json",
+                "application/x-www-form-urlencoded",
+            ):
                 data = parse_json_or_none(obj.content.read_nowait().decode())
                 if data:
                     return {
                         "method": obj.method,
                         "path": obj.path,
                         "headers": dict(obj.headers),
                         "body": data,
                     }
             elif obj.content_type == "multipart/form-data":
                 data = {}
-                for k,v in asyncio.run(obj.post()):
+                for k, v in asyncio.run(obj.post()):
                     _v = None
                     try:
                         _v = loads(v)
                     except ValueError:
                         _v = "file"
                     data[k] = v
             else:
@@ -159,15 +149,14 @@
                 return {
                     "method": obj.method,
                     "query_params": dict(obj.query),
                     "path_params": dict(obj.match_info),
                     "headers": dict(obj.headers),
                     "body": data,
                 }
-            
 
 
 class JSONModel(BaseModel):
     """
     A model class for JSON serialization and deserialization.
 
     Methods:
@@ -236,15 +225,15 @@
         Returns:
         -------
         dict
             The model's attributes as a dictionary.
         """
 
         return self.to_dict(**kwargs)
-    
+
     @override
     def json(self, **kwargs) -> str:
         """
         Alias for to_json() method.
 
         Parameters:
         ----------
@@ -253,8 +242,8 @@
 
         Returns:
         -------
         str
             The model's attributes as a JSON string.
         """
 
-        return self.to_json(**kwargs)
+        return self.to_json(**kwargs)
```

### Comparing `aiofauna-0.0.9/aiofauna/objects.py` & `aiofauna-0.1.0/aiofauna/objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
 Types used in queries and responses.
 See the `docs <https://app.fauna.com/documentation/reference/queryapi#simple-type>`__.
 """
 from datetime import datetime
 from iso8601 import parse_date
-from aiofauna.deprecated import deprecated
-from aiofauna.query import Expr
+from .deprecated import deprecated
+from .query import Expr
+
 
 class Ref(Expr):
     """
     ```python
     Ref(id, cls=None, db=None)
     ```
     A reference to a document in a collection or index.
-    
+
     :param id: The document's ID.
     :param cls: The collection or index class.
     :param db: The database.
 
-    `Ref` 
-    
+    `Ref`
+
     Is a special type in FaunaDB. It is used to represent a document in a collection or index.
-    
-    It is serialized to JSON as an object with the `@ref` key. Passing the `id` to the response. 
-    
+
+    It is serialized to JSON as an object with the `@ref` key. Passing the `id` to the response.
+
     """
 
     def __init__(self, id, cls=None, db=None):
         if id is None:
             raise ValueError("The Ref must have an id.")
 
         value = {"id": id}
@@ -38,35 +39,35 @@
         if db != None:
             value["database"] = db
 
         super(Ref, self).__init__(value)
 
     def collection(self):
         """
-    Gets the collection part out of the Ref.
-    """
+        Gets the collection part out of the Ref.
+        """
         return self.value.get("collection")
 
     @deprecated("use collection instead")
     def class_(self):
         """
-    Gets the class part out of the Ref.
-    """
+        Gets the class part out of the Ref.
+        """
         return self.value.get("collection")
 
     def database(self):
         """
-    Gets the database part out of the Ref.
-    """
+        Gets the database part out of the Ref.
+        """
         return self.value.get("database")
 
     def id(self):
         """
-    Gets the id part out of the Ref.
-    """
+        Gets the id part out of the Ref.
+        """
         return self.value["id"]
 
     def to_fauna_json(self):
         return {"@ref": self.value}
 
     def __str__(self):
         col = (
@@ -115,18 +116,18 @@
     @classmethod
     def from_name(cls, name):
         return getattr(cls, name.upper(), Ref(name))
 
 
 class SetRef(Expr):
     """
-  FaunaDB Set.
-  This represents a set returned as part of a response.
-  For query sets see :doc:`query`.
-  """
+    FaunaDB Set.
+    This represents a set returned as part of a response.
+    For query sets see :doc:`query`.
+    """
 
     def __init__(self, set_ref):
         if isinstance(set_ref, Expr):
             value = set_ref.value
         else:
             value = set_ref
 
@@ -144,39 +145,39 @@
     def __ne__(self, other):
         # pylint: disable=unneeded-not
         return not self == other
 
 
 class FaunaTime(Expr):
     """
-  FaunaDB time. See the `docs <https://app.fauna.com/documentation/reference/queryapi#special-type>`__.
+    FaunaDB time. See the `docs <https://app.fauna.com/documentation/reference/queryapi#special-type>`__.
 
-  For dates, regular :class:`datetime.date` objects are used.
-  """
+    For dates, regular :class:`datetime.date` objects are used.
+    """
 
     def __init__(self, value):
         """
-    :param value:
-      If a :class:`datetime.datetime` is passed, it is converted to a string.
-      Must include an offset.
-    """
+        :param value:
+          If a :class:`datetime.datetime` is passed, it is converted to a string.
+          Must include an offset.
+        """
         if isinstance(value, datetime):
             if value.utcoffset() is None:
                 raise ValueError("FaunaTime requires offset-aware datetimes")
             value = value.isoformat()
 
         # Convert +00:00 offset to zulu for comparison equality
         # We don't check for +0000 or +00 as they are not valid in FaunaDB
         super(FaunaTime, self).__init__(value.replace("+00:00", "Z"))
 
     def to_datetime(self):
         """
-    Convert to an offset-aware datetime object.
-    This is lossy as datetimes have microsecond rather than nanosecond precision.
-    """
+        Convert to an offset-aware datetime object.
+        This is lossy as datetimes have microsecond rather than nanosecond precision.
+        """
         return parse_date(self.value)
 
     def to_fauna_json(self):
         return {"@ts": self.value}
 
     def __repr__(self):
         return "FaunaTime(%s)" % repr(self.value)
@@ -187,23 +188,28 @@
     def __ne__(self, other):
         # pylint: disable=unneeded-not
         return not self == other
 
 
 class Query(Expr):
     """
-  Represents a `@query` type in FaunaDB.
-  See the `docs <https://app.fauna.com/documentation/reference/queryapi#special-type>`__.
-  """
+    Represents a `@query` type in FaunaDB.
+    See the `docs <https://app.fauna.com/documentation/reference/queryapi#special-type>`__.
+    """
 
     def to_fauna_json(self):
         return {"@query": self.value}
 
     def __repr__(self):
         return "Query(%s)" % repr(self.value)
 
     def __eq__(self, other):
         return isinstance(other, Query) and self.value == other.value
 
     def __ne__(self, other):
         # pylint: disable=unneeded-not
         return not self == other
+
+
+"""
+(c) 2016 Fauna, Inc.
+"""
```

### Comparing `aiofauna-0.0.9/aiofauna/odm.py` & `aiofauna-0.1.0/aiofauna/odm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,343 +1,299 @@
 """Lightweight ORM to perform simple CRUD operations on FaunaDB collections and provision indexes
 
+
    the fauna query object is available also within the class for further customization
 """
 
-from __future__ import annotations
-
-import asyncio
-
-from typing import List, Optional, Any, Callable
-
-from aiofauna import query as q
-
-from aiofauna.errors import AioFaunaException
-
-from aiofauna.json import JSONModel  # pylint: disable=no-name-in-module
-
-from aiofauna.client import AsyncFaunaClient
-
-
-class AsyncFaunaModel(JSONModel):
-    """
-
-    A base model class for interacting with FaunaDB using asynchronous operations.
-
-
-    Attributes:
-    -----------
 
-    ref: Optional[str]
-
-        The FaunaDB reference ID of the model instance.
+from __future__ import annotations
 
-    ts: Optional[int]
 
-        The timestamp of the model instance.
+import logging
 
+import os
 
-    Methods:
-    --------
+import asyncio
 
-    client() -> AsyncFaunaClient:
 
-        Returns an instance of AsyncFaunaClient to interact with FaunaDB.
+from typing import List, Optional, Any, Callable, Union
 
-    q() -> Expr:
+try:
+    import query as q
+except ImportError:
+    from . import query as q
 
-        Returns an instance of Expr to build queries for FaunaDB.
+from .errors import AioFaunaException
 
-    async provision() -> None:
 
-        Creates a collection and indexes for the model if they don't exist in FaunaDB.
+from .json import JSONModel  # pylint: disable=no-name-in-module
 
-    exists(ref: str) -> bool:
 
-        Checks if a document exists in FaunaDB.
+from .client import AsyncFaunaClient
 
-    find_unique(field: str, value: Any) -> Optional[AsyncFaunaModel]:
 
-        Finds a document in FaunaDB by a unique field.
+from pydantic import BaseModel  # pylint: disable=no-name-in-module
 
-    find_many(field: str, value: Any) -> Optional[List[AsyncFaunaModel]]:
 
-        Finds documents in FaunaDB by a field.
+from dotenv import load_dotenv
 
-    find(ref: str) -> Optional[AsyncFaunaModel]:
 
-        Finds a document in FaunaDB by its ID.
+load_dotenv()
 
-    find_all() -> Optional[List[AsyncFaunaModel]]:
 
-        Finds all documents of the model in FaunaDB.
+class Fql(BaseModel):
+    field: str
 
-    delete_unique(field: str, value: Any) -> bool:
+    operator: str
 
-        Deletes a document in FaunaDB by a unique field.
+    value: Any
 
-    create() -> Optional[AsyncFaunaModel]:
 
-        Creates a new document in FaunaDB.
-
-    update(ref: str, **kwargs) -> Optional[AsyncFaunaModel]:
-
-        Updates a document in FaunaDB.
-
-    upsert() -> Optional[AsyncFaunaModel]:
-
-        Upserts a document in FaunaDB.
-
-    query(query: str) -> Optional[List[AsyncFaunaModel]]:
+class AsyncFaunaModel(JSONModel):
+    """
 
-        Runs a query in FaunaDB.
+    FaunaDB Base Model
     """
 
     ref: Optional[str] = None
 
-    ts: Optional[int] = None
-
+    ts: Optional[str] = None
 
     def __init__(self, **data: Any) -> None:
 
-        for field in self.__fields__.values():
+        super().__init__(**data)
 
+        for field in self.__fields__.values():
             try:
-                
                 one_of = field.field_info.extra.get("oneOf")
-                
+
                 if isinstance(one_of, list):
-                
                     if data.get(field.name) not in one_of:
-                    
                         raise ValueError(f"{field.name} must be one of {one_of}")
-                    
-            except KeyError:
-                
+
+            except Exception:  # pylint: disable=broad-except
                 continue
 
-        super().__init__(**data)
+
 
     @classmethod
     def client(cls) -> AsyncFaunaClient:
-        """
-
-        Returns an instance of AsyncFaunaClient to interact with FaunaDB.
-
-
-        Returns:
-        --------
-
-        AsyncFaunaClient:
-
-            An instance of AsyncFaunaClient.
-        """
-
-        return AsyncFaunaClient()  # pylint: disable=no-value-for-parameter
+        
+        fauna_secret = os.getenv("FAUNA_SECRET")
+              
+        return AsyncFaunaClient(secret=fauna_secret)
 
     @classmethod
     def q(cls) -> Callable:
-        """
-
-        Returns an instance of Expr to build queries for FaunaDB.
-
-
-        Returns:
-        --------
-
-        Expr:
-
-            An instance of Expr.
-        """
-
+        
         return cls.client().query
 
     @classmethod
-    async def provision(cls) -> None:
-        """
-
-        Creates a collection and indexes for the model if they don't exist in FaunaDB.
-
-
-        Returns:
-        --------
-
-        None:
-
-            None.
-        """
-
+    async def provision(cls) -> bool:
+        
         _q = cls.q()
-
         try:
-
             if not await _q(q.exists(q.collection(cls.__name__.lower()))):
-
                 await _q(q.create_collection({"name": cls.__name__.lower()}))
 
-                print(f"Created collection {cls.__name__.lower()}")
+                print("Created collection %s", cls.__name__.lower())
 
+            if not await _q(q.exists(q.index(cls.__name__.lower()))):
                 await _q(
                     q.create_index(
                         {
                             "name": cls.__name__.lower(),
                             "source": q.collection(cls.__name__.lower()),
                         }
                     )
                 )
 
                 print(f"Created index {cls.__name__.lower()}")
 
             for field in cls.__fields__.values():
-
                 if field.field_info.extra.get("unique"):
+                    if not await _q(
+                        q.exists(q.index(f"{cls.__name__.lower()}_{field.name}_unique"))
+                    ):
+                        await _q(
+                            q.create_index(
+                                {
+                                    "name": f"{cls.__name__.lower()}_{field.name}_unique",
+                                    "source": q.collection(cls.__name__.lower()),
+                                    "terms": [{"field": ["data", field.name]}],
+                                    "unique": True,
+                                }
+                            )
+                        )
 
-                    await _q(
-                        q.create_index(
-                            {
-                                "name": f"{cls.__name__.lower()}_{field.name}_unique",
-                                "source": q.collection(cls.__name__.lower()),
-                                "terms": [{"field": ["data", field.name]}],
-                                "unique": True,
-                            }
+                        print(
+                            cls.__name__.lower(),
+                            field.name,
                         )
-                    )
 
                     print(
-                        f"Created unique index {cls.__name__.lower()}_{field.name}_unique"
+                        "Created unique index %s_%s",
+                        cls.__name__.lower(),
+                        field.name,
                     )
+
                     continue
 
                 if field.field_info.extra.get("index"):
+                    if not await _q(
+                        q.exists(q.index(f"{cls.__name__.lower()}_{field.name}"))
+                    ):
+                        await _q(
+                            q.create_index(
+                                {
+                                    "name": f"{cls.__name__.lower()}_{field.name}",
+                                    "source": q.collection(cls.__name__.lower()),
+                                    "terms": [{"field": ["data", field.name]}],
+                                }
+                            )
+                        )
 
-                    await _q(
-                        q.create_index(
-                            {
-                                "name": f"{cls.__name__.lower()}_{field.name}",
-                                "source": q.collection(cls.__name__.lower()),
-                                "terms": [{"field": ["data", field.name]}],
-                            }
+                        print(
+                            "Created index %s_%s", cls.__name__.lower(), field.name
                         )
-                    )
+                        continue
 
-                    print(f"Created index {cls.__name__.lower()}_{field.name}")
-                    continue
+            return True
 
         except AioFaunaException as exc:
+            logging.error(exc)
 
-            print(exc)
-
-            return None
+            return False
 
     @classmethod
     async def exists(cls, ref: str) -> bool:
         """
 
+
         Checks if a document exists in FaunaDB.
 
 
+
         Parameters:
         -----------
-        ref: str
+        ref: int
+
 
             The reference ID of the document to check.
 
 
+
         Returns:
         --------
 
+
         bool:
 
+
             True if the document exists, False otherwise.
         """
 
         try:
-
             return await cls.q()(
                 q.exists(q.ref(q.collection(cls.__name__.lower()), ref))
             )
 
         except AioFaunaException as exc:
-
-            print(exc)
+            logging.error(exc)
 
             return False
 
     @classmethod
-    async def find_unique(cls, field: str, value: Any) -> Optional[AsyncFaunaModel]:
+    async def find_unique(
+        cls, field: str, value: Any
+    ) -> Union[AsyncFaunaModel, BaseModel]:
         """
 
+
         Finds a document in FaunaDB by a unique field.
 
 
+
         Parameters:
         -----------
         field: str
 
+
             The name of the field to search.
 
+
         value: Any
 
+
             The value to search for.
 
 
+
         Returns:
         --------
 
-        Optional[AsyncFaunaModel]:
+
+        Union[AsyncFaunaModel,BaseModel]:
+
 
             An instance of the model if found, None otherwise.
         """
 
         try:
-
             data = await cls.q()(
                 q.get(q.match(q.index(f"{cls.__name__.lower()}_{field}_unique"), value))
             )
             return cls(
                 **{
                     **data["data"],
                     "ref": data["ref"]["@ref"]["id"],
                     "ts": data["ts"] / 1000,
                 }
             )
 
         except AioFaunaException as exc:
-            print(exc)
+            logging.error(exc)
 
-            return None
+            return await ExceptionModel(message=str(exc), status="error").create()
 
     @classmethod
-    async def find_many(cls, field: str, value: Any) -> Optional[List[AsyncFaunaModel]]:
+    async def find_many(cls, field: str, value: Any) -> List[AsyncFaunaModel]:
         """
 
+
         Finds documents in FaunaDB by a field.
 
 
+
         Parameters:
         -----------
         field: str
 
+
             The name of the field to search.
 
+
         value: Any
 
+
             The value to search for.
 
 
+
         Returns:
         --------
 
-        Optional[List[AsyncFaunaModel]]:
+
+        List[AsyncFaunaModel]:
+
 
             A list of instances of the model if found, None otherwise.
         """
 
         try:
-
             _q = cls.q()
 
             refs = (
                 await _q(
                     q.paginate(
                         q.match(q.index(f"{cls.__name__.lower()}_{field}"), value)
                     )
@@ -359,75 +315,81 @@
                 cls(
                     **{**d["data"], "ref": d["ref"]["@ref"]["id"], "ts": d["ts"] / 1000}
                 )
                 for d in data
             ]
 
         except AioFaunaException as exc:
+            logging.error(exc)
 
-            print(exc)
-
-            return None
+            return []
 
     @classmethod
-    async def find(cls, ref: str) -> Optional[AsyncFaunaModel]:
+    async def find(cls, ref: str) -> Union[AsyncFaunaModel, BaseModel]:
         """
 
+
         Finds a document in FaunaDB by its ID.
 
 
+
         Parameters:
         -----------
-        ref: str
+        ref: int
+
 
             The reference ID of the document to find.
 
 
+
         Returns:
         --------
 
-        Optional[AsyncFaunaModel]:
+
+        Union[AsyncFaunaModel,BaseModel]:
+
 
             An instance of the model if found, None otherwise.
         """
 
         try:
-
             data = await cls.q()(q.get(q.ref(q.collection(cls.__name__.lower()), ref)))
             return cls(
                 **{
                     **data["data"],
                     "ref": data["ref"]["@ref"]["id"],
                     "ts": data["ts"] / 1000,
                 }
             )
 
         except AioFaunaException as exc:
+            logging.error(exc)
 
-            print(exc)
-
-            return None
+            return await ExceptionModel(message=str(exc), status="error").create()
 
     @classmethod
-    async def find_all(cls) -> Optional[List[AsyncFaunaModel]]:
+    async def find_all(cls, limit: int, offset: int) -> List[AsyncFaunaModel]:
         """
 
+
         Finds all documents of the model in FaunaDB.
 
 
+
         Returns:
         --------
 
-        Optional[List[AsyncFaunaModel]]:
+
+        List[AsyncFaunaModel]:
+
 
             A list of instances of the model if found, None otherwise.
         """
 
         try:
-
             _q = cls.q()
 
             refs = (await _q(q.paginate(q.match(q.index(cls.__name__.lower())))))[
                 "data"
             ]
 
             data = await asyncio.gather(
@@ -445,240 +407,214 @@
                 cls(
                     **{**d["data"], "ref": d["ref"]["@ref"]["id"], "ts": d["ts"] / 1000}
                 )
                 for d in data
             ]
 
         except AioFaunaException as exc:
+            logging.error(exc)
 
-            print(exc)
-
-            return None
+            return []
 
     @classmethod
     async def delete_unique(cls, field: str, value: Any) -> bool:
         """
 
-        Deletes a document in FaunaDB by a unique field.
 
+                Deletes a document in FaunaDB by a unique field.
 
-        Parameters:
-        -----------
-        field: str
 
-            The name of the unique field to use in the search.
 
-        value: Any
+                Parameters:
+                -----------
+                field: str
 
-            The value of the unique field to use in the search.
 
+                    The name of the unique field to use in the search.
 
-        Returns:
-        --------
 
-        bool:
+                value: Any
+
+
+                    The value of the unique field to use in the search.
+
 
-            True if the document is deleted, False otherwise.
+
+                Returns:
+                --------
+
+
+                bool:
+        t
+
+                    True if the document is deleted, False otherwise.
         """
 
         try:
-
             _q = cls.q()
 
             ref = await _q(
                 q.get(q.match(q.index(f"{cls.__name__.lower()}_{field}_unique"), value))
             )
 
             await _q(q.delete(ref))
 
             return True
 
         except AioFaunaException as exc:
-
-            print(exc)
+            logging.error(exc)
 
             return False
 
     @classmethod
     async def delete(cls, ref: str) -> bool:
-
         """Delete a document by id"""
 
         try:
-
             await cls.q()(q.delete(q.ref(q.collection(cls.__name__.lower()), ref)))
 
             return True
 
         except AioFaunaException as exc:
-
-            print(exc)
+            logging.error(exc)
 
             return False
 
-    async def create(self) -> Optional[AsyncFaunaModel]:
+    async def create(self) -> AsyncFaunaModel:
         """
 
+
         Creates a new document in FaunaDB.
 
 
+
         Parameters:
         -----------
 
+
         **kwargs:
 
+
             The data to create the new document with.
 
 
+
         Returns:
         --------
 
-        Optional[AsyncFaunaModel]:
+
+        Union[AsyncFaunaModel,BaseModel]:
+
 
             An instance of the model if created successfully, None otherwise.
         """
 
         try:
-
             for field in self.__fields__.values():
-
                 if field.field_info.extra.get("unique"):
-
-                    instance = await self.find_unique(
-                        field.name, self.dict()[field.name]  # type: ignore
-                    )
-                    if instance:
-                        return instance
-
-            data = await self.q()(
-                q.create(
-                    q.collection(self.__class__.__name__.lower()), {"data": self.dict()}
+                    if await self.__class__.find_unique(field.name, getattr(self, field.name)):
+                        raise Exception(
+                            f"Document with {field.name} {getattr(self, field.name)} already exists"
+                        ) 
+                return self.__class__(
+                    **{
+                        **(await self.__class__.q()(q.create(q.collection(self.__class__.__name__.lower()), {"data": self.dict()}))),
+                        "ref": self.ref,
+                        "ts": self.ts,
+                    }
                 )
-            )
-            return self.__class__(
-                **{
-                    **data["data"],
-                    "ref": data["ref"]["@ref"]["id"],
-                    "ts": data["ts"] / 1000,
-                }
-            )
+                
 
         except AioFaunaException as exc:
+            logging.error(exc)
 
-            print(exc)
-
-            return None
+            return await ExceptionModel(message=str(exc), status="error").create()
 
     @classmethod
-    async def update(cls, ref: str, **kwargs) -> Optional[AsyncFaunaModel]:
-        """
-
-        Creates a new document in FaunaDB.
-
-
-        Parameters:
-        -----------
-
-        **kwargs:
-
-            The data to create the new document with.
-
-
-        Returns:
-        --------
-
-        Optional[AsyncFaunaModel]:
-
-            An instance of the model if created successfully, None otherwise.
+    async def query(cls, query: str) -> List[AsyncFaunaModel]:
         """
 
-        try:
-
-            data = await cls.q()(
-                q.update(
-                    q.ref(q.collection(cls.__name__.lower()), ref), {"data": kwargs}
-                )
-            )
-            return cls(
-                **{
-                    **data["data"],
-                    "ref": data["ref"]["@ref"]["id"],
-                    "ts": data["ts"] / 1000,
-                }
-            )
 
-        except AioFaunaException as exc:
-
-            print(exc)
-
-            return None
+        Queries FaunaDB using a string query and returns a list of instances of the model.
 
-    async def upsert(self) -> Optional[AsyncFaunaModel]:
-        """
 
-        Creates a new document in FaunaDB.
 
+        Args:
 
-        Parameters:
-        -----------
 
-        **kwargs:
+            query (str): The query to use.
 
-            The data to create the new document with.
 
 
         Returns:
-        --------
 
-        Optional[AsyncFaunaModel]:
 
-            An instance of the model if created successfully, None otherwise.
+            List[AsyncFaunaModel]: A list of instances of the model if found, None otherwises.
         """
 
         try:
-            if not self.ref:
+            refs = (await cls.q()(q.paginate(q.match(q.query(query)))))["data"]
 
-                return await self.create()
+            data = await asyncio.gather(*[cls.q()(q.get(ref)) for ref in refs])
 
-            return await self.update(self.ref, **self.dict())  # type: ignore
+            return [
+                cls(
+                    **{**d["data"], "ref": d["ref"]["@ref"]["id"], "ts": d["ts"] / 1000}
+                )
+                for d in data
+            ]
 
         except AioFaunaException as exc:
+            logging.error(exc)
 
-            print(exc)
-
-            return None
+            return []
 
     @classmethod
-    async def query(cls, query: str) -> Optional[List[AsyncFaunaModel]]:
-        """
+    async def update(cls, ref: str, **kwargs) -> AsyncFaunaModel:
+        try:
+            instance = await cls.find(ref)
+            if isinstance(instance, cls):
+                instance_updated = await cls.q()(
+                    q.update(
+                        q.ref(q.collection(cls.__name__.lower()), ref), {"data": kwargs}
+                    )
+                )
+                return cls(
+                    **{
+                        **instance_updated["data"],
+                        "ref": instance_updated["ref"]["@ref"]["id"],
+                        "ts": instance_updated["ts"] / 1000,
+                    }
+                )
+            else:
+                raise ValueError(f"Field {ref} not found")
+        except AioFaunaException as exc:
+            logging.error(exc)
+            raise ValueError(f"Field {ref} not found")
 
-        Queries FaunaDB using a string query and returns a list of instances of the model.
+    async def save(self) -> AsyncFaunaModel:
+        """
 
 
-        Args:
+        Saves a document in FaunaDB.
 
-            query (str): The query to use.
 
 
         Returns:
+        --------
 
-            Optional[List[AsyncFaunaModel]]: A list of instances of the model if found, None otherwises.
-        """
 
-        try:
+        Union[AsyncFaunaModel,BaseModel]:
 
-            refs = (await cls.q()(q.paginate(q.match(q.query(query)))))["data"]
 
-            data = await asyncio.gather(*[cls.q()(q.get(ref)) for ref in refs])
+            An instance of the model if saved successfully, None otherwise.
+        """
 
-            return [
-                cls(
-                    **{**d["data"], "ref": d["ref"]["@ref"]["id"], "ts": d["ts"] / 1000}
-                )
-                for d in data
-            ]
+        if isinstance(self.ref, str) and len(self.ref) == 18:
+            return await self.update(self.ref, kwargs=self.dict())
+        return await self.create()
 
-        except AioFaunaException as exc:
 
-            print(exc)
+class ExceptionModel(AsyncFaunaModel):
+    message: Optional[str]
+    status: Optional[str]
 
-            return None
```

### Comparing `aiofauna-0.0.9/aiofauna/page.py` & `aiofauna-0.1.0/aiofauna/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from aiofauna import query
+try:
+    import query as q
+except ImportError:
+    from . import query as q
 
 
 class Page(object):
     """
-  Represents a single pagination result.
-  See ``paginate`` in the `docs <https://app.fauna.com/documentation/reference/queryapi#read-functions>`__.
-  You must convert to Page yourself using :py:meth:`from_raw`.
-  """
+    Represents a single pagination result.
+    See ``paginate`` in the `docs <https://app.fauna.com/documentation/reference/queryapi#read-functions>`__.
+    You must convert to Page yourself using :py:meth:`from_raw`.
+    """
 
     @staticmethod
     def from_raw(raw):
         """Convert a raw response dict to a Page."""
         return Page(raw["data"], raw.get("before"), raw.get("after"))
 
     def __init__(self, data, before=None, after=None):
@@ -39,25 +42,25 @@
             and self.before == other.before
             and self.after == other.after
         )
 
     @staticmethod
     def set_iterator(client, set_query, map_lambda=None, mapper=None, page_size=None):
         """
-    Iterator that keeps getting new pages of a set.
+        Iterator that keeps getting new pages of a set.
 
-    :param map_lambda:
-      If present, a :any:`lambda_` for mapping set elements.
-    :param mapper:
-      Mapping Python function used on each page element.
-    :param page_size:
-      Number of instances to be fetched at a time.
-    :return:
-      Iterator through all elements in the set.
-    """
+        :param map_lambda:
+          If present, a :any:`lambda_` for mapping set elements.
+        :param mapper:
+          Mapping Python function used on each page element.
+        :param page_size:
+          Number of instances to be fetched at a time.
+        :return:
+          Iterator through all elements in the set.
+        """
 
         def get_page(**kwargs):
             queried = query.paginate(set_query, **kwargs)
             if map_lambda is not None:
                 queried = query.map_(map_lambda, queried)
             return Page.from_raw(client.query(queried))
 
@@ -69,7 +72,12 @@
 
         while getattr(page, next_cursor) is not None:
             page = get_page(
                 **{"size": page_size, next_cursor: getattr(page, next_cursor)}
             )
             for val in page.data:
                 yield val if mapper is None else mapper(val)
+
+
+"""
+(c) 2016 Fauna, Inc.
+"""
```

### Comparing `aiofauna-0.0.9/aiofauna/query.py` & `aiofauna-0.1.0/aiofauna/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 For example: ``select("a", {"a": Ref("123", Ref("widgets", Native.CLASSES))})``.
 """
 
 # pylint: disable=invalid-name, redefined-builtin
 
 from types import FunctionType
-from aiofauna import deprecated
+from . import deprecated
 
 # region Basic forms
 
 
 def abort(msg):
     """See the `docs <https://docs.fauna.com/fauna/current/api/fql/functions/abort>`__."""
     return _fn({"abort": msg})
@@ -132,33 +132,33 @@
 def do(*expressions):
     """See the `docs <https://docs.fauna.com/fauna/current/api/fql/functions/do>`__."""
     return _fn({"do": expressions})
 
 
 def lambda_query(func):
     """
-  See the `docs <https://app.fauna.com/documentation/reference/queryapi#basic-forms>`__.
-  This form generates :any:`var` objects for you, and is called like::
+    See the `docs <https://app.fauna.com/documentation/reference/queryapi#basic-forms>`__.
+    This form generates :any:`var` objects for you, and is called like::
 
-      query.lambda_query(lambda a: query.add(a, a))
-      # Produces: {
-      #  "lambda": "a",
-      #  "expr": {"add": ({"var": "a"}, {"var": "a"})}
-      # }
-
-  You usually don't need to call this directly as lambdas in queries will be converted for you.
-  For example: ``query.map_(lambda a: query.add(a, 1), collection)``.
-
-  You can also use :any:`lambda_` directly.
-
-  :param func:
-    Takes one or more :any:`var` expressions and uses them to construct an expression.
-    If this has more than one argument, the lambda destructures an array argument.
-    (To destructure single-element arrays use :any:`lambda_`.)
-  """
+        query.lambda_query(lambda a: query.add(a, a))
+        # Produces: {
+        #  "lambda": "a",
+        #  "expr": {"add": ({"var": "a"}, {"var": "a"})}
+        # }
+
+    You usually don't need to call this directly as lambdas in queries will be converted for you.
+    For example: ``query.map_(lambda a: query.add(a, 1), collection)``.
+
+    You can also use :any:`lambda_` directly.
+
+    :param func:
+      Takes one or more :any:`var` expressions and uses them to construct an expression.
+      If this has more than one argument, the lambda destructures an array argument.
+      (To destructure single-element arrays use :any:`lambda_`.)
+    """
 
     vars = func.__code__.co_varnames
     n_args = len(vars)
 
     if n_args == 0:
         raise ValueError("Function must take at least 1 argument.")
     elif n_args == 1:
@@ -388,17 +388,17 @@
     return _fn({"key_from_secret": secret})
 
 
 def paginate(
     set, size=None, ts=None, after=None, before=None, events=None, sources=None
 ):
     """
-  See the `docs <https://app.fauna.com/documentation/reference/queryapi#read-functions>`__.
-  You may want to convert the result of this to a :any:`Page`.
-  """
+    See the `docs <https://app.fauna.com/documentation/reference/queryapi#read-functions>`__.
+    You may want to convert the result of this to a :any:`Page`.
+    """
     # pylint: disable=too-many-arguments
     # pylint: disable=redefined-outer-name
     opts = {
         "size": size,
         "ts": ts,
         "after": after,
         "before": before,
@@ -867,16 +867,16 @@
 
 
 _NO_DEFAULT = object()
 
 
 def select(path, from_, default=_NO_DEFAULT):
     """
-  See the `docs <https://docs.fauna.com/fauna/current/api/fql/functions/select>`__.
-  See also :py:func:`select_with_default`."""
+    See the `docs <https://docs.fauna.com/fauna/current/api/fql/functions/select>`__.
+    See also :py:func:`select_with_default`."""
     _dict = {"select": path, "from": from_}
     if default is not _NO_DEFAULT:
         _dict["default"] = default
     return _fn(_dict)
 
 
 @deprecated.deprecated("Use `select` instead")
@@ -1230,16 +1230,16 @@
 # endregion
 
 # region Helpers
 
 
 class Expr(object):
     """
-  Used to mark values that have been wrapped.
-  """
+    Used to mark values that have been wrapped.
+    """
 
     def __init__(self, value):
         self.value = value
 
     def to_fauna_json(self):
         return self.value
 
@@ -1276,15 +1276,19 @@
         if val is not None:
             main_params[key] = val
     return _fn(main_params)
 
 
 def _varargs(values):
     """
-  Called on ``*args`` arguments.
-  This ensures that a single value passed is not put in an array, so
-  ``query.add([1, 2])`` will work as well as ``query.add(1, 2)``.
-  """
+    Called on ``*args`` arguments.
+    This ensures that a single value passed is not put in an array, so
+    ``query.add([1, 2])`` will work as well as ``query.add(1, 2)``.
+    """
     return values[0] if len(values) == 1 else values
 
 
 # endregion
+
+"""
+(c) 2016 Fauna, Inc.
+"""
```

### Comparing `aiofauna-0.0.9/LICENSE` & `aiofauna-0.1.0/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Copyright (c) 2012-2022, Oscar Bahamonde <oscar.bahamonde.dev@gmail.com> and contributors
-
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+Copyright (c) 2012-2023, Oscar Bahamonde <oscar.bahamonde.dev@gmail.com> and contributors
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

