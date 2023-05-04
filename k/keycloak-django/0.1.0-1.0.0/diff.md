# Comparing `tmp/keycloak_django-0.1.0.tar.gz` & `tmp/keycloak_django-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-0.1.0.tar", max compression
+gzip compressed data, was "keycloak_django-1.0.0.tar", max compression
```

## Comparing `keycloak_django-0.1.0.tar` & `keycloak_django-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,27 @@
--rw-r--r--   0        0        0        0 2023-05-03 16:50:38.505163 keycloak_django-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-03 16:50:38.505163 keycloak_django-0.1.0/django_keycloak/__init__.py
--rw-r--r--   0        0        0      172 2023-05-03 16:58:02.995172 keycloak_django-0.1.0/django_keycloak/admin/__init__.py
--rw-r--r--   0        0        0      475 2023-05-03 16:58:03.005172 keycloak_django-0.1.0/django_keycloak/admin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3308 2023-05-03 16:58:03.005172 keycloak_django-0.1.0/django_keycloak/admin/__pycache__/realm.cpython-311.pyc
--rw-r--r--   0        0        0     4379 2023-05-03 16:58:03.005172 keycloak_django-0.1.0/django_keycloak/admin/realm.py
--rw-r--r--   0        0        0      168 2023-05-03 16:58:02.745172 keycloak_django-0.1.0/django_keycloak/apps.py
--rw-r--r--   0        0        0      705 2023-05-03 16:58:02.705172 keycloak_django-0.1.0/django_keycloak/authentication.py
--rw-r--r--   0        0        0     1722 2023-05-03 16:58:02.665172 keycloak_django-0.1.0/django_keycloak/groups_permissions.py
--rw-r--r--   0        0        0    16738 2023-05-03 16:58:02.625172 keycloak_django-0.1.0/django_keycloak/keycloak.py
--rw-r--r--   0        0        0        0 2023-05-03 16:58:02.935172 keycloak_django-0.1.0/django_keycloak/management/__init__.py
--rw-r--r--   0        0        0      152 2023-05-03 16:58:02.935172 keycloak_django-0.1.0/django_keycloak/management/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-05-03 16:58:02.935172 keycloak_django-0.1.0/django_keycloak/management/commands/__init__.py
--rw-r--r--   0        0        0     9512 2023-05-03 16:58:02.935172 keycloak_django-0.1.0/django_keycloak/management/commands/user_consumer.py
--rw-r--r--   0        0        0     9899 2023-05-03 16:58:51.635173 keycloak_django-0.1.0/django_keycloak/middleware.py
--rw-r--r--   0        0        0     3029 2023-05-03 16:58:02.875172 keycloak_django-0.1.0/django_keycloak/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-03 16:58:02.875172 keycloak_django-0.1.0/django_keycloak/migrations/__init__.py
--rw-r--r--   0        0        0     3149 2023-05-03 16:58:02.875172 keycloak_django-0.1.0/django_keycloak/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0        0        0      182 2023-05-03 16:58:02.875172 keycloak_django-0.1.0/django_keycloak/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    13748 2023-05-03 16:58:02.545172 keycloak_django-0.1.0/django_keycloak/models.py
--rw-r--r--   0        0        0     2896 2023-05-03 16:58:02.515172 keycloak_django-0.1.0/django_keycloak/security.py
--rw-r--r--   0        0        0        0 2023-05-03 16:58:02.795172 keycloak_django-0.1.0/django_keycloak/services/__init__.py
--rw-r--r--   0        0        0      180 2023-05-03 16:58:02.795172 keycloak_django-0.1.0/django_keycloak/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2387 2023-05-03 16:58:02.795172 keycloak_django-0.1.0/django_keycloak/services/__pycache__/client_repository.cpython-311.pyc
--rw-r--r--   0        0        0     6807 2023-05-03 16:58:02.795172 keycloak_django-0.1.0/django_keycloak/services/__pycache__/permission_repository.cpython-311.pyc
--rw-r--r--   0        0        0     2911 2023-05-03 16:58:02.795172 keycloak_django-0.1.0/django_keycloak/services/__pycache__/realm_repository.cpython-311.pyc
--rw-r--r--   0        0        0     2939 2023-05-03 16:58:02.795172 keycloak_django-0.1.0/django_keycloak/services/__pycache__/role_repository.cpython-311.pyc
--rw-r--r--   0        0        0     8905 2023-05-03 16:58:02.795172 keycloak_django-0.1.0/django_keycloak/services/__pycache__/synchronize.cpython-311.pyc
--rw-r--r--   0        0        0     5927 2023-05-03 16:58:02.795172 keycloak_django-0.1.0/django_keycloak/services/__pycache__/user_repository.cpython-311.pyc
--rw-r--r--   0        0        0     1507 2023-05-03 16:58:02.795172 keycloak_django-0.1.0/django_keycloak/services/client_repository.py
--rw-r--r--   0        0        0     4418 2023-05-03 16:58:02.805172 keycloak_django-0.1.0/django_keycloak/services/permission_repository.py
--rw-r--r--   0        0        0     2704 2023-05-03 16:58:02.805172 keycloak_django-0.1.0/django_keycloak/services/realm_repository.py
--rw-r--r--   0        0        0     2064 2023-05-03 16:58:02.805172 keycloak_django-0.1.0/django_keycloak/services/role_repository.py
--rw-r--r--   0        0        0     4963 2023-05-03 16:58:02.805172 keycloak_django-0.1.0/django_keycloak/services/synchronize.py
--rw-r--r--   0        0        0     4087 2023-05-03 16:58:02.805172 keycloak_django-0.1.0/django_keycloak/services/user_repository.py
--rw-r--r--   0        0        0     2218 2023-05-03 16:58:02.475172 keycloak_django-0.1.0/django_keycloak/tools.py
--rw-r--r--   0        0        0      412 2023-05-03 17:13:49.485191 keycloak_django-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 keycloak_django-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-04 22:04:27.724646 keycloak_django-1.0.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-04 21:59:56.117966 keycloak_django-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-04 22:08:13.324804 keycloak_django-1.0.0/README.md
+-rwxr-xr-x   0        0        0      985 2023-05-04 21:58:55.145728 keycloak_django-1.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0      113 2023-05-04 21:47:37.576472 keycloak_django-1.0.0/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-04 05:07:15.600530 keycloak_django-1.0.0/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-04 05:20:13.376184 keycloak_django-1.0.0/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-04 05:30:39.925884 keycloak_django-1.0.0/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-04 05:30:36.468184 keycloak_django-1.0.0/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      671 2023-05-04 05:45:27.964426 keycloak_django-1.0.0/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-04 01:02:27.341142 keycloak_django-1.0.0/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-04 01:02:27.338142 keycloak_django-1.0.0/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-04 05:11:06.671182 keycloak_django-1.0.0/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    14581 2023-05-04 21:30:29.323843 keycloak_django-1.0.0/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7902 2023-05-04 21:32:50.939666 keycloak_django-1.0.0/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0      995 2023-05-04 05:14:58.618115 keycloak_django-1.0.0/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-04 01:02:27.413484 keycloak_django-1.0.0/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11384 2023-05-04 05:04:03.980713 keycloak_django-1.0.0/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2754 2023-05-04 05:13:22.645094 keycloak_django-1.0.0/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-04 01:02:27.413484 keycloak_django-1.0.0/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     1478 2023-05-04 01:02:28.213629 keycloak_django-1.0.0/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4329 2023-05-04 01:02:28.299592 keycloak_django-1.0.0/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     2648 2023-05-04 01:02:28.253941 keycloak_django-1.0.0/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2019 2023-05-04 01:02:28.325778 keycloak_django-1.0.0/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     3955 2023-05-04 01:02:28.359297 keycloak_django-1.0.0/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1445 2023-05-04 21:29:37.252394 keycloak_django-1.0.0/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 keycloak_django-1.0.0/PKG-INFO
```

### Comparing `keycloak_django-0.1.0/django_keycloak/authentication.py` & `keycloak_django-1.0.0/src/keycloak_django/authentication.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from rest_framework.authentication import BaseAuthentication
-
-class TokenAuthentication(BaseAuthentication):
-    """
-    Use Django's session framework for authentication.
-    """
-
-    def authenticate(self, request):
-        """
-        Returns a `User` if the request session currently has a logged in user.
-        Otherwise returns `None`.
-        """
-
-        # Get the session-based user from the underlying HttpRequest object
-        user = getattr(request._request, 'user', None)
-
-        # Unauthenticated, CSRF validation not required
-        if not user or not user.is_active:
-            return None
-
-        # CSRF passed with authenticated user
+from rest_framework.authentication import BaseAuthentication
+
+class TokenAuthentication(BaseAuthentication):
+    """
+    Use Django's session framework for authentication.
+    """
+
+    def authenticate(self, request):
+        """
+        Returns a `User` if the request session currently has a logged in user.
+        Otherwise returns `None`.
+        """
+
+        # Get the session-based user from the underlying HttpRequest object
+        user = getattr(request._request, 'user', None)
+
+        # Unauthenticated, CSRF validation not required
+        if not user or not user.is_active:
+            return None
+
+        # CSRF passed with authenticated user
         return user, None
```

### Comparing `keycloak_django-0.1.0/django_keycloak/middleware.py` & `keycloak_django-1.0.0/src/keycloak_django/middleware.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,277 +1,234 @@
-# -*- coding: utf-8 -*-
-from django.utils import timezone
-from django.conf import settings
-from django.http.response import JsonResponse
-from django.utils.deprecation import MiddlewareMixin
-from .tools import get_user_model_keycloak, set_profile
-from .keycloak import KeycloakOpenID
-from keycloak.exceptions import KeycloakInvalidTokenError
-from rest_framework.exceptions import PermissionDenied, AuthenticationFailed, NotAuthenticated
-from django.contrib.auth import get_user_model
-from django_keycloak.models import keycloakUserAbstract
-from django.contrib.auth import login
-from django.contrib.auth import logout
-
-
-class KeycloakMiddleware(MiddlewareMixin):
-
-    def __init__(self, get_response):
-        """
-        :param get_response:
-        """
-
-        self.config = settings.KEYCLOAK
-
-        # Read configurations
-        try:
-            self.server_url = self.config['SERVER_URL']
-            self.client_id = self.config['CLIENT_ID']
-            self.audience_client = self.config.get(
-                'AUDIENCE_CLIENT', self.client_id)
-            self.realm = self.config['REALM_NAME']
-        except KeyError as e:
-            raise Exception(
-                "KEYCLOAK_SERVER_URL, KEYCLOAK_CLIENT_ID or KEYCLOAK_REALM not found.")
-
-        self.client_secret_key = self.config.get('CLIENT_SECRET_KEY', None)
-        self.client_public_key = self.config.get('PUBLIC_KEY', None)
-        self.default_access = self.config.get('DEFAULT_ACCESS', "DENY")
-        self.method_validate_token = self.config.get(
-            'METHOD_VALIDATE_TOKEN', "INTROSPECT")
-        self.keycloak_authorization_config = self.config.get(
-            'AUTHORIZATION_CONFIG', None)
-        self.client_id_valids = self.config.get('CLIENT_ID_VALIDS', [])
-        self.create_user_if_not_exist = self.config.get(
-            'CREATE_USER_IF_NOT_EXIST', False)
-        self.attributes_fillable = self.config.get('ATTRIBUTES_FILLABLE', None)
-        self.update_user_only_login = self.config.get(
-            'UPDATE_USER_ONLY_LOGIN', None)
-        self.method_create_user = self.config.get('CREATE_USER_METHOD', None)
-        self.public_key_validate = self.config.get(
-            'PUBLIC_KEY_VALIDATE', 'inter')
-
-        # Create Keycloak instance
-        self.keycloak = KeycloakOpenID(server_url=self.server_url,
-                                       client_id=self.client_id,
-                                       realm_name=self.realm,
-                                       client_secret_key=self.client_secret_key,
-                                       client_id_valids=self.client_id_valids)
-
-        # Read policies
-        if self.keycloak_authorization_config:
-            self.keycloak.load_authorization_config(
-                self.keycloak_authorization_config)
-
-        # Django
-        self.get_response = get_response
-
-    def __call__(self, request):
-        """
-        :param request:
-        :return:
-        """
-        return self.get_response(request)
-
-    def process_view(self, request, view_func, view_args, view_kwargs):
-        """
-        Validate only the token introspect.
-        :param request: django request
-        :param view_func:
-        :param view_args: view args
-        :param view_kwargs: view kwargs
-        :return:
-        """
-
-        if 'HTTP_AUTHORIZATION' not in request.META:
-            return None
-
-        token = request.META.get('HTTP_AUTHORIZATION')
-        self.realm = self.config['REALM_NAME']
-
-        try:
-            user_groups, user_permissions, user_info = self.keycloak.get_roles_permissions_user(token.replace('Bearer ', ''),
-                                                                                                public_key_validate=self.public_key_validate,
-                                                                                                method_token_info=self.method_validate_token.lower(),
-                                                                                                key=self.client_public_key, audience=self.audience_client)
-        except KeycloakInvalidTokenError as e:
-            logout(request=request)
-            return JsonResponse({"detail": AuthenticationFailed.default_detail},
-                                status=AuthenticationFailed.status_code)
-
-        UserModel = get_user_model()
-
-        try:
-            print(user_info['sub'])
-            user = UserModel.objects.get(id=user_info['sub'])
-            print(user)
-            print(user_groups)
-            print(user_permissions)
-            user.last_login = timezone.now()
-            user.groups = user_groups
-            user.permissions = user_permissions
-            user.save()
-            # if self.update_user_only_login and request.get_full_path() == self.update_user_only_login:
-            #     set_profile(user, user_groups, user_permissions)
-
-        except UserModel.DoesNotExist:
-            # if self.method_create_user and self.method_create_user.to == 'KAFKA':
-            #     return JsonResponse({"detail": AuthenticationFailed.default_detail},
-            #                     status=AuthenticationFailed.status_code)
-            # update_profile = False
-            payload = {}
-            for config in self.attributes_fillable:
-                # if config in ["permissions", "groups"]:
-                #     update_profile = True
-                #     continue
-                if isinstance(config, tuple):
-                    payload[config[0]] = user_info[config[1]]
-                    continue
-                payload[config] = user_info[config]
-            user = None
-            if self.create_user_if_not_exist:
-                user = UserModel(**payload)
-                # if update_profile:
-                #     set_profile(user, user_groups, user_permissions)
-                # user.save()
-                user.last_login = timezone.now()
-                user.groups = user_groups
-                user.permissions = user_permissions
-                user.save()
-            if user:
-                login(request, user)
-            else:
-                User = get_user_model_keycloak()
-                user = User(**payload)
-                user.groups = user_groups
-                user.permissions = user_permissions
-                # if update_profile and isinstance(user, keycloakUserAbstract):
-                #     user.permissions = user_permissions
-                #     user.groups = user_groups
-
-        request.user = user
-
-        if self.default_access == "DENY" and not user_permissions and not user_groups:
-            # User Permission Denied
-            return JsonResponse({"detail": PermissionDenied.default_detail},
-                                status=PermissionDenied.status_code)
-        return None
-
-    @property
-    def keycloak(self):
-        return self._keycloak
-
-    @keycloak.setter
-    def keycloak(self, value):
-        self._keycloak = value
-
-    @property
-    def config(self):
-        return self._config
-
-    @config.setter
-    def config(self, value):
-        self._config = value
-
-    @property
-    def server_url(self):
-        return self._server_url
-
-    @server_url.setter
-    def server_url(self, value):
-        self._server_url = value
-
-    @property
-    def update_user_only_login(self):
-        return self._update_user_only_login
-
-    @update_user_only_login.setter
-    def update_user_only_login(self, value):
-        self._update_user_only_login = value
-
-    @property
-    def client_id(self):
-        return self._client_id
-
-    @client_id.setter
-    def client_id(self, value):
-        self._client_id = value
-
-    @property
-    def create_user_if_not_exist(self):
-        return self._create_user_ifnotexist
-
-    @create_user_if_not_exist.setter
-    def create_user_if_not_exist(self, value):
-        self._create_user_ifnotexist = value
-
-    @property
-    def attributes_fillable(self):
-        return self._atributes_fillable
-
-    @attributes_fillable.setter
-    def attributes_fillable(self, value):
-        self._atributes_fillable = value
-
-    @property
-    def client_id_valids(self):
-        return self._client_id_valids
-
-    @client_id_valids.setter
-    def client_id_valids(self, value):
-        self._client_id_valids = value
-
-    @property
-    def audience_client(self):
-        return self._audience_client
-
-    @audience_client.setter
-    def audience_client(self, value):
-        self._audience_client = value
-
-    @property
-    def client_secret_key(self):
-        return self._client_secret_key
-
-    @client_secret_key.setter
-    def client_secret_key(self, value):
-        self._client_secret_key = value
-
-    @property
-    def client_public_key(self):
-        return self._client_public_key
-
-    @client_public_key.setter
-    def client_public_key(self, value):
-        self._client_public_key = value
-
-    @property
-    def realm(self):
-        return self._realm
-
-    @realm.setter
-    def realm(self, value):
-        self._realm = value
-
-    @property
-    def keycloak_authorization_config(self):
-        return self._keycloak_authorization_config
-
-    @keycloak_authorization_config.setter
-    def keycloak_authorization_config(self, value):
-        self._keycloak_authorization_config = value
-
-    @property
-    def method_validate_token(self):
-        return self._method_validate_token
-
-    @method_validate_token.setter
-    def method_validate_token(self, value):
-        self._method_validate_token = value
-
-    @property
-    def method_create_user(self):
-        return self._method_create_user
-
-    @method_create_user.setter
-    def method_create_user(self, value):
-        self._method_create_user = value
+# -*- coding: utf-8 -*-
+from django.utils import timezone
+from django.conf import settings
+from django.http.response import JsonResponse
+from django.utils.deprecation import MiddlewareMixin
+from .tools import fill_user_model_keycloak, get_user_model_keycloak, set_profile
+from .keycloak import KeycloakOpenID
+from keycloak.exceptions import KeycloakInvalidTokenError
+from rest_framework.exceptions import PermissionDenied, AuthenticationFailed, NotAuthenticated
+from django.contrib.auth import get_user_model
+from django_keycloak.models import keycloakUserAbstract
+from django.contrib.auth import login
+from django.contrib.auth import logout
+
+
+class KeycloakMiddleware(MiddlewareMixin):
+
+    def __init__(self, get_response):
+        """
+        :param get_response:
+        """
+
+        self.config = settings.KEYCLOAK
+
+        # Read configurations
+        try:
+            self.server_url = self.config['SERVER_URL']
+            self.client_id = self.config['CLIENT_ID']
+            self.audience_client = self.config.get(
+                'AUDIENCE_CLIENT', self.client_id)
+            self.realm = self.config['REALM_NAME']
+        except KeyError as e:
+            raise Exception(
+                "KEYCLOAK_SERVER_URL, KEYCLOAK_CLIENT_ID or KEYCLOAK_REALM not found.")
+
+        self.client_secret_key = self.config.get('CLIENT_SECRET_KEY', None)
+        self.client_public_key = self.config.get('PUBLIC_KEY', None)
+        self.default_access = self.config.get('DEFAULT_ACCESS', "DENY")
+        self.method_validate_token = self.config.get(
+            'METHOD_VALIDATE_TOKEN', "INTROSPECT")
+        self.keycloak_authorization_config = self.config.get(
+            'AUTHORIZATION_CONFIG', None)
+        self.create_user_if_not_exist = self.config.get(
+            'CREATE_USER_IF_NOT_EXIST', False)
+        self.attributes_fillable = self.config.get('ATTRIBUTES_FILLABLE', None)
+        self.public_key_validate = self.config.get(
+            'PUBLIC_KEY_VALIDATE', 'inter')
+
+        # Create Keycloak instance
+        self.keycloak = KeycloakOpenID(server_url=self.server_url,
+                                       client_id=self.client_id,
+                                       realm_name=self.realm,
+                                       client_secret_key=self.client_secret_key)
+
+        # Read policies
+        if self.keycloak_authorization_config:
+            self.keycloak.load_authorization_config(
+                self.keycloak_authorization_config)
+
+        # Django
+        self.get_response = get_response
+
+    def __call__(self, request):
+        """
+        :param request:
+        :return:
+        """
+        return self.get_response(request)
+
+    def process_view(self, request, view_func, view_args, view_kwargs):
+        """
+        Validate only the token introspect.
+        :param request: django request
+        :param view_func:
+        :param view_args: view args
+        :param view_kwargs: view kwargs
+        :return:
+        """
+        # logout(request)
+
+        if 'HTTP_AUTHORIZATION' not in request.META:
+            return None
+
+        token = request.META.get('HTTP_AUTHORIZATION')
+        self.realm = self.config['REALM_NAME']
+
+        try:
+            user_groups, user_permissions, user_info = self.keycloak.get_roles_permissions_user(token.replace('Bearer ', ''),
+                                                                                                public_key_validate=self.public_key_validate,
+                                                                                                method_token_info=self.method_validate_token.lower(),
+                                                                                                key=self.client_public_key, audience=self.audience_client)
+        except KeycloakInvalidTokenError as e:
+            logout(request=request)
+            return JsonResponse({"detail": AuthenticationFailed.default_detail},
+                                status=AuthenticationFailed.status_code)
+
+        UserModel = get_user_model()
+
+        try:
+            user = UserModel.objects.get(id=user_info['sub'])
+            user = set_profile(user=user, groups=user_groups, permissions=user_permissions, user_info=user_info)
+
+            login(request, user)
+        except UserModel.DoesNotExist:
+            payload = {}
+            for config in self.attributes_fillable:
+                if isinstance(config, tuple):
+                    payload[config[0]] = user_info[config[1]]
+                    continue
+                payload[config] = user_info[config]
+            user = None
+            if self.create_user_if_not_exist:
+                user = UserModel(**payload)
+                user = set_profile(user=user, groups=user_groups, permissions=user_permissions, user_info=user_info)
+            if user:
+                login(request, user)
+            else:
+                User = get_user_model_keycloak()
+                user = User(**payload)
+                user.groups = user_groups
+                user.permissions = user_permissions
+                fill_user_model_keycloak(user=user, user_info=user_info)
+
+        request.user = user
+
+        if self.default_access == "DENY" and (not user_permissions or not user_groups):
+            # User Permission Denied
+            return JsonResponse({"detail": PermissionDenied.default_detail},
+                                status=PermissionDenied.status_code)
+        return None
+
+    @property
+    def keycloak(self):
+        return self._keycloak
+
+    @keycloak.setter
+    def keycloak(self, value):
+        self._keycloak = value
+
+    @property
+    def config(self):
+        return self._config
+
+    @config.setter
+    def config(self, value):
+        self._config = value
+
+    @property
+    def server_url(self):
+        return self._server_url
+
+    @server_url.setter
+    def server_url(self, value):
+        self._server_url = value
+
+    @property
+    def client_id(self):
+        return self._client_id
+
+    @client_id.setter
+    def client_id(self, value):
+        self._client_id = value
+
+    @property
+    def create_user_if_not_exist(self):
+        return self._create_user_ifnotexist
+
+    @create_user_if_not_exist.setter
+    def create_user_if_not_exist(self, value):
+        self._create_user_ifnotexist = value
+
+    @property
+    def attributes_fillable(self):
+        return self._atributes_fillable
+
+    @attributes_fillable.setter
+    def attributes_fillable(self, value):
+        self._atributes_fillable = value
+
+    @property
+    def audience_client(self):
+        return self._audience_client
+
+    @audience_client.setter
+    def audience_client(self, value):
+        self._audience_client = value
+
+    @property
+    def client_secret_key(self):
+        return self._client_secret_key
+
+    @client_secret_key.setter
+    def client_secret_key(self, value):
+        self._client_secret_key = value
+
+    @property
+    def client_public_key(self):
+        return self._client_public_key
+
+    @client_public_key.setter
+    def client_public_key(self, value):
+        self._client_public_key = value
+
+    @property
+    def realm(self):
+        return self._realm
+
+    @realm.setter
+    def realm(self, value):
+        self._realm = value
+
+    @property
+    def keycloak_authorization_config(self):
+        return self._keycloak_authorization_config
+
+    @keycloak_authorization_config.setter
+    def keycloak_authorization_config(self, value):
+        self._keycloak_authorization_config = value
+
+    @property
+    def method_validate_token(self):
+        return self._method_validate_token
+
+    @method_validate_token.setter
+    def method_validate_token(self, value):
+        self._method_validate_token = value
+
+    @property
+    def method_create_user(self):
+        return self._method_create_user
+
+    @method_create_user.setter
+    def method_create_user(self, value):
+        self._method_create_user = value
```

### Comparing `keycloak_django-0.1.0/django_keycloak/security.py` & `keycloak_django-1.0.0/src/keycloak_django/security.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,69 @@
-from rest_framework import permissions
-from django.core.exceptions import PermissionDenied
-from typing import List
-import inspect
-from django.contrib.auth.models import Group, Permission
-
-class ValidatePermissions(permissions.BasePermission):
-    """
-    Allows access only to authenticated users.
-    """
-
-    def _has_list_has_permissions(self, permissions_list: List, request, view):
-        for per in permissions_list:
-            if not (
-                    per().has_permission(request, view) if (
-                            callable(per) and 'has_permission' in dir(per())) else request.user.has_perm(per)):
-                return False
-        return True
-
-    def _validate_permission(self, permission, request, view):
-        if callable(permission) and 'has_permission' in dir(permission()):
-            return permission().has_permission(request, view)
-
-        if isinstance(permission, str):
-            return request.user.has_perm(permission)
-
-        if not permission and isinstance(permission, List):
-            return True
-
-        if permission and isinstance(permission, List):
-            return self._has_list_has_permissions(permission, request, view)
-
-        return False
-
-    def has_permission(self, request, view):
-        valid = False
-        if request.user and request.user.is_authenticated and hasattr(view,
-                                                                      'validate_permissions') and view.validate_permissions:
-            if isinstance(view.validate_permissions, str) or isinstance(view.validate_permissions, List) or callable(
-                    view.validate_permissions) and 'has_permission' in dir(view.validate_permissions()):
-                permission = view.validate_permissions
-            else:
-                if not view.action in view.validate_permissions:
-                    return True
-                permission = view.validate_permissions[view.action]
-            valid = self._validate_permission(permission, request, view)
-
-        # In case the 403 handler should be called raise the exception
-        if hasattr(view, 'raise_exception_validate') and view.raise_exception_validate and not valid:
-            raise PermissionDenied
-        return valid
-
-
-def single_permission(permission: str):
-    class C(permissions.BasePermission):
-        def has_permission(self, request, view):
-            if request.user and request.user.is_authenticated:
-                return request.user.has_perm(permission)
-            return False
-
-    return C
-
-
-def single_group(group: str):
-    class C(permissions.BasePermission):
-        def has_permission(self, request, view):
-            if request.user and request.user.is_authenticated:
-                return group in [g.name for g in request.user.groups.all()]
-            return False
-
+from rest_framework import permissions
+from django.core.exceptions import PermissionDenied
+from typing import List
+
+class ValidatePermissions(permissions.BasePermission):
+    """
+    Allows access only to authenticated users.
+    """
+
+    def _has_list_has_permissions(self, permissions_list: List, request, view):
+        for per in permissions_list:
+            if not (
+                    per().has_permission(request, view) if (
+                            callable(per) and 'has_permission' in dir(per())) else request.user.has_perm(per)):
+                return False
+        return True
+
+    def _validate_permission(self, permission, request, view):
+        if callable(permission) and 'has_permission' in dir(permission()):
+            return permission().has_permission(request, view)
+
+        if isinstance(permission, str):
+            return request.user.has_perm(permission)
+
+        if not permission and isinstance(permission, List):
+            return True
+
+        if permission and isinstance(permission, List):
+            return self._has_list_has_permissions(permission, request, view)
+
+        return False
+
+    def has_permission(self, request, view):
+        valid = False
+        if request.user and request.user.is_authenticated and hasattr(view,
+                                                                      'validate_permissions') and view.validate_permissions:
+            if isinstance(view.validate_permissions, str) or isinstance(view.validate_permissions, List) or callable(
+                    view.validate_permissions) and 'has_permission' in dir(view.validate_permissions()):
+                permission = view.validate_permissions
+            else:
+                if not view.action in view.validate_permissions:
+                    return True
+                permission = view.validate_permissions[view.action]
+            valid = self._validate_permission(permission, request, view)
+
+        # In case the 403 handler should be called raise the exception
+        if hasattr(view, 'raise_exception_validate') and view.raise_exception_validate and not valid:
+            raise PermissionDenied
+        return valid
+
+
+def single_permission(permission: str):
+    class C(permissions.BasePermission):
+        def has_permission(self, request, view):
+            if request.user and request.user.is_authenticated:
+                return request.user.has_perm(permission)
+            return False
+
+    return C
+
+
+def single_group(group: str):
+    class C(permissions.BasePermission):
+        def has_permission(self, request, view):
+            if request.user and request.user.is_authenticated:
+                return group in [g.name for g in request.user.groups.all()]
+            return False
+
     return C
```

### Comparing `keycloak_django-0.1.0/django_keycloak/services/client_repository.py` & `keycloak_django-1.0.0/src/keycloak_django/services/client_repository.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from django_keycloak.keycloak import get_default_master_keycloak_admin
-
-
-def create_client_by_app_owner(client_model, realm_model, id=None):
-    keycloak_admin = get_default_master_keycloak_admin()
-    payload = dict(client_model.base_config)
-    if id:
-        payload['id'] = str(id)
-    payload['clientId'] = client_model.client_id
-    payload['name'] = client_model.name
-    payload['rootUrl'] = client_model.rootUrl
-    payload['baseUrl'] = client_model.baseUrl
-    payload['enabled'] = client_model.active
-    payload['publicClient'] = not client_model.is_api
-    if not client_model.is_api:
-        payload['redirectUris'] = client_model.redirectUris.split(",")
-        payload['webOrigins'] = client_model.webOrigins.split(",")
-        payload['attributes']['post.logout.redirect.uris'] = "##".join(client_model.logoutUris.split(","))
-    keycloak_admin.create_client_by_realm_name(realm_name=realm_model.realm, payload=payload)
-    if client_model.is_api:
-        keycloak_admin.set_realm_name(realm_name=realm_model.realm)
-        client_id = keycloak_admin.get_client_id(client_model.client_id)
-        keycloak_admin.generate_client_secrets(client_id=client_id)
-
-
-def delete_client_by_app_owner(client_model, realm_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=realm_model.realm)
-    client_id = keycloak_admin.get_client_id(client_model.client_id)
+from django_keycloak.keycloak import get_default_master_keycloak_admin
+
+
+def create_client_by_app_owner(client_model, realm_model, id=None):
+    keycloak_admin = get_default_master_keycloak_admin()
+    payload = dict(client_model.base_config)
+    if id:
+        payload['id'] = str(id)
+    payload['clientId'] = client_model.client_id
+    payload['name'] = client_model.name
+    payload['rootUrl'] = client_model.rootUrl
+    payload['baseUrl'] = client_model.baseUrl
+    payload['enabled'] = client_model.active
+    payload['publicClient'] = not client_model.is_api
+    if not client_model.is_api:
+        payload['redirectUris'] = client_model.redirectUris.split(",")
+        payload['webOrigins'] = client_model.webOrigins.split(",")
+        payload['attributes']['post.logout.redirect.uris'] = "##".join(client_model.logoutUris.split(","))
+    keycloak_admin.create_client_by_realm_name(realm_name=realm_model.realm, payload=payload)
+    if client_model.is_api:
+        keycloak_admin.set_realm_name(realm_name=realm_model.realm)
+        client_id = keycloak_admin.get_client_id(client_model.client_id)
+        keycloak_admin.generate_client_secrets(client_id=client_id)
+
+
+def delete_client_by_app_owner(client_model, realm_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=realm_model.realm)
+    client_id = keycloak_admin.get_client_id(client_model.client_id)
     keycloak_admin.delete_client(client_id=client_id)
```

### Comparing `keycloak_django-0.1.0/django_keycloak/services/permission_repository.py` & `keycloak_django-1.0.0/src/keycloak_django/services/permission_repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from django_keycloak.keycloak import get_default_master_keycloak_admin
-
-
-def get_permissions_by_app(apps_owners_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=apps_owners_model.owner.name)
-    roles = keycloak_admin.get_client_roles(client_id=apps_owners_model.id)
-    return [p for p in roles if p['name'].endswith('_permission')]
-
-
-def create_permission_by_app(earp_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(
-        realm_name=earp_model.app_role.apps_owner.owner.name)
-    permissions = get_permissions_by_app(earp_model.app_role.apps_owner)
-    permissions_names = [p['name'] for p in permissions]
-    name = earp_model.endpoint.name
-    name = name.replace(' ', '_').lower()
-    all_permissions = [f'{name}_allow_read_permission',
-                       f'{name}_allow_add_permission',
-                       f'{name}_allow_delete_permission',
-                       f'{name}_allow_update_permission',
-                       f'{name}_allow_execute_permission']
-    permissions_create = [
-        p for p in all_permissions if p not in permissions_names]
-    for p in permissions_create:
-        payload = {
-            "name": p,
-            "description": p.replace("_", " "),
-            "clientRole": True,
-            "attributes": {
-                "is_editable": [False],
-                "is_role": [False]
-            }
-        }
-        client_role_id = keycloak_admin.get_client_id(
-            client_id=earp_model.app_role.apps_owner.app.client_id)
-        keycloak_admin.create_client_role(
-            client_role_id=client_role_id, payload=payload)
-
-
-def add_permission_by_role_app(earp_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(
-        realm_name=earp_model.app_role.apps_owner.owner.name)
-    permissions = get_permissions_by_app(earp_model.app_role.apps_owner)
-    name = earp_model.endpoint.name
-    name = name.replace(' ', '_').lower()
-    all_permissions = []
-    if earp_model.allow_read:
-        all_permissions.append(f'{name}_allow_read_permission')
-    if earp_model.allow_add:
-        all_permissions.append(f'{name}_allow_add_permission')
-    if earp_model.allow_delete:
-        all_permissions.append(f'{name}_allow_delete_permission')
-    if earp_model.allow_update:
-        all_permissions.append(f'{name}_allow_update_permission')
-    if earp_model.allow_execute:
-        all_permissions.append(f'{name}_allow_execute_permission')
-
-    permissions_append = [
-        p for p in permissions if p['name'] in all_permissions]
-    client_role_id = keycloak_admin.get_client_id(
-        client_id=earp_model.app_role.apps_owner.app.client_id)
-    role_name = earp_model.app_role.role.name.replace(' ', '_').lower()
-    delete_roles = keycloak_admin.get_composite_client_roles_to_role(
-        client_role_id=client_role_id, role_name=f'{role_name}_role')
-    delete_roles = [r for r in delete_roles if r['name'].startswith(f'{name}_allow')]
-    if delete_roles:
-        keycloak_admin.remove_composite_client_roles_to_role(
-            client_role_id=client_role_id, role_name=f'{role_name}_role', roles=delete_roles)
-    keycloak_admin.add_composite_client_roles_to_role(client_role_id=client_role_id, role_name=f'{role_name}_role', roles=permissions_append)
-
-
-def delete_permission_by_app(earp_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(
-        realm_name=earp_model.app_role.apps_owner.owner.name)
-    permissions = get_permissions_by_app(earp_model.app_role.apps_owner)
-    permissions_names = [p['name'] for p in permissions]
-    name = earp_model.endpoint.name
-    all_permissions = [f'{name}_allow_read_permission',
-                       f'{name}_allow_add_permission',
-                       f'{name}_allow_delete_permission',
-                       f'{name}_allow_update_permission',
-                       f'{name}_allow_execute_permission']
-    permissions_delete = [
-        p for p in permissions_names if p in all_permissions]
-    client_role_id = keycloak_admin.get_client_id(
-        client_id=earp_model.app.client_id)
-    for p in permissions_delete:
-        keycloak_admin.delete_client_role(client_role_id=client_role_id, role_name=p)
-
+from django_keycloak.keycloak import get_default_master_keycloak_admin
+
+
+def get_permissions_by_app(apps_owners_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=apps_owners_model.owner.realm)
+    roles = keycloak_admin.get_client_roles(client_id=apps_owners_model.id)
+    return [p for p in roles if p['name'].endswith('_permission')]
+
+
+def create_permission_by_app(earp_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(
+        realm_name=earp_model.app_role.apps_owner.owner.realm)
+    permissions = get_permissions_by_app(earp_model.app_role.apps_owner)
+    permissions_names = [p['name'] for p in permissions]
+    name = earp_model.endpoint.name
+    name = name.replace(' ', '_').lower()
+    all_permissions = [f'{name}_allow_read_permission',
+                       f'{name}_allow_add_permission',
+                       f'{name}_allow_delete_permission',
+                       f'{name}_allow_update_permission',
+                       f'{name}_allow_execute_permission']
+    permissions_create = [
+        p for p in all_permissions if p not in permissions_names]
+    for p in permissions_create:
+        payload = {
+            "name": p,
+            "description": p.replace("_", " "),
+            "clientRole": True,
+            "attributes": {
+                "is_editable": [False],
+                "is_role": [False]
+            }
+        }
+        client_role_id = keycloak_admin.get_client_id(
+            client_id=earp_model.app_role.apps_owner.app.client_id)
+        keycloak_admin.create_client_role(
+            client_role_id=client_role_id, payload=payload)
+
+
+def add_permission_by_role_app(earp_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(
+        realm_name=earp_model.app_role.apps_owner.owner.realm)
+    permissions = get_permissions_by_app(earp_model.app_role.apps_owner)
+    name = earp_model.endpoint.name
+    name = name.replace(' ', '_').lower()
+    all_permissions = []
+    if earp_model.allow_read:
+        all_permissions.append(f'{name}_allow_read_permission')
+    if earp_model.allow_add:
+        all_permissions.append(f'{name}_allow_add_permission')
+    if earp_model.allow_delete:
+        all_permissions.append(f'{name}_allow_delete_permission')
+    if earp_model.allow_update:
+        all_permissions.append(f'{name}_allow_update_permission')
+    if earp_model.allow_execute:
+        all_permissions.append(f'{name}_allow_execute_permission')
+
+    permissions_append = [
+        p for p in permissions if p['name'] in all_permissions]
+    client_role_id = keycloak_admin.get_client_id(
+        client_id=earp_model.app_role.apps_owner.app.client_id)
+    role_name = earp_model.app_role.role.name.replace(' ', '_').lower()
+    delete_roles = keycloak_admin.get_composite_client_roles_to_role(
+        client_role_id=client_role_id, role_name=f'{role_name}_role')
+    delete_roles = [r for r in delete_roles if r['name'].startswith(f'{name}_allow')]
+    if delete_roles:
+        keycloak_admin.remove_composite_client_roles_to_role(
+            client_role_id=client_role_id, role_name=f'{role_name}_role', roles=delete_roles)
+    keycloak_admin.add_composite_client_roles_to_role(client_role_id=client_role_id, role_name=f'{role_name}_role', roles=permissions_append)
+
+
+def delete_permission_by_app(earp_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(
+        realm_name=earp_model.app_role.apps_owner.owner.realm)
+    permissions = get_permissions_by_app(earp_model.app_role.apps_owner)
+    permissions_names = [p['name'] for p in permissions]
+    name = earp_model.endpoint.name
+    all_permissions = [f'{name}_allow_read_permission',
+                       f'{name}_allow_add_permission',
+                       f'{name}_allow_delete_permission',
+                       f'{name}_allow_update_permission',
+                       f'{name}_allow_execute_permission']
+    permissions_delete = [
+        p for p in permissions_names if p in all_permissions]
+    client_role_id = keycloak_admin.get_client_id(
+        client_id=earp_model.app.client_id)
+    for p in permissions_delete:
+        keycloak_admin.delete_client_role(client_role_id=client_role_id, role_name=p)
+
```

### Comparing `keycloak_django-0.1.0/django_keycloak/services/realm_repository.py` & `keycloak_django-1.0.0/src/keycloak_django/services/realm_repository.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from django_keycloak.keycloak import get_default_master_keycloak_admin
-
-
-def create_realm_by_owner(realm_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    payload = dict(realm_model.base_config)
-    payload['id'] = str(realm_model.id)
-    payload['realm'] = realm_model.realm
-    if realm_model.email_realm_config:
-        payload['smtpServer'] = {
-            "replyToDisplayName": realm_model.email_realm_config.replyToDisplayName,
-            "starttls": realm_model.email_realm_config.starttls,
-            "auth": realm_model.email_realm_config.auth,
-            "envelopeFrom": realm_model.email_realm_config.envelopeFrom,
-            "ssl": realm_model.email_realm_config.ssl,
-            "password": realm_model.email_realm_config.password,
-            "port": realm_model.email_realm_config.port,
-            "replyTo": realm_model.email_realm_config.replyTo,
-            "host": realm_model.email_realm_config.host,
-            "from": realm_model.email_realm_config.from_email,
-            "fromDisplayName": realm_model.email_realm_config.fromDisplayName,
-            "user": realm_model.email_realm_config.user
-        }
-    else:
-        payload.pop('smtpServer')
-
-    keycloak_admin.create_realm(payload=payload)
-
-
-def update_realm_by_owner(realm_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    payload = dict(realm_model.base_config)
-    payload.pop('id')
-    payload.pop('realm')
-    payload['smtpServer'] = {}
-    keycloak_admin.update_realm(realm_name=realm_model.realm, payload=payload)
-    if realm_model.email_realm_config:
-        payload['smtpServer'] = {
-            "replyToDisplayName": realm_model.email_realm_config.replyToDisplayName,
-            "starttls": realm_model.email_realm_config.starttls,
-            "auth": realm_model.email_realm_config.auth,
-            "envelopeFrom": realm_model.email_realm_config.envelopeFrom,
-            "ssl": realm_model.email_realm_config.ssl,
-            "password": realm_model.email_realm_config.password,
-            "port": realm_model.email_realm_config.port,
-            "replyTo": realm_model.email_realm_config.replyTo,
-            "host": realm_model.email_realm_config.host,
-            "from": realm_model.email_realm_config.from_email,
-            "fromDisplayName": realm_model.email_realm_config.fromDisplayName,
-            "user": realm_model.email_realm_config.user
-        }
-        keycloak_admin.update_realm(realm_name=realm_model.realm, payload=payload)
-
-
-def delete_realm_by_owner(realm_model):
-    keycloak_admin = get_default_master_keycloak_admin()
+from django_keycloak.keycloak import get_default_master_keycloak_admin
+
+
+def create_realm_by_owner(realm_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    payload = dict(realm_model.base_config)
+    payload['id'] = str(realm_model.id)
+    payload['realm'] = realm_model.realm
+    if realm_model.email_realm_config:
+        payload['smtpServer'] = {
+            "replyToDisplayName": realm_model.email_realm_config.replyToDisplayName,
+            "starttls": realm_model.email_realm_config.starttls,
+            "auth": realm_model.email_realm_config.auth,
+            "envelopeFrom": realm_model.email_realm_config.envelopeFrom,
+            "ssl": realm_model.email_realm_config.ssl,
+            "password": realm_model.email_realm_config.password,
+            "port": realm_model.email_realm_config.port,
+            "replyTo": realm_model.email_realm_config.replyTo,
+            "host": realm_model.email_realm_config.host,
+            "from": realm_model.email_realm_config.from_email,
+            "fromDisplayName": realm_model.email_realm_config.fromDisplayName,
+            "user": realm_model.email_realm_config.user
+        }
+    else:
+        payload.pop('smtpServer')
+
+    keycloak_admin.create_realm(payload=payload)
+
+
+def update_realm_by_owner(realm_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    payload = dict(realm_model.base_config)
+    payload.pop('id')
+    payload.pop('realm')
+    payload['smtpServer'] = {}
+    keycloak_admin.update_realm(realm_name=realm_model.realm, payload=payload)
+    if realm_model.email_realm_config:
+        payload['smtpServer'] = {
+            "replyToDisplayName": realm_model.email_realm_config.replyToDisplayName,
+            "starttls": realm_model.email_realm_config.starttls,
+            "auth": realm_model.email_realm_config.auth,
+            "envelopeFrom": realm_model.email_realm_config.envelopeFrom,
+            "ssl": realm_model.email_realm_config.ssl,
+            "password": realm_model.email_realm_config.password,
+            "port": realm_model.email_realm_config.port,
+            "replyTo": realm_model.email_realm_config.replyTo,
+            "host": realm_model.email_realm_config.host,
+            "from": realm_model.email_realm_config.from_email,
+            "fromDisplayName": realm_model.email_realm_config.fromDisplayName,
+            "user": realm_model.email_realm_config.user
+        }
+        keycloak_admin.update_realm(realm_name=realm_model.realm, payload=payload)
+
+
+def delete_realm_by_owner(realm_model):
+    keycloak_admin = get_default_master_keycloak_admin()
     keycloak_admin.delete_realm(realm_name=realm_model.realm)
```

### Comparing `keycloak_django-0.1.0/django_keycloak/services/role_repository.py` & `keycloak_django-1.0.0/src/keycloak_django/services/role_repository.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from django_keycloak.keycloak import get_default_master_keycloak_admin
-
-
-def create_role_by_owner(role_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=role_model.owner.name)
-    payload = {
-        "id": str(role_model.id),
-        "name": role_model.role.name.replace(' ', '_').lower() + '_role',
-        "description": role_model.role.description,
-        "clientRole": False,
-        "attributes": {
-            "is_editable": [role_model.role.is_editable],
-            "is_role": [True]
-        }
-    }
-    keycloak_admin.create_realm_role(payload=payload)
-
-
-def create_role_by_app(role_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=role_model.apps_owner.owner.name)
-    payload = {
-        "id": str(role_model.id),
-        "name": role_model.role.name.replace(' ', '_').lower() + '_role',
-        "description": role_model.role.description,
-        "clientRole": True,
-        "attributes": {
-            "is_editable": [role_model.role.is_editable],
-            "is_role": [True]
-        }
-    }
-    client_role_id = keycloak_admin.get_client_id(
-        client_id=role_model.apps_owner.app.client_id)
-    keycloak_admin.create_client_role(
-        client_role_id=client_role_id, payload=payload)
-
-
-def delete_role_by_owner(role_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=role_model.owner.name)
-    keycloak_admin.delete_realm_role(role_name=f"{role_model.role.name.replace(' ', '_').lower()}_role")
-
-
-def delete_role_by_app(role_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=role_model.apps_owner.owner.name)
-    client_role_id = keycloak_admin.get_client_id(
-        client_id=role_model.apps_owner.app.client_id)
+from django_keycloak.keycloak import get_default_master_keycloak_admin
+
+
+def create_role_by_owner(role_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=role_model.owner.realm)
+    payload = {
+        "id": str(role_model.id),
+        "name": role_model.role.name.replace(' ', '_').lower() + '_role',
+        "description": role_model.role.description,
+        "clientRole": False,
+        "attributes": {
+            "is_editable": [role_model.role.is_editable],
+            "is_role": [True]
+        }
+    }
+    keycloak_admin.create_realm_role(payload=payload)
+
+
+def create_role_by_app(role_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=role_model.apps_owner.owner.realm)
+    payload = {
+        "id": str(role_model.id),
+        "name": role_model.role.name.replace(' ', '_').lower() + '_role',
+        "description": role_model.role.description,
+        "clientRole": True,
+        "attributes": {
+            "is_editable": [role_model.role.is_editable],
+            "is_role": [True]
+        }
+    }
+    client_role_id = keycloak_admin.get_client_id(
+        client_id=role_model.apps_owner.app.client_id)
+    keycloak_admin.create_client_role(
+        client_role_id=client_role_id, payload=payload)
+
+
+def delete_role_by_owner(role_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=role_model.owner.realm)
+    keycloak_admin.delete_realm_role(role_name=f"{role_model.role.name.replace(' ', '_').lower()}_role")
+
+
+def delete_role_by_app(role_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=role_model.apps_owner.owner.realm)
+    client_role_id = keycloak_admin.get_client_id(
+        client_id=role_model.apps_owner.app.client_id)
     keycloak_admin.delete_client_role(client_role_id=client_role_id,role_name=f"{role_model.role.name.replace(' ', '_').lower()}_role")
```

### Comparing `keycloak_django-0.1.0/django_keycloak/services/user_repository.py` & `keycloak_django-1.0.0/src/keycloak_django/services/user_repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,112 @@
-import json
-
-from django.db.models import QuerySet
-
-from django_keycloak.keycloak import get_default_master_keycloak_admin
-
-
-def get_base_user(user_model, password):
-    return {
-        "id": str(user_model.id),
-        "email": user_model.email,
-        "emailVerified": user_model.email_verified,
-        "enabled": True,
-        "firstName": user_model.first_name,
-        "lastName": user_model.last_name,
-        "username": user_model.username,
-        "attributes": {
-            "is_staff": user_model.is_staff,
-            "is_superuser": user_model.is_superuser
-        },
-        "credentials": [{
-            "type": "password",
-            "value": password,
-            "temporary": False
-        }]
-    }
-
-
-def create_user_by_owner(user_model, password):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
-    payload = get_base_user(user_model, password)
-    keycloak_admin.create_user(payload=payload)
-    return keycloak_admin.get_user_id(user_model.username)
-
-
-def create_user_by_master(user_model, password):
-    keycloak_admin = get_default_master_keycloak_admin()
-    payload = get_base_user(user_model, password)
-    keycloak_admin.create_user(payload=payload)
-
-
-def get_roles_representation(role_names, client_id, keycloak_admin):
-    roles_representations = keycloak_admin.get_client_roles(client_id=client_id)
-    return [r for r in roles_representations if r['name'] in role_names]
-
-
-def assign_client_role_to_user(user_model, role_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
-
-    if not isinstance(role_model, QuerySet):
-        roles = [f"{role_model.role.name.replace(' ', '_').lower()}_role"]
-    else:
-        roles = [f"{r.role.name.replace(' ', '_').lower()}_role" for r in role_model]
-
-    client_id = keycloak_admin.get_client_id(
-        client_id=role_model[0].apps_owner.app.client_id)
-    roles = get_roles_representation(role_names=roles,client_id=client_id,keycloak_admin=keycloak_admin)
-    keycloak_admin.assign_client_role(user_id=str(user_model.id), client_id=client_id, roles=roles)
-
-
-def get_base_business_unit(business_units_model):
-    business_unit_dict= {
-        "id" : business_units_model.id,
-        "name": business_units_model.name
-    }
-    return json.dumps(business_unit_dict)
-
-
-def get_attributes(user_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
-    user_representation = keycloak_admin.get_user(user_id=str(user_model.id))
-    if not 'attributes' in user_representation:
-        return {}
-    return user_representation['attributes']
-
-
-def assign_business_units_to_user(user_model, business_units):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
-    attributes = get_attributes(user_model)
-    # if not 'business_units' in attributes:
-    #     attributes['business_units'] = []
-    attributes['business_units'] = business_units
-    payload = {
-        "attributes": {
-            **attributes
-        }
-    }
-    keycloak_admin.update_user(user_id=str(user_model.id), payload=payload)
-
-
-def delete_business_units_to_user(user_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
-    attributes = get_attributes(user_model)
-    if 'business_units' in attributes:
-        attributes.pop('business_units')
-    payload = {
-        "attributes": {
-            **attributes
-        }
-    }
-    keycloak_admin.update_user(user_id=str(user_model.id), payload=payload)
-
-
-def delete_user_by_owner(user_model):
-    keycloak_admin = get_default_master_keycloak_admin()
-    print(user_model)
-    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
+import json
+
+from django.db.models import QuerySet
+
+from django_keycloak.keycloak import get_default_master_keycloak_admin
+
+
+def get_base_user(user_model, password):
+    return {
+        "id": str(user_model.id),
+        "email": user_model.email,
+        "emailVerified": user_model.email_verified,
+        "enabled": True,
+        "firstName": user_model.first_name,
+        "lastName": user_model.last_name,
+        "username": user_model.username,
+        "attributes": {
+            "is_staff": user_model.is_staff,
+            "is_superuser": user_model.is_superuser
+        },
+        "credentials": [{
+            "type": "password",
+            "value": password,
+            "temporary": False
+        }]
+    }
+
+
+def create_user_by_owner(user_model, password):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
+    payload = get_base_user(user_model, password)
+    keycloak_admin.create_user(payload=payload)
+    return keycloak_admin.get_user_id(user_model.username)
+
+
+def create_user_by_master(user_model, password):
+    keycloak_admin = get_default_master_keycloak_admin()
+    payload = get_base_user(user_model, password)
+    keycloak_admin.create_user(payload=payload)
+
+
+def get_roles_representation(role_names, client_id, keycloak_admin):
+    roles_representations = keycloak_admin.get_client_roles(client_id=client_id)
+    return [r for r in roles_representations if r['name'] in role_names]
+
+
+def assign_client_role_to_user(user_model, role_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
+
+    if not isinstance(role_model, QuerySet):
+        roles = [f"{role_model.role.name.replace(' ', '_').lower()}_role"]
+    else:
+        roles = [f"{r.role.name.replace(' ', '_').lower()}_role" for r in role_model]
+
+    client_id = keycloak_admin.get_client_id(
+        client_id=role_model[0].apps_owner.app.client_id)
+    roles = get_roles_representation(role_names=roles, client_id=client_id, keycloak_admin=keycloak_admin)
+    keycloak_admin.assign_client_role(user_id=str(user_model.id), client_id=client_id, roles=roles)
+
+
+def get_base_business_unit(business_units_model):
+    business_unit_dict = {
+        "id": business_units_model.id,
+        "name": business_units_model.name
+    }
+    return json.dumps(business_unit_dict)
+
+
+def get_attributes(user_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
+    user_representation = keycloak_admin.get_user(user_id=str(user_model.id))
+    if not 'attributes' in user_representation:
+        return {}
+    return user_representation['attributes']
+
+
+def assign_business_units_to_user(user_model, business_units):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
+    attributes = get_attributes(user_model)
+    # if not 'business_units' in attributes:
+    #     attributes['business_units'] = []
+    attributes['business_units'] = business_units
+    payload = {
+        "attributes": {
+            **attributes
+        }
+    }
+    keycloak_admin.update_user(user_id=str(user_model.id), payload=payload)
+
+
+def delete_business_units_to_user(user_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
+    attributes = get_attributes(user_model)
+    if 'business_units' in attributes:
+        attributes.pop('business_units')
+    payload = {
+        "attributes": {
+            **attributes
+        }
+    }
+    keycloak_admin.update_user(user_id=str(user_model.id), payload=payload)
+
+
+def delete_user_by_owner(user_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
     keycloak_admin.delete_user(user_id=user_model.id)
```

