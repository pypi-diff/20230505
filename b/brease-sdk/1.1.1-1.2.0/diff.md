# Comparing `tmp/brease-sdk-1.1.1.tar.gz` & `tmp/brease-sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brease-sdk-1.1.1.tar", last modified: Sat Apr 29 00:41:56 2023, max compression
+gzip compressed data, was "brease-sdk-1.2.0.tar", last modified: Fri May  5 00:40:03 2023, max compression
```

## Comparing `brease-sdk-1.1.1.tar` & `brease-sdk-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.530219 brease-sdk-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-29 00:41:56.530219 brease-sdk-1.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2649 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:41:56.530219 brease-sdk-1.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/brease_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-29 00:41:56.000000 brease-sdk-1.1.1/src/brease_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/contextid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.522219 brease-sdk-1.1.1/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/addrule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1308 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/evaluaterules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/getallrules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/removerule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/operations/replacerule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.526219 brease-sdk-1.1.1/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/addruleinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/apiaddruleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/apiallrulesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/apievaluaterulesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/apireplaceruleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/condition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      506 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/conditionbasekey.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/conditionbaseref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/conditiontype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/evaluaterulesinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1483 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/expressionarray.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/modelsevaluationresult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2126 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/modelsrule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/modelstarget.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/models/shared/replaceruleinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:41:56.530219 brease-sdk-1.1.1/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-29 00:41:37.000000 brease-sdk-1.1.1/src/sdk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:40:03.324728 brease-sdk-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-05 00:40:03.324728 brease-sdk-1.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2672 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 00:40:03.324728 brease-sdk-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:40:03.320728 brease-sdk-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:40:03.320728 brease-sdk-1.2.0/src/brease_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-05 00:40:03.000000 brease-sdk-1.2.0/src/brease_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-05 00:40:03.000000 brease-sdk-1.2.0/src/brease_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:40:03.000000 brease-sdk-1.2.0/src/brease_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 00:40:03.000000 brease-sdk-1.2.0/src/brease_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 00:40:03.000000 brease-sdk-1.2.0/src/brease_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:40:03.320728 brease-sdk-1.2.0/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/contextid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:40:03.320728 brease-sdk-1.2.0/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:40:03.320728 brease-sdk-1.2.0/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/operations/addrule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1308 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/operations/evaluaterules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/operations/getallrules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/operations/removerule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/operations/replacerule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:40:03.324728 brease-sdk-1.2.0/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/addruleinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/apiaddruleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/apiallrulesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/apievaluaterulesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/apireplaceruleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/condition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      506 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/conditionbasekey.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/conditionbaseref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/conditiontype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/evaluaterulesinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1483 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/expressionarray.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/modelsevaluationresult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2126 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/modelsrule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/modelstarget.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/models/shared/replaceruleinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:40:03.324728 brease-sdk-1.2.0/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25540 2023-05-05 00:39:53.000000 brease-sdk-1.2.0/src/sdk/utils/utils.py
```

### Comparing `brease-sdk-1.1.1/LICENSE.md` & `brease-sdk-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/PKG-INFO` & `brease-sdk-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brease-sdk
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: dotindustries
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -28,37 +28,37 @@
 
 s = sdk.SDK()
 
 
 req = operations.AddRuleRequest(
     add_rule_input=shared.AddRuleInput(
         rule=shared.ModelsRule(
-            action="corrupti",
-            description="provident",
+            action='corrupti',
+            description='provident',
             expression=shared.ModelsRuleExpression3(
                 condition=shared.Condition(
                     base=shared.ConditionBase2(
                         ref=shared.ConditionBaseRef(
-                            dst="unde",
-                            src="nulla",
+                            dst='unde',
+                            src='nulla',
                         ),
                     ),
                     parameter=False,
-                    type="rgx",
+                    type=shared.ConditionTypeEnum.RGX,
                 ),
             ),
-            id="69a674e0-f467-4cc8-b96e-d151a05dfc2d",
+            id='69a674e0-f467-4cc8-b96e-d151a05dfc2d',
             target=shared.ModelsTarget(
-                target="at",
-                target_value="maiores",
-                type="molestiae",
+                target='at',
+                target_value='maiores',
+                type='molestiae',
             ),
         ),
     ),
-    context_id="quod",
+    context_id='quod',
 )
 
 res = s.context_id.add_rule(req, operations.AddRuleSecurity(
     api_token="Bearer YOUR_BEARER_TOKEN_HERE",
 ))
 
 if res.api_add_rule_response is not None:
```

### Comparing `brease-sdk-1.1.1/README.md` & `brease-sdk-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,37 +16,37 @@
 
 s = sdk.SDK()
 
 
 req = operations.AddRuleRequest(
     add_rule_input=shared.AddRuleInput(
         rule=shared.ModelsRule(
-            action="corrupti",
-            description="provident",
+            action='corrupti',
+            description='provident',
             expression=shared.ModelsRuleExpression3(
                 condition=shared.Condition(
                     base=shared.ConditionBase2(
                         ref=shared.ConditionBaseRef(
-                            dst="unde",
-                            src="nulla",
+                            dst='unde',
+                            src='nulla',
                         ),
                     ),
                     parameter=False,
-                    type="rgx",
+                    type=shared.ConditionTypeEnum.RGX,
                 ),
             ),
-            id="69a674e0-f467-4cc8-b96e-d151a05dfc2d",
+            id='69a674e0-f467-4cc8-b96e-d151a05dfc2d',
             target=shared.ModelsTarget(
-                target="at",
-                target_value="maiores",
-                type="molestiae",
+                target='at',
+                target_value='maiores',
+                type='molestiae',
             ),
         ),
     ),
-    context_id="quod",
+    context_id='quod',
 )
 
 res = s.context_id.add_rule(req, operations.AddRuleSecurity(
     api_token="Bearer YOUR_BEARER_TOKEN_HERE",
 ))
 
 if res.api_add_rule_response is not None:
```

### Comparing `brease-sdk-1.1.1/setup.py` & `brease-sdk-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="brease-sdk",
-    version="1.1.1",
+    version="1.2.0",
     author="dotindustries",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `brease-sdk-1.1.1/src/brease_sdk.egg-info/PKG-INFO` & `brease-sdk-1.2.0/src/brease_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brease-sdk
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: dotindustries
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -28,37 +28,37 @@
 
 s = sdk.SDK()
 
 
 req = operations.AddRuleRequest(
     add_rule_input=shared.AddRuleInput(
         rule=shared.ModelsRule(
-            action="corrupti",
-            description="provident",
+            action='corrupti',
+            description='provident',
             expression=shared.ModelsRuleExpression3(
                 condition=shared.Condition(
                     base=shared.ConditionBase2(
                         ref=shared.ConditionBaseRef(
-                            dst="unde",
-                            src="nulla",
+                            dst='unde',
+                            src='nulla',
                         ),
                     ),
                     parameter=False,
-                    type="rgx",
+                    type=shared.ConditionTypeEnum.RGX,
                 ),
             ),
-            id="69a674e0-f467-4cc8-b96e-d151a05dfc2d",
+            id='69a674e0-f467-4cc8-b96e-d151a05dfc2d',
             target=shared.ModelsTarget(
-                target="at",
-                target_value="maiores",
-                type="molestiae",
+                target='at',
+                target_value='maiores',
+                type='molestiae',
             ),
         ),
     ),
-    context_id="quod",
+    context_id='quod',
 )
 
 res = s.context_id.add_rule(req, operations.AddRuleSecurity(
     api_token="Bearer YOUR_BEARER_TOKEN_HERE",
 ))
 
 if res.api_add_rule_response is not None:
```

### Comparing `brease-sdk-1.1.1/src/brease_sdk.egg-info/SOURCES.txt` & `brease-sdk-1.2.0/src/brease_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/contextid.py` & `brease-sdk-1.2.0/src/sdk/contextid.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/operations/__init__.py` & `brease-sdk-1.2.0/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/operations/addrule.py` & `brease-sdk-1.2.0/src/sdk/models/operations/addrule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/operations/evaluaterules.py` & `brease-sdk-1.2.0/src/sdk/models/operations/evaluaterules.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/operations/getallrules.py` & `brease-sdk-1.2.0/src/sdk/models/operations/getallrules.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/operations/removerule.py` & `brease-sdk-1.2.0/src/sdk/models/operations/removerule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/operations/replacerule.py` & `brease-sdk-1.2.0/src/sdk/models/operations/replacerule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/__init__.py` & `brease-sdk-1.2.0/src/sdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/addruleinput.py` & `brease-sdk-1.2.0/src/sdk/models/shared/addruleinput.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/apiaddruleresponse.py` & `brease-sdk-1.2.0/src/sdk/models/shared/apiaddruleresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/apiallrulesresponse.py` & `brease-sdk-1.2.0/src/sdk/models/shared/apiallrulesresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/apievaluaterulesresponse.py` & `brease-sdk-1.2.0/src/sdk/models/shared/apievaluaterulesresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/apireplaceruleresponse.py` & `brease-sdk-1.2.0/src/sdk/models/shared/apireplaceruleresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/condition.py` & `brease-sdk-1.2.0/src/sdk/models/shared/condition.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/conditionbaseref.py` & `brease-sdk-1.2.0/src/sdk/models/shared/conditionbaseref.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/evaluaterulesinput.py` & `brease-sdk-1.2.0/src/sdk/models/shared/evaluaterulesinput.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/expressionarray.py` & `brease-sdk-1.2.0/src/sdk/models/shared/expressionarray.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/modelsevaluationresult.py` & `brease-sdk-1.2.0/src/sdk/models/shared/modelsevaluationresult.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/modelsrule.py` & `brease-sdk-1.2.0/src/sdk/models/shared/modelsrule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/models/shared/modelstarget.py` & `brease-sdk-1.2.0/src/sdk/models/shared/modelstarget.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/sdk.py` & `brease-sdk-1.2.0/src/sdk/sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     context_id: ContextID
     r"""Rule domain context"""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "1.1.1"
-    _gen_version: str = "2.23.4"
+    _sdk_version: str = "1.2.0"
+    _gen_version: str = "2.24.0"
 
     def __init__(self,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
```

### Comparing `brease-sdk-1.1.1/src/sdk/utils/retries.py` & `brease-sdk-1.2.0/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.1.1/src/sdk/utils/utils.py` & `brease-sdk-1.2.0/src/sdk/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,15 +727,15 @@
 
 def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
     if isinstance(val, Enum):
-        return val.value
+        return str(val.value)
 
     return str(val)
 
 
 def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: dict[str, dict[str, dict[str, Any]]]):
     if value is None and gbls is not None:
         if 'parameters' in gbls:
```

