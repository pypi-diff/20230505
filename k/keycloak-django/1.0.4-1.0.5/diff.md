# Comparing `tmp/keycloak_django-1.0.4.tar.gz` & `tmp/keycloak_django-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.0.4.tar", max compression
+gzip compressed data, was "keycloak_django-1.0.5.tar", max compression
```

## Comparing `keycloak_django-1.0.4.tar` & `keycloak_django-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.4/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.4/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.4/README.md
--rwxr-xr-x   0        0        0      971 2023-05-05 19:54:16.356489 keycloak_django-1.0.4/pyproject.toml
--rwxr-xr-x   0        0        0      113 2023-05-05 19:54:27.485193 keycloak_django-1.0.4/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.4/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.4/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.4/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.4/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      671 2023-05-05 04:43:24.794624 keycloak_django-1.0.4/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.4/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.4/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.4/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    15212 2023-05-05 04:43:24.957503 keycloak_django-1.0.4/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.4/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0      995 2023-05-05 04:43:25.024955 keycloak_django-1.0.4/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.4/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11384 2023-05-05 04:43:25.089664 keycloak_django-1.0.4/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2754 2023-05-05 04:43:25.126576 keycloak_django-1.0.4/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.4/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     1464 2023-05-05 04:43:25.156477 keycloak_django-1.0.4/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.4/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     2634 2023-05-05 04:43:25.215958 keycloak_django-1.0.4/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.4/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     3941 2023-05-05 04:43:25.273702 keycloak_django-1.0.4/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1445 2023-05-05 04:43:25.329684 keycloak_django-1.0.4/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.5/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.5/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.5/README.md
+-rwxr-xr-x   0        0        0      971 2023-05-05 20:21:55.583273 keycloak_django-1.0.5/pyproject.toml
+-rwxr-xr-x   0        0        0      113 2023-05-05 20:21:48.872754 keycloak_django-1.0.5/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.5/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.5/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.5/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.5/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      671 2023-05-05 04:43:24.794624 keycloak_django-1.0.5/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.5/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.5/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.5/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    15212 2023-05-05 04:43:24.957503 keycloak_django-1.0.5/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.5/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0      995 2023-05-05 04:43:25.024955 keycloak_django-1.0.5/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.5/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11384 2023-05-05 04:43:25.089664 keycloak_django-1.0.5/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.5/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.5/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     1464 2023-05-05 04:43:25.156477 keycloak_django-1.0.5/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.5/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     2634 2023-05-05 04:43:25.215958 keycloak_django-1.0.5/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.5/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     3941 2023-05-05 04:43:25.273702 keycloak_django-1.0.5/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1445 2023-05-05 04:43:25.329684 keycloak_django-1.0.5/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.5/PKG-INFO
```

### Comparing `keycloak_django-1.0.4/LICENSE` & `keycloak_django-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/pyproject.toml` & `keycloak_django-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.0.4"
+version = "1.0.5"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `keycloak_django-1.0.4/src/keycloak_django/api/viewsets.py` & `keycloak_django-1.0.5/src/keycloak_django/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/authentication.py` & `keycloak_django-1.0.5/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.0.5/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/keycloak.py` & `keycloak_django-1.0.5/src/keycloak_django/keycloak.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/middleware.py` & `keycloak_django-1.0.5/src/keycloak_django/middleware.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/migrations/0001_initial.py` & `keycloak_django-1.0.5/src/keycloak_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/models.py` & `keycloak_django-1.0.5/src/keycloak_django/models.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/security.py` & `keycloak_django-1.0.5/src/keycloak_django/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from rest_framework import permissions
 from django.core.exceptions import PermissionDenied
 from typing import List
 
+
 class ValidatePermissions(permissions.BasePermission):
     """
     Allows access only to authenticated users.
     """
 
     def _has_list_has_permissions(self, permissions_list: List, request, view):
         for per in permissions_list:
             if not (
                     per().has_permission(request, view) if (
-                            callable(per) and 'has_permission' in dir(per())) else request.user.has_perm(per)):
+                        callable(per) and 'has_permission' in dir(per())) else request.user.has_perm(per)):
                 return False
         return True
 
     def _validate_permission(self, permission, request, view):
         if callable(permission) and 'has_permission' in dir(permission()):
             return permission().has_permission(request, view)
 
@@ -34,14 +35,17 @@
         valid = False
         if request.user and request.user.is_authenticated and hasattr(view,
                                                                       'validate_permissions') and view.validate_permissions:
             if isinstance(view.validate_permissions, str) or isinstance(view.validate_permissions, List) or callable(
                     view.validate_permissions) and 'has_permission' in dir(view.validate_permissions()):
                 permission = view.validate_permissions
             else:
+                if not hasattr(view, 'action'):
+                    view.action = request.method
+                view.action = view.action.lower()
                 if not view.action in view.validate_permissions:
                     return True
                 permission = view.validate_permissions[view.action]
             valid = self._validate_permission(permission, request, view)
 
         # In case the 403 handler should be called raise the exception
         if hasattr(view, 'raise_exception_validate') and view.raise_exception_validate and not valid:
@@ -62,8 +66,8 @@
 def single_group(group: str):
     class C(permissions.BasePermission):
         def has_permission(self, request, view):
             if request.user and request.user.is_authenticated:
                 return group in [g.name for g in request.user.groups.all()]
             return False
 
-    return C
+    return C
```

### Comparing `keycloak_django-1.0.4/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.0.5/src/keycloak_django/services/client_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.0.5/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.0.5/src/keycloak_django/services/realm_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.0.5/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.0.5/src/keycloak_django/services/user_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/src/keycloak_django/tools.py` & `keycloak_django-1.0.5/src/keycloak_django/tools.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.4/PKG-INFO` & `keycloak_django-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.0.4
+Version: 1.0.5
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

