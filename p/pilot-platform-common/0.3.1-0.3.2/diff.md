# Comparing `tmp/pilot-platform-common-0.3.1.tar.gz` & `tmp/pilot-platform-common-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot-platform-common-0.3.1.tar", last modified: Tue Apr 25 16:58:14 2023, max compression
+gzip compressed data, was "pilot-platform-common-0.3.2.tar", last modified: Fri May  5 18:50:55 2023, max compression
```

## Comparing `pilot-platform-common-0.3.1.tar` & `pilot-platform-common-0.3.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/geid/
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/geid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/geid/geid_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/jwt_handler/
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/jwt_handler/JWTHandler.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/jwt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/jwt_handler/jwt_handler_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/lineage/entity_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     8976 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/lineage/lineage_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/lineage/lineage_object.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/logger/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logger/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logger/logger_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/logging/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/models/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/models/config_center_policy.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/models/service_id_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/common/object_storage_adaptor/
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/base_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/boto3_admin_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    16665 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/boto3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/minio_policy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/common/permissions/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/permissions/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/common/project/
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8182 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/project/project_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/project/project_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/common/vault/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/vault/vault_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/vault/vault_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7606 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/fixtures/fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_geid_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_lineage_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_logger_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_project_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_vault_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/geid/
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/geid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/geid/geid_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/jwt_handler/
+-rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/jwt_handler/JWTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/jwt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/jwt_handler/jwt_handler_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/lineage/entity_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8976 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/lineage/lineage_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/lineage/lineage_object.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logger/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logger/logger_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.336308 pilot-platform-common-0.3.2/common/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/models/config_center_policy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/models/service_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/common/object_storage_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/boto3_admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16665 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/boto3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/object_storage_adaptor/minio_policy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/common/permissions/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/permissions/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/common/project/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8203 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/project/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/project/project_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/common/vault/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/vault/vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/common/vault/vault_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.340308 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-05 18:50:55.000000 pilot-platform-common-0.3.2/pilot_platform_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8104 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:50:55.344308 pilot-platform-common-0.3.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/fixtures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_geid_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4019 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_lineage_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_logger_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_project_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-05 18:49:45.000000 pilot-platform-common-0.3.2/tests/test_vault_client.py
```

### Comparing `pilot-platform-common-0.3.1/PKG-INFO` & `pilot-platform-common-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.3.1
+Version: 0.3.2
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Research
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.3.1/README.md` & `pilot-platform-common-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/__init__.py` & `pilot-platform-common-0.3.2/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/geid/geid_client.py` & `pilot-platform-common-0.3.2/common/geid/geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/jwt_handler/JWTHandler.py` & `pilot-platform-common-0.3.2/common/jwt_handler/JWTHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,11 +87,9 @@
         return {
             'user_id': user['id'],
             'username': username,
             'role': user['role'] if 'role' in user else None,
             'email': user['email'],
             'first_name': user['first_name'],
             'last_name': user['last_name'],
-            'realm_roles': decoded_token['realm_access']['roles']
-            if ('realm_access' in decoded_token and 'roles' in decoded_token['realm_access'])
-            else [],
+            'realm_roles': user['realm_roles'],
         }
```

### Comparing `pilot-platform-common-0.3.1/common/lineage/entity_object.py` & `pilot-platform-common-0.3.2/common/lineage/entity_object.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/lineage/lineage_client.py` & `pilot-platform-common-0.3.2/common/lineage/lineage_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/lineage/lineage_object.py` & `pilot-platform-common-0.3.2/common/lineage/lineage_object.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/logger/formatter.py` & `pilot-platform-common-0.3.2/common/logger/formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/logger/logger_factory.py` & `pilot-platform-common-0.3.2/common/logger/logger_factory.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/logging/logging.py` & `pilot-platform-common-0.3.2/common/logging/logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/models/config_center_policy.py` & `pilot-platform-common-0.3.2/common/models/config_center_policy.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/object_storage_adaptor/base_client.py` & `pilot-platform-common-0.3.2/common/object_storage_adaptor/base_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/object_storage_adaptor/boto3_admin_client.py` & `pilot-platform-common-0.3.2/common/object_storage_adaptor/boto3_admin_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/object_storage_adaptor/boto3_client.py` & `pilot-platform-common-0.3.2/common/object_storage_adaptor/boto3_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/object_storage_adaptor/minio_policy_client.py` & `pilot-platform-common-0.3.2/common/object_storage_adaptor/minio_policy_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/permissions/permissions.py` & `pilot-platform-common-0.3.2/common/permissions/permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/project/project_client.py` & `pilot-platform-common-0.3.2/common/project/project_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
 import asyncio
 import json
 import logging
 
-import aioredis
 import httpx
+from redis.asyncio.utils import from_url
+from redis.exceptions import ConnectionError
 
 from .project_exceptions import ProjectException
 from .project_exceptions import ProjectNotFoundException
 
 CACHE_PREFIX = 'project_client-'
 CACHE_EXPIRY = 300
 
@@ -93,15 +94,15 @@
         self.redis_url = redis_url
         if is_async:
             self.project_object = ProjectObject
         else:
             self.project_object = ProjectObjectSync
 
     async def connect_redis(self):
-        self.redis = await aioredis.from_url(self.redis_url)
+        self.redis = await from_url(self.redis_url)
 
     async def search(
         self,
         page=None,
         page_size=None,
         order_by=None,
         order_type=None,
@@ -149,28 +150,28 @@
         else:
             project_id = code
 
         project_key = CACHE_PREFIX + project_id
         try:
             if self.enable_cache and await self.redis.exists(project_key):
                 return self.project_object(json.loads(await self.redis.get(project_key)), self)
-        except aioredis.exceptions.ConnectionError:
+        except ConnectionError:
             logger.error(f"Couldn't connect to redis, skipping cache: {self.redis}")
 
         async with httpx.AsyncClient() as client:
             response = await client.get(self.base_url + f'/v1/projects/{project_id}')
         if response.status_code == 404:
             raise ProjectNotFoundException
         elif response.status_code != 200:
             raise ProjectException(status_code=response.status_code, error_msg=response.json())
 
         try:
             if self.enable_cache and self.redis:
                 await self.redis.setex(project_key, CACHE_EXPIRY, json.dumps(response.json()))
-        except aioredis.exceptions.ConnectionError:
+        except ConnectionError:
             logger.error(f"Couldn't connect to redis, skipping cache: {self.redis}")
         return self.project_object(response.json(), self)
 
     async def create(self, code, name, description, image_url=None, tags=None, system_tags=None, is_discoverable=True):
         if tags is None:
             tags = []
         if system_tags is None:
```

### Comparing `pilot-platform-common-0.3.1/common/project/project_exceptions.py` & `pilot-platform-common-0.3.2/common/project/project_exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/common/vault/vault_client.py` & `pilot-platform-common-0.3.2/common/vault/vault_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/pilot_platform_common.egg-info/PKG-INFO` & `pilot-platform-common-0.3.2/pilot_platform_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.3.1
+Version: 0.3.2
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Research
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.3.1/pilot_platform_common.egg-info/SOURCES.txt` & `pilot-platform-common-0.3.2/pilot_platform_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/pyproject.toml` & `pilot-platform-common-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "common"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Indoc Research"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-dotenv = ">=0.19.1"
-aioredis = "^2.0.1"
 python-json-logger = ">= 0.1.11, <= 2.02"
 aioboto3 = "^9.6.0"
 xmltodict = "^0.13.0"
 minio = "^7.1.8"
 httpx = "^0.23.0"
 pyjwt = "2.6.0"
+redis = "^4.5"
 starlette = "^0.25.0"
 cryptography = "39.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.1"
 pytest-asyncio = "0.20.3"
 pytest-cov = "4.0.0"
```

### Comparing `pilot-platform-common-0.3.1/setup.py` & `pilot-platform-common-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pilot-platform-common',
-    version='0.3.1',
+    version='0.3.2',
     author='Indoc Research',
     author_email='etaylor@indocresearch.org',
     description='Generates entity ID and connects with Vault (secret engine) to retrieve credentials',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     install_requires=[
         'python-dotenv==0.19.1',
         'httpx==0.23.0',
-        'aioredis>=2.0.0,<3.0.0',
+        'redis>=4.5.0,<5.0.0',
         'aioboto3==9.6.0',
         'xmltodict==0.13.0',
         'minio==7.1.8',
         'python-json-logger==2.0.2',
         'pyjwt==2.6.0',
         'starlette>=0.25.0,<0.27.0',
         'cryptography==39.0.0',
```

### Comparing `pilot-platform-common-0.3.1/tests/conftest.py` & `pilot-platform-common-0.3.2/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -155,15 +155,33 @@
 def mock_jwt_collaborator(mock_rsa_keys):
     payload = get_mock_jwt_payload(platform_role='member', project_role='collaborator', project_code='testproject')
     token = jwt.encode(payload=payload, key=mock_rsa_keys['private_key'], algorithm='RS256')
     yield {'private_key': mock_rsa_keys['private_key'], 'public_key': mock_rsa_keys['public_key'], 'token': token}
 
 
 @pytest.fixture
+def mock_get_user_from_auth_contrib(httpx_mock):
+    mock_get_user(httpx_mock, 'contributor')
+
+
+@pytest.fixture
+def mock_get_user_from_auth_collab(httpx_mock):
+    mock_get_user(httpx_mock, 'collaborator')
+
+
+@pytest.fixture
 def mock_get_user_from_auth(httpx_mock):
+    mock_get_user(httpx_mock, 'platform-admin')
+
+
+def mock_get_user(httpx_mock, role='platform-admin'):
+    if role == 'platform-admin':
+        realm_roles = ['platform-admin']
+    else:
+        realm_roles = [f'testproject-{role}']
     response = {
         'result': {
             'id': '44c756a8-94f9-46df-970e-7f6be0f876ad',
             'createdTimestamp': 1665685498762,
             'username': 'test',
             'enabled': True,
             'totp': False,
@@ -187,14 +205,15 @@
                 'impersonate': False,
                 'manage': True,
             },
             'first_name': 'test',
             'last_name': 'test',
             'name': 'test',
             'role': 'member',
+            'realm_roles': realm_roles,
         }
     }
     httpx_mock.add_response(
         method='GET',
         url='http://AUTH_SERVICE/v1/admin/user?username=test&exact=true',
         json=response,
         status_code=200,
```

### Comparing `pilot-platform-common-0.3.1/tests/test_formatter.py` & `pilot-platform-common-0.3.2/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/tests/test_jwt_handler.py` & `pilot-platform-common-0.3.2/tests/test_jwt_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,29 +41,29 @@
         assert current_identity['username'] == 'test'
         assert current_identity['role']
         assert current_identity['email'] == 'test@test.com'
         assert current_identity['first_name'] == 'test'
         assert current_identity['last_name'] == 'test'
         assert current_identity['realm_roles'] == ['platform-admin']
 
-    async def test_get_current_identity_contributor(self, mock_jwt_contributor, mock_get_user_from_auth):
+    async def test_get_current_identity_contributor(self, mock_jwt_contributor, mock_get_user_from_auth_contrib):
         client = JWTHandler(mock_jwt_contributor['public_key'])
         decoded_token = client.decode_validate_token(mock_jwt_contributor['token'])
         current_identity = await client.get_current_identity(
             auth_service=self.AUTH_SERVICE, decoded_token=decoded_token
         )
         assert current_identity['user_id']
         assert current_identity['username'] == 'test'
         assert current_identity['role']
         assert current_identity['email'] == 'test@test.com'
         assert current_identity['first_name'] == 'test'
         assert current_identity['last_name'] == 'test'
         assert current_identity['realm_roles'] == ['testproject-contributor']
 
-    async def test_get_current_identity_collaborator(self, mock_jwt_collaborator, mock_get_user_from_auth):
+    async def test_get_current_identity_collaborator(self, mock_jwt_collaborator, mock_get_user_from_auth_collab):
         client = JWTHandler(mock_jwt_collaborator['public_key'])
         decoded_token = client.decode_validate_token(mock_jwt_collaborator['token'])
         current_identity = await client.get_current_identity(
             auth_service=self.AUTH_SERVICE, decoded_token=decoded_token
         )
         assert current_identity['user_id']
         assert current_identity['username'] == 'test'
```

### Comparing `pilot-platform-common-0.3.1/tests/test_lineage_client.py` & `pilot-platform-common-0.3.2/tests/test_lineage_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/tests/test_logger_factory.py` & `pilot-platform-common-0.3.2/tests/test_logger_factory.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/tests/test_logging.py` & `pilot-platform-common-0.3.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/tests/test_permissions.py` & `pilot-platform-common-0.3.2/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/tests/test_project_client.py` & `pilot-platform-common-0.3.2/tests/test_project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.1/tests/test_vault_client.py` & `pilot-platform-common-0.3.2/tests/test_vault_client.py`

 * *Files identical despite different names*

