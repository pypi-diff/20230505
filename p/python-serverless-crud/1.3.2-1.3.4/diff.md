# Comparing `tmp/python-serverless-crud-1.3.2.tar.gz` & `tmp/python_serverless_crud-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-serverless-crud-1.3.2.tar", last modified: Mon Oct 17 15:55:10 2022, max compression
+gzip compressed data, was "python_serverless_crud-1.3.4.tar", max compression
```

## Comparing `python-serverless-crud-1.3.2.tar` & `python_serverless_crud-1.3.4.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     1067 2022-10-17 15:54:51.037067 python-serverless-crud-1.3.2/LICENSE
--rw-r--r--   0        0        0     8336 2022-10-17 15:54:51.037067 python-serverless-crud-1.3.2/README.md
--rw-r--r--   0        0        0     1304 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      119 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/__init__.py
--rw-r--r--   0        0        0      182 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/actions/__init__.py
--rw-r--r--   0        0        0     1289 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/actions/base.py
--rw-r--r--   0        0        0     1045 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/actions/create.py
--rw-r--r--   0        0        0     1417 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/actions/delete.py
--rw-r--r--   0        0        0     1223 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/actions/get.py
--rw-r--r--   0        0        0     5432 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/actions/search.py
--rw-r--r--   0        0        0     1583 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/actions/update.py
--rw-r--r--   0        0        0     3950 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/api.py
--rw-r--r--   0        0        0       28 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/appsync/__init__.py
--rw-r--r--   0        0        0     4648 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/appsync/api.py
--rw-r--r--   0        0        0      831 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/appsync/utils.py
--rw-r--r--   0        0        0        0 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/aws/__init__.py
--rw-r--r--   0        0        0     1925 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/aws/iam.py
--rw-r--r--   0        0        0        0 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/builders/__init__.py
--rw-r--r--   0        0        0     5427 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/builders/graphql.py
--rw-r--r--   0        0        0      582 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/dynamodb/__init__.py
--rw-r--r--   0        0        0     2897 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/dynamodb/annotation.py
--rw-r--r--   0        0        0     2749 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/dynamodb/builder.py
--rw-r--r--   0        0        0     1189 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/dynamodb/utils.py
--rw-r--r--   0        0        0     1473 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/exceptions.py
--rw-r--r--   0        0        0       28 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/graphql/__init__.py
--rw-r--r--   0        0        0     4382 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/graphql/api.py
--rw-r--r--   0        0        0       60 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/logger.py
--rw-r--r--   0        0        0     1468 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/model.py
--rw-r--r--   0        0        0       25 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/rest/__init__.py
--rw-r--r--   0        0        0     5150 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/rest/api.py
--rw-r--r--   0        0        0      348 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/rest/http.py
--rw-r--r--   0        0        0      694 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/rest/utils.py
--rw-r--r--   0        0        0     2126 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/service.py
--rw-r--r--   0        0        0     1559 2022-10-17 15:54:51.041067 python-serverless-crud-1.3.2/serverless_crud/utils.py
--rw-r--r--   0        0        0     9733 2022-10-17 15:55:10.711845 python-serverless-crud-1.3.2/setup.py
--rw-r--r--   0        0        0     9425 2022-10-17 15:55:10.712567 python-serverless-crud-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-05 12:42:58.427987 python_serverless_crud-1.3.4/LICENSE
+-rw-r--r--   0        0        0     8336 2023-05-05 12:42:58.427987 python_serverless_crud-1.3.4/README.md
+-rw-r--r--   0        0        0     1304 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/actions/__init__.py
+-rw-r--r--   0        0        0     1289 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/actions/base.py
+-rw-r--r--   0        0        0     1045 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/actions/create.py
+-rw-r--r--   0        0        0     1417 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/actions/delete.py
+-rw-r--r--   0        0        0     1223 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/actions/get.py
+-rw-r--r--   0        0        0     6004 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/actions/search.py
+-rw-r--r--   0        0        0     1583 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/actions/update.py
+-rw-r--r--   0        0        0     3950 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/api.py
+-rw-r--r--   0        0        0       28 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/appsync/__init__.py
+-rw-r--r--   0        0        0     4648 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/appsync/api.py
+-rw-r--r--   0        0        0      831 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/appsync/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/aws/__init__.py
+-rw-r--r--   0        0        0     1925 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/aws/iam.py
+-rw-r--r--   0        0        0        0 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/builders/__init__.py
+-rw-r--r--   0        0        0     5427 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/builders/graphql.py
+-rw-r--r--   0        0        0      582 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/dynamodb/__init__.py
+-rw-r--r--   0        0        0     2897 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/dynamodb/annotation.py
+-rw-r--r--   0        0        0     2749 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/dynamodb/builder.py
+-rw-r--r--   0        0        0     1189 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/dynamodb/utils.py
+-rw-r--r--   0        0        0     1473 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/exceptions.py
+-rw-r--r--   0        0        0       28 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/graphql/__init__.py
+-rw-r--r--   0        0        0     4382 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/graphql/api.py
+-rw-r--r--   0        0        0       60 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/logger.py
+-rw-r--r--   0        0        0     1468 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/model.py
+-rw-r--r--   0        0        0       25 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/rest/__init__.py
+-rw-r--r--   0        0        0     5150 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/rest/api.py
+-rw-r--r--   0        0        0      348 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/rest/http.py
+-rw-r--r--   0        0        0      694 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/rest/utils.py
+-rw-r--r--   0        0        0     2126 2023-05-05 12:42:58.431988 python_serverless_crud-1.3.4/serverless_crud/service.py
+-rw-r--r--   0        0        0     1559 2023-05-05 12:42:58.439988 python_serverless_crud-1.3.4/serverless_crud/utils.py
+-rw-r--r--   0        0        0     9676 1970-01-01 00:00:00.000000 python_serverless_crud-1.3.4/PKG-INFO
```

### Comparing `python-serverless-crud-1.3.2/LICENSE` & `python_serverless_crud-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/README.md` & `python_serverless_crud-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/pyproject.toml` & `python_serverless_crud-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-serverless-crud"
-version = "1.3.2"
+version = "1.3.4"
 description="Simple and powerful tool for quick serverless data management via API. "
 keywords = ["library", "serverless"]
 authors = ["Epsy <engineering@epsyhealth.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/epsylabs/python-serverless-crud"
 repository = "https://github.com/epsylabs/python-serverless-crud"
```

### Comparing `python-serverless-crud-1.3.2/serverless_crud/actions/base.py` & `python_serverless_crud-1.3.4/serverless_crud/actions/base.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/actions/create.py` & `python_serverless_crud-1.3.4/serverless_crud/actions/create.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/actions/delete.py` & `python_serverless_crud-1.3.4/serverless_crud/actions/delete.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/actions/get.py` & `python_serverless_crud-1.3.4/serverless_crud/actions/get.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/actions/search.py` & `python_serverless_crud-1.3.4/serverless_crud/actions/search.py`

 * *Files 20% similar despite different names*

```diff
@@ -49,39 +49,59 @@
         query["ExpressionAttributeValues"] = attributes
 
         names = query.get("ExpressionAttributeNames", {})
         names.update({f"#{self.model._meta.owner_field}": self.model._meta.owner_field})
         query["ExpressionAttributeNames"] = names
 
     @abc.abstractmethod
-    def _fetch_items(self, event: Union[BaseProxyEvent, AppSyncResolverEvent], dynamodb, table, index):
+    def _fetch_items(
+        self, event: Union[BaseProxyEvent, AppSyncResolverEvent], dynamodb, table, index, next_token=None, limit=100
+    ):
         pass
 
     def _extract_fields(self, expression):
         regex = r"#[\w\d]+"
         matches = re.findall(regex, expression)
 
         return {m: m.strip("#") for m in matches}
 
     @with_dynamodb
-    def handle(self, event: APIGatewayProxyEvent, context, dynamodb, table, index_name=None, *args, **kwargs):
+    def handle(
+        self,
+        event: APIGatewayProxyEvent,
+        context,
+        dynamodb,
+        table,
+        index_name=None,
+        next_token=None,
+        limit=100,
+        *args,
+        **kwargs,
+    ):
         try:
             index = self.model._meta.get_index(index_name)
-            response = self._fetch_items(event, dynamodb, table, index)
+            response = self._fetch_items(
+                event, dynamodb, table, index, next_token=kwargs.get("nextToken", next_token), limit=limit
+            )
 
             return response, dict(
                 items=[self.model(**i).dict() for i in response["Items"]], nextToken=response.get("LastEvaluatedKey")
             )
         except ValidationError as e:
             raise ValidationException(e)
 
 
 class ScanAction(SearchAction):
-    def _fetch_items(self, event: Union[BaseProxyEvent, AppSyncResolverEvent], dynamodb, table, index, _next=None):
-        query = {**dict(Limit=100), **self._get_query_target(table, index)}
+    def _fetch_items(
+        self, event: Union[BaseProxyEvent, AppSyncResolverEvent], dynamodb, table, index, next_token=None, limit=100
+    ):
+        query = {**dict(Limit=limit), **self._get_query_target(table, index)}
+
+        if next_token:
+            query["ExclusiveStartKey"] = next_token
 
         if isinstance(event, BaseProxyEvent):
             payload = ScanPayload(**event.json_body)
             if payload.expression:
                 query.update(
                     dict(
                         FilterExpression=payload.expression,
@@ -95,29 +115,34 @@
 
         logger.debug("dynamodb.scan", extra=query)
 
         return table.scan(**query)
 
 
 class QueryAction(SearchAction):
-    def _fetch_items(self, event: Union[BaseProxyEvent, AppSyncResolverEvent], dynamodb, table, index, _next=None):
+    def _fetch_items(
+        self, event: Union[BaseProxyEvent, AppSyncResolverEvent], dynamodb, table, index, next_token=None, limit=100
+    ):
         payload = QueryPayload(**event.json_body)
 
         expression = str(payload.filter_expression) + " " + str(payload.key_expression)
 
         query = {
-            **dict(Limit=100),
+            **dict(Limit=limit),
             **dict(
                 KeyConditionExpression=payload.key_expression,
                 ExpressionAttributeNames=self._extract_fields(expression),
                 ExpressionAttributeValues=payload.values,
             ),
             **self._get_query_target(table, index),
         }
 
+        if next_token:
+            query["ExclusiveStartKey"] = next_token
+
         if payload.filter_expression:
             query["FilterExpression"] = payload.filter_expression
 
         if payload.checkOwner:
             self._add_owner_condition(query, event, "FilterExpression")
 
         logger.debug("dynamodb.query", extra=query)
@@ -133,17 +158,22 @@
         is_owner_part_of_index = index and index.fields.get(owner_field) == KeyFieldTypes.HASH
 
         if not (is_owner_field_pk or is_owner_part_of_index):
             raise InvalidPayloadException(
                 "You can only use list method only on tables or indexes with record owner for partition key"
             )
 
-    def _fetch_items(self, event: Union[BaseProxyEvent, AppSyncResolverEvent], dynamodb, table, index, _next=None):
+    def _fetch_items(
+        self, event: Union[BaseProxyEvent, AppSyncResolverEvent], dynamodb, table, index, next_token=None, limit=100
+    ):
         self.validate(index)
 
-        query = {**dict(Limit=100), **self._get_query_target(table, index)}
+        query = {**dict(Limit=limit), **self._get_query_target(table, index)}
+
+        if next_token:
+            query["ExclusiveStartKey"] = next_token
 
         self._add_owner_condition(query, event)
 
         logger.debug("dynamodb.query", extra=query)
 
         return table.query(**query)
```

### Comparing `python-serverless-crud-1.3.2/serverless_crud/actions/update.py` & `python_serverless_crud-1.3.4/serverless_crud/actions/update.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/api.py` & `python_serverless_crud-1.3.4/serverless_crud/api.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/appsync/api.py` & `python_serverless_crud-1.3.4/serverless_crud/appsync/api.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/appsync/utils.py` & `python_serverless_crud-1.3.4/serverless_crud/appsync/utils.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/aws/iam.py` & `python_serverless_crud-1.3.4/serverless_crud/aws/iam.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/builders/graphql.py` & `python_serverless_crud-1.3.4/serverless_crud/builders/graphql.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/dynamodb/__init__.py` & `python_serverless_crud-1.3.4/serverless_crud/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/dynamodb/annotation.py` & `python_serverless_crud-1.3.4/serverless_crud/dynamodb/annotation.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/dynamodb/builder.py` & `python_serverless_crud-1.3.4/serverless_crud/dynamodb/builder.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/dynamodb/utils.py` & `python_serverless_crud-1.3.4/serverless_crud/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/exceptions.py` & `python_serverless_crud-1.3.4/serverless_crud/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/graphql/api.py` & `python_serverless_crud-1.3.4/serverless_crud/graphql/api.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/model.py` & `python_serverless_crud-1.3.4/serverless_crud/model.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/rest/api.py` & `python_serverless_crud-1.3.4/serverless_crud/rest/api.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/rest/utils.py` & `python_serverless_crud-1.3.4/serverless_crud/rest/utils.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/service.py` & `python_serverless_crud-1.3.4/serverless_crud/service.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/serverless_crud/utils.py` & `python_serverless_crud-1.3.4/serverless_crud/utils.py`

 * *Files identical despite different names*

### Comparing `python-serverless-crud-1.3.2/setup.py` & `python_serverless_crud-1.3.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,264 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: python-serverless-crud
+Version: 1.3.4
+Summary: Simple and powerful tool for quick serverless data management via API. 
+Home-page: https://github.com/epsylabs/python-serverless-crud
+License: MIT
+Keywords: library,serverless
+Author: Epsy
+Author-email: engineering@epsyhealth.com
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Provides-Extra: sentry
+Requires-Dist: PyJWT (>=2.4,<3.0)
+Requires-Dist: aws-lambda-powertools[pydantic] (>=1.24,<2.0)
+Requires-Dist: graphene (>=3.0,<4.0)
+Requires-Dist: graphene-pydantic (>=0.3.0,<0.4.0)
+Requires-Dist: inflect (>=5.3.0,<6.0.0)
+Requires-Dist: sentry-sdk (>=1.5,<2.0) ; extra == "sentry"
+Requires-Dist: stringcase (>=1.2.0,<2.0.0)
+Project-URL: Repository, https://github.com/epsylabs/python-serverless-crud
+Description-Content-Type: text/markdown
 
-packages = \
-['serverless_crud',
- 'serverless_crud.actions',
- 'serverless_crud.appsync',
- 'serverless_crud.aws',
- 'serverless_crud.builders',
- 'serverless_crud.dynamodb',
- 'serverless_crud.graphql',
- 'serverless_crud.rest']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyJWT>=2.4,<3.0',
- 'aws-lambda-powertools[pydantic]>=1.24,<2.0',
- 'graphene-pydantic>=0.3.0,<0.4.0',
- 'graphene>=3.0,<4.0',
- 'inflect>=5.3.0,<6.0.0',
- 'stringcase>=1.2.0,<2.0.0']
-
-extras_require = \
-{'sentry': ['sentry-sdk>=1.5,<2.0']}
-
-setup_kwargs = {
-    'name': 'python-serverless-crud',
-    'version': '1.3.2',
-    'description': 'Simple and powerful tool for quick serverless data management via API. ',
-    'long_description': '# python-serverless-crud\n\n## The idea \n\nSimple and powerful tool for quick serverless data management via API. \n\n## Key concepts\n\n- Don\'t Repeat Yourself - easy model definition with schema and cloud formation generation support\n- Best practices applied by default (created with AWS LambdaPower Tools)\n- Flexibility - enable, extend and modify what is needed\n- One ring to rule them all - support for REST API, GraphQL (via API Gateway), AppSync GraphQL (direct resolvers)\n\n\n## Features\n\n- Full CRUD support with validation\n- Native support for DynamoDB (including CloudFormation creation via troposphere)\n  - GlobalSecondaryIndex support\n  - LocalSecondaryIndex support\n  - Primary Key with and without sort keys\n- Support for Scan, Query operations on the tables and indexes\n- Virtual List method on the table or index\n- Integrated record owner feature with KeyCondition and FilterCondition support (auto-detect)\n\n# Documentation\n\n## Sample service\n\n```python\nfrom aws_lambda_powertools import Tracer\nfrom aws_lambda_powertools.logging import correlation_paths\nfrom serverless_crud import api\nfrom serverless_crud.dynamodb import annotation as db\nfrom serverless_crud.model import BaseModel\nfrom serverless_crud.logger import logger\n\ntracer = Tracer()\n\n\n@db.Model(\n    key=db.PrimaryKey(id=db.KeyFieldTypes.HASH),\n    indexes=(\n            db.GlobalSecondaryIndex("by_user", user=db.KeyFieldTypes.HASH, created=db.KeyFieldTypes.RANGE),\n    ),\n    owner_field="user"\n)\nclass Device(BaseModel):\n    id: str\n    created: int\n    user: str = None\n\n\napi.rest.registry(Device, alias="device")\n\n\n@logger.inject_lambda_context(correlation_id_path=correlation_paths.API_GATEWAY_REST)\n@tracer.capture_lambda_handler\ndef rest_handler(event, context):\n    return api.rest.handle(event, context)\n```\n\nWith just a few lines of the code we are able to create `Device` model service which then can be extended. \nIn this example we:\n\n1. Defined our `Device` model with some extra metadata, used by our generators. That includes:\n   1. Table key definition\n   2. GlobalSecondaryIndex\n   3. Definition of the field which will hold `owner` of the record (identity provided by cognito)\n2. Registered our `Device` model into rest API under `device` alias\n3. Created rest handler which then can be referred in our `serverless.yml` file \n\nA few notes here:\n- we need to define `rest_handler` function if we would like to use it as a target for local execution with serverless freamework\n- Lambda Power Tools are build around functions and they don\'t work properly with object methods\n- We use one function per API type, and we relay on internal router provided by each API implementation \n\n### Serverless integration\n\nIf you use (serverless-builder)[https://github.com/epsyhealth/serverless-builder] you can create your `serverless.yml` with just a few lines of code (including DynamodbTables)\n\n```python\nfrom serverless import Service, Configuration\nfrom serverless.aws.features import XRay\nfrom serverless.aws.functions.http import HTTPFunction\nfrom serverless.plugins import PythonRequirements, Prune\nfrom serverless.provider import AWSProvider\nfrom troposphere import dynamodb\n\nfrom timemachine_api.handlers import api\n\nservice = Service(\n    "timemachine-api",\n    "Collect events in chronological order",\n    AWSProvider(),\n    config=Configuration(\n        domain="epsy.app"\n    )\n)\nservice.provider.timeout = 5\n\nservice.plugins.add(Prune())\nservice.plugins.add(PythonRequirements(layer=False, useStaticCache=False, dockerSsh=True))\n\nservice.enable(XRay())\n\nfor name, table_specification in api.dynamodb_table_specifications().items():\n    service.resources.add(dynamodb.Table(name, **table_specification))\n\nauthorizer = dict(name="auth",\n                  arn="arn:aws:cognito-idp:us-east-1:772962929486:userpool/us-east-1_FCl7gKtHC")\n\nservice.builder.function.http("rest", "Time machine REST API", "/rest/{proxy+}", HTTPFunction.ANY,\n                              handler="timemachine_api.handlers.rest_handler", authorizer=authorizer)\n\n\nservice.render()\n```\n\n## Internals\n\n### Annotations\n\n`serverless-crud` project provides one annotation which must be used for all managed models.\n\n```python\nfrom serverless_crud.dynamodb import annotation as db\n@db.Model(\n    key=db.PrimaryKey(name=db.KeyFieldTypes.HASH),\n    indexes=(\n        db.GlobalSecondaryIndex(...),\n        db.LocalSecondaryIndex(...)\n    ),\n    owner_field="field"\n)\n```\n\nModel annotation accepts:\n- `key` - primary key definition, in form of `kwargs` where name of parameter would be a field name which should \n be used  in key, and value should be a value of `KeyFieldTypes` enum\n- `indexes` - list of indexes GlobalSecondaryIndex|LocalSecondaryIndex. Indexes are defined in same way as primary key\n- `owner_field` - name of the field which should be used for data filtering (based on the cognito identity)\n\n\n### Data owner \n\n`serverless-crud` can enforce some base data filtering on all kind of operations using Dynamodb conditional operations. \nIf you would like to use this feature you must set `owner_field` on each model you would like to use this feature.\n\nLibrary will use this field for:\n- setting its value on model creation / update (it will overwrite any value provided by user)\n- as an extra `ConditionExpression` during `GET` and `DELETE` operations\n- as a part of either `FilterExpression` or `KeyExpression` for Scan, Query and List operations\n\n\n### Model registration\n\nTo be able to manage given model, you must first register it with specific API. \nThis can be done with a single line of code:\n\n```python\napi.rest.registry(Device, alias="device")\n```\n\nYou need to provide only a model type to `registry` method, all other parameters are optional. \nIf you like, you can omit `alias` parameter, in that case framework will use model class name.\n\n### Customizing endpoint behaviour\n\nFramework defines a set of classes located in `serverless_crud.actions`:\n- CreateAction\n- DeleteAction\n- GetAction\n- ScanAction, ListAction, QueryAction\n- UpdateAction\n\nall those classes are subclasses of `serverless_crud.actions.base.Action` class and can be extended if needed. \n\nYou may need to execute custom logic after object creation, that can be done with custom `CreateAction` subclass\n```python\n\nfrom serverless_crud.actions import CreateAction\n\nclass CreateDeviceAction(CreateAction):\n    def handle(self, event: APIGatewayProxyEvent, context):\n        super().handle(event, context)\n        \n        # custom logic\n\n\napi.rest.registry(Device, create=CreateDeviceAction)\n```\n\nYou can set custom handlers for each supported operation:\n\n```python\ndef registry(self, model, alias=None, get=GetAction, create=CreateAction, update=UpdateAction, delete=DeleteAction,\n             lookup_list=ListAction, lookup_scan=ScanAction, lookup_query=QueryAction):\n```\n\nAs you can see, all actions are defined by default. That also means that all actions are enabled by default, but\neach action can be disabled.\n\nIf you need to disable action you need to set action handler to `None`, that will prevent framework from creating\nroute for given action, and it will disable whole logic behind it. \n\n### Routes\n\nREST API specific feature. \n\nFramework will create multiple routes for each register model, using `alias` as a URL namespace. \nGenerated routes: \n\n- GET /rest/{alias}/{pk} - fetch object by PK (see notes about PK below)\n- POST /rest/{alias} - create new record\n- PUT /rest/{alias}/{pk} - update record with given PK \n- DELETE /rest/{alias}/{pk} - delete record with given PK \n- GET /rest/lookup/{alias}/list - list all the records of given type using Query on the table\n- GET /rest/lookup/{alias}/list/{index_name} - list all the records of the given type using Query on specific index\n- POST /rest/lookup/{alias}/query - perform a query on given table\n- POST /rest/lookup/{alias}/query/{index_name} - perform a query on given index\n- POST /rest/lookup/{alias}/scan - perform a scan on given table\n- POST /rest/lookup/{alias}/scan/{index_name} - perform a scan on given index\n\n#### Primary Keys\n> *Please remember that with DynamoDB key is a Partition Key with optional Sort Key. \nIn case you define Sort Key DynamoDB will require a value for it while getting / deleting key.\nIn that case framework will modify routes to include sort key as an extra path parameter* \n\n\n## Endpoints\n',
-    'author': 'Epsy',
-    'author_email': 'engineering@epsyhealth.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/epsylabs/python-serverless-crud',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
+# python-serverless-crud
 
+## The idea 
+
+Simple and powerful tool for quick serverless data management via API. 
+
+## Key concepts
+
+- Don't Repeat Yourself - easy model definition with schema and cloud formation generation support
+- Best practices applied by default (created with AWS LambdaPower Tools)
+- Flexibility - enable, extend and modify what is needed
+- One ring to rule them all - support for REST API, GraphQL (via API Gateway), AppSync GraphQL (direct resolvers)
+
+
+## Features
+
+- Full CRUD support with validation
+- Native support for DynamoDB (including CloudFormation creation via troposphere)
+  - GlobalSecondaryIndex support
+  - LocalSecondaryIndex support
+  - Primary Key with and without sort keys
+- Support for Scan, Query operations on the tables and indexes
+- Virtual List method on the table or index
+- Integrated record owner feature with KeyCondition and FilterCondition support (auto-detect)
+
+# Documentation
+
+## Sample service
+
+```python
+from aws_lambda_powertools import Tracer
+from aws_lambda_powertools.logging import correlation_paths
+from serverless_crud import api
+from serverless_crud.dynamodb import annotation as db
+from serverless_crud.model import BaseModel
+from serverless_crud.logger import logger
+
+tracer = Tracer()
+
+
+@db.Model(
+    key=db.PrimaryKey(id=db.KeyFieldTypes.HASH),
+    indexes=(
+            db.GlobalSecondaryIndex("by_user", user=db.KeyFieldTypes.HASH, created=db.KeyFieldTypes.RANGE),
+    ),
+    owner_field="user"
+)
+class Device(BaseModel):
+    id: str
+    created: int
+    user: str = None
+
+
+api.rest.registry(Device, alias="device")
+
+
+@logger.inject_lambda_context(correlation_id_path=correlation_paths.API_GATEWAY_REST)
+@tracer.capture_lambda_handler
+def rest_handler(event, context):
+    return api.rest.handle(event, context)
+```
+
+With just a few lines of the code we are able to create `Device` model service which then can be extended. 
+In this example we:
+
+1. Defined our `Device` model with some extra metadata, used by our generators. That includes:
+   1. Table key definition
+   2. GlobalSecondaryIndex
+   3. Definition of the field which will hold `owner` of the record (identity provided by cognito)
+2. Registered our `Device` model into rest API under `device` alias
+3. Created rest handler which then can be referred in our `serverless.yml` file 
+
+A few notes here:
+- we need to define `rest_handler` function if we would like to use it as a target for local execution with serverless freamework
+- Lambda Power Tools are build around functions and they don't work properly with object methods
+- We use one function per API type, and we relay on internal router provided by each API implementation 
+
+### Serverless integration
+
+If you use (serverless-builder)[https://github.com/epsyhealth/serverless-builder] you can create your `serverless.yml` with just a few lines of code (including DynamodbTables)
+
+```python
+from serverless import Service, Configuration
+from serverless.aws.features import XRay
+from serverless.aws.functions.http import HTTPFunction
+from serverless.plugins import PythonRequirements, Prune
+from serverless.provider import AWSProvider
+from troposphere import dynamodb
+
+from timemachine_api.handlers import api
+
+service = Service(
+    "timemachine-api",
+    "Collect events in chronological order",
+    AWSProvider(),
+    config=Configuration(
+        domain="epsy.app"
+    )
+)
+service.provider.timeout = 5
+
+service.plugins.add(Prune())
+service.plugins.add(PythonRequirements(layer=False, useStaticCache=False, dockerSsh=True))
+
+service.enable(XRay())
+
+for name, table_specification in api.dynamodb_table_specifications().items():
+    service.resources.add(dynamodb.Table(name, **table_specification))
+
+authorizer = dict(name="auth",
+                  arn="arn:aws:cognito-idp:us-east-1:772962929486:userpool/us-east-1_FCl7gKtHC")
+
+service.builder.function.http("rest", "Time machine REST API", "/rest/{proxy+}", HTTPFunction.ANY,
+                              handler="timemachine_api.handlers.rest_handler", authorizer=authorizer)
+
+
+service.render()
+```
+
+## Internals
+
+### Annotations
+
+`serverless-crud` project provides one annotation which must be used for all managed models.
+
+```python
+from serverless_crud.dynamodb import annotation as db
+@db.Model(
+    key=db.PrimaryKey(name=db.KeyFieldTypes.HASH),
+    indexes=(
+        db.GlobalSecondaryIndex(...),
+        db.LocalSecondaryIndex(...)
+    ),
+    owner_field="field"
+)
+```
+
+Model annotation accepts:
+- `key` - primary key definition, in form of `kwargs` where name of parameter would be a field name which should 
+ be used  in key, and value should be a value of `KeyFieldTypes` enum
+- `indexes` - list of indexes GlobalSecondaryIndex|LocalSecondaryIndex. Indexes are defined in same way as primary key
+- `owner_field` - name of the field which should be used for data filtering (based on the cognito identity)
+
+
+### Data owner 
+
+`serverless-crud` can enforce some base data filtering on all kind of operations using Dynamodb conditional operations. 
+If you would like to use this feature you must set `owner_field` on each model you would like to use this feature.
+
+Library will use this field for:
+- setting its value on model creation / update (it will overwrite any value provided by user)
+- as an extra `ConditionExpression` during `GET` and `DELETE` operations
+- as a part of either `FilterExpression` or `KeyExpression` for Scan, Query and List operations
+
+
+### Model registration
+
+To be able to manage given model, you must first register it with specific API. 
+This can be done with a single line of code:
+
+```python
+api.rest.registry(Device, alias="device")
+```
+
+You need to provide only a model type to `registry` method, all other parameters are optional. 
+If you like, you can omit `alias` parameter, in that case framework will use model class name.
+
+### Customizing endpoint behaviour
+
+Framework defines a set of classes located in `serverless_crud.actions`:
+- CreateAction
+- DeleteAction
+- GetAction
+- ScanAction, ListAction, QueryAction
+- UpdateAction
+
+all those classes are subclasses of `serverless_crud.actions.base.Action` class and can be extended if needed. 
+
+You may need to execute custom logic after object creation, that can be done with custom `CreateAction` subclass
+```python
+
+from serverless_crud.actions import CreateAction
+
+class CreateDeviceAction(CreateAction):
+    def handle(self, event: APIGatewayProxyEvent, context):
+        super().handle(event, context)
+        
+        # custom logic
+
+
+api.rest.registry(Device, create=CreateDeviceAction)
+```
+
+You can set custom handlers for each supported operation:
+
+```python
+def registry(self, model, alias=None, get=GetAction, create=CreateAction, update=UpdateAction, delete=DeleteAction,
+             lookup_list=ListAction, lookup_scan=ScanAction, lookup_query=QueryAction):
+```
+
+As you can see, all actions are defined by default. That also means that all actions are enabled by default, but
+each action can be disabled.
+
+If you need to disable action you need to set action handler to `None`, that will prevent framework from creating
+route for given action, and it will disable whole logic behind it. 
+
+### Routes
+
+REST API specific feature. 
+
+Framework will create multiple routes for each register model, using `alias` as a URL namespace. 
+Generated routes: 
+
+- GET /rest/{alias}/{pk} - fetch object by PK (see notes about PK below)
+- POST /rest/{alias} - create new record
+- PUT /rest/{alias}/{pk} - update record with given PK 
+- DELETE /rest/{alias}/{pk} - delete record with given PK 
+- GET /rest/lookup/{alias}/list - list all the records of given type using Query on the table
+- GET /rest/lookup/{alias}/list/{index_name} - list all the records of the given type using Query on specific index
+- POST /rest/lookup/{alias}/query - perform a query on given table
+- POST /rest/lookup/{alias}/query/{index_name} - perform a query on given index
+- POST /rest/lookup/{alias}/scan - perform a scan on given table
+- POST /rest/lookup/{alias}/scan/{index_name} - perform a scan on given index
+
+#### Primary Keys
+> *Please remember that with DynamoDB key is a Partition Key with optional Sort Key. 
+In case you define Sort Key DynamoDB will require a value for it while getting / deleting key.
+In that case framework will modify routes to include sort key as an extra path parameter* 
+
+
+## Endpoints
 
-setup(**setup_kwargs)
```

