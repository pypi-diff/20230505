# Comparing `tmp/garpix_company-2.7.0.tar.gz` & `tmp/garpix_company-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_company-2.7.0.tar", last modified: Thu May  4 14:33:26 2023, max compression
+gzip compressed data, was "garpix_company-2.7.1.tar", last modified: Fri May  5 07:23:46 2023, max compression
```

## Comparing `garpix_company-2.7.0.tar` & `garpix_company-2.7.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.997221 garpix_company-2.7.0/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-05-04 14:33:26.000000 garpix_company-2.7.0/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3893 2023-05-04 14:33:26.997074 garpix_company-2.7.0/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.992749 garpix_company-2.7.0/garpix_company/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2441 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3323 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.993768 garpix_company-2.7.0/garpix_company/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/admin/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.7.0/garpix_company/admin/company_invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/helpers.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.994070 garpix_company-2.7.0/garpix_company/managers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/managers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/managers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/managers/invite.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.994191 garpix_company-2.7.0/garpix_company/migrations/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/migrations/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.994289 garpix_company-2.7.0/garpix_company/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.994493 garpix_company-2.7.0/garpix_company/mixins/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/mixins/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.7.0/garpix_company/mixins/views/company_mixin.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.995044 garpix_company-2.7.0/garpix_company/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      222 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6003 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/models/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/models/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4095 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/models/user_company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/models/user_role.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.995609 garpix_company-2.7.0/garpix_company/permissions/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.7.0/garpix_company/permissions/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1035 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/permissions/company_admin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      656 2023-02-02 07:34:38.000000 garpix_company-2.7.0/garpix_company/permissions/company_owner.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.7.0/garpix_company/permissions/company_user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      420 2022-12-09 14:51:29.000000 garpix_company-2.7.0/garpix_company/permissions/invite_receiver.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.996259 garpix_company-2.7.0/garpix_company/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/serializers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5620 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/serializers/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/serializers/role.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.7.0/garpix_company/serializers/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      851 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/serializers/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.996457 garpix_company-2.7.0/garpix_company/services/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/services/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      609 2023-01-30 05:54:06.000000 garpix_company-2.7.0/garpix_company/services/role_service.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.7.0/garpix_company/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.7.0/garpix_company/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.7.0/garpix_company/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.996908 garpix_company-2.7.0/garpix_company/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.7.0/garpix_company/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5446 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/views/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2127 2023-02-06 10:05:38.000000 garpix_company-2.7.0/garpix_company/views/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3588 2023-05-04 14:33:02.000000 garpix_company-2.7.0/garpix_company/views/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-04 14:33:26.993419 garpix_company-2.7.0/garpix_company.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3893 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-05-04 14:33:26.000000 garpix_company-2.7.0/garpix_company.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-04 14:33:26.997263 garpix_company-2.7.0/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-04 14:33:26.000000 garpix_company-2.7.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.458270 garpix_company-2.7.1/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-05-05 07:23:46.000000 garpix_company-2.7.1/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3893 2023-05-05 07:23:46.458133 garpix_company-2.7.1/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.453843 garpix_company-2.7.1/garpix_company/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2441 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3323 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.454869 garpix_company-2.7.1/garpix_company/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/admin/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.7.1/garpix_company/admin/company_invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/helpers.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.455172 garpix_company-2.7.1/garpix_company/managers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/managers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/managers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/managers/invite.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.455281 garpix_company-2.7.1/garpix_company/migrations/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/migrations/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.455369 garpix_company-2.7.1/garpix_company/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.455561 garpix_company-2.7.1/garpix_company/mixins/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/mixins/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.7.1/garpix_company/mixins/views/company_mixin.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.456106 garpix_company-2.7.1/garpix_company/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-05-05 07:20:15.000000 garpix_company-2.7.1/garpix_company/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6008 2023-05-04 15:07:22.000000 garpix_company-2.7.1/garpix_company/models/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/models/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4101 2023-05-05 07:20:15.000000 garpix_company-2.7.1/garpix_company/models/user_company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.7.1/garpix_company/models/user_role.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.456679 garpix_company-2.7.1/garpix_company/permissions/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.7.1/garpix_company/permissions/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1035 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/permissions/company_admin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      706 2023-05-04 15:00:30.000000 garpix_company-2.7.1/garpix_company/permissions/company_owner.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.7.1/garpix_company/permissions/company_user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      420 2022-12-09 14:51:29.000000 garpix_company-2.7.1/garpix_company/permissions/invite_receiver.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.457347 garpix_company-2.7.1/garpix_company/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.7.1/garpix_company/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/serializers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5620 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/serializers/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.7.1/garpix_company/serializers/role.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.7.1/garpix_company/serializers/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      851 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/serializers/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.457540 garpix_company-2.7.1/garpix_company/services/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.7.1/garpix_company/services/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      609 2023-01-30 05:54:06.000000 garpix_company-2.7.1/garpix_company/services/role_service.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.7.1/garpix_company/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-05 07:21:06.000000 garpix_company-2.7.1/garpix_company/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.7.1/garpix_company/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.7.1/garpix_company/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.457967 garpix_company-2.7.1/garpix_company/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.7.1/garpix_company/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5446 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/views/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2127 2023-02-06 10:05:38.000000 garpix_company-2.7.1/garpix_company/views/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3588 2023-05-04 14:33:02.000000 garpix_company-2.7.1/garpix_company/views/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-05 07:23:46.454522 garpix_company-2.7.1/garpix_company.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3893 2023-05-05 07:23:46.000000 garpix_company-2.7.1/garpix_company.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-05-05 07:23:46.000000 garpix_company-2.7.1/garpix_company.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-05 07:23:46.000000 garpix_company-2.7.1/garpix_company.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-05 07:23:46.000000 garpix_company-2.7.1/garpix_company.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-05-05 07:23:46.000000 garpix_company-2.7.1/garpix_company.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-05-05 07:23:46.000000 garpix_company-2.7.1/garpix_company.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-05 07:23:46.458309 garpix_company-2.7.1/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-05 07:23:46.000000 garpix_company-2.7.1/setup.py
```

### Comparing `garpix_company-2.7.0/PKG-INFO` & `garpix_company-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_company
-Version: 2.7.0
+Version: 2.7.1
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.7.0/garpix_company/CHANGELOG.md` & `garpix_company-2.7.1/garpix_company/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/CONTRIBUTING.md` & `garpix_company-2.7.1/garpix_company/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/README.md` & `garpix_company-2.7.1/garpix_company/README.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/helpers.py` & `garpix_company-2.7.1/garpix_company/helpers.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/models/company.py` & `garpix_company-2.7.1/garpix_company/models/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import models
 from django.utils.translation import ugettext_lazy as _
 from django_fsm import FSMField, transition, can_proceed
 from django.contrib.auth import get_user_model
-
 from garpix_company.helpers import COMPANY_STATUS_ENUM
 from garpix_company.managers.company import CompanyActiveManager
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.apps import apps as django_apps
 
@@ -30,15 +29,15 @@
     bank_title = models.CharField(max_length=100, null=True, blank=True, verbose_name=_("Наименование банка"))
     bic = models.CharField(max_length=100, null=True, blank=True, verbose_name=_("БИК банка"))
     schet = models.CharField(max_length=50, null=True, blank=True, verbose_name=_("Номер счета"))
     korschet = models.CharField(max_length=50, null=True, blank=True, verbose_name=_("Кор. счет"))
     ur_address = models.CharField(max_length=300, verbose_name=_("Юридический адрес"))
     fact_address = models.CharField(max_length=300, verbose_name=_("Фактический адрес"))
     status = FSMField(default=COMPANY_STATUS.ACTIVE, choices=COMPANY_STATUS.CHOICES, verbose_name=_('Статус'))
-    participants = models.ManyToManyField(User, through='garpix_company.UserCompany',
+    participants = models.ManyToManyField(User, through=settings.GARPIX_USER_COMPANY_MODEL,
                                           verbose_name=_('Участники компании'))
     created_at = models.DateTimeField(auto_now_add=True, verbose_name=_('Дата создания'))
     updated_at = models.DateTimeField(auto_now=True, verbose_name=_('Дата изменения'))
     objects = models.Manager()
     active_objects = CompanyActiveManager()
 
     class Meta:
```

### Comparing `garpix_company-2.7.0/garpix_company/models/invite.py` & `garpix_company-2.7.1/garpix_company/models/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/models/user_company.py` & `garpix_company-2.7.1/garpix_company/models/user_company.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,18 +77,18 @@
         if role == CompanyRole.get_owner_role():
             return False, _('Нельзя сделать пользователя владельцем. Воспользуйтесь функционалом смены владельца')
         if role == CompanyRole.get_admin_role() and self.is_blocked:
             return False, _('Нельзя сделать администратором заблокированного пользователя')
         self.role = role
         self.save()
         return True, None
-
-
-class UserCompany(AbstractUserCompany):
-    pass
+#
+#
+# class UserCompany(AbstractUserCompany):
+#     pass
 
 
 def get_user_company_model():
     """
     Return the UserCompany model that is active in this project.
     """
     try:
```

### Comparing `garpix_company-2.7.0/garpix_company/models/user_role.py` & `garpix_company-2.7.1/garpix_company/models/user_role.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/permissions/company_admin.py` & `garpix_company-2.7.1/garpix_company/permissions/company_admin.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/serializers/company.py` & `garpix_company-2.7.1/garpix_company/serializers/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/serializers/invite.py` & `garpix_company-2.7.1/garpix_company/serializers/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/serializers/user_company.py` & `garpix_company-2.7.1/garpix_company/serializers/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/services/role_service.py` & `garpix_company-2.7.1/garpix_company/services/role_service.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/settings.py` & `garpix_company-2.7.1/garpix_company/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/setup.py` & `garpix_company-2.7.1/garpix_company/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.7.0',
+    version='2.7.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_company-2.7.0/garpix_company/urls.py` & `garpix_company-2.7.1/garpix_company/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/views/company.py` & `garpix_company-2.7.1/garpix_company/views/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/views/invite.py` & `garpix_company-2.7.1/garpix_company/views/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company/views/user_company.py` & `garpix_company-2.7.1/garpix_company/views/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/garpix_company.egg-info/PKG-INFO` & `garpix_company-2.7.1/garpix_company.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-company
-Version: 2.7.0
+Version: 2.7.1
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.7.0/garpix_company.egg-info/SOURCES.txt` & `garpix_company-2.7.1/garpix_company.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_company-2.7.0/setup.py` & `garpix_company-2.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.7.0',
+    version='2.7.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

