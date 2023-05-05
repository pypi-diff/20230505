# Comparing `tmp/alibabacloud_documentautoml20221229-1.0.8.tar.gz` & `tmp/alibabacloud_documentautoml20221229-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_documentautoml20221229-1.0.8.tar", last modified: Mon Apr 10 07:44:31 2023, max compression
+gzip compressed data, was "dist/alibabacloud_documentautoml20221229-1.0.9.tar", last modified: Mon Apr 10 11:23:16 2023, max compression
```

## Comparing `alibabacloud_documentautoml20221229-1.0.8.tar` & `alibabacloud_documentautoml20221229-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      344 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18171 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/client.py
--rw-r--r--   0 root         (0) root         (0)    20554 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2665 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19227 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229/client.py
+-rw-r--r--   0 root         (0) root         (0)    20554 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-04-10 11:23:16.000000 alibabacloud_documentautoml20221229-1.0.9/setup.py
```

### Comparing `alibabacloud_documentautoml20221229-1.0.8/LICENSE` & `alibabacloud_documentautoml20221229-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229-1.0.8/PKG-INFO` & `alibabacloud_documentautoml20221229-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_documentautoml20221229
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud documentAutoml (20221229) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_documentautoml20221229-1.0.8/README-CN.md` & `alibabacloud_documentautoml20221229-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229-1.0.8/README.md` & `alibabacloud_documentautoml20221229-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/client.py` & `alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,17 +56,20 @@
             query['ModelId'] = request.model_id
         if not UtilClient.is_unset(request.model_version):
             query['ModelVersion'] = request.model_version
         if not UtilClient.is_unset(request.service_name):
             query['ServiceName'] = request.service_name
         if not UtilClient.is_unset(request.service_version):
             query['ServiceVersion'] = request.service_version
+        body = {}
+        if not UtilClient.is_unset(request.body):
+            body['Body'] = request.body
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=request.body
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateModelAsyncPredict',
             version='2022-12-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -95,17 +98,20 @@
             query['ModelId'] = request.model_id
         if not UtilClient.is_unset(request.model_version):
             query['ModelVersion'] = request.model_version
         if not UtilClient.is_unset(request.service_name):
             query['ServiceName'] = request.service_name
         if not UtilClient.is_unset(request.service_version):
             query['ServiceVersion'] = request.service_version
+        body = {}
+        if not UtilClient.is_unset(request.body):
+            body['Body'] = request.body
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=request.body
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateModelAsyncPredict',
             version='2022-12-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -212,17 +218,20 @@
         query = {}
         if not UtilClient.is_unset(request.auto_prediction):
             query['AutoPrediction'] = request.auto_prediction
         if not UtilClient.is_unset(request.classifier_id):
             query['ClassifierId'] = request.classifier_id
         if not UtilClient.is_unset(request.content):
             query['Content'] = request.content
+        body = {}
+        if not UtilClient.is_unset(request.body):
+            body['Body'] = request.body
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=request.body
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PredictClassifierModel',
             version='2022-12-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -245,17 +254,20 @@
         query = {}
         if not UtilClient.is_unset(request.auto_prediction):
             query['AutoPrediction'] = request.auto_prediction
         if not UtilClient.is_unset(request.classifier_id):
             query['ClassifierId'] = request.classifier_id
         if not UtilClient.is_unset(request.content):
             query['Content'] = request.content
+        body = {}
+        if not UtilClient.is_unset(request.body):
+            body['Body'] = request.body
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=request.body
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PredictClassifierModel',
             version='2022-12-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -294,17 +306,20 @@
             query['BinaryToText'] = request.binary_to_text
         if not UtilClient.is_unset(request.content):
             query['Content'] = request.content
         if not UtilClient.is_unset(request.model_id):
             query['ModelId'] = request.model_id
         if not UtilClient.is_unset(request.model_version):
             query['ModelVersion'] = request.model_version
+        body = {}
+        if not UtilClient.is_unset(request.body):
+            body['Body'] = request.body
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=request.body
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PredictModel',
             version='2022-12-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -329,17 +344,20 @@
             query['BinaryToText'] = request.binary_to_text
         if not UtilClient.is_unset(request.content):
             query['Content'] = request.content
         if not UtilClient.is_unset(request.model_id):
             query['ModelId'] = request.model_id
         if not UtilClient.is_unset(request.model_version):
             query['ModelVersion'] = request.model_version
+        body = {}
+        if not UtilClient.is_unset(request.body):
+            body['Body'] = request.body
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=request.body
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PredictModel',
             version='2022-12-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -376,17 +394,20 @@
         query = {}
         if not UtilClient.is_unset(request.binary_to_text):
             query['BinaryToText'] = request.binary_to_text
         if not UtilClient.is_unset(request.content):
             query['Content'] = request.content
         if not UtilClient.is_unset(request.task_id):
             query['TaskId'] = request.task_id
+        body = {}
+        if not UtilClient.is_unset(request.body):
+            body['Body'] = request.body
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=request.body
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PredictTemplateModel',
             version='2022-12-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -409,17 +430,20 @@
         query = {}
         if not UtilClient.is_unset(request.binary_to_text):
             query['BinaryToText'] = request.binary_to_text
         if not UtilClient.is_unset(request.content):
             query['Content'] = request.content
         if not UtilClient.is_unset(request.task_id):
             query['TaskId'] = request.task_id
+        body = {}
+        if not UtilClient.is_unset(request.body):
+            body['Body'] = request.body
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=request.body
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PredictTemplateModel',
             version='2022-12-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
```

### Comparing `alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/models.py` & `alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,70 +4,70 @@
 from typing import Dict, Any
 
 
 class CreateModelAsyncPredictRequest(TeaModel):
     def __init__(
         self,
         binary_to_text: bool = None,
+        body: str = None,
         content: str = None,
         model_id: int = None,
         model_version: str = None,
         service_name: str = None,
         service_version: str = None,
-        body: str = None,
     ):
         self.binary_to_text = binary_to_text
+        self.body = body
         self.content = content
         self.model_id = model_id
         self.model_version = model_version
         self.service_name = service_name
         self.service_version = service_version
-        self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.binary_to_text is not None:
             result['BinaryToText'] = self.binary_to_text
+        if self.body is not None:
+            result['Body'] = self.body
         if self.content is not None:
             result['Content'] = self.content
         if self.model_id is not None:
             result['ModelId'] = self.model_id
         if self.model_version is not None:
             result['ModelVersion'] = self.model_version
         if self.service_name is not None:
             result['ServiceName'] = self.service_name
         if self.service_version is not None:
             result['ServiceVersion'] = self.service_version
-        if self.body is not None:
-            result['body'] = self.body
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BinaryToText') is not None:
             self.binary_to_text = m.get('BinaryToText')
+        if m.get('Body') is not None:
+            self.body = m.get('Body')
         if m.get('Content') is not None:
             self.content = m.get('Content')
         if m.get('ModelId') is not None:
             self.model_id = m.get('ModelId')
         if m.get('ModelVersion') is not None:
             self.model_version = m.get('ModelVersion')
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
         if m.get('ServiceVersion') is not None:
             self.service_version = m.get('ServiceVersion')
-        if m.get('body') is not None:
-            self.body = m.get('body')
         return self
 
 
 class CreateModelAsyncPredictResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -274,52 +274,52 @@
         return self
 
 
 class PredictClassifierModelRequest(TeaModel):
     def __init__(
         self,
         auto_prediction: bool = None,
+        body: str = None,
         classifier_id: int = None,
         content: str = None,
-        body: str = None,
     ):
         self.auto_prediction = auto_prediction
+        self.body = body
         self.classifier_id = classifier_id
         self.content = content
-        self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auto_prediction is not None:
             result['AutoPrediction'] = self.auto_prediction
+        if self.body is not None:
+            result['Body'] = self.body
         if self.classifier_id is not None:
             result['ClassifierId'] = self.classifier_id
         if self.content is not None:
             result['Content'] = self.content
-        if self.body is not None:
-            result['body'] = self.body
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AutoPrediction') is not None:
             self.auto_prediction = m.get('AutoPrediction')
+        if m.get('Body') is not None:
+            self.body = m.get('Body')
         if m.get('ClassifierId') is not None:
             self.classifier_id = m.get('ClassifierId')
         if m.get('Content') is not None:
             self.content = m.get('Content')
-        if m.get('body') is not None:
-            self.body = m.get('body')
         return self
 
 
 class PredictClassifierModelResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -409,58 +409,58 @@
         return self
 
 
 class PredictModelRequest(TeaModel):
     def __init__(
         self,
         binary_to_text: bool = None,
+        body: str = None,
         content: str = None,
         model_id: int = None,
         model_version: str = None,
-        body: str = None,
     ):
         self.binary_to_text = binary_to_text
+        self.body = body
         self.content = content
         self.model_id = model_id
         self.model_version = model_version
-        self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.binary_to_text is not None:
             result['BinaryToText'] = self.binary_to_text
+        if self.body is not None:
+            result['Body'] = self.body
         if self.content is not None:
             result['Content'] = self.content
         if self.model_id is not None:
             result['ModelId'] = self.model_id
         if self.model_version is not None:
             result['ModelVersion'] = self.model_version
-        if self.body is not None:
-            result['body'] = self.body
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BinaryToText') is not None:
             self.binary_to_text = m.get('BinaryToText')
+        if m.get('Body') is not None:
+            self.body = m.get('Body')
         if m.get('Content') is not None:
             self.content = m.get('Content')
         if m.get('ModelId') is not None:
             self.model_id = m.get('ModelId')
         if m.get('ModelVersion') is not None:
             self.model_version = m.get('ModelVersion')
-        if m.get('body') is not None:
-            self.body = m.get('body')
         return self
 
 
 class PredictModelResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -550,52 +550,52 @@
         return self
 
 
 class PredictTemplateModelRequest(TeaModel):
     def __init__(
         self,
         binary_to_text: bool = None,
+        body: str = None,
         content: str = None,
         task_id: int = None,
-        body: str = None,
     ):
         self.binary_to_text = binary_to_text
+        self.body = body
         self.content = content
         self.task_id = task_id
-        self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.binary_to_text is not None:
             result['BinaryToText'] = self.binary_to_text
+        if self.body is not None:
+            result['Body'] = self.body
         if self.content is not None:
             result['Content'] = self.content
         if self.task_id is not None:
             result['TaskId'] = self.task_id
-        if self.body is not None:
-            result['body'] = self.body
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BinaryToText') is not None:
             self.binary_to_text = m.get('BinaryToText')
+        if m.get('Body') is not None:
+            self.body = m.get('Body')
         if m.get('Content') is not None:
             self.content = m.get('Content')
         if m.get('TaskId') is not None:
             self.task_id = m.get('TaskId')
-        if m.get('body') is not None:
-            self.body = m.get('body')
         return self
 
 
 class PredictTemplateModelResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
```

### Comparing `alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/PKG-INFO` & `alibabacloud_documentautoml20221229-1.0.9/alibabacloud_documentautoml20221229.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-documentautoml20221229
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud documentAutoml (20221229) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_documentautoml20221229-1.0.8/setup.py` & `alibabacloud_documentautoml20221229-1.0.9/setup.py`

 * *Files identical despite different names*

