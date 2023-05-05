# Comparing `tmp/mypy-boto3-sqs-1.26.127.tar.gz` & `tmp/mypy-boto3-sqs-1.26.128.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sqs-1.26.127.tar", last modified: Thu May  4 21:08:52 2023, max compression
+gzip compressed data, was "mypy-boto3-sqs-1.26.128.tar", last modified: Fri May  5 18:07:52 2023, max compression
```

## Comparing `mypy-boto3-sqs-1.26.127.tar` & `mypy-boto3-sqs-1.26.128.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:08:52.664633 mypy-boto3-sqs-1.26.127/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-04 21:08:52.664633 mypy-boto3-sqs-1.26.127/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:08:52.652633 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-05-04 21:08:29.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18940 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-05-04 21:08:29.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21880 2023-05-04 21:08:29.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:08:52.664633 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:08:52.664633 mypy-boto3-sqs-1.26.127/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:07:52.552104 mypy-boto3-sqs-1.26.128/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-05 18:07:52.540102 mypy-boto3-sqs-1.26.128/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:07:52.540102 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21885 2023-05-05 18:07:42.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 18:07:41.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:07:52.540102 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-05 18:07:52.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-05 18:07:52.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:07:52.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:07:52.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 18:07:52.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 18:07:52.000000 mypy-boto3-sqs-1.26.128/mypy_boto3_sqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:07:52.552104 mypy-boto3-sqs-1.26.128/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-05 18:07:40.000000 mypy-boto3-sqs-1.26.128/setup.py
```

### Comparing `mypy-boto3-sqs-1.26.127/LICENSE` & `mypy-boto3-sqs-1.26.128/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.127/PKG-INFO` & `mypy-boto3-sqs-1.26.128/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.26.127
-Summary: Type annotations for boto3.SQS 1.26.127 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.128
+Summary: Type annotations for boto3.SQS 1.26.128 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.26.127](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.26.128](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -417,58 +417,58 @@
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
+    ResponseMetadataTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
-    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
-    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
     ListQueueTagsRequestRequestTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
-    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
+    CreateQueueResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetQueueAttributesResultTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesResultTypeDef,
+    SendMessageResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
```

### Comparing `mypy-boto3-sqs-1.26.127/README.md` & `mypy-boto3-sqs-1.26.128/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.26.127](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.26.128](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -385,58 +385,58 @@
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
+    ResponseMetadataTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
-    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
-    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
     ListQueueTagsRequestRequestTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
-    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
+    CreateQueueResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetQueueAttributesResultTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesResultTypeDef,
+    SendMessageResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__init__.py` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__init__.pyi` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__main__.py` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SQS 1.26.127\nVersion:         1.26.127\nBuilder version:"
+        "Type annotations for boto3.SQS 1.26.128\nVersion:         1.26.128\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.127")
+    print("1.26.128")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/client.py` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -41,57 +41,42 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SQSClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BatchEntryIdsNotDistinct: Type[BotocoreClientError]
     BatchRequestTooLong: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     EmptyBatchRequest: Type[BotocoreClientError]
-    InvalidAddress: Type[BotocoreClientError]
     InvalidAttributeName: Type[BotocoreClientError]
-    InvalidAttributeValue: Type[BotocoreClientError]
     InvalidBatchEntryId: Type[BotocoreClientError]
     InvalidIdFormat: Type[BotocoreClientError]
     InvalidMessageContents: Type[BotocoreClientError]
-    InvalidSecurity: Type[BotocoreClientError]
-    KmsAccessDenied: Type[BotocoreClientError]
-    KmsDisabled: Type[BotocoreClientError]
-    KmsInvalidKeyUsage: Type[BotocoreClientError]
-    KmsInvalidState: Type[BotocoreClientError]
-    KmsNotFound: Type[BotocoreClientError]
-    KmsOptInRequired: Type[BotocoreClientError]
-    KmsThrottled: Type[BotocoreClientError]
     MessageNotInflight: Type[BotocoreClientError]
     OverLimit: Type[BotocoreClientError]
     PurgeQueueInProgress: Type[BotocoreClientError]
     QueueDeletedRecently: Type[BotocoreClientError]
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
-    RequestThrottled: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
-
 class SQSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/)
     """
 
     meta: ClientMeta
@@ -100,174 +85,157 @@
     def exceptions(self) -> Exceptions:
         """
         SQSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#exceptions)
         """
-
     def add_permission(
         self, *, QueueUrl: str, Label: str, AWSAccountIds: Sequence[str], Actions: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds a permission to a queue for a specific
         [principal](https://docs.aws.amazon.com/general/latest/gr/glos-chap.html#P)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.add_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#add_permission)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#can_paginate)
         """
-
     def change_message_visibility(
         self, *, QueueUrl: str, ReceiptHandle: str, VisibilityTimeout: int
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the visibility timeout of a specified message in a queue to a new value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#change_message_visibility)
         """
-
     def change_message_visibility_batch(
         self, *, QueueUrl: str, Entries: Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef]
     ) -> ChangeMessageVisibilityBatchResultTypeDef:
         """
         Changes the visibility timeout of multiple messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#change_message_visibility_batch)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#close)
         """
-
     def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateQueueResultTypeDef:
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#create_queue)
         """
-
     def delete_message(self, *, QueueUrl: str, ReceiptHandle: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified message from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_message)
         """
-
     def delete_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[DeleteMessageBatchRequestEntryTypeDef]
     ) -> DeleteMessageBatchResultTypeDef:
         """
         Deletes up to ten messages from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_message_batch)
         """
-
     def delete_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the queue specified by the `QueueUrl`, regardless of the queue's
         contents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_queue)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#generate_presigned_url)
         """
-
     def get_queue_attributes(
         self, *, QueueUrl: str, AttributeNames: Sequence[QueueAttributeFilterType] = ...
     ) -> GetQueueAttributesResultTypeDef:
         """
         Gets attributes for the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_queue_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#get_queue_attributes)
         """
-
     def get_queue_url(
         self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...
     ) -> GetQueueUrlResultTypeDef:
         """
         Returns the URL of an existing Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_queue_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#get_queue_url)
         """
-
     def list_dead_letter_source_queues(
         self, *, QueueUrl: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDeadLetterSourceQueuesResultTypeDef:
         """
         Returns a list of your queues that have the `RedrivePolicy` queue attribute
         configured with a dead-letter queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_dead_letter_source_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_dead_letter_source_queues)
         """
-
     def list_queue_tags(self, *, QueueUrl: str) -> ListQueueTagsResultTypeDef:
         """
         List all cost allocation tags added to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queue_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_queue_tags)
         """
-
     def list_queues(
         self, *, QueueNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListQueuesResultTypeDef:
         """
         Returns a list of your queues in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_queues)
         """
-
     def purge_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the messages in a queue specified by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.purge_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#purge_queue)
         """
-
     def receive_message(
         self,
         *,
         QueueUrl: str,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
@@ -277,24 +245,22 @@
     ) -> ReceiveMessageResultTypeDef:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.receive_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#receive_message)
         """
-
     def remove_permission(self, *, QueueUrl: str, Label: str) -> EmptyResponseMetadataTypeDef:
         """
         Revokes any permissions in the queue policy that matches the specified `Label`
         parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.remove_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#remove_permission)
         """
-
     def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
@@ -306,61 +272,53 @@
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message)
         """
-
     def send_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
-        by assigning either identical or different values to each message (or by not
-        assigning values at all).
+        Delivers up to ten messages to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message_batch)
         """
-
     def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the value of one or more queue attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.set_queue_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#set_queue_attributes)
         """
-
     def tag_queue(self, *, QueueUrl: str, Tags: Mapping[str, str]) -> EmptyResponseMetadataTypeDef:
         """
         Add cost allocation tags to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.tag_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#tag_queue)
         """
-
     def untag_queue(self, *, QueueUrl: str, TagKeys: Sequence[str]) -> EmptyResponseMetadataTypeDef:
         """
         Remove cost allocation tags from the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.untag_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#untag_queue)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dead_letter_source_queues"]
     ) -> ListDeadLetterSourceQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_queues"]) -> ListQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/client.pyi` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,53 +41,46 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SQSClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BatchEntryIdsNotDistinct: Type[BotocoreClientError]
     BatchRequestTooLong: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     EmptyBatchRequest: Type[BotocoreClientError]
-    InvalidAddress: Type[BotocoreClientError]
     InvalidAttributeName: Type[BotocoreClientError]
-    InvalidAttributeValue: Type[BotocoreClientError]
     InvalidBatchEntryId: Type[BotocoreClientError]
     InvalidIdFormat: Type[BotocoreClientError]
     InvalidMessageContents: Type[BotocoreClientError]
-    InvalidSecurity: Type[BotocoreClientError]
-    KmsAccessDenied: Type[BotocoreClientError]
-    KmsDisabled: Type[BotocoreClientError]
-    KmsInvalidKeyUsage: Type[BotocoreClientError]
-    KmsInvalidState: Type[BotocoreClientError]
-    KmsNotFound: Type[BotocoreClientError]
-    KmsOptInRequired: Type[BotocoreClientError]
-    KmsThrottled: Type[BotocoreClientError]
     MessageNotInflight: Type[BotocoreClientError]
     OverLimit: Type[BotocoreClientError]
     PurgeQueueInProgress: Type[BotocoreClientError]
     QueueDeletedRecently: Type[BotocoreClientError]
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
-    RequestThrottled: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
+
 class SQSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/)
     """
 
     meta: ClientMeta
@@ -96,157 +89,174 @@
     def exceptions(self) -> Exceptions:
         """
         SQSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#exceptions)
         """
+
     def add_permission(
         self, *, QueueUrl: str, Label: str, AWSAccountIds: Sequence[str], Actions: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds a permission to a queue for a specific
         [principal](https://docs.aws.amazon.com/general/latest/gr/glos-chap.html#P)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.add_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#add_permission)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#can_paginate)
         """
+
     def change_message_visibility(
         self, *, QueueUrl: str, ReceiptHandle: str, VisibilityTimeout: int
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the visibility timeout of a specified message in a queue to a new value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#change_message_visibility)
         """
+
     def change_message_visibility_batch(
         self, *, QueueUrl: str, Entries: Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef]
     ) -> ChangeMessageVisibilityBatchResultTypeDef:
         """
         Changes the visibility timeout of multiple messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#change_message_visibility_batch)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#close)
         """
+
     def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateQueueResultTypeDef:
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#create_queue)
         """
+
     def delete_message(self, *, QueueUrl: str, ReceiptHandle: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified message from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_message)
         """
+
     def delete_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[DeleteMessageBatchRequestEntryTypeDef]
     ) -> DeleteMessageBatchResultTypeDef:
         """
         Deletes up to ten messages from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_message_batch)
         """
+
     def delete_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the queue specified by the `QueueUrl`, regardless of the queue's
         contents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_queue)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#generate_presigned_url)
         """
+
     def get_queue_attributes(
         self, *, QueueUrl: str, AttributeNames: Sequence[QueueAttributeFilterType] = ...
     ) -> GetQueueAttributesResultTypeDef:
         """
         Gets attributes for the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_queue_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#get_queue_attributes)
         """
+
     def get_queue_url(
         self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...
     ) -> GetQueueUrlResultTypeDef:
         """
         Returns the URL of an existing Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_queue_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#get_queue_url)
         """
+
     def list_dead_letter_source_queues(
         self, *, QueueUrl: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDeadLetterSourceQueuesResultTypeDef:
         """
         Returns a list of your queues that have the `RedrivePolicy` queue attribute
         configured with a dead-letter queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_dead_letter_source_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_dead_letter_source_queues)
         """
+
     def list_queue_tags(self, *, QueueUrl: str) -> ListQueueTagsResultTypeDef:
         """
         List all cost allocation tags added to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queue_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_queue_tags)
         """
+
     def list_queues(
         self, *, QueueNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListQueuesResultTypeDef:
         """
         Returns a list of your queues in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_queues)
         """
+
     def purge_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the messages in a queue specified by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.purge_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#purge_queue)
         """
+
     def receive_message(
         self,
         *,
         QueueUrl: str,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
@@ -256,22 +266,24 @@
     ) -> ReceiveMessageResultTypeDef:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.receive_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#receive_message)
         """
+
     def remove_permission(self, *, QueueUrl: str, Label: str) -> EmptyResponseMetadataTypeDef:
         """
         Revokes any permissions in the queue policy that matches the specified `Label`
         parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.remove_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#remove_permission)
         """
+
     def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
@@ -283,55 +295,59 @@
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message)
         """
+
     def send_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
-        by assigning either identical or different values to each message (or by not
-        assigning values at all).
+        Delivers up to ten messages to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message_batch)
         """
+
     def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the value of one or more queue attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.set_queue_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#set_queue_attributes)
         """
+
     def tag_queue(self, *, QueueUrl: str, Tags: Mapping[str, str]) -> EmptyResponseMetadataTypeDef:
         """
         Add cost allocation tags to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.tag_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#tag_queue)
         """
+
     def untag_queue(self, *, QueueUrl: str, TagKeys: Sequence[str]) -> EmptyResponseMetadataTypeDef:
         """
         Remove cost allocation tags from the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.untag_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#untag_queue)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dead_letter_source_queues"]
     ) -> ListDeadLetterSourceQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_queues"]) -> ListQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/literals.py` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/literals.pyi` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/paginator.py` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
-        self, *, QueueUrl: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
 
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
-        self, *, QueueNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueueNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/paginator.pyi` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
-        self, *, QueueUrl: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
-        self, *, QueueNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueueNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/service_resource.py` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,17 +336,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_message-method)
         """
 
     def send_messages(
         self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
-        by assigning either identical or different values to each message (or by not
-        assigning values at all).
+        Delivers up to ten messages to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_messages-method)
         """
 
     def set_attributes(self, *, Attributes: Mapping[QueueAttributeNameType, str]) -> None:
         """
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/service_resource.pyi` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -305,17 +305,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_message-method)
         """
     def send_messages(
         self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
-        by assigning either identical or different values to each message (or by not
-        assigning values at all).
+        Delivers up to ten messages to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_messages-method)
         """
     def set_attributes(self, *, Attributes: Mapping[QueueAttributeNameType, str]) -> None:
         """
         Sets the value of one or more queue attributes.
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/type_defs.py` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,58 +34,58 @@
 
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "CreateQueueRequestServiceResourceCreateQueueTypeDef",
-    "CreateQueueResultTypeDef",
     "DeleteMessageBatchRequestEntryTypeDef",
     "DeleteMessageBatchResultEntryTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesRequestRequestTypeDef",
-    "GetQueueAttributesResultTypeDef",
     "GetQueueUrlRequestRequestTypeDef",
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
-    "GetQueueUrlResultTypeDef",
-    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
-    "ListDeadLetterSourceQueuesResultTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
-    "ListQueueTagsResultTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "ListQueuesResultTypeDef",
     "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
-    "PaginatorConfigTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SendMessageBatchResultEntryTypeDef",
-    "SendMessageResultTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     "ChangeMessageVisibilityBatchRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchResultTypeDef",
+    "CreateQueueResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetQueueAttributesResultTypeDef",
+    "GetQueueUrlResultTypeDef",
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    "ListQueueTagsResultTypeDef",
+    "ListQueuesResultTypeDef",
+    "SendMessageResultTypeDef",
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
+    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "MessageTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
     "SendMessageRequestRequestTypeDef",
     "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
@@ -160,14 +160,25 @@
 ChangeMessageVisibilityBatchResultEntryTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     {
         "Id": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef = TypedDict(
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     {
         "VisibilityTimeout": int,
     },
 )
 
@@ -221,22 +232,14 @@
 class CreateQueueRequestServiceResourceCreateQueueTypeDef(
     _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef,
     _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef,
 ):
     pass
 
 
-CreateQueueResultTypeDef = TypedDict(
-    "CreateQueueResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMessageBatchRequestEntryTypeDef = TypedDict(
     "DeleteMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -259,21 +262,14 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalGetQueueAttributesRequestRequestTypeDef = TypedDict(
@@ -288,22 +284,14 @@
 class GetQueueAttributesRequestRequestTypeDef(
     _RequiredGetQueueAttributesRequestRequestTypeDef,
     _OptionalGetQueueAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-GetQueueAttributesResultTypeDef = TypedDict(
-    "GetQueueAttributesResultTypeDef",
-    {
-        "Attributes": Dict[QueueAttributeNameType, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetQueueUrlRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestRequestTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalGetQueueUrlRequestRequestTypeDef = TypedDict(
@@ -339,44 +327,24 @@
 class GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef(
     _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
     _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
 ):
     pass
 
 
-GetQueueUrlResultTypeDef = TypedDict(
-    "GetQueueUrlResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "QueueUrl": str,
-    },
-)
-_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
-    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListDeadLetterSourceQueuesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
@@ -392,66 +360,31 @@
 class ListDeadLetterSourceQueuesRequestRequestTypeDef(
     _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef,
     _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef,
 ):
     pass
 
 
-ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    {
-        "queueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListQueueTagsRequestRequestTypeDef = TypedDict(
     "ListQueueTagsRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
-ListQueueTagsResultTypeDef = TypedDict(
-    "ListQueueTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "QueueNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListQueuesResultTypeDef = TypedDict(
-    "ListQueuesResultTypeDef",
-    {
-        "QueueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMessageAttributeValueTypeDef = TypedDict(
     "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageAttributeValueTypeDef = TypedDict(
@@ -492,24 +425,14 @@
 
 class MessageSystemAttributeValueTypeDef(
     _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
@@ -563,25 +486,14 @@
     "RemovePermissionRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Label": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSendMessageBatchResultEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "MD5OfMessageBody": str,
     },
@@ -599,26 +511,14 @@
 
 class SendMessageBatchResultEntryTypeDef(
     _RequiredSendMessageBatchResultEntryTypeDef, _OptionalSendMessageBatchResultEntryTypeDef
 ):
     pass
 
 
-SendMessageResultTypeDef = TypedDict(
-    "SendMessageResultTypeDef",
-    {
-        "MD5OfMessageBody": str,
-        "MD5OfMessageAttributes": str,
-        "MD5OfMessageSystemAttributes": str,
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetQueueAttributesRequestQueueSetAttributesTypeDef = TypedDict(
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
     },
 )
 
@@ -662,15 +562,84 @@
 )
 
 ChangeMessageVisibilityBatchResultTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultTypeDef",
     {
         "Successful": List[ChangeMessageVisibilityBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateQueueResultTypeDef = TypedDict(
+    "CreateQueueResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueueAttributesResultTypeDef = TypedDict(
+    "GetQueueAttributesResultTypeDef",
+    {
+        "Attributes": Dict[QueueAttributeNameType, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueueUrlResultTypeDef = TypedDict(
+    "GetQueueUrlResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    {
+        "queueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueueTagsResultTypeDef = TypedDict(
+    "ListQueueTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueuesResultTypeDef = TypedDict(
+    "ListQueuesResultTypeDef",
+    {
+        "QueueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendMessageResultTypeDef = TypedDict(
+    "SendMessageResultTypeDef",
+    {
+        "MD5OfMessageBody": str,
+        "MD5OfMessageAttributes": str,
+        "MD5OfMessageSystemAttributes": str,
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMessageBatchRequestQueueDeleteMessagesTypeDef = TypedDict(
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     {
         "Entries": Sequence[DeleteMessageBatchRequestEntryTypeDef],
@@ -686,18 +655,49 @@
 )
 
 DeleteMessageBatchResultTypeDef = TypedDict(
     "DeleteMessageBatchResultTypeDef",
     {
         "Successful": List[DeleteMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "QueueUrl": str,
+    },
+)
+_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
+    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+):
+    pass
+
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "QueueNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageId": str,
         "ReceiptHandle": str,
         "MD5OfBody": str,
         "Body": str,
@@ -793,23 +793,23 @@
 
 
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReceiveMessageResultTypeDef = TypedDict(
     "ReceiveMessageResultTypeDef",
     {
         "Messages": List[MessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/type_defs.pyi` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,58 +33,58 @@
 
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "CreateQueueRequestServiceResourceCreateQueueTypeDef",
-    "CreateQueueResultTypeDef",
     "DeleteMessageBatchRequestEntryTypeDef",
     "DeleteMessageBatchResultEntryTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesRequestRequestTypeDef",
-    "GetQueueAttributesResultTypeDef",
     "GetQueueUrlRequestRequestTypeDef",
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
-    "GetQueueUrlResultTypeDef",
-    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
-    "ListDeadLetterSourceQueuesResultTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
-    "ListQueueTagsResultTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "ListQueuesResultTypeDef",
     "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
-    "PaginatorConfigTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SendMessageBatchResultEntryTypeDef",
-    "SendMessageResultTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     "ChangeMessageVisibilityBatchRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchResultTypeDef",
+    "CreateQueueResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetQueueAttributesResultTypeDef",
+    "GetQueueUrlResultTypeDef",
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    "ListQueueTagsResultTypeDef",
+    "ListQueuesResultTypeDef",
+    "SendMessageResultTypeDef",
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
+    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "MessageTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
     "SendMessageRequestRequestTypeDef",
     "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
@@ -155,14 +155,25 @@
 ChangeMessageVisibilityBatchResultEntryTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     {
         "Id": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef = TypedDict(
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     {
         "VisibilityTimeout": int,
     },
 )
 
@@ -212,22 +223,14 @@
 
 class CreateQueueRequestServiceResourceCreateQueueTypeDef(
     _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef,
     _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef,
 ):
     pass
 
-CreateQueueResultTypeDef = TypedDict(
-    "CreateQueueResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMessageBatchRequestEntryTypeDef = TypedDict(
     "DeleteMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -250,21 +253,14 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalGetQueueAttributesRequestRequestTypeDef = TypedDict(
@@ -277,22 +273,14 @@
 
 class GetQueueAttributesRequestRequestTypeDef(
     _RequiredGetQueueAttributesRequestRequestTypeDef,
     _OptionalGetQueueAttributesRequestRequestTypeDef,
 ):
     pass
 
-GetQueueAttributesResultTypeDef = TypedDict(
-    "GetQueueAttributesResultTypeDef",
-    {
-        "Attributes": Dict[QueueAttributeNameType, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetQueueUrlRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestRequestTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalGetQueueUrlRequestRequestTypeDef = TypedDict(
@@ -324,42 +312,24 @@
 
 class GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef(
     _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
     _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
 ):
     pass
 
-GetQueueUrlResultTypeDef = TypedDict(
-    "GetQueueUrlResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "QueueUrl": str,
-    },
-)
-_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
-    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListDeadLetterSourceQueuesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
@@ -373,66 +343,31 @@
 
 class ListDeadLetterSourceQueuesRequestRequestTypeDef(
     _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef,
     _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef,
 ):
     pass
 
-ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    {
-        "queueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListQueueTagsRequestRequestTypeDef = TypedDict(
     "ListQueueTagsRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
-ListQueueTagsResultTypeDef = TypedDict(
-    "ListQueueTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "QueueNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListQueuesResultTypeDef = TypedDict(
-    "ListQueuesResultTypeDef",
-    {
-        "QueueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMessageAttributeValueTypeDef = TypedDict(
     "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageAttributeValueTypeDef = TypedDict(
@@ -469,24 +404,14 @@
 )
 
 class MessageSystemAttributeValueTypeDef(
     _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
@@ -538,25 +463,14 @@
     "RemovePermissionRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Label": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSendMessageBatchResultEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "MD5OfMessageBody": str,
     },
@@ -572,26 +486,14 @@
 )
 
 class SendMessageBatchResultEntryTypeDef(
     _RequiredSendMessageBatchResultEntryTypeDef, _OptionalSendMessageBatchResultEntryTypeDef
 ):
     pass
 
-SendMessageResultTypeDef = TypedDict(
-    "SendMessageResultTypeDef",
-    {
-        "MD5OfMessageBody": str,
-        "MD5OfMessageAttributes": str,
-        "MD5OfMessageSystemAttributes": str,
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetQueueAttributesRequestQueueSetAttributesTypeDef = TypedDict(
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
     },
 )
 
@@ -635,15 +537,84 @@
 )
 
 ChangeMessageVisibilityBatchResultTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultTypeDef",
     {
         "Successful": List[ChangeMessageVisibilityBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateQueueResultTypeDef = TypedDict(
+    "CreateQueueResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueueAttributesResultTypeDef = TypedDict(
+    "GetQueueAttributesResultTypeDef",
+    {
+        "Attributes": Dict[QueueAttributeNameType, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueueUrlResultTypeDef = TypedDict(
+    "GetQueueUrlResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    {
+        "queueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueueTagsResultTypeDef = TypedDict(
+    "ListQueueTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueuesResultTypeDef = TypedDict(
+    "ListQueuesResultTypeDef",
+    {
+        "QueueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendMessageResultTypeDef = TypedDict(
+    "SendMessageResultTypeDef",
+    {
+        "MD5OfMessageBody": str,
+        "MD5OfMessageAttributes": str,
+        "MD5OfMessageSystemAttributes": str,
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMessageBatchRequestQueueDeleteMessagesTypeDef = TypedDict(
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     {
         "Entries": Sequence[DeleteMessageBatchRequestEntryTypeDef],
@@ -659,18 +630,47 @@
 )
 
 DeleteMessageBatchResultTypeDef = TypedDict(
     "DeleteMessageBatchResultTypeDef",
     {
         "Successful": List[DeleteMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "QueueUrl": str,
+    },
+)
+_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
+    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+):
+    pass
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "QueueNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageId": str,
         "ReceiptHandle": str,
         "MD5OfBody": str,
         "Body": str,
@@ -760,23 +760,23 @@
     pass
 
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReceiveMessageResultTypeDef = TypedDict(
     "ReceiveMessageResultTypeDef",
     {
         "Messages": List[MessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/PKG-INFO` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.26.127
-Summary: Type annotations for boto3.SQS 1.26.127 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.128
+Summary: Type annotations for boto3.SQS 1.26.128 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.26.127](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.26.128](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -417,58 +417,58 @@
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
+    ResponseMetadataTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
-    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
-    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
     ListQueueTagsRequestRequestTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
-    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
+    CreateQueueResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetQueueAttributesResultTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesResultTypeDef,
+    SendMessageResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
```

### Comparing `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/SOURCES.txt` & `mypy-boto3-sqs-1.26.128/mypy_boto3_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.127/setup.py` & `mypy-boto3-sqs-1.26.128/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sqs",
-    version="1.26.127",
+    version="1.26.128",
     packages=["mypy_boto3_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SQS 1.26.127 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SQS 1.26.128 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

