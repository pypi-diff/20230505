# Comparing `tmp/keycloak_django-1.0.3.tar.gz` & `tmp/keycloak_django-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.0.3.tar", max compression
+gzip compressed data, was "keycloak_django-1.0.4.tar", max compression
```

## Comparing `keycloak_django-1.0.3.tar` & `keycloak_django-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-04 22:04:27.724646 keycloak_django-1.0.3/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-04 21:59:56.117966 keycloak_django-1.0.3/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-04 22:08:13.324804 keycloak_django-1.0.3/README.md
--rwxr-xr-x   0        0        0      985 2023-05-04 23:20:44.992981 keycloak_django-1.0.3/pyproject.toml
--rwxr-xr-x   0        0        0      113 2023-05-04 23:20:50.813813 keycloak_django-1.0.3/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-04 05:07:15.600530 keycloak_django-1.0.3/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-04 05:20:13.376184 keycloak_django-1.0.3/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-04 05:30:39.925884 keycloak_django-1.0.3/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-04 05:30:36.468184 keycloak_django-1.0.3/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      671 2023-05-04 05:45:27.964426 keycloak_django-1.0.3/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-04 22:41:49.944532 keycloak_django-1.0.3/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-04 01:02:27.338142 keycloak_django-1.0.3/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-04 05:11:06.671182 keycloak_django-1.0.3/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    15212 2023-05-04 23:20:18.382341 keycloak_django-1.0.3/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7613 2023-05-04 22:33:31.692522 keycloak_django-1.0.3/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0      995 2023-05-04 05:14:58.618115 keycloak_django-1.0.3/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-04 01:02:27.413484 keycloak_django-1.0.3/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11384 2023-05-04 05:04:03.980713 keycloak_django-1.0.3/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2754 2023-05-04 05:13:22.645094 keycloak_django-1.0.3/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-04 01:02:27.413484 keycloak_django-1.0.3/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     1464 2023-05-04 22:42:18.284199 keycloak_django-1.0.3/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4315 2023-05-04 22:42:29.530982 keycloak_django-1.0.3/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     2634 2023-05-04 22:42:37.236539 keycloak_django-1.0.3/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2005 2023-05-04 22:42:45.436718 keycloak_django-1.0.3/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     3941 2023-05-04 22:42:54.166312 keycloak_django-1.0.3/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1445 2023-05-04 21:29:37.252394 keycloak_django-1.0.3/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 keycloak_django-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.4/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.4/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.4/README.md
+-rwxr-xr-x   0        0        0      971 2023-05-05 19:54:16.356489 keycloak_django-1.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0      113 2023-05-05 19:54:27.485193 keycloak_django-1.0.4/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.4/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.4/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.4/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.4/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      671 2023-05-05 04:43:24.794624 keycloak_django-1.0.4/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.4/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.4/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.4/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    15212 2023-05-05 04:43:24.957503 keycloak_django-1.0.4/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.4/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0      995 2023-05-05 04:43:25.024955 keycloak_django-1.0.4/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.4/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11384 2023-05-05 04:43:25.089664 keycloak_django-1.0.4/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2754 2023-05-05 04:43:25.126576 keycloak_django-1.0.4/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.4/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     1464 2023-05-05 04:43:25.156477 keycloak_django-1.0.4/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.4/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     2634 2023-05-05 04:43:25.215958 keycloak_django-1.0.4/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.4/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     3941 2023-05-05 04:43:25.273702 keycloak_django-1.0.4/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1445 2023-05-05 04:43:25.329684 keycloak_django-1.0.4/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.4/PKG-INFO
```

### Comparing `keycloak_django-1.0.3/LICENSE` & `keycloak_django-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/pyproject.toml` & `keycloak_django-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.0.3"
+version = "1.0.4"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -19,14 +19,14 @@
     {include = "keycloak_django/**/*.py", from = "src/"},
 ]
 include = ["LICENSE", "CHANGELOG.md", "CONTRIBUTING.md"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-keycloak = "^2.16.1"
-django = "4.1.6"
-djangorestframework = "3.14.0"
-django-redis = "^5.2.0"
+django = "*"
+djangorestframework = "*"
+django-redis = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `keycloak_django-1.0.3/src/keycloak_django/api/viewsets.py` & `keycloak_django-1.0.4/src/keycloak_django/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/authentication.py` & `keycloak_django-1.0.4/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.0.4/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/keycloak.py` & `keycloak_django-1.0.4/src/keycloak_django/keycloak.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/middleware.py` & `keycloak_django-1.0.4/src/keycloak_django/middleware.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/migrations/0001_initial.py` & `keycloak_django-1.0.4/src/keycloak_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/models.py` & `keycloak_django-1.0.4/src/keycloak_django/models.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/security.py` & `keycloak_django-1.0.4/src/keycloak_django/security.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.0.4/src/keycloak_django/services/client_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.0.4/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.0.4/src/keycloak_django/services/realm_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.0.4/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.0.4/src/keycloak_django/services/user_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/src/keycloak_django/tools.py` & `keycloak_django-1.0.4/src/keycloak_django/tools.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.3/PKG-INFO` & `keycloak_django-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.0.3
+Version: 1.0.4
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires-Dist: django (==4.1.6)
-Requires-Dist: django-redis (>=5.2.0,<6.0.0)
-Requires-Dist: djangorestframework (==3.14.0)
+Requires-Dist: django
+Requires-Dist: django-redis
+Requires-Dist: djangorestframework
 Requires-Dist: python-keycloak (>=2.16.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Keycloak Django
 
 **keycloak-django** is Python package
```

