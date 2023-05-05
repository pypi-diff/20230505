# Comparing `tmp/coguard-cli-0.2.7.tar.gz` & `tmp/coguard-cli-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coguard-cli-0.2.7.tar", last modified: Wed Apr 12 16:13:13 2023, max compression
+gzip compressed data, was "coguard-cli-0.2.8.tar", last modified: Fri May  5 13:06:22 2023, max compression
```

## Comparing `coguard-cli-0.2.7.tar` & `coguard-cli-0.2.8.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.836614 coguard-cli-0.2.7/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1071 2022-06-21 06:40:28.000000 coguard-cli-0.2.7/LICENSE
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-04-12 16:13:13.836614 coguard-cli-0.2.7/PKG-INFO
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8931 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/README.md
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8748 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/README_PYPI.md
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       84 2022-06-21 06:40:28.000000 coguard-cli-0.2.7/pyproject.toml
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      980 2023-04-12 16:13:13.836614 coguard-cli-0.2.7/setup.cfg
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.823281 coguard-cli-0.2.7/src/
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    23004 2023-04-12 16:13:07.000000 coguard-cli-0.2.7/src/coguard_cli/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6592 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/__main__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7702 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/api_connection.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/auth/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8534 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/auth/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1860 2022-07-03 06:44:40.000000 coguard-cli-0.2.7/src/coguard_cli/auth/auth_config.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6313 2023-02-24 03:10:28.000000 coguard-cli-0.2.7/src/coguard_cli/auth/token.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      269 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/auth/util.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/ci_cd/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1011 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_provider_abc.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      502 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_provider_factory.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2193 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.823281 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_scripts/
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_scripts/github/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      485 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_scripts/github/github_coguard_action.yml
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-22 20:18:10.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/__init__.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1431 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      799 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-24 03:43:49.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5713 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2078 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7364 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2716 2023-03-31 15:08:41.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      232 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/versions.tf
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4492 2023-03-31 15:08:41.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7608 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finder_abc.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2518 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finder_factory.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    25095 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6096 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4258 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4176 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3668 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6197 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3615 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6035 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3490 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5011 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7401 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7047 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5979 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8639 2023-04-12 16:13:07.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9482 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9241 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3849 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11379 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11573 2023-03-31 15:08:41.000000 coguard-cli-0.2.7/src/coguard_cli/docker_dao.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/folder_scan/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9227 2023-02-19 03:22:05.000000 coguard-cli-0.2.7/src/coguard_cli/folder_scan/__init__.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/image_check/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8557 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/image_check/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      239 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/print_colors.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/tests/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13023 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/tests/api_connection_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/auth/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/auth/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      675 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/auth/auth_config_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4927 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/tests/auth/common_auth_function_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8441 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/tests/auth/token_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      595 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2099 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11605 2023-02-24 03:10:28.000000 coguard-cli-0.2.7/src/coguard_cli/tests/common_functions_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/__init__.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      640 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8905 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4269 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11454 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3339 2023-01-25 15:30:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      637 2023-01-25 15:30:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13736 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6934 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6597 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5465 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5865 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5736 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5634 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7029 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5883 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6248 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6932 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6899 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6324 2023-04-12 16:13:07.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8168 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7506 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5657 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9100 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/folder_scan/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-23 19:31:49.000000 coguard-cli-0.2.7/src/coguard_cli/tests/folder_scan/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13956 2023-02-19 03:22:05.000000 coguard-cli-0.2.7/src/coguard_cli/tests/folder_scan/common_functions_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.836614 coguard-cli-0.2.7/src/coguard_cli/tests/image_check/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/image_check/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    10470 2023-02-24 03:10:28.000000 coguard-cli-0.2.7/src/coguard_cli/tests/image_check/common_functions_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13136 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/tests/image_check/docker_dao_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6243 2023-02-23 02:56:51.000000 coguard-cli-0.2.7/src/coguard_cli/tests/util_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5506 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/util.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli.egg-info/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/PKG-INFO
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6340 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/SOURCES.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        1 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/dependency_links.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       54 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/entry_points.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       62 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/requires.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       12 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/top_level.txt
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.043087 coguard-cli-0.2.8/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1071 2022-06-21 06:40:28.000000 coguard-cli-0.2.8/LICENSE
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-05-05 13:06:22.043087 coguard-cli-0.2.8/PKG-INFO
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8931 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/README.md
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8748 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/README_PYPI.md
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       84 2022-06-21 06:40:28.000000 coguard-cli-0.2.8/pyproject.toml
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      980 2023-05-05 13:06:22.043087 coguard-cli-0.2.8/setup.cfg
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.019754 coguard-cli-0.2.8/src/
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.023087 coguard-cli-0.2.8/src/coguard_cli/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    30759 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6842 2023-05-03 17:35:40.000000 coguard-cli-0.2.8/src/coguard_cli/__main__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    10619 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/api_connection.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.023087 coguard-cli-0.2.8/src/coguard_cli/auth/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8534 2023-04-24 14:18:39.000000 coguard-cli-0.2.8/src/coguard_cli/auth/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1860 2022-07-03 06:44:40.000000 coguard-cli-0.2.8/src/coguard_cli/auth/auth_config.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6313 2023-02-24 03:10:28.000000 coguard-cli-0.2.8/src/coguard_cli/auth/token.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      269 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/auth/util.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/ci_cd/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1011 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_provider_abc.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      502 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_provider_factory.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2193 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.019754 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_scripts/
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_scripts/github/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      485 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_scripts/github/github_coguard_action.yml
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-22 20:18:10.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/__init__.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1431 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      799 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-24 03:43:49.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5713 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2078 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7364 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2716 2023-03-31 15:08:41.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      232 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/versions.tf
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4492 2023-03-31 15:08:41.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7608 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finder_abc.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2636 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finder_factory.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    25095 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6096 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3470 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_aws_cfn.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4258 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4176 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3668 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6197 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3615 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6035 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3490 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5011 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7401 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7047 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5979 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8639 2023-04-12 16:13:07.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9482 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9241 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3849 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11379 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11573 2023-03-31 15:08:41.000000 coguard-cli-0.2.8/src/coguard_cli/docker_dao.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/folder_scan/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9403 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/folder_scan/__init__.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/image_check/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8557 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/image_check/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      239 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/print_colors.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/tests/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    18437 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/tests/api_connection_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/tests/auth/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/auth/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      675 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/auth/auth_config_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4927 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/tests/auth/common_auth_function_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8441 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/tests/auth/token_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      595 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.036421 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2099 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    26999 2023-05-03 17:35:40.000000 coguard-cli-0.2.8/src/coguard_cli/tests/common_functions_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.036421 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/__init__.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.036421 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      640 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.036421 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8905 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4269 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11454 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3339 2023-01-25 15:30:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      637 2023-01-25 15:30:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.039754 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13736 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6934 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6597 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5465 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5865 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5736 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5634 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7029 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5883 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6248 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6932 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6899 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6324 2023-04-12 16:13:07.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8168 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7506 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5657 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9100 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.039754 coguard-cli-0.2.8/src/coguard_cli/tests/folder_scan/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-23 19:31:49.000000 coguard-cli-0.2.8/src/coguard_cli/tests/folder_scan/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13956 2023-02-19 03:22:05.000000 coguard-cli-0.2.8/src/coguard_cli/tests/folder_scan/common_functions_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.043087 coguard-cli-0.2.8/src/coguard_cli/tests/image_check/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/image_check/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    10470 2023-02-24 03:10:28.000000 coguard-cli-0.2.8/src/coguard_cli/tests/image_check/common_functions_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13136 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/tests/image_check/docker_dao_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6243 2023-02-23 02:56:51.000000 coguard-cli-0.2.8/src/coguard_cli/tests/util_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5506 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/util.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.023087 coguard-cli-0.2.8/src/coguard_cli.egg-info/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/PKG-INFO
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6416 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        1 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       54 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/entry_points.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       62 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/requires.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       12 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/top_level.txt
```

### Comparing `coguard-cli-0.2.7/LICENSE` & `coguard-cli-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/PKG-INFO` & `coguard-cli-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coguard-cli
-Version: 0.2.7
+Version: 0.2.8
 Summary: A command line interface for scanning configuration files with CoGuard
 Home-page: https://github.com/coguardio/coguard-cli
 Author: Heinle Solutions Inc.
 Author-email: albert@coguard.io
 Project-URL: Bug Tracker, https://github.com/coguardio/coguard-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coguard-cli-0.2.7/README.md` & `coguard-cli-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/README_PYPI.md` & `coguard-cli-0.2.8/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/setup.cfg` & `coguard-cli-0.2.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = coguard-cli
-version = 0.2.7
+version = 0.2.8
 author = Heinle Solutions Inc.
 author_email = albert@coguard.io
 description = A command line interface for scanning configuration files with CoGuard
 long_description = file: README_PYPI.md
 long_description_content_type = text/markdown
 url = https://github.com/coguardio/coguard-cli
 project_urls =
```

### Comparing `coguard-cli-0.2.7/src/coguard_cli/__init__.py` & `coguard-cli-0.2.8/src/coguard_cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 from enum import Enum
 import json
 import shutil
 import os
 import sys
 import textwrap
 import logging
+import tempfile
+from zipfile import ZipFile
 from pathlib import Path
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Tuple, List
 
 from coguard_cli import image_check
 from coguard_cli import folder_scan
 from coguard_cli import docker_dao
 from coguard_cli import util
 from coguard_cli.discovery.cloud_discovery.cloud_provider_factory import cloud_provider_factory
 from coguard_cli.ci_cd.ci_cd_provider_factory import ci_cd_provider_factory
 from coguard_cli import auth
 from coguard_cli import api_connection
+from coguard_cli.auth.token import Token
 from coguard_cli.print_colors import COLOR_TERMINATION, \
     COLOR_RED, COLOR_GRAY, COLOR_CYAN, COLOR_YELLOW
 
 def extract_reference_string(entry_dict: Dict, manifest_dict: Dict):
     """
     This is a helper function to extract the respective file in the manifest
     corresponding to an entry in the failed rules.
@@ -56,26 +59,30 @@
                             entry_dict.get("service")
                     ).get("configFileList", [])
                 ]
             if config_file_list_of_container:
                 reference = f" (affected files: {', '.join(config_file_list_of_container)})"
     return reference
 
-def print_failed_check(color: str, entry: Dict, manifest_dict: Dict):
+def print_failed_check(color: str,
+                       entry: Dict,
+                       manifest_dict: Dict,
+                       fixable_checks: List[str]):
     """
     This is the function to print a failed check entry, given a color.
 
     :param color: The color to use. see e.g. :const:`COLOR_RED`
     :param entry: The entry as returned by the CoGuard API.
     :param manifest_dict: The manifest dictionary containing information about the included
                           configuration files
     """
     reference = extract_reference_string(entry, manifest_dict)
+    fix_icon = "🔧 " if entry["rule"]["name"] in fixable_checks else ""
     print(
-        f'{color} X Severity {entry["rule"]["severity"]}: '
+        f'{fix_icon}{color} X Severity {entry["rule"]["severity"]}: '
         f'{entry["rule"]["name"]}{COLOR_TERMINATION}'
         f'{reference}'
     )
     prefix = "Documentation: "
     try:
         terminal_size = os.get_terminal_size().columns
     except OSError:
@@ -98,15 +105,21 @@
         Remediation: {remediation}
 
         Source:
         {sources}
         """.replace("        ", "")
         print(wrapper.fill(documentation_string))
 
-def output_result_json_from_coguard(result_json: Dict, manifest_dict: Dict):
+def output_result_json_from_coguard(
+        result_json: Dict,
+        manifest_dict: Dict,
+        token: Token,
+        coguard_api_url: str,
+        user_name: Optional[str],
+        organization: Optional[str]):
     """
     The function which outputs the result json in a pretty format to the screen.
 
     :param result_json: The output from the API call to CoGuard.
     :param manifest_dict: The manifest dictionary containing information about the included
                           configuration files
     """
@@ -114,24 +127,35 @@
                    if entry["rule"]["severity"] > 3]
     high_checks.sort(key = lambda x: x["rule"]["severity"], reverse=True)
     medium_checks = [entry for entry in result_json.get("failed", []) \
                      if entry["rule"]["severity"] == 3]
     medium_checks.sort(key = lambda x: x["rule"]["severity"], reverse=True)
     low_checks = [entry for entry in result_json.get("failed", []) if entry["rule"]["severity"] < 3]
     low_checks.sort(key = lambda x: x["rule"]["severity"], reverse=True)
-    print(f'Scan result_jsons: {len(result_json.get("failed", []))} checks failed, '
-          f"{COLOR_RED}{len(high_checks)} High{COLOR_TERMINATION}/"
-          f"{COLOR_YELLOW}{len(medium_checks)} Medium{COLOR_TERMINATION}/"
-          f"{COLOR_GRAY}{len(low_checks)} Low{COLOR_TERMINATION}")
+    fixable_check_list = api_connection.get_fixable_rule_list(
+        token,
+        coguard_api_url,
+        user_name,
+        organization
+    )
+    fixable_checks = [entry for entry in result_json.get("failed", []) \
+                      if entry["rule"]["name"] in fixable_check_list]
+    summary = (f'Scan result: {len(result_json.get("failed", []))} checks failed, '
+               f"{COLOR_RED}{len(high_checks)} High{COLOR_TERMINATION}/"
+               f"{COLOR_YELLOW}{len(medium_checks)} Medium{COLOR_TERMINATION}/"
+               f"{COLOR_GRAY}{len(low_checks)} Low{COLOR_TERMINATION} "
+               f"(🔧 {len(fixable_checks)} candidates for auto-remediation)")
+    print(summary)
     for entry in high_checks:
-        print_failed_check(COLOR_RED, entry, manifest_dict)
+        print_failed_check(COLOR_RED, entry, manifest_dict, fixable_check_list)
     for entry in medium_checks:
-        print_failed_check(COLOR_YELLOW, entry, manifest_dict)
+        print_failed_check(COLOR_YELLOW, entry, manifest_dict, fixable_check_list)
     for entry in low_checks:
-        print_failed_check(COLOR_GRAY, entry, manifest_dict)
+        print_failed_check(COLOR_GRAY, entry, manifest_dict, fixable_check_list)
+    print(summary)
 
 class SubParserNames(Enum):
     """
     The enumeration capturing the different supported sub-parsers.
     """
     DOCKER_IMAGE = "docker-image"
     FOLDER_SCAN = "folder"
@@ -172,16 +196,15 @@
         auth_config: Optional[auth.auth_config.CoGuardCliConfig],
         deal_type,
         token: auth.token.Token,
         coguard_api_url: str,
         scan_identifier: str,
         output_format: str,
         fail_level: int,
-        organization: Optional[str]
-):
+        organization: Optional[str]):
     """
     The common function to upload a zip file, as generated by the
     helper functions, and evaluate the returned result.
     """
     if zip_candidate is None:
         print(
             f"{COLOR_YELLOW}Unable to identify any known configuration files.{COLOR_TERMINATION}"
@@ -192,34 +215,153 @@
         zip_file,
         auth_config.get_username(),
         token,
         coguard_api_url,
         scan_identifier,
         organization
     )
+    if result is None:
+        print(
+            f"{COLOR_RED} An error occurred while scanning. Please file a "
+            f"bug report, and include the file located at {zip_file}, if possible. "
+            f"{COLOR_TERMINATION}"
+        )
     logging.debug("The result from the api is: %s",
                   str(result))
     print(f"{COLOR_CYAN}SCANNING OF{COLOR_TERMINATION} {scan_identifier}"
           f" {COLOR_CYAN}COMPLETED{COLOR_TERMINATION}")
     if output_format == 'formatted':
-        output_result_json_from_coguard(result or {}, manifest_dict)
+        output_result_json_from_coguard(
+            result or {},
+            manifest_dict,
+            token,
+            coguard_api_url,
+            auth_config.get_username(),
+            organization
+        )
     else:
         print(json.dumps(result or {}))
     if deal_type != auth.util.DealEnum.ENTERPRISE:
         print("""
         🔧 Save time. Automatically find and fix vulnerabilities.
            Upgrade to auto-remediate issues.
         """)
     os.remove(zip_file)
     max_fail_severity = max(
         entry["rule"]["severity"] for entry in result.get("failed", [])
     ) if (result and result.get("failed", [])) else 0
     if max_fail_severity >= fail_level:
         sys.exit(1)
 
+def apply_fixes_to_folder(fix_folder: str, target_folder: str, zip_manifest: Dict):
+    """
+    The helper function to apply the fixes found in fix_folder to the target folder.
+
+    It identifies all configuration files, tries to map them in the target folder
+    using the manifest information, and then performs the move.
+
+    If everything weng according to plan, the fix_folder will be deleted. Otherwise,
+    it will be left for the purpose of review.
+    """
+    files_to_move = []
+    different_services_objects = []
+    for service_name, service in zip_manifest.get('clusterServices', {}).items():
+        different_services_objects.append((os.path.join('clusterServices', service_name), service))
+    for machine_name, machine in zip_manifest.get('machines', {}).items():
+        for service_name, service in machine.get('services', {}).items():
+            different_services_objects.append(
+                (os.path.join(machine_name, service_name), service)
+            )
+    for pth, service in different_services_objects:
+        for config_file in service.get("configFileList", []):
+            files_to_move.append(
+                (
+                    os.path.join(
+                        pth,
+                        config_file.get("subPath"),
+                        config_file.get("fileName")
+                    ),
+                    os.path.join(
+                        config_file.get("subPath"),
+                        config_file.get("fileName")
+                    )
+                )
+            )
+        for config_file in service.get("complimentaryFileList", []):
+            files_to_move.append(
+                (
+                    os.path.join(
+                        pth,
+                        config_file.get("subPath"),
+                        config_file.get("fileName")
+                    ),
+                    os.path.join(
+                        config_file.get("subPath"),
+                        config_file.get("fileName")
+                    )
+                )
+            )
+    all_files_found = True
+    for file_pth_fix, file_pth_folder in files_to_move:
+        if not os.path.exists(os.path.join(target_folder, file_pth_folder)):
+            logging.error("File %s did not exist in %s", file_pth_folder, target_folder)
+            all_files_found = False
+            continue
+        try:
+            shutil.copyfile(
+                os.path.join(fix_folder, file_pth_fix),
+                os.path.join(target_folder, file_pth_folder)
+            )
+        except OSError as err:
+            all_files_found = False
+            logging.error("Could not copy %s to %s: %s",
+                          file_pth_fix,
+                          file_pth_folder,
+                          err)
+    if not all_files_found:
+        print(f"{COLOR_RED} Not all files were possible to be fixed.")
+        print(f"You can review the extracted and fixed files at {fix_folder}.{COLOR_TERMINATION}")
+    else:
+        shutil.rmtree(fix_folder)
+
+
+def upload_and_fix_zip_candidate(
+        zip_candidate: Optional[Tuple[str, Dict]],
+        folder_path: str,
+        token: auth.token.Token,
+        coguard_api_url: str,
+        organization: Optional[str]) -> None:
+    """
+    The common function to upload and a zip file, as generated by the
+    helper functions.
+    """
+    if zip_candidate is None:
+        print(
+            f"{COLOR_YELLOW}Unable to identify any known configuration files.{COLOR_TERMINATION}"
+        )
+        return
+    zip_file, zip_manifest = zip_candidate
+    api_result = api_connection.send_zip_file_for_fixing(
+        zip_file,
+        token,
+        coguard_api_url,
+        organization
+    )
+    os.remove(zip_file)
+    if api_result is None:
+        print(f"{COLOR_RED} There was an error uploading the zip candidate.{COLOR_TERMINATION}")
+        return
+    print(f'{COLOR_CYAN} Applying the changes.{COLOR_TERMINATION}')
+    temp_folder = tempfile.mkdtemp(prefix="coguard_cli_fix_extract")
+    with ZipFile(api_result, 'r') as zip_stream:
+        zip_stream.extractall(temp_folder)
+    os.remove(api_result)
+    apply_fixes_to_folder(temp_folder, folder_path, zip_manifest)
+    print(f'{COLOR_CYAN} Done applying the changes. {COLOR_TERMINATION}')
+
 def perform_docker_image_scan(
         docker_image: Optional[str],
         auth_config: auth.CoGuardCliConfig,
         deal_type: auth.util.DealEnum,
         token: auth.token.Token,
         organization: str,
         coguard_api_url: Optional[str],
@@ -282,25 +424,28 @@
             fail_level,
             organization
         )
 
 # pylint: disable=bare-except
 def _find_and_merge_included_docker_images(
         collected_config_file_tuple: Tuple[str, Dict],
-        auth_config: auth.CoGuardCliConfig):
+        auth_config: auth.CoGuardCliConfig,
+        additional_failed_rules: List[str]):
     docker_images_extracted = folder_scan.extract_included_docker_images(
         collected_config_file_tuple
     )
+    to_add = False
     for image, location in docker_images_extracted:
         print(
             f"{COLOR_CYAN}Found referenced docker image "
             f"{image} in configuration file {location}."
             f"{COLOR_TERMINATION}"
         )
         try:
+            to_add = True
             temp_folder, temp_inspection, temp_image = image_check.extract_image_to_file_system(
                 image
             ) or (None, None, None)
             if temp_folder is None or temp_inspection is None or temp_image is None:
                 continue
             collected_docker_config_file_tuple = image_check.find_configuration_files_and_collect(
                 image,
@@ -315,15 +460,18 @@
             )
             # cleanup
             collected_location, _ = collected_docker_config_file_tuple
             shutil.rmtree(collected_location, ignore_errors=True)
             shutil.rmtree(temp_folder, ignore_errors=True)
             docker_dao.rm_temporary_container_name(temp_image)
         except:
+            to_add = True
             logging.error("Failed to extract the referenced Docker image.")
+    if to_add:
+        additional_failed_rules.append("cluster_docker_images_with_failed_checks_included")
 
 def perform_folder_scan(
         folder_name: Optional[str],
         deal_type: auth.util.DealEnum,
         auth_config: auth.CoGuardCliConfig,
         token: auth.token.Token,
         organization: str,
@@ -335,25 +483,28 @@
     the current working directory is being used.
     """
     folder_name = folder_name or "."
     printed_folder_name = os.path.basename(os.path.dirname(folder_name + os.sep))
     print(f"{COLOR_CYAN}SCANNING FOLDER {COLOR_TERMINATION}{printed_folder_name}")
     collected_config_file_tuple = folder_scan.find_configuration_files_and_collect(
         folder_name,
-        organization
+        organization or auth_config.get_username()
     )
     if collected_config_file_tuple is None:
         print(f"{COLOR_YELLOW}FOLDER {printed_folder_name} - NO CONFIGURATION FILES FOUND.")
         return
+    additional_failed_rules = []
     _find_and_merge_included_docker_images(
         collected_config_file_tuple,
-        auth_config
+        auth_config,
+        additional_failed_rules
     )
     zip_candidate = folder_scan.create_zip_to_upload_from_file_system(
-        collected_config_file_tuple
+        collected_config_file_tuple,
+        additional_failed_rules
     )
     collected_location, _ = collected_config_file_tuple
     shutil.rmtree(collected_location, ignore_errors=True)
     if zip_candidate is None:
         print(f"{COLOR_YELLOW}FOLDER {printed_folder_name} - NO CONFIGURATION FILES FOUND.")
         return
     upload_and_evaluate_zip_candidate(
@@ -364,14 +515,54 @@
         coguard_api_url,
         printed_folder_name,
         output_format,
         fail_level,
         organization
     )
 
+def perform_folder_fix(
+        folder_name: Optional[str],
+        deal_type: auth.util.DealEnum,
+        token: auth.token.Token,
+        organization: str,
+        coguard_api_url: Optional[str]):
+    """
+    Helper function to run a fix on a folder. If the folder_name parameter is None,
+    the current working directory is being used.
+    """
+    if deal_type != auth.util.DealEnum.ENTERPRISE:
+        print(f"{COLOR_RED} AUTO-REMEDIATION is only available for Enterprise "
+              f"subscriptions {COLOR_TERMINATION}")
+        return
+    folder_name = folder_name or "."
+    printed_folder_name = os.path.basename(os.path.dirname(folder_name + os.sep))
+    print(f"{COLOR_CYAN}SCANNING FOLDER {COLOR_TERMINATION}{printed_folder_name}")
+    collected_config_file_tuple = folder_scan.find_configuration_files_and_collect(
+        folder_name,
+        organization
+    )
+    if collected_config_file_tuple is None:
+        print(f"{COLOR_YELLOW}FOLDER {printed_folder_name} - NO CONFIGURATION FILES FOUND.")
+        return
+    zip_candidate = folder_scan.create_zip_to_upload_from_file_system(
+        collected_config_file_tuple
+    )
+    collected_location, _ = collected_config_file_tuple
+    shutil.rmtree(collected_location, ignore_errors=True)
+    if zip_candidate is None:
+        print(f"{COLOR_YELLOW}FOLDER {printed_folder_name} - NO CONFIGURATION FILES FOUND.")
+        return
+    upload_and_fix_zip_candidate(
+        zip_candidate,
+        folder_name,
+        token,
+        coguard_api_url,
+        organization
+    )
+
 def perform_cloud_provider_scan(
         cloud_provider_name: Optional[str],
         credentials_file: Optional[str],
         deal_type: auth.util.DealEnum,
         auth_config: auth.CoGuardCliConfig,
         token: auth.token.Token,
         organization: str,
@@ -398,15 +589,15 @@
     )
     if not folder_name:
         logging.error("Unable to extract the requested cloud provider %s.",
                       provider_name)
         return
     collected_config_file_tuple = folder_scan.find_configuration_files_and_collect(
         folder_name,
-        organization,
+        organization or auth_config.get_username(),
         f"{provider_name}_extraction"
     )
     zip_candidate = folder_scan.create_zip_to_upload_from_file_system(
         collected_config_file_tuple
     )
     collected_location, _ = collected_config_file_tuple
     shutil.rmtree(collected_location, ignore_errors=True)
@@ -451,14 +642,15 @@
             sys.exit(1)
     else:
         print(f"Invalid command: {ci_cd_command}.")
         sys.exit(1)
     print(ci_cd_provider_instance.post_string())
 
 
+#pylint: disable=too-many-branches
 def entrypoint(args):
     """
     The main entrypoint for the CLI. Takes the :mod:`argparse` parsing
     object as parameter.
 
     :param args: The parsed command line parameters.
     """
@@ -512,24 +704,33 @@
     elif args.subparsers_location == SubParserNames.FOLDER_SCAN.value:
         folder_name = args.folder_name or \
             args.scan or \
             None # args.scan is a trick to
                  # think there is a positional argument
         if folder_name is not None:
             folder_name = os.path.abspath(folder_name)
-        perform_folder_scan(
-            folder_name,
-            deal_type,
-            auth_config,
-            token,
-            organization,
-            args.coguard_api_url,
-            args.output_format,
-            args.fail_level
-        )
+        if args.fix_flag:
+            perform_folder_fix(
+                folder_name,
+                deal_type,
+                token,
+                organization,
+                args.coguard_api_url
+            )
+        else:
+            perform_folder_scan(
+                folder_name,
+                deal_type,
+                auth_config,
+                token,
+                organization,
+                args.coguard_api_url,
+                args.output_format,
+                args.fail_level
+            )
     elif args.subparsers_location == SubParserNames.CLOUD_SCAN.value:
         cloud_provider_name = args.cloud_provider_name or args.scan or None
         # args.scan is a trick to
         # think there is a positional argument
         perform_cloud_provider_scan(
             cloud_provider_name,
             args.credentials_file,
```

### Comparing `coguard-cli-0.2.7/src/coguard_cli/__main__.py` & `coguard-cli-0.2.8/src/coguard_cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,22 @@
               "which means all images are being scanned.")
     )
     folder_scanning_parser = subparsers.add_parser(
         SubParserNames.FOLDER_SCAN.value,
         help="The sub-command to find configuration files within a folder and scan them."
     )
     folder_scanning_parser.add_argument(
+        "--fix",
+        type=bool,
+        dest='fix_flag',
+        default=False,
+        required=False,
+        help="Upload the configuration files inside this folder and retrieve a fixed version."
+    )
+    folder_scanning_parser.add_argument(
         SubParserNames.SCAN.value,
         type=str,
         default="",
         nargs='?',
         help=("The indicator that we are aiming to do a scan.")
     )
     folder_scanning_parser.add_argument(
```

### Comparing `coguard-cli-0.2.7/src/coguard_cli/api_connection.py` & `coguard-cli-0.2.8/src/coguard_cli/api_connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 The coguard CLI module which contains all api-connection
 logic, so that it is modularized.
 """
 
 import logging
+import tempfile
+import os
 from typing import Dict, Optional
 import requests
 
 from coguard_cli.auth.token import Token
 from coguard_cli.util import replace_special_chars_with_underscore
 
 def run_report(
@@ -140,14 +142,56 @@
                 timeout=300)
     if resp.status_code != 200:
         logging.error("There was an error in the API call: %s",
                       resp.reason)
         return None
     return resp.json()
 
+def send_zip_file_for_fixing(
+        zip_file: str,
+        auth_token: Token,
+        coguard_api_url: str,
+        organization: Optional[str]) -> Optional[str]:
+    """
+    The helper function to send a zip file for scanning to the back-end.
+    The return value will be an optional dictionary value as per the
+    result jsons produced by the coguard engine.
+
+    :param zip_file: The path to the zip file.
+    :param user_name: The user name associated.
+    :param auth_token: The authentication token to be used.
+    :param coguard_api_url: The url to be used to contact CoGuard.
+    :param organization: The optional organization string, indicating that
+                         we want to upload it to an org instead of the free account.
+    :returns: Either `None`, or a dictionary as returned by CoGuard after
+              scanning.
+    """
+    with open(zip_file, 'rb') as file_to_send:
+        resp_upload = requests.post(
+            (f"{coguard_api_url}/cluster/"
+             f"fix-cluster-zip?organizationName={organization}"),
+            headers={
+                "Authorization": f'Bearer {auth_token.get_token()}',
+                "Content-Type": "application/octet-stream"
+            },
+            data=file_to_send.read(),
+            timeout=300)
+        if resp_upload.status_code != 200:
+            logging.debug("There was an issue uploading the zip file")
+            logging.debug("Reason %s", resp_upload.reason)
+            return None
+        (file_handle, temp_zip) = tempfile.mkstemp(
+            prefix="coguard_cli_zip_to_fix", suffix=".zip"
+        )
+        os.close(file_handle)
+        with open(temp_zip, 'wb') as zip_to_write:
+            zip_to_write.write(resp_upload.content)
+    return temp_zip
+
+
 def does_user_with_email_already_exist(
         user_name: str,
         coguard_url: str) -> Optional[bool]:
     """
     Given a user_name, which is an email, we will check if
     a user with this given name already exists.
 
@@ -203,7 +247,41 @@
         f"{coguard_url}/registration/referrer-capture",
         headers={"content-type": "application/json"},
         json={"userName": user_name, "referrer": referrer},
         timeout=300
     )
     if resp.status_code != 204:
         logging.error("Could not capture referrer. Please send this error to info@coguard.io")
+
+def get_fixable_rule_list(
+        token: Token,
+        coguard_api_url: str,
+        user_name: Optional[str],
+        organization: Optional[str]):
+    """
+    The call to the endpoint to determine a list of fixable rule identifiers.
+    """
+    if organization:
+        resp = requests.get(
+            f"{coguard_api_url}/cluster/get-fixable-list?organizationName={organization}",
+            headers={
+                "Authorization": f'Bearer {token.get_token()}'
+            },
+            timeout=300
+        )
+        if resp.status_code != 200:
+            logging.error("There was an issue getting the fixable list. ")
+            logging.debug("Reason %s", resp.reason)
+            return []
+        return resp.json()
+    resp = requests.get(
+        f"{coguard_api_url}/coguard-cli/get-fixable-list?userName={user_name}",
+        headers={
+            "Authorization": f'Bearer {token.get_token()}'
+        },
+        timeout=300
+    )
+    if resp.status_code != 200:
+        logging.error("There was an issue getting the fixable list. ")
+        logging.debug("Reason %s", resp.reason)
+        return []
+    return resp.json()
```

### Comparing `coguard-cli-0.2.7/src/coguard_cli/auth/__init__.py` & `coguard-cli-0.2.8/src/coguard_cli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/auth/auth_config.py` & `coguard-cli-0.2.8/src/coguard_cli/auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/auth/token.py` & `coguard-cli-0.2.8/src/coguard_cli/auth/token.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_provider_abc.py` & `coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_provider_abc.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py` & `coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile` & `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile` & `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finder_abc.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finder_abc.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finder_factory.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finder_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     import ConfigFileFinderDockerCompose
 from coguard_cli.discovery.config_file_finders.config_file_finder_kubernetes \
     import ConfigFileFinderKubernetes
 from coguard_cli.discovery.config_file_finders.config_file_finder_helm \
     import ConfigFileFinderHelm
 from coguard_cli.discovery.config_file_finders.config_file_finder_terraform \
     import ConfigFileFinderTerraform
+from coguard_cli.discovery.config_file_finders.config_file_finder_aws_cfn \
+    import ConfigFileFinderCloudformation
 from coguard_cli.discovery.config_file_finder_abc import ConfigFileFinder
 
 def config_file_finder_factory() -> Generator[ConfigFileFinder, None, None]:
     """
     The factory to get different instances to find configuration files.
 
     :returns: A generator continuously yielding subclasses of :class:`ConfigFileFinder`.
```

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/__init__.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py` & `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/docker_dao.py` & `coguard-cli-0.2.8/src/coguard_cli/docker_dao.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/folder_scan/__init__.py` & `coguard-cli-0.2.8/src/coguard_cli/folder_scan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
         for (_, directory_to_delete) in tuple_list
     ]
     for directory_to_delete in directories_to_delete:
         shutil.rmtree(directory_to_delete, ignore_errors=True)
     return (final_location, manifest_blueprint)
 
 def create_zip_to_upload_from_file_system(
-        collected_location_manifest_tuple: Optional[Tuple[str, Dict]]
-) -> Optional[Tuple[str, Dict]]:
+        collected_location_manifest_tuple: Optional[Tuple[str, Dict]],
+        additional_failed_rules: List[str] = None) -> Optional[Tuple[str, Dict]]:
     """
     This function creates a zip file from the tuple provided as input, which
     comes from the `find_configuration_files_and_collect` function.
 
     Keep in mind that whoever is calling this function is in charge of deleting
     the zip file afterwards.
     """
@@ -125,14 +125,16 @@
     (file_handle, temp_zip) = tempfile.mkstemp(prefix="coguard_cli_zip_to_upload", suffix=".zip")
     os.close(file_handle)
     with zipfile.ZipFile(temp_zip, "w") as upload_zip:
         for (dir_path, _, file_names) in os.walk(collected_location):
             for file_name in file_names:
                 file_path = os.path.join(dir_path, file_name)
                 upload_zip.write(file_path, arcname=file_path[len(collected_location):])
+        if additional_failed_rules:
+            upload_zip.writestr("failed_rules.json", json.dumps(additional_failed_rules))
     return (temp_zip, manifest_dict)
 
 def _find_images_recursively(
         config: Union[Dict, List]) -> List[str]:
     """
     Helper function for `_find_and_extract_docker_images_from_config_files`.
     It takes in a config object, tries to find keys referencing "image" and returns
```

### Comparing `coguard-cli-0.2.7/src/coguard_cli/image_check/__init__.py` & `coguard-cli-0.2.8/src/coguard_cli/image_check/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/api_connection_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/api_connection_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -182,14 +182,64 @@
                 unittest.mock.Mock(
                     return_value = lambda: "token"),
                 "biz",
                 "zip",
                 "org"
             ), {"foo": "bar"})
 
+    def test_send_zip_file_for_fixing_non_200_status(self):
+        """
+        Testing the function and send a non 200 code.
+        """
+        mock_response = unittest.mock.Mock(status_code = 200)
+        with unittest.mock.patch(
+                'builtins.open',
+                unittest.mock.mock_open()), \
+                unittest.mock.patch(
+                    'requests.post',
+                    new_callable=lambda: lambda url, headers, data, timeout: mock_response
+                ), \
+            unittest.mock.patch(
+                'tempfile.mkstemp',
+                new_callable = lambda: lambda prefix, suffix: (0, "temp_zip")
+            ), \
+            unittest.mock.patch(
+                'os.close'
+            ):
+            self.assertEqual(
+                api_connection.send_zip_file_for_fixing(
+                    "foo",
+                    unittest.mock.Mock(
+                        return_value = lambda: "token"),
+                    "portal.coguard.io",
+                    "ma_org"
+                ),
+                "temp_zip"
+            )
+
+    def test_send_zip_file_for_fixing(self):
+        """
+        Testing the function and send a non 200 code.
+        """
+        mock_response = unittest.mock.Mock(status_code = 404)
+        with unittest.mock.patch(
+                'builtins.open',
+                unittest.mock.mock_open()), \
+                unittest.mock.patch(
+                    'requests.post',
+                    new_callable=lambda: lambda url, headers, data, timeout: mock_response
+                ):
+            self.assertIsNone(api_connection.send_zip_file_for_fixing(
+                "foo",
+                unittest.mock.Mock(
+                    return_value = lambda: "token"),
+                "portal.coguard.io",
+                "ma_org"
+            ))
+
     def test_does_user_with_email_already_exist_200_status(self):
         """
         Checks the existence of the user function
         """
         mock_response = unittest.mock.Mock(
             status_code = 200,
             text = "true"
@@ -370,7 +420,106 @@
                 unittest.mock.Mock(
                     return_value = lambda: "token"),
                 "https://portal.coguard.io",
                 "scan_identifier",
                 "organization"
             )
             self.assertEqual(result, mock_result)
+
+    def test_get_latest_report_bad_response(self):
+        """
+        Checks the retrieval of the latest report with bad response.
+        """
+        mock_response = unittest.mock.Mock(
+            status_code = 420
+        )
+        with unittest.mock.patch(
+                'requests.get',
+                new_callable=lambda: lambda url, headers, timeout: mock_response):
+            result = api_connection.get_latest_report(
+                unittest.mock.Mock(
+                    return_value = lambda: "token"),
+                "https://portal.coguard.io",
+                "scan_identifier",
+                "organization"
+            )
+            self.assertIsNone(result)
+
+    def test_get_fixable_rule_list_bad_response_ogranization(self):
+        """
+        Checks the retrieval of the latest report with bad response.
+        """
+        mock_response = unittest.mock.Mock(
+            status_code = 420,
+            json = lambda: []
+        )
+        with unittest.mock.patch(
+                'requests.get',
+                new_callable=lambda: lambda url, headers, timeout: mock_response):
+            result = api_connection.get_fixable_rule_list(
+                unittest.mock.Mock(
+                    return_value = lambda: "token"),
+                "https://portal.coguard.io",
+                None,
+                'organization'
+            )
+            self.assertListEqual(result, [])
+
+    def test_get_fixable_rule_list_ogranization(self):
+        """
+        Checks the retrieval of the latest report with bad response.
+        """
+        mock_response = unittest.mock.Mock(
+            status_code = 200,
+            json = lambda: ["foo"]
+        )
+        with unittest.mock.patch(
+                'requests.get',
+                new_callable=lambda: lambda url, headers, timeout: mock_response):
+            result = api_connection.get_fixable_rule_list(
+                unittest.mock.Mock(
+                    return_value = lambda: "token"),
+                "https://portal.coguard.io",
+                None,
+                'organization'
+            )
+            self.assertListEqual(result, ["foo"])
+
+    def test_get_fixable_rule_list_bad_response_user_name(self):
+        """
+        Checks the retrieval of the latest report with bad response.
+        """
+        mock_response = unittest.mock.Mock(
+            status_code = 420,
+            json = lambda: []
+        )
+        with unittest.mock.patch(
+                'requests.get',
+                new_callable=lambda: lambda url, headers, timeout: mock_response):
+            result = api_connection.get_fixable_rule_list(
+                unittest.mock.Mock(
+                    return_value = lambda: "token"),
+                "https://portal.coguard.io",
+                'user_name',
+                None
+            )
+            self.assertListEqual(result, [])
+
+    def test_get_fixable_rule_list_user_name(self):
+        """
+        Checks the retrieval of the latest report with bad response.
+        """
+        mock_response = unittest.mock.Mock(
+            status_code = 200,
+            json = lambda: ["foo"]
+        )
+        with unittest.mock.patch(
+                'requests.get',
+                new_callable=lambda: lambda url, headers, timeout: mock_response):
+            result = api_connection.get_fixable_rule_list(
+                unittest.mock.Mock(
+                    return_value = lambda: "token"),
+                "https://portal.coguard.io",
+                'user_name',
+                None
+            )
+            self.assertListEqual(result, ["foo"])
```

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/auth/auth_config_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/auth/auth_config_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/auth/common_auth_function_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/auth/common_auth_function_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/auth/token_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/auth/token_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/folder_scan/common_functions_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/folder_scan/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/image_check/common_functions_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/image_check/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/image_check/docker_dao_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/image_check/docker_dao_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/tests/util_test.py` & `coguard-cli-0.2.8/src/coguard_cli/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli/util.py` & `coguard-cli-0.2.8/src/coguard_cli/util.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.7/src/coguard_cli.egg-info/PKG-INFO` & `coguard-cli-0.2.8/src/coguard_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coguard-cli
-Version: 0.2.7
+Version: 0.2.8
 Summary: A command line interface for scanning configuration files with CoGuard
 Home-page: https://github.com/coguardio/coguard-cli
 Author: Heinle Solutions Inc.
 Author-email: albert@coguard.io
 Project-URL: Bug Tracker, https://github.com/coguardio/coguard-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coguard-cli-0.2.7/src/coguard_cli.egg-info/SOURCES.txt` & `coguard-cli-0.2.8/src/coguard_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py
 src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py
 src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile
 src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/versions.tf
 src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile
 src/coguard_cli/discovery/config_file_finders/__init__.py
 src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py
+src/coguard_cli/discovery/config_file_finders/config_file_finder_aws_cfn.py
 src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py
 src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py
 src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py
 src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py
 src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py
 src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py
 src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py
```

