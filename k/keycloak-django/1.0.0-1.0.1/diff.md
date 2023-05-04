# Comparing `tmp/keycloak_django-1.0.0.tar.gz` & `tmp/keycloak_django-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.0.0.tar", max compression
+gzip compressed data, was "keycloak_django-1.0.1.tar", max compression
```

## Comparing `keycloak_django-1.0.0.tar` & `keycloak_django-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-04 22:04:27.724646 keycloak_django-1.0.0/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-04 21:59:56.117966 keycloak_django-1.0.0/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-04 22:08:13.324804 keycloak_django-1.0.0/README.md
--rwxr-xr-x   0        0        0      985 2023-05-04 21:58:55.145728 keycloak_django-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0      113 2023-05-04 21:47:37.576472 keycloak_django-1.0.0/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-04 05:07:15.600530 keycloak_django-1.0.0/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-04 05:20:13.376184 keycloak_django-1.0.0/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-04 05:30:39.925884 keycloak_django-1.0.0/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-04 05:30:36.468184 keycloak_django-1.0.0/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      671 2023-05-04 05:45:27.964426 keycloak_django-1.0.0/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-04 01:02:27.341142 keycloak_django-1.0.0/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-04 01:02:27.338142 keycloak_django-1.0.0/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-04 05:11:06.671182 keycloak_django-1.0.0/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    14581 2023-05-04 21:30:29.323843 keycloak_django-1.0.0/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7902 2023-05-04 21:32:50.939666 keycloak_django-1.0.0/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0      995 2023-05-04 05:14:58.618115 keycloak_django-1.0.0/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-04 01:02:27.413484 keycloak_django-1.0.0/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11384 2023-05-04 05:04:03.980713 keycloak_django-1.0.0/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2754 2023-05-04 05:13:22.645094 keycloak_django-1.0.0/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-04 01:02:27.413484 keycloak_django-1.0.0/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     1478 2023-05-04 01:02:28.213629 keycloak_django-1.0.0/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4329 2023-05-04 01:02:28.299592 keycloak_django-1.0.0/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     2648 2023-05-04 01:02:28.253941 keycloak_django-1.0.0/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2019 2023-05-04 01:02:28.325778 keycloak_django-1.0.0/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     3955 2023-05-04 01:02:28.359297 keycloak_django-1.0.0/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1445 2023-05-04 21:29:37.252394 keycloak_django-1.0.0/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 keycloak_django-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-04 22:04:27.724646 keycloak_django-1.0.1/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-04 21:59:56.117966 keycloak_django-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-04 22:08:13.324804 keycloak_django-1.0.1/README.md
+-rwxr-xr-x   0        0        0      985 2023-05-04 22:33:47.594498 keycloak_django-1.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0      113 2023-05-04 22:33:54.926475 keycloak_django-1.0.1/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-04 05:07:15.600530 keycloak_django-1.0.1/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-04 05:20:13.376184 keycloak_django-1.0.1/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-04 05:30:39.925884 keycloak_django-1.0.1/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-04 05:30:36.468184 keycloak_django-1.0.1/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      671 2023-05-04 05:45:27.964426 keycloak_django-1.0.1/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-04 01:02:27.341142 keycloak_django-1.0.1/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-04 01:02:27.338142 keycloak_django-1.0.1/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-04 05:11:06.671182 keycloak_django-1.0.1/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    14581 2023-05-04 21:30:29.323843 keycloak_django-1.0.1/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7613 2023-05-04 22:33:31.692522 keycloak_django-1.0.1/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0      995 2023-05-04 05:14:58.618115 keycloak_django-1.0.1/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-04 01:02:27.413484 keycloak_django-1.0.1/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11384 2023-05-04 05:04:03.980713 keycloak_django-1.0.1/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2754 2023-05-04 05:13:22.645094 keycloak_django-1.0.1/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-04 01:02:27.413484 keycloak_django-1.0.1/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     1478 2023-05-04 01:02:28.213629 keycloak_django-1.0.1/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4329 2023-05-04 01:02:28.299592 keycloak_django-1.0.1/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     2648 2023-05-04 01:02:28.253941 keycloak_django-1.0.1/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2019 2023-05-04 01:02:28.325778 keycloak_django-1.0.1/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     3955 2023-05-04 01:02:28.359297 keycloak_django-1.0.1/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1445 2023-05-04 21:29:37.252394 keycloak_django-1.0.1/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 keycloak_django-1.0.1/PKG-INFO
```

### Comparing `keycloak_django-1.0.0/LICENSE` & `keycloak_django-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/pyproject.toml` & `keycloak_django-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.0.0"
+version = "1.0.1"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `keycloak_django-1.0.0/src/keycloak_django/api/viewsets.py` & `keycloak_django-1.0.1/src/keycloak_django/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/authentication.py` & `keycloak_django-1.0.1/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.0.1/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/keycloak.py` & `keycloak_django-1.0.1/src/keycloak_django/keycloak.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/middleware.py` & `keycloak_django-1.0.1/src/keycloak_django/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # -*- coding: utf-8 -*-
-from django.utils import timezone
 from django.conf import settings
 from django.http.response import JsonResponse
 from django.utils.deprecation import MiddlewareMixin
 from .tools import fill_user_model_keycloak, get_user_model_keycloak, set_profile
-from .keycloak import KeycloakOpenID
 from keycloak.exceptions import KeycloakInvalidTokenError
-from rest_framework.exceptions import PermissionDenied, AuthenticationFailed, NotAuthenticated
+from rest_framework.exceptions import PermissionDenied, AuthenticationFailed
 from django.contrib.auth import get_user_model
-from django_keycloak.models import keycloakUserAbstract
 from django.contrib.auth import login
 from django.contrib.auth import logout
+from .keycloak import KeycloakToken
 
 
 class KeycloakMiddleware(MiddlewareMixin):
 
     def __init__(self, get_response):
         """
         :param get_response:
@@ -43,23 +41,20 @@
         self.create_user_if_not_exist = self.config.get(
             'CREATE_USER_IF_NOT_EXIST', False)
         self.attributes_fillable = self.config.get('ATTRIBUTES_FILLABLE', None)
         self.public_key_validate = self.config.get(
             'PUBLIC_KEY_VALIDATE', 'inter')
 
         # Create Keycloak instance
-        self.keycloak = KeycloakOpenID(server_url=self.server_url,
-                                       client_id=self.client_id,
-                                       realm_name=self.realm,
-                                       client_secret_key=self.client_secret_key)
-
-        # Read policies
-        if self.keycloak_authorization_config:
-            self.keycloak.load_authorization_config(
-                self.keycloak_authorization_config)
+        self.keycloak = KeycloakToken(client_id=self.client_id, realm_name=self.realm)
+
+        # # Read policies
+        # if self.keycloak_authorization_config:
+        #     self.keycloak.load_authorization_config(
+        #         self.keycloak_authorization_config)
 
         # Django
         self.get_response = get_response
 
     def __call__(self, request):
         """
         :param request:
```

### Comparing `keycloak_django-1.0.0/src/keycloak_django/migrations/0001_initial.py` & `keycloak_django-1.0.1/src/keycloak_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/models.py` & `keycloak_django-1.0.1/src/keycloak_django/models.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/security.py` & `keycloak_django-1.0.1/src/keycloak_django/security.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.0.1/src/keycloak_django/services/client_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.0.1/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.0.1/src/keycloak_django/services/realm_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.0.1/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.0.1/src/keycloak_django/services/user_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/src/keycloak_django/tools.py` & `keycloak_django-1.0.1/src/keycloak_django/tools.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.0/PKG-INFO` & `keycloak_django-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.0.0
+Version: 1.0.1
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

