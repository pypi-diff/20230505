# Comparing `tmp/alibabacloud_documentautoml20221229_py2-1.0.8.tar.gz` & `tmp/alibabacloud_documentautoml20221229_py2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_documentautoml20221229_py2-1.0.8.tar", last modified: Mon Apr 10 07:44:13 2023, max compression
+gzip compressed data, was "dist/alibabacloud_documentautoml20221229_py2-1.0.9.tar", last modified: Mon Apr 10 11:22:56 2023, max compression
```

## Comparing `alibabacloud_documentautoml20221229_py2-1.0.8.tar` & `alibabacloud_documentautoml20221229_py2-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:44:13.000000 alibabacloud_documentautoml20221229_py2-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      344 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2538 2023-04-10 07:44:13.000000 alibabacloud_documentautoml20221229_py2-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1066 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1149 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:44:13.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7964 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229/client.py
--rw-r--r--   0 root         (0) root         (0)    20606 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:44:13.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2538 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      528 2023-04-10 07:44:13.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 07:44:13.000000 alibabacloud_documentautoml20221229_py2-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2958 2023-04-10 07:44:12.000000 alibabacloud_documentautoml20221229_py2-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8492 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229/client.py
+-rw-r--r--   0 root         (0) root         (0)    20606 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      528 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-04-10 11:22:56.000000 alibabacloud_documentautoml20221229_py2-1.0.9/setup.py
```

### Comparing `alibabacloud_documentautoml20221229_py2-1.0.8/LICENSE` & `alibabacloud_documentautoml20221229_py2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229_py2-1.0.8/PKG-INFO` & `alibabacloud_documentautoml20221229_py2-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_documentautoml20221229_py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud documentAutoml (20221229) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_documentautoml20221229_py2-1.0.8/README-CN.md` & `alibabacloud_documentautoml20221229_py2-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229_py2-1.0.8/README.md` & `alibabacloud_documentautoml20221229_py2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229/client.py` & `alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,17 +41,20 @@
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
@@ -102,17 +105,20 @@
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
@@ -137,17 +143,20 @@
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
@@ -170,17 +179,20 @@
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

### Comparing `alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229/models.py` & `alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class CreateModelAsyncPredictRequest(TeaModel):
-    def __init__(self, binary_to_text=None, content=None, model_id=None, model_version=None, service_name=None,
-                 service_version=None, body=None):
+    def __init__(self, binary_to_text=None, body=None, content=None, model_id=None, model_version=None,
+                 service_name=None, service_version=None):
         self.binary_to_text = binary_to_text  # type: bool
+        self.body = body  # type: str
         self.content = content  # type: str
         self.model_id = model_id  # type: long
         self.model_version = model_version  # type: str
         self.service_name = service_name  # type: str
         self.service_version = service_version  # type: str
-        self.body = body  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateModelAsyncPredictRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: int
         self.data = data  # type: str
@@ -237,49 +237,49 @@
         if m.get('body') is not None:
             temp_model = GetModelAsyncPredictResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PredictClassifierModelRequest(TeaModel):
-    def __init__(self, auto_prediction=None, classifier_id=None, content=None, body=None):
+    def __init__(self, auto_prediction=None, body=None, classifier_id=None, content=None):
         self.auto_prediction = auto_prediction  # type: bool
+        self.body = body  # type: str
         self.classifier_id = classifier_id  # type: long
         self.content = content  # type: str
-        self.body = body  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PredictClassifierModelRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: int
         self.data = data  # type: dict[str, any]
@@ -355,54 +355,54 @@
         if m.get('body') is not None:
             temp_model = PredictClassifierModelResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PredictModelRequest(TeaModel):
-    def __init__(self, binary_to_text=None, content=None, model_id=None, model_version=None, body=None):
+    def __init__(self, binary_to_text=None, body=None, content=None, model_id=None, model_version=None):
         self.binary_to_text = binary_to_text  # type: bool
+        self.body = body  # type: str
         self.content = content  # type: str
         self.model_id = model_id  # type: long
         self.model_version = model_version  # type: str
-        self.body = body  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PredictModelRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: int
         self.data = data  # type: dict[str, any]
@@ -478,49 +478,49 @@
         if m.get('body') is not None:
             temp_model = PredictModelResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PredictTemplateModelRequest(TeaModel):
-    def __init__(self, binary_to_text=None, content=None, task_id=None, body=None):
+    def __init__(self, binary_to_text=None, body=None, content=None, task_id=None):
         self.binary_to_text = binary_to_text  # type: bool
+        self.body = body  # type: str
         self.content = content  # type: str
         self.task_id = task_id  # type: long
-        self.body = body  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PredictTemplateModelRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: str
         self.data = data  # type: dict[str, any]
```

### Comparing `alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229_py2.egg-info/PKG-INFO` & `alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229_py2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-documentautoml20221229-py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud documentAutoml (20221229) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_documentautoml20221229_py2-1.0.8/alibabacloud_documentautoml20221229_py2.egg-info/SOURCES.txt` & `alibabacloud_documentautoml20221229_py2-1.0.9/alibabacloud_documentautoml20221229_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229_py2-1.0.8/setup.py` & `alibabacloud_documentautoml20221229_py2-1.0.9/setup.py`

 * *Files identical despite different names*

