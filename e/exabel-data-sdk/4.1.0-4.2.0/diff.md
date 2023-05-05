# Comparing `tmp/exabel-data-sdk-4.1.0.tar.gz` & `tmp/exabel-data-sdk-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exabel-data-sdk-4.1.0.tar", last modified: Fri Jan 27 12:29:38 2023, max compression
+gzip compressed data, was "dist/exabel-data-sdk-4.2.0.tar", last modified: Thu May  4 11:24:22 2023, max compression
```

## Comparing `exabel-data-sdk-4.1.0.tar` & `exabel-data-sdk-4.2.0.tar`

### file list

```diff
@@ -1,409 +1,411 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/entity_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/library_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/namespace_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/prediction_model_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/signal_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/tag_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/user_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/bulk_insert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/folder_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/paging_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_set_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/derived_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/export_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/library_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/namespace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/pagable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/prediction_model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/resource_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/search_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/time_series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/exabel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/client/user_login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/examples/create_time_series_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/examples/get_company_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/query/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/query/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/query/literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/query/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/query/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/query/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/base_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/command_line_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/csv_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_entity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_folder_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_relationship_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/load_entities_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/load_relationships_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/load_time_series_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/load_time_series_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/move_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/search_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/share_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/read_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/read_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/read_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/sql_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/unshare_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/update_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/update_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/update_relationship_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_loading_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_relationship_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/entity_mapping_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_loading_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    32943 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_time_series_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_writer_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/athena_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/sql_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/sql_reader_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18374 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/api_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/mock_entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/mock_resource_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/mock_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_export_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_namespace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_pagable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_time_series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/exabel_mock_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/query/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/test_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/test_exabel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/test_user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_command_line_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23337 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_file_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_file_writer_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/test_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_batcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_parse_property_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_type_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/batcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/case_insensitive_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/deprecate_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/handle_missing_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/parse_property_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/resource_name_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk/util/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/exabel_data_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 12:29:38.000000 exabel-data-sdk-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-01-27 12:27:38.000000 exabel-data-sdk-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/entity_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/library_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/namespace_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/prediction_model_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/signal_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/tag_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/user_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/bulk_insert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/paging_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_set_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/derived_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/export_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/library_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/namespace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/pageable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/prediction_model_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/resource_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/search_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25471 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/time_series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/exabel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/user_login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/examples/create_time_series_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/examples/get_company_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/base_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/command_line_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/csv_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_folder_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_relationship_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_entities_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_relationships_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_time_series_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_time_series_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/move_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/search_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/share_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/sql_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/unshare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_relationship_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_loading_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_relationship_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/entity_mapping_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_loading_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34075 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_time_series_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_writer_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/athena_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/sql_reader_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_resource_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_export_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_namespace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_time_series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/exabel_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/query/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_exabel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_command_line_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23337 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_writer_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_parse_property_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_type_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/batcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/case_insensitive_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/deprecate_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/handle_missing_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/parse_property_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/resource_name_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/setup.py
```

### Comparing `exabel-data-sdk-4.1.0/LICENSE` & `exabel-data-sdk-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/PKG-INFO` & `exabel-data-sdk-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabel-data-sdk
-Version: 4.1.0
+Version: 4.2.0
 Summary: Python SDK for the Exabel Data API
 Home-page: https://github.com/Exabel/python-sdk
 Author: Exabel
 Author-email: support@exabel.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `exabel-data-sdk-4.1.0/README.md` & `exabel-data-sdk-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/entity_api_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/entity_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     ListFolderAccessorsRequest,
     ListFolderAccessorsResponse,
     ListFoldersRequest,
     ListFoldersResponse,
     ListItemsRequest,
     ListItemsResponse,
     MoveItemsRequest,
+    SearchItemsRequest,
+    SearchItemsResponse,
     ShareFolderRequest,
     UnshareFolderRequest,
     UpdateFolderRequest,
 )
 
 
 class LibraryGrpcClient(LibraryApiClient, BaseGrpcClient):
@@ -70,7 +72,11 @@
     @handle_grpc_error
     def share_folder(self, request: ShareFolderRequest) -> None:
         return self.stub.ShareFolder(request, metadata=self.metadata, timeout=self.config.timeout)
 
     @handle_grpc_error
     def unshare_folder(self, request: UnshareFolderRequest) -> None:
         return self.stub.UnshareFolder(request, metadata=self.metadata, timeout=self.config.timeout)
+
+    @handle_grpc_error
+    def search_items(self, request: SearchItemsRequest) -> SearchItemsResponse:
+        return self.stub.SearchItems(request, metadata=self.metadata, timeout=self.config.timeout)
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/library_api_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/library_api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     ListFolderAccessorsRequest,
     ListFolderAccessorsResponse,
     ListFoldersRequest,
     ListFoldersResponse,
     ListItemsRequest,
     ListItemsResponse,
     MoveItemsRequest,
+    SearchItemsRequest,
+    SearchItemsResponse,
     ShareFolderRequest,
     UnshareFolderRequest,
     UpdateFolderRequest,
 )
 
 
 class LibraryApiClient(ABC):
@@ -60,7 +62,11 @@
     @abstractmethod
     def share_folder(self, request: ShareFolderRequest) -> None:
         """Share a folder with a group."""
 
     @abstractmethod
     def unshare_folder(self, request: UnshareFolderRequest) -> None:
         """Remove sharing of a folder with a group."""
+
+    @abstractmethod
+    def search_items(self, request: SearchItemsRequest) -> SearchItemsResponse:
+        """Search for folder items."""
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/signal_api_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/signal_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/tag_api_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/tag_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/api_client/user_api_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/user_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/bulk_import.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/bulk_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import logging
 from collections.abc import Sequence as SequenceABC
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
 from itertools import chain
 from time import sleep, time
-from typing import Callable, Generic, Mapping, Optional, Sequence
+from typing import Callable, Generic, Mapping, Optional, Sequence, Union
 
 import pandas as pd
 
 from exabel_data_sdk.client.api.bulk_insert import BulkInsertFailedError, _get_backoff, _raise_error
 from exabel_data_sdk.client.api.data_classes.request_error import ErrorType, RequestError, Violation
 from exabel_data_sdk.client.api.data_classes.time_series import TimeSeriesResourceName
 from exabel_data_sdk.client.api.resource_creation_result import (
     ResourceCreationResult,
     ResourceCreationResults,
     ResourceCreationStatus,
     ResourceT,
 )
-from exabel_data_sdk.services.csv_loading_constants import MAX_THREADS_FOR_IMPORT
+from exabel_data_sdk.services.csv_loading_constants import (
+    DEFAULT_NUMBER_OF_RETRIES,
+    DEFAULT_NUMBER_OF_THREADS_FOR_IMPORT,
+    MAX_THREADS_FOR_IMPORT,
+)
 from exabel_data_sdk.util.deprecate_arguments import deprecate_arguments
 from exabel_data_sdk.util.import_ import get_batches_for_import
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -83,15 +87,18 @@
             return ResourceCreationResult(ResourceCreationStatus.EXISTS, None, self.request_error)
         return ResourceCreationResult(ResourceCreationStatus.FAILED, resource, self.request_error)
 
 
 def _process(
     results: ResourceCreationResults[ResourceT],
     resources: Sequence[ResourceT],
-    import_func: Callable[[Sequence[ResourceT]], Sequence[ResourceCreationStatus]],
+    import_func: Callable[
+        [Sequence[ResourceT]],
+        Union[Sequence[ResourceCreationStatus], Sequence[ResourceCreationResult]],
+    ],
     abort: Callable,
 ) -> None:
     """
     Import a sequence of resources using the provided function. Catches and handles RequestErrors.
 
     Args:
         results:     The result set to append to.
@@ -100,17 +107,22 @@
         import_func: The function to call to import the resources.
         abort:       The function to call when the insert is aborted.
     """
     if results.abort:
         abort()
         return
     try:
-        statuses_batch = import_func(resources)
-        for resource, status in zip(resources, statuses_batch):
-            results.add(ResourceCreationResult(status, resource))
+        results_batch = import_func(resources)
+
+        for resource, result in zip(resources, results_batch):
+            if isinstance(result, ResourceCreationResult):
+                results.add(result)
+            elif isinstance(result, ResourceCreationStatus):
+                results.add(ResourceCreationResult(result, resource))
+
     except RequestError as error:
         failure_handler = ResourceFailureHandler(error)
         for resource in resources:
             results.add(failure_handler.get_resource_creation_result(resource))
     except TypeError as error:
         # Raised when proto message is not constructable (as a result of invalid argument types).
         for resource in resources:
@@ -124,17 +136,20 @@
     resources_batches="resources",
     threads_for_import_func="threads",
     threads_for_insert_func=None,
     insert_func=None,
 )
 def bulk_import(
     resources: Sequence[ResourceT],
-    import_func: Callable[[Sequence[ResourceT]], Sequence[ResourceCreationStatus]],
-    threads: int = 4,
-    retries: int = 5,
+    import_func: Callable[
+        [Sequence[ResourceT]],
+        Union[Sequence[ResourceCreationStatus], Sequence[ResourceCreationResult]],
+    ],
+    threads: int = DEFAULT_NUMBER_OF_THREADS_FOR_IMPORT,
+    retries: int = DEFAULT_NUMBER_OF_RETRIES,
     abort_threshold: Optional[float] = 0.5,
     # Deprecated arguments
     resources_batches: Optional[  # pylint: disable=unused-argument
         Sequence[Sequence[ResourceT]]
     ] = None,
     threads_for_import_func: Optional[int] = None,  # pylint: disable=unused-argument
     threads_for_insert_func: Optional[int] = None,  # pylint: disable=unused-argument
@@ -198,15 +213,18 @@
         results.print_summary()
     return results
 
 
 def _bulk_import(
     results: ResourceCreationResults[ResourceT],
     resources: Sequence[ResourceT],
-    import_func: Callable[[Sequence[ResourceT]], Sequence[ResourceCreationStatus]],
+    import_func: Callable[
+        [Sequence[ResourceT]],
+        Union[Sequence[ResourceCreationStatus], Sequence[ResourceCreationResult]],
+    ],
     threads: int,
 ) -> None:
     """
     Call the provided import function with batches of the provided resources, while catching errors
     and tracking progress.
 
     Args:
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/bulk_insert.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/bulk_insert.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/data_set.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/data_set.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/derived_signal.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/entity.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/entity_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/folder.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,79 @@
-from typing import Sequence
+from typing import Optional, Sequence
 
 from exabel_data_sdk.client.api.data_classes.folder_item import FolderItem
 from exabel_data_sdk.stubs.exabel.api.management.v1.all_pb2 import Folder as ProtoFolder
 
 
 class Folder:
     """
     A folder resource in the Management API.
 
     Attributes:
         name (str):         The resource name of the folder, for example "folders/123".
         display_name (str): The display name of the folder.
         write (bool):       Whether the caller has write access to the folder.
         items (list):       The items in the folder.
+        description (str)   An optional description of the folder.
     """
 
-    def __init__(self, name: str, display_name: str, write: bool, items: Sequence[FolderItem]):
+    def __init__(
+        self,
+        name: str,
+        display_name: str,
+        write: bool,
+        items: Sequence[FolderItem],
+        description: Optional[str] = None,
+    ):
         """
         Create a Folder.
 
         Args:
             name (str):         The resource name of the folder, for example "folders/123".
             display_name (str): The display name of the folder.
             write (bool):       Whether the caller has write access to the folder.
             items (list):       The items in the folder.
+            description (str)   An optional description of the folder.
         """
         self.name = name
         self.display_name = display_name
         self.write = write
         self.items = items
+        self.description = description
 
     @staticmethod
     def from_proto(folder: ProtoFolder) -> "Folder":
         """Create a Folder from the given protobuf Folder."""
         return Folder(
             name=folder.name,
             display_name=folder.display_name,
             write=folder.write,
             items=[FolderItem.from_proto(item) for item in folder.items],
+            description=folder.description if folder.description else None,
         )
 
     def to_proto(self) -> ProtoFolder:
         """Create a proto Folder from this Folder."""
         return ProtoFolder(
             name=self.name,
             display_name=self.display_name,
             write=self.write,
             items=[item.to_proto() for item in self.items],
+            description=self.description if self.description is not None else "",
         )
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Folder):
             return False
         return (
             self.name == other.name
             and self.display_name == other.display_name
             and self.write == other.write
+            and self.description == other.description
             and sorted(self.items) == sorted(other.items)
         )
 
     def __repr__(self) -> str:
         return (
             f"Folder(name='{self.name}', display_name='{self.display_name}', "
-            f"write={self.write}, items={self.items})"
+            f"write={self.write}, items={self.items}, description={repr(self.description)})"
         )
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/folder_item.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from exabel_data_sdk.stubs.exabel.api.management.v1.all_pb2 import FolderItem as ProtoFolderItem
 from exabel_data_sdk.stubs.exabel.api.management.v1.all_pb2 import (
     FolderItemType as ProtoFolderItemType,
 )
 
 
 class FolderItemType(Enum):
-    """Enum representing the type of a folder item."""
+    """Enum representing the type of folder item."""
 
     # Derived signal.
     DERIVED_SIGNAL = ProtoFolderItemType.DERIVED_SIGNAL
     # Prediction model.
     PREDICTION_MODEL = ProtoFolderItemType.PREDICTION_MODEL
     # Portfolio strategy.
     PORTFOLIO_STRATEGY = ProtoFolderItemType.PORTFOLIO_STRATEGY
@@ -24,14 +24,18 @@
     DASHBOARD = ProtoFolderItemType.DASHBOARD
     # Entity drill down view.
     DRILL_DOWN = ProtoFolderItemType.DRILL_DOWN
     # Static tag.
     TAG = ProtoFolderItemType.TAG
     # Screen.
     SCREEN = ProtoFolderItemType.SCREEN
+    # Financial Model
+    FINANCIAL_MODEL = ProtoFolderItemType.FINANCIAL_MODEL
+    # Chart
+    CHART = ProtoFolderItemType.CHART
 
 
 class FolderItem:
     """
     A folder item resource in the Management API.
 
     Attributes:
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/group.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/namespace.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/namespace.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/paging_result.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/paging_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/relationship.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/relationship_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/request_error.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/request_error.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/signal.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/tag.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/tag.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/time_series.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_classes/user.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/data_set_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_set_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/derived_signal_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/derived_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/entity_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/entity_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from exabel_data_sdk.client.api.api_client.grpc.entity_grpc_client import EntityGrpcClient
 from exabel_data_sdk.client.api.bulk_insert import bulk_insert
 from exabel_data_sdk.client.api.data_classes.entity import Entity
 from exabel_data_sdk.client.api.data_classes.entity_type import EntityType
 from exabel_data_sdk.client.api.data_classes.paging_result import PagingResult
 from exabel_data_sdk.client.api.data_classes.request_error import ErrorType, RequestError
-from exabel_data_sdk.client.api.pagable_resource import PagableResourceMixin
+from exabel_data_sdk.client.api.pageable_resource import PageableResourceMixin
 from exabel_data_sdk.client.api.resource_creation_result import (
     ResourceCreationResults,
     ResourceCreationStatus,
 )
 from exabel_data_sdk.client.api.search_service import SearchService
 from exabel_data_sdk.client.client_config import ClientConfig
 from exabel_data_sdk.stubs.exabel.api.data.v1.all_pb2 import (
@@ -28,15 +28,15 @@
     SearchEntitiesRequest,
     SearchTerm,
     UpdateEntityRequest,
     UpdateEntityTypeRequest,
 )
 
 
-class EntityApi(PagableResourceMixin):
+class EntityApi(PageableResourceMixin):
     """
     API class for CRUD operations on entities and entity types.
 
     Attributes:
         search: a SearchService which contains a number of utility methods for searching
     """
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/error_handler.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/error_handler.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/export_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/export_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/library_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/library_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 from google.protobuf.field_mask_pb2 import FieldMask
 
 from exabel_data_sdk.client.api.api_client.grpc.library_grpc_client import LibraryGrpcClient
 from exabel_data_sdk.client.api.data_classes.folder import Folder
 from exabel_data_sdk.client.api.data_classes.folder_accessor import FolderAccessor
 from exabel_data_sdk.client.api.data_classes.folder_item import FolderItem, FolderItemType
+from exabel_data_sdk.client.api.data_classes.paging_result import PagingResult
 from exabel_data_sdk.client.client_config import ClientConfig
 from exabel_data_sdk.stubs.exabel.api.management.v1.library_service_pb2 import (
     CreateFolderRequest,
     DeleteFolderRequest,
     GetFolderRequest,
     ListFolderAccessorsRequest,
     ListFoldersRequest,
     ListItemsRequest,
     MoveItemsRequest,
+    SearchItemsRequest,
     ShareFolderRequest,
     UnshareFolderRequest,
     UpdateFolderRequest,
 )
 
 
 class LibraryApi:
@@ -47,28 +49,29 @@
         return Folder.from_proto(proto_folder)
 
     def create_folder(self, folder: Folder) -> Folder:
         """
         Create a new folder.
 
         Args:
-            folder: The new folder. Only the display name is used.
+            folder: The new folder. Only the display name and description is
+            used.
         """
         proto_folder = self.client.create_folder(
             request=CreateFolderRequest(folder=folder.to_proto())
         )
         return Folder.from_proto(proto_folder)
 
     def update_folder(
         self, folder: Folder, update_mask: Optional[FieldMask] = None, allow_missing: bool = False
     ) -> Folder:
         """
         Update a folder.
 
-        Note that only the folder display name can be updated through this method.
+        Note that only the folder display name and description can be updated through this method.
 
         Args:
             folder:        The updated folder object.
             update_mask:   The fields to update. If not specified, the update behaves as a full
                            update, overwriting all existing fields and properties.
             allow_missing: If set to true, and the resource is not found, a new resource will be
                            created. In this situation the "update_mask" and "folder.name" are
@@ -154,7 +157,39 @@
         Remove sharing of a folder with a group.
 
         Args:
             folder_name:    Resource name of the folder, for example "folders/123".
             group_name:     Resource name of the group, for example "groups/123".
         """
         self.client.unshare_folder(UnshareFolderRequest(folder=folder_name, group=group_name))
+
+    def search_items(
+        self,
+        query: str,
+        folder_item_type: Optional[FolderItemType] = None,
+        page_size: Optional[int] = None,
+        page_token: Optional[str] = None,
+    ) -> PagingResult[FolderItem]:
+        """
+        Search for folder items.
+
+        The field total_size is not calculated for this operation, and will
+        always be set to -1.
+
+        Args:
+            query:              The search query.
+            folder_item_type:   The FolderItemType to search for. If not set,
+                                items of all types are searched.
+            page_size:          The maximum number of items to return.
+            page_token:         A token used to fetch the next page of results.
+        """
+        response = self.client.search_items(
+            SearchItemsRequest(
+                folder="folders/-",
+                query=query,
+                item_type=folder_item_type.value if folder_item_type is not None else None,
+                page_size=page_size,
+                page_token=page_token,
+            )
+        )
+        items = [FolderItem.from_proto(result.item) for result in response.results]
+        return PagingResult(results=items, next_page_token=response.next_page_token, total_size=-1)
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/namespace_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/namespace_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/pagable_resource.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/pageable_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,42 @@
 from exabel_data_sdk.client.api.data_classes.entity_type import EntityType
 from exabel_data_sdk.client.api.data_classes.paging_result import PagingResult
 from exabel_data_sdk.client.api.data_classes.relationship import Relationship
 from exabel_data_sdk.client.api.data_classes.relationship_type import RelationshipType
 from exabel_data_sdk.client.api.data_classes.signal import Signal
 from exabel_data_sdk.client.api.data_classes.tag import Tag
 
-PagableResourceT = TypeVar(
-    "PagableResourceT",
+PageableResourceT = TypeVar(
+    "PageableResourceT",
     DataSet,
     Entity,
     EntityType,
     Relationship,
     RelationshipType,
     Signal,
     Tag,
     str,  # for paging through time series
 )
 
 
-class PagableResourceMixin:
-    """Mixin class for APIs that contain methods with pagable resources."""
+class PageableResourceMixin:
+    """Mixin class for APIs that contain methods with pageable resources."""
 
     @staticmethod
     def _get_resource_iterator(
-        pagable_func: Callable[..., PagingResult[PagableResourceT]],
+        pageable_func: Callable[..., PagingResult[PageableResourceT]],
         **kwargs: str,
-    ) -> Iterator[PagableResourceT]:
+    ) -> Iterator[PageableResourceT]:
         """
         Return an iterator with all the resources returnable by function, paging through the
         results.
         """
         page_token: Optional[str] = None
         resource_count = 0
         while True:
-            result = pagable_func(**kwargs, page_token=page_token)
+            result = pageable_func(**kwargs, page_token=page_token)
             for resource in result.results:
                 yield resource
             page_token = result.next_page_token
             resource_count += len(result.results)
             if resource_count >= result.total_size:
                 break
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/prediction_model_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/prediction_model_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/proto_utils.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/proto_utils.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/relationship_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/relationship_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from functools import partial
 from typing import Iterator, Optional, Sequence
 
 from google.protobuf.field_mask_pb2 import FieldMask
 
 from exabel_data_sdk.client.api.api_client.grpc.relationship_grpc_client import (
     RelationshipGrpcClient,
 )
 from exabel_data_sdk.client.api.bulk_insert import bulk_insert
 from exabel_data_sdk.client.api.data_classes.paging_result import PagingResult
 from exabel_data_sdk.client.api.data_classes.relationship import Relationship
 from exabel_data_sdk.client.api.data_classes.relationship_type import RelationshipType
 from exabel_data_sdk.client.api.data_classes.request_error import ErrorType, RequestError
-from exabel_data_sdk.client.api.pagable_resource import PagableResourceMixin
+from exabel_data_sdk.client.api.pageable_resource import PageableResourceMixin
 from exabel_data_sdk.client.api.resource_creation_result import (
     ResourceCreationResults,
     ResourceCreationStatus,
 )
 from exabel_data_sdk.client.client_config import ClientConfig
 from exabel_data_sdk.stubs.exabel.api.data.v1.all_pb2 import (
     CreateRelationshipRequest,
@@ -26,15 +27,15 @@
     ListRelationshipsRequest,
     ListRelationshipTypesRequest,
     UpdateRelationshipRequest,
     UpdateRelationshipTypeRequest,
 )
 
 
-class RelationshipApi(PagableResourceMixin):
+class RelationshipApi(PageableResourceMixin):
     """
     API class for entity relationship CRUD operations.
     """
 
     def __init__(self, config: ClientConfig):
         self.client = RelationshipGrpcClient(config)
 
@@ -248,18 +249,20 @@
         )
         return PagingResult(
             results=[Relationship.from_proto(r) for r in response.relationships],
             next_page_token=response.next_page_token,
             total_size=response.total_size,
         )
 
-    def get_relationships_iterator(self, relationship_type: str) -> Iterator[Relationship]:
+    def get_relationships_iterator(
+        self, relationship_type: str, page_size: int = 1000
+    ) -> Iterator[Relationship]:
         """Return an iterator with all relationships of the given relationship type."""
         return self._get_resource_iterator(
-            self.list_relationships,
+            partial(self.list_relationships, page_size=page_size),
             relationship_type=relationship_type,
         )
 
     def get_relationship(
         self, relationship_type: str, from_entity: str, to_entity: str
     ) -> Optional[Relationship]:
         """
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/resource_creation_result.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/resource_creation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,16 @@
         Set the member field 'abort' to True if the fraction of errors exceeds the abort threshold.
         """
         fraction_error = self.count(ResourceCreationStatus.FAILED) / self.count()
         if fraction_error > self.abort_threshold and not self.abort:
             self.abort = True
             if self.do_print_status:
                 logger.error(
-                    "Aborting - more than %.0f of the requests are failing.", self.abort_threshold
+                    "Aborting - more than %.0f%% of the requests are failing.",
+                    self.abort_threshold * 100,
                 )
 
     def print_summary(self) -> None:
         """Prints a human legible summary of the resource creation results to screen."""
         if self.counter[ResourceCreationStatus.CREATED]:
             logger.info("%s new resources created", self.counter[ResourceCreationStatus.CREATED])
         if self.counter[ResourceCreationStatus.EXISTS]:
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/search_service.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/search_service.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/signal_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/signal_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from google.protobuf.field_mask_pb2 import FieldMask
 
 from exabel_data_sdk.client.api.api_client.grpc.signal_grpc_client import SignalGrpcClient
 from exabel_data_sdk.client.api.data_classes.paging_result import PagingResult
 from exabel_data_sdk.client.api.data_classes.request_error import ErrorType, RequestError
 from exabel_data_sdk.client.api.data_classes.signal import Signal
-from exabel_data_sdk.client.api.pagable_resource import PagableResourceMixin
+from exabel_data_sdk.client.api.pageable_resource import PageableResourceMixin
 from exabel_data_sdk.client.client_config import ClientConfig
 from exabel_data_sdk.stubs.exabel.api.data.v1.all_pb2 import (
     CreateSignalRequest,
     DeleteSignalRequest,
     GetSignalRequest,
     ListSignalsRequest,
     UpdateSignalRequest,
 )
 
 
-class SignalApi(PagableResourceMixin):
+class SignalApi(PageableResourceMixin):
     """
     API class for Signal CRUD operations.
     """
 
     def __init__(self, config: ClientConfig):
         self.client = SignalGrpcClient(config)
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/tag_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/tag_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Iterator, List, Optional
 
 from exabel_data_sdk.client.api.api_client.grpc.tag_grpc_client import TagGrpcClient
 from exabel_data_sdk.client.api.data_classes.paging_result import PagingResult
 from exabel_data_sdk.client.api.data_classes.request_error import ErrorType, RequestError
 from exabel_data_sdk.client.api.data_classes.tag import Tag
-from exabel_data_sdk.client.api.pagable_resource import PagableResourceMixin
+from exabel_data_sdk.client.api.pageable_resource import PageableResourceMixin
 from exabel_data_sdk.client.client_config import ClientConfig
 from exabel_data_sdk.stubs.exabel.api.analytics.v1.all_pb2 import (
     AddEntitiesRequest,
     CreateTagRequest,
     DeleteTagRequest,
     GetTagRequest,
     ListTagEntitiesRequest,
     ListTagsRequest,
     RemoveEntitiesRequest,
     UpdateTagRequest,
 )
 
 
-class TagApi(PagableResourceMixin):
+class TagApi(PageableResourceMixin):
     """
     API class for tag operations.
     """
 
     def __init__(self, config: ClientConfig):
         self.client = TagGrpcClient(config)
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/time_series_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/time_series_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from typing import Iterator, Optional, Sequence
 
 import pandas as pd
 from dateutil import tz
 from google.protobuf import timestamp_pb2
 from google.protobuf.wrappers_pb2 import DoubleValue
+from google.rpc.code_pb2 import Code as CodeProto
+from grpc import StatusCode
 
 from exabel_data_sdk.client.api.api_client.grpc.time_series_grpc_client import TimeSeriesGrpcClient
 from exabel_data_sdk.client.api.bulk_import import bulk_import
 from exabel_data_sdk.client.api.data_classes.paging_result import PagingResult
 from exabel_data_sdk.client.api.data_classes.request_error import ErrorType, RequestError
-from exabel_data_sdk.client.api.pagable_resource import PagableResourceMixin
+from exabel_data_sdk.client.api.error_handler import grpc_status_to_error_type
+from exabel_data_sdk.client.api.pageable_resource import PageableResourceMixin
 from exabel_data_sdk.client.api.resource_creation_result import (
+    ResourceCreationResult,
     ResourceCreationResults,
     ResourceCreationStatus,
 )
 from exabel_data_sdk.client.client_config import ClientConfig
 from exabel_data_sdk.services.csv_loading_constants import (
     DEFAULT_NUMBER_OF_RETRIES,
     DEFAULT_NUMBER_OF_THREADS_FOR_IMPORT,
@@ -34,15 +38,15 @@
     TimeSeriesView,
     UpdateTimeSeriesRequest,
 )
 from exabel_data_sdk.stubs.exabel.api.time.time_range_pb2 import TimeRange
 from exabel_data_sdk.util.deprecate_arguments import deprecate_arguments
 
 
-class TimeSeriesApi(PagableResourceMixin):
+class TimeSeriesApi(PageableResourceMixin):
     """
     API class for time series CRUD operations.
     """
 
     def __init__(self, config: ClientConfig):
         self.client = TimeSeriesGrpcClient(config)
 
@@ -275,15 +279,16 @@
     def import_time_series(
         self,
         parent: str,
         series: Sequence[pd.Series],
         default_known_time: Optional[DefaultKnownTime] = None,
         allow_missing: bool = False,
         create_tag: bool = False,
-    ) -> None:
+        status_in_response: bool = False,
+    ) -> Optional[Sequence[ResourceCreationResult]]:
         """
         Import multiple time series.
 
         If the time series contains data points that already exist, these data points will be
         overwritten.
 
         Args:
@@ -295,28 +300,62 @@
                             explicitly have a known time set. If not set, the time of insertion is
                             used as the default known time (`current_time = true`).
             allow_missing:  If set to true, and a time series is not found, a new time series will
                             be created.
             create_tag:     Set to true to create a tag for every entity type a signal has time
                             series for. If a tag already exists, it will be updated when time series
                             are created (or deleted) regardless of the value of this flag.
+            status_in_response:
+                            If set to true, the status of each time series will be reported as a
+                            ResourceCreationResult.
+                            If set to false, a failure for one time series will fail the entire
+                            request, and a sample of the failures will be reported in the exception.
+        Returns:
+            If status_in_response is set to true, a list of ResourceCreationResult will be returned.
+            Otherwise, None is returned.
         """
-        self.client.import_time_series(
+        response = self.client.import_time_series(
             ImportTimeSeriesRequest(
                 parent=parent,
                 time_series=[
                     ProtoTimeSeries(name=ts.name, points=self._series_to_time_series_points(ts))
                     for ts in series
                 ],
                 default_known_time=default_known_time,
                 allow_missing=allow_missing,
                 create_tag=create_tag,
+                status_in_response=status_in_response,
             ),
         )
 
+        if status_in_response:
+            time_series_results = []
+            for single_time_series_response, single_time_series in zip(response.responses, series):
+                # The code (integer) given in the response corresponds to google.rpc.Code enum.
+                status_code = StatusCode[CodeProto.Name(single_time_series_response.status.code)]
+
+                if status_code == StatusCode.OK:
+                    time_series_results.append(
+                        ResourceCreationResult(ResourceCreationStatus.UPSERTED, single_time_series)
+                    )
+                else:
+                    error = RequestError(
+                        error_type=grpc_status_to_error_type(status_code),
+                        message=single_time_series_response.status.message,
+                    )
+                    time_series_results.append(
+                        ResourceCreationResult(
+                            ResourceCreationStatus.FAILED, single_time_series, error
+                        )
+                    )
+
+            return time_series_results
+
+        return None
+
     def append_time_series_data_and_return(
         self,
         name: str,
         series: pd.Series,
         default_known_time: Optional[DefaultKnownTime] = None,
         allow_missing: Optional[bool] = False,
         create_tag: Optional[bool] = False,
@@ -411,25 +450,31 @@
                             the Known Time for data points where a specific known time timestamp
                             has not been given. If not provided, the Exabel API defaults to the
                             current time (upload time) as the Known Time.
             retries:        Maximum number of retries to make for each failed request.
             abort_threshold:
                             The threshold for the proportion of failed requests that will cause the
                             upload to be aborted; if it is `None`, the upload is never aborted.
+
+        Returns:
+            ResourceCreationResults containing the status for each time series that was imported.
         """
 
-        def import_func(ts_sequence: Sequence[pd.Series]) -> Sequence[ResourceCreationStatus]:
-            self.import_time_series(
+        def import_func(ts_sequence: Sequence[pd.Series]) -> Sequence[ResourceCreationResult]:
+
+            result = self.import_time_series(
                 parent="signals/-",
                 series=ts_sequence,
                 default_known_time=default_known_time,
                 allow_missing=True,
                 create_tag=create_tag,
+                status_in_response=True,
             )
-            return [ResourceCreationStatus.UPSERTED] * len(ts_sequence)
+            assert result is not None
+            return result
 
         return bulk_import(
             series,
             import_func,
             threads,
             retries,
             abort_threshold,
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/api/user_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/client_config.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/client_config.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/exabel_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/exabel_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/client/user_login.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/client/user_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,15 @@
                 httpd = HTTPServer(server_address, handler)
             except OSError as error:
                 if error.errno != errno.EADDRINUSE:
                     raise error
         if httpd is None:
             raise Exception("Cannot start a local HTTP server to receive the login token.")
 
-        thread = threading.Thread(target=httpd.serve_forever)
-        thread.setDaemon(True)
+        thread = threading.Thread(target=httpd.serve_forever, daemon=True)
         thread.start()
         return httpd
 
     def read_refresh_token(self) -> None:
         """Read the refresh token from the user’s home directory."""
         filename = os.path.expanduser(DEFAULT_TOKEN_FILE_PATH)
         if os.path.isfile(filename):
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/examples/create_time_series_example.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/examples/create_time_series_example.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/examples/get_company_example.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/examples/get_company_example.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/query/column.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/query/column.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/query/dashboard.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/query/dashboard.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/query/literal.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/query/literal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/query/predicate.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/query/predicate.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/query/query.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/query/query.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/query/signals.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/query/signals.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/actions.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/actions.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/base_script.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/base_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/command_line_script.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/command_line_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_derived_signal.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_entity.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_entity_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_folder.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_prediction_model_run.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_prediction_model_run.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_relationship.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_relationship_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/create_signal.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/csv_script.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/csv_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_entities.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_entity.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_entity_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_folder.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_relationship.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_relationship_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/delete_signal.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/export_data.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/export_data.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_entity.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_entity_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_folder.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_relationship.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_relationship_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_signal.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/get_time_series.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_entities.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_entity_types.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_entity_types.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_folder_accessors.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_folder_accessors.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_folders.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_folders.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_items.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_items.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_relationship_types.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_relationship_types.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_relationships.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_relationships.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 import sys
-from typing import List, Sequence
+from typing import Sequence
 
 from exabel_data_sdk import ExabelClient
-from exabel_data_sdk.client.api.data_classes.relationship import Relationship
 from exabel_data_sdk.client.api.data_classes.request_error import RequestError
 from exabel_data_sdk.scripts.base_script import BaseScript
 
 
 class ListRelationships(BaseScript):
     """
     Lists all entities of a given entity type.
@@ -34,46 +33,44 @@
             "--to-entity",
             required=False,
             type=str,
             help="The resource name of the entity the relationships go to",
         )
 
     def run_script(self, client: ExabelClient, args: argparse.Namespace) -> None:
-        if (args.from_entity is None) == (args.to_entity is None):
-            raise ValueError("Specify either the from entity or the to entity.")
+        if args.from_entity and args.to_entity:
+            raise ValueError("Specify either the from entity or the to entity, not both.")
         entity = args.from_entity or args.to_entity
-        try:
-            client.entity_api.get_entity(entity)
-        except RequestError as error:
-            print(error.message)
-            return
-        page_token = None
-        all_relationships: List[Relationship] = []
-        while True:
-            if args.from_entity is not None:
-                result = client.relationship_api.get_relationships_from_entity(
-                    relationship_type=args.relationship_type,
-                    from_entity=args.from_entity,
-                    page_size=1000,
-                    page_token=page_token,
+        if entity:
+            # Check that the entity actually exists
+            try:
+                client.entity_api.get_entity(entity)
+            except RequestError as error:
+                print(error.message)
+                return
+        relationship_type = args.relationship_type
+        if args.from_entity is not None:
+            all_relationships = list(
+                client.relationship_api.get_relationships_from_entity_iterator(
+                    relationship_type, entity
                 )
-            else:
-                result = client.relationship_api.get_relationships_to_entity(
-                    relationship_type=args.relationship_type,
-                    to_entity=args.to_entity,
-                    page_size=1000,
-                    page_token=page_token,
+            )
+        elif args.to_entity is not None:
+            all_relationships = list(
+                client.relationship_api.get_relationships_to_entity_iterator(
+                    relationship_type, entity
                 )
-            all_relationships.extend(result.results)
-            page_token = result.next_page_token
-            if len(all_relationships) == result.total_size:
-                break
+            )
+        else:
+            all_relationships = list(
+                client.relationship_api.get_relationships_iterator(relationship_type)
+            )
 
         if not all_relationships:
-            print("No relationships of the given type.")
+            print("No relationships found")
 
         for relationship in all_relationships:
             print(relationship)
 
 
 if __name__ == "__main__":
     ListRelationships(sys.argv, "Lists relationships of a given type.").run()
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_signals.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_signals.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/list_time_series.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/load_entities_from_csv.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_entities_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/load_relationships_from_csv.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_relationships_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/load_time_series_from_file.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_time_series_from_file.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/login.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/login.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/move_items.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/move_items.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/search_entities.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/search_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/share_folder.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/share_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/read_athena.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_athena.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/read_bigquery.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_bigquery.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/read_snowflake.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_snowflake.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/sql/sql_script.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/sql_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/unshare_folder.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/unshare_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/update_entity_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/update_folder.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/scripts/update_relationship_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_entity_loader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_entity_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         threads: int = DEFAULT_NUMBER_OF_THREADS,
         upsert: bool = False,
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = 0.5,
         batch_size: Optional[int] = None,
+        return_results: bool = True,
         # Deprecated arguments
         name_column: Optional[str] = None,  # pylint: disable=unused-argument
         namespace: Optional[str] = None,  # pylint: disable=unused-argument
     ) -> FileLoadingResult:
         """
         Load a CSV file and upload the entities specified therein to the Exabel Data API.
 
@@ -140,15 +141,16 @@
                 threads=threads,
                 upsert=upsert,
                 dry_run=dry_run,
                 error_on_any_failure=error_on_any_failure,
                 retries=retries,
                 abort_threshold=abort_threshold,
             )
-            combined_result.update(result)
+            if return_results:
+                combined_result.update(result)
 
         return combined_result
 
     def _load_entities(
         self,
         *,
         data_frame: DataFrame,
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_reader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_relationship_loader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_relationship_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,15 @@
         threads: int = DEFAULT_NUMBER_OF_THREADS,
         upsert: bool = False,
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = 0.5,
         batch_size: Optional[int] = None,
+        return_results: bool = True,
         # Deprecated arguments:
         entity_from_column: Optional[str] = None,  # pylint: disable=unused-argument
         entity_to_column: Optional[str] = None,  # pylint: disable=unused-argument
         namespace: Optional[str] = None,  # pylint: disable=unused-argument
     ) -> FileLoadingResult:
         """
         Load a CSV file and upload the relationships specified therein to the Exabel Data API.
@@ -378,15 +379,16 @@
                 threads=threads,
                 upsert=upsert,
                 dry_run=dry_run,
                 error_on_any_failure=error_on_any_failure,
                 retries=retries,
                 abort_threshold=abort_threshold,
             )
-            combined_result.update(result)
+            if return_results:
+                combined_result.update(result)
         return combined_result
 
     def _load_relationships(
         self,
         data_frame: DataFrame,
         entity_mapping: Optional[Mapping[str, Mapping[str, str]]],
         relationship_type_name: str,
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_time_series_loader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_time_series_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/csv_writer.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_writer.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/entity_mapping_file_reader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/entity_mapping_file_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_loading_exception.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_loading_exception.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_loading_result.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_loading_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_time_series_loader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_time_series_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         threads: int = DEFAULT_NUMBER_OF_THREADS_FOR_IMPORT,
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = 0.5,
         batch_size: Optional[int] = None,
         skip_validation: bool = False,
+        return_results: bool = True,
         # Deprecated arguments
         namespace: Optional[str] = None,  # pylint: disable=unused-argument
     ) -> Sequence[TimeSeriesFileLoadingResult]:
         """
         Load a file and upload the time series to the Exabel Data API
 
         If the file has multiple sheets, time series from all the sheets are loaded.
@@ -117,34 +118,34 @@
         for batch_no, parser in enumerate(
             TimeSeriesFileParser.from_file(filename, separator, batch_size), 1
         ):
             if parser.sheet_name():
                 logger.info("Uploading sheet: %s", parser.sheet_name())
             elif batch_size is not None:
                 logger.info("Uploading batch no: %d", batch_no)
-            results.append(
-                self._load_time_series(
-                    parser=parser,
-                    entity_mapping=entity_mapping,
-                    entity_type=entity_type,
-                    identifier_type=identifier_type,
-                    pit_current_time=pit_current_time,
-                    pit_offset=pit_offset,
-                    create_missing_signals=create_missing_signals,
-                    create_tag=create_tag,
-                    create_library_signal=create_library_signal,
-                    global_time_series=global_time_series,
-                    threads=threads,
-                    dry_run=dry_run,
-                    error_on_any_failure=error_on_any_failure,
-                    retries=retries,
-                    abort_threshold=abort_threshold,
-                    skip_validation=skip_validation,
-                )
+            result = self._load_time_series(
+                parser=parser,
+                entity_mapping=entity_mapping,
+                entity_type=entity_type,
+                identifier_type=identifier_type,
+                pit_current_time=pit_current_time,
+                pit_offset=pit_offset,
+                create_missing_signals=create_missing_signals,
+                create_tag=create_tag,
+                create_library_signal=create_library_signal,
+                global_time_series=global_time_series,
+                threads=threads,
+                dry_run=dry_run,
+                error_on_any_failure=error_on_any_failure,
+                retries=retries,
+                abort_threshold=abort_threshold,
+                skip_validation=skip_validation,
             )
+            if return_results:
+                results.append(result)
         return results
 
     def _load_time_series(
         self,
         *,
         parser: TimeSeriesFileParser,
         entity_mapping: Optional[Mapping[str, Mapping[str, str]]] = None,
@@ -264,24 +265,28 @@
         # lexicographically.
         all_signals = {
             signal.name.lower(): signal
             for signal in reversed(list(self._client.signal_api.get_signal_iterator()))
         }
 
         missing_signals = []
-        columns_to_rename = {}
+        signals_to_rename = {}
         for signal in signals:
             lowered_signal_name = prefix + signal.lower()
             if lowered_signal_name not in all_signals:
                 missing_signals.append(lowered_signal_name)
+                if isinstance(parsed_file, SignalNamesInRows) and signal != signal.lower():
+                    signals_to_rename[signal] = signal.lower()
             else:
                 signal_match = all_signals[lowered_signal_name]
-                if lowered_signal_name != signal_match.name:
-                    columns_to_rename[signal] = signal_match.name.split(".")[-1]
-        parsed_file.data = parsed_file.data.rename(columns=columns_to_rename)
+                signal_name = signal_match.name.split(".")[-1]
+                if lowered_signal_name != signal_match.name or (
+                    isinstance(parsed_file, SignalNamesInRows) and signal != signal_name
+                ):
+                    signals_to_rename[signal] = signal_name
 
         if missing_signals:
             logger.info("The following signals are missing:\n%s", missing_signals)
             if create_missing_signals:
                 logger.info("Creating the missing signals.")
                 if not dry_run:
                     for signal in missing_signals:
@@ -290,14 +295,20 @@
                             create_library_signal=create_library_signal,
                         )
             else:
                 raise FileLoadingException(
                     "Aborting script. Please create the missing signals, and try again."
                 )
 
+        if signals_to_rename:
+            if isinstance(parsed_file, SignalNamesInRows):
+                parsed_file.data["signal"] = parsed_file.data["signal"].replace(signals_to_rename)
+            else:
+                parsed_file.data = parsed_file.data.rename(columns=signals_to_rename)
+
         entity_mapping_result = EntityMappingResult(
             parsed_file.get_entity_lookup_result().mapping,
             parsed_file.get_entity_lookup_result().identifier_type,
             parsed_file.get_entity_names(),
             [w.query for w in parsed_file.get_entity_lookup_result().warnings],
         )
         series, invalid_series = parsed_file.get_series(
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_time_series_parser.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_time_series_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Any, Iterable, Iterator, Mapping, NamedTuple, Optional, Sequence, Set, Tuple
 
 import numpy as np
 import pandas as pd
 from dateutil import tz
 from pandas.core.dtypes.common import is_numeric_dtype
 
+from exabel_data_sdk.client.api.data_classes.request_error import ErrorType, RequestError
 from exabel_data_sdk.client.api.entity_api import EntityApi
 from exabel_data_sdk.client.api.resource_creation_result import (
     ResourceCreationResult,
     ResourceCreationStatus,
 )
 from exabel_data_sdk.services import file_constants
 from exabel_data_sdk.services.csv_reader import CsvReader
@@ -271,22 +272,40 @@
             )
             series_with_duplicate_indexes_names = set(s.name for s in series_with_duplicate_indexes)
             series = [
                 ts
                 for ts in series_without_duplicate_data_points
                 if ts.name not in series_with_duplicate_indexes_names
             ]
+            duplicates = self._entity_lookup_result.get_duplicates()
             failures.extend(
                 [
-                    ResourceCreationResult(ResourceCreationStatus.FAILED, ts)
+                    ResourceCreationResult(
+                        ResourceCreationStatus.FAILED,
+                        ts,
+                        RequestError(
+                            ErrorType.INVALID_ARGUMENT,
+                            message=self._format_duplicate_message(str(ts.name), duplicates),
+                        ),
+                    )
                     for ts in series_with_duplicate_indexes
                 ]
             )
         return self.ValidatedTimeSeries(series, failures)
 
+    @staticmethod
+    def _format_duplicate_message(name: str, duplicates: Mapping[str, Sequence[str]]) -> str:
+        entity_name = "/".join(name.split("/")[0:4])
+        if entity_name in duplicates:
+            return (
+                f"Duplicate data points for {name}. Multiple identifiers map to the same entity: "
+                f"{', '.join(duplicates[entity_name][:5])}."
+            )
+        return f"Duplicate data points for {name}."
+
     def get_warnings(self) -> Sequence[str]:
         """Get the warnings generated during mapping of entities."""
         return list(map(str, self._entity_lookup_result.warnings))
 
     def get_entity_lookup_result(self) -> EntityResourceNames:
         """Get the result from the entity lookup."""
         return self._entity_lookup_result
@@ -767,14 +786,19 @@
         namespace: str,
         entity_mapping: Optional[Mapping[str, Mapping[str, str]]] = None,
         entity_type: Optional[str] = None,
     ) -> Tuple[pd.DataFrame, EntityResourceNames]:
         identifiers = pd.Series(data.columns.get_level_values(1))
         identifiers.name = entity_type
         lookup_result = cls._lookup_entities(identifiers, entity_api, namespace, entity_mapping)
+        duplicates = lookup_result.get_duplicates()
+        if len(duplicates) > 0:
+            raise FileLoadingException(
+                f"Multiple identifiers map to the same entity: {next(iter(duplicates.values()))}"
+            )
         data.columns = pd.MultiIndex.from_tuples(
             [(c[0], e) for c, e in zip(data.columns, lookup_result.names)]
         )
         data = data.loc[:, ~data.columns.get_level_values(1).isnull()]
         return data, lookup_result
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/file_writer_provider.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_writer_provider.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/athena_reader_configuration.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/athena_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/sql_reader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/sql_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/services/sql/sql_reader_configuration.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/sql_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateDerivedSignal(self, request, context):
         """Updates a derived signal.
 
-        Note that that this method will update all fields unless `update_mask` is set.
+        Note that this method will update all fields unless `update_mask` is set.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteDerivedSignal(self, request, context):
         """Deletes a derived signal.
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7exabel/api/analytics/v1/prediction_model_messages.proto\x12\x17exabel.api.analytics.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"~\n\x12PredictionModelRun\x123\n\x04name\x18\x01 \x01(\tB%\xe0A\x03\x92A\x1fJ\x1d"predictionModels/123/runs/3"\x123\n\x0bdescription\x18\x02 \x01(\tB\x1e\x92A\x1bJ\x19"Initated by API request"BZ\n\x1bcom.exabel.api.analytics.v1B\x1cPredictionModelMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7exabel/api/analytics/v1/prediction_model_messages.proto\x12\x17exabel.api.analytics.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x96\x02\n\x12PredictionModelRun\x123\n\x04name\x18\x01 \x01(\tB%\xe0A\x03\x92A\x1fJ\x1d"predictionModels/123/runs/3"\x124\n\x0bdescription\x18\x02 \x01(\tB\x1f\x92A\x1cJ\x1a"Initiated by API request"\x12B\n\rconfiguration\x18\x03 \x01(\x0e2+.exabel.api.analytics.v1.ModelConfiguration\x12!\n\x14configuration_source\x18\x04 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\rauto_activate\x18\x05 \x01(\x08B\x17\n\x15_configuration_source*e\n\x12ModelConfiguration\x12%\n!MODEL_CONFIGURATION_NOT_SPECIFIED\x10\x00\x12\n\n\x06LATEST\x10\x01\x12\n\n\x06ACTIVE\x10\x02\x12\x10\n\x0cSPECIFIC_RUN\x10\x03BZ\n\x1bcom.exabel.api.analytics.v1B\x1cPredictionModelMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.prediction_model_messages_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x1cPredictionModelMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1'
     _PREDICTIONMODELRUN.fields_by_name['name']._options = None
     _PREDICTIONMODELRUN.fields_by_name['name']._serialized_options = b'\xe0A\x03\x92A\x1fJ\x1d"predictionModels/123/runs/3"'
     _PREDICTIONMODELRUN.fields_by_name['description']._options = None
-    _PREDICTIONMODELRUN.fields_by_name['description']._serialized_options = b'\x92A\x1bJ\x19"Initated by API request"'
-    _PREDICTIONMODELRUN._serialized_start = 165
-    _PREDICTIONMODELRUN._serialized_end = 291
+    _PREDICTIONMODELRUN.fields_by_name['description']._serialized_options = b'\x92A\x1cJ\x1a"Initiated by API request"'
+    _MODELCONFIGURATION._serialized_start = 446
+    _MODELCONFIGURATION._serialized_end = 547
+    _PREDICTIONMODELRUN._serialized_start = 166
+    _PREDICTIONMODELRUN._serialized_end = 444
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 _sym_db = _symbol_database.Default()
 from .....exabel.api.analytics.v1 import item_messages_pb2 as exabel_dot_api_dot_analytics_dot_v1_dot_item__messages__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*exabel/api/analytics/v1/tag_messages.proto\x12\x17exabel.api.analytics.v1\x1a+exabel/api/analytics/v1/item_messages.proto\x1a\x1fgoogle/api/field_behavior.proto"\x9b\x01\n\x03Tag\x12\x11\n\x04name\x18\x01 \x01(\tB\x03\xe0A\x03\x12\x14\n\x0cdisplay_name\x18\x02 \x01(\t\x12\x13\n\x0bdescription\x18\x03 \x01(\t\x12\x18\n\x0bentity_type\x18\x04 \x01(\tB\x03\xe0A\x03\x12<\n\x08metadata\x18\x05 \x01(\x0b2%.exabel.api.analytics.v1.ItemMetadataB\x03\xe0A\x03BN\n\x1bcom.exabel.api.analytics.v1B\x10TagMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
+from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*exabel/api/analytics/v1/tag_messages.proto\x12\x17exabel.api.analytics.v1\x1a+exabel/api/analytics/v1/item_messages.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xc5\x01\n\x03Tag\x12\x11\n\x04name\x18\x01 \x01(\tB\x03\xe0A\x03\x12#\n\x0cdisplay_name\x18\x02 \x01(\tB\r\x92A\nJ\x08"My tag"\x12.\n\x0bdescription\x18\x03 \x01(\tB\x19\x92A\x16J\x14"My tag description"\x12\x18\n\x0bentity_type\x18\x04 \x01(\tB\x03\xe0A\x03\x12<\n\x08metadata\x18\x05 \x01(\x0b2%.exabel.api.analytics.v1.ItemMetadataB\x03\xe0A\x03BN\n\x1bcom.exabel.api.analytics.v1B\x10TagMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1b\x06proto3')
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.analytics.v1.tag_messages_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1bcom.exabel.api.analytics.v1B\x10TagMessagesProtoP\x01Z\x1bexabel.com/api/analytics/v1'
     _TAG.fields_by_name['name']._options = None
     _TAG.fields_by_name['name']._serialized_options = b'\xe0A\x03'
+    _TAG.fields_by_name['display_name']._options = None
+    _TAG.fields_by_name['display_name']._serialized_options = b'\x92A\nJ\x08"My tag"'
+    _TAG.fields_by_name['description']._options = None
+    _TAG.fields_by_name['description']._serialized_options = b'\x92A\x16J\x14"My tag description"'
     _TAG.fields_by_name['entity_type']._options = None
     _TAG.fields_by_name['entity_type']._serialized_options = b'\xe0A\x03'
     _TAG.fields_by_name['metadata']._options = None
     _TAG.fields_by_name['metadata']._serialized_options = b'\xe0A\x03'
-    _TAG._serialized_start = 150
-    _TAG._serialized_end = 305
+    _TAG._serialized_start = 198
+    _TAG._serialized_end = 395
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 from .....exabel.api.analytics.v1 import tag_messages_pb2 as exabel_dot_api_dot_analytics_dot_v1_dot_tag__messages__pb2
 from .....exabel.api.analytics.v1 import tag_service_pb2 as exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 class TagServiceStub(object):
-    """Service for managing tags. See the User Guide for more information about tags.
+    """Service for managing tags. See the User Guide for more information about tags:
+    https://help.exabel.com/docs/tags-screens
 
     Requests to the TagService are executed in the context of the customer's service account (SA).
     The SA is a special user that is a member of the customer user group, giving it access to all
     folders that are shared with this user group, but not to private folders.
     Hence, only tags that are in folders shared to the SA, via the customer user group,
     will be accessible via the TagService.
     """
@@ -26,15 +27,16 @@
         self.DeleteTag = channel.unary_unary('/exabel.api.analytics.v1.TagService/DeleteTag', request_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.DeleteTagRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
         self.ListTags = channel.unary_unary('/exabel.api.analytics.v1.TagService/ListTags', request_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.ListTagsRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.ListTagsResponse.FromString)
         self.AddEntities = channel.unary_unary('/exabel.api.analytics.v1.TagService/AddEntities', request_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.AddEntitiesRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.AddEntitiesResponse.FromString)
         self.RemoveEntities = channel.unary_unary('/exabel.api.analytics.v1.TagService/RemoveEntities', request_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.RemoveEntitiesRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.RemoveEntitiesResponse.FromString)
         self.ListTagEntities = channel.unary_unary('/exabel.api.analytics.v1.TagService/ListTagEntities', request_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.ListTagEntitiesRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.ListTagEntitiesResponse.FromString)
 
 class TagServiceServicer(object):
-    """Service for managing tags. See the User Guide for more information about tags.
+    """Service for managing tags. See the User Guide for more information about tags:
+    https://help.exabel.com/docs/tags-screens
 
     Requests to the TagService are executed in the context of the customer's service account (SA).
     The SA is a special user that is a member of the customer user group, giving it access to all
     folders that are shared with this user group, but not to private folders.
     Hence, only tags that are in folders shared to the SA, via the customer user group,
     will be accessible via the TagService.
     """
@@ -52,15 +54,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateTag(self, request, context):
         """Update a tag.
 
-        Note that that this method will update all fields unless `update_mask` is set.
+        Note that this method will update all fields unless `update_mask` is set.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteTag(self, request, context):
         """Delete a tag.
@@ -101,15 +103,16 @@
 
 def add_TagServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {'CreateTag': grpc.unary_unary_rpc_method_handler(servicer.CreateTag, request_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.CreateTagRequest.FromString, response_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__messages__pb2.Tag.SerializeToString), 'GetTag': grpc.unary_unary_rpc_method_handler(servicer.GetTag, request_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.GetTagRequest.FromString, response_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__messages__pb2.Tag.SerializeToString), 'UpdateTag': grpc.unary_unary_rpc_method_handler(servicer.UpdateTag, request_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.UpdateTagRequest.FromString, response_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__messages__pb2.Tag.SerializeToString), 'DeleteTag': grpc.unary_unary_rpc_method_handler(servicer.DeleteTag, request_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.DeleteTagRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'ListTags': grpc.unary_unary_rpc_method_handler(servicer.ListTags, request_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.ListTagsRequest.FromString, response_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.ListTagsResponse.SerializeToString), 'AddEntities': grpc.unary_unary_rpc_method_handler(servicer.AddEntities, request_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.AddEntitiesRequest.FromString, response_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.AddEntitiesResponse.SerializeToString), 'RemoveEntities': grpc.unary_unary_rpc_method_handler(servicer.RemoveEntities, request_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.RemoveEntitiesRequest.FromString, response_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.RemoveEntitiesResponse.SerializeToString), 'ListTagEntities': grpc.unary_unary_rpc_method_handler(servicer.ListTagEntities, request_deserializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.ListTagEntitiesRequest.FromString, response_serializer=exabel_dot_api_dot_analytics_dot_v1_dot_tag__service__pb2.ListTagEntitiesResponse.SerializeToString)}
     generic_handler = grpc.method_handlers_generic_handler('exabel.api.analytics.v1.TagService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 class TagService(object):
-    """Service for managing tags. See the User Guide for more information about tags.
+    """Service for managing tags. See the User Guide for more information about tags:
+    https://help.exabel.com/docs/tags-screens
 
     Requests to the TagService are executed in the context of the customer's service account (SA).
     The SA is a special user that is a member of the customer user group, giving it access to all
     folders that are shared with this user group, but not to private folders.
     Hence, only tags that are in folders shared to the SA, via the customer user group,
     will be accessible via the TagService.
     """
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by generate_protobuf.sh.
 # Contains all messages in *_pb2.py in a single module.
 
 from .data_set_messages_pb2 import *
 from .data_set_service_pb2 import *
 from .entity_messages_pb2 import *
 from .entity_service_pb2 import *
+from .import_job_service_pb2 import *
 from .namespace_service_pb2 import *
 from .namespaces_messages_pb2 import *
 from .relationship_messages_pb2 import *
 from .relationship_service_pb2 import *
 from .search_messages_pb2 import *
 from .service_pb2 import *
 from .signal_messages_pb2 import *
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by generate_protobuf.sh.
 # Contains all messages in *_pb2_grpc.py in a single module.
 
 from .data_set_messages_pb2_grpc import *
 from .data_set_service_pb2_grpc import *
 from .entity_messages_pb2_grpc import *
 from .entity_service_pb2_grpc import *
+from .import_job_service_pb2_grpc import *
 from .namespace_service_pb2_grpc import *
 from .namespaces_messages_pb2_grpc import *
 from .relationship_messages_pb2_grpc import *
 from .relationship_service_pb2_grpc import *
 from .search_messages_pb2_grpc import *
 from .service_pb2_grpc import *
 from .signal_messages_pb2_grpc import *
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     """Service for managing data sets. Data sets are collections of signals that you may define and
     manage, often to group data by source/vendor. The companies and entities that have time series
     data for these signals are also part of the data set, and searchable within the data set in the
     Exabel app.
 
     You may access data sets by subscribing to an Exabel data partner, or create your own data sets
     from the data you import.
+
+    See the User Guide for more information about data sets: https://help.exabel.com/docs/data-sets
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -30,14 +32,16 @@
     """Service for managing data sets. Data sets are collections of signals that you may define and
     manage, often to group data by source/vendor. The companies and entities that have time series
     data for these signals are also part of the data set, and searchable within the data set in the
     Exabel app.
 
     You may access data sets by subscribing to an Exabel data partner, or create your own data sets
     from the data you import.
+
+    See the User Guide for more information about data sets: https://help.exabel.com/docs/data-sets
     """
 
     def ListDataSets(self, request, context):
         """Lists all data sets.
 
         Lists all data sets available to your customer, including both your own data sets as well as
         those that you have subscribed to.
@@ -51,25 +55,28 @@
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateDataSet(self, request, context):
         """Creates one data set and returns it.
+
+        It is also possible to create a data set by calling `UpdateDataSet`
+        with `allow_missing` set to `true`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateDataSet(self, request, context):
         """Updates one data set and returns it.
 
         This can also be used to create a data set by setting `allow_missing` to `true`.
 
-        Note that that this method will update all fields unless `update_mask` is set.
+        Note that this method will update all fields unless `update_mask` is set.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteDataSet(self, request, context):
         """Deletes one data set.
@@ -87,14 +94,16 @@
     """Service for managing data sets. Data sets are collections of signals that you may define and
     manage, often to group data by source/vendor. The companies and entities that have time series
     data for these signals are also part of the data set, and searchable within the data set in the
     Exabel app.
 
     You may access data sets by subscribing to an Exabel data partner, or create your own data sets
     from the data you import.
+
+    See the User Guide for more information about data sets: https://help.exabel.com/docs/data-sets
     """
 
     @staticmethod
     def ListDataSets(request, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
         return grpc.experimental.unary_unary(request, target, '/exabel.api.data.v1.DataSetService/ListDataSets', exabel_dot_api_dot_data_dot_v1_dot_data__set__service__pb2.ListDataSetsRequest.SerializeToString, exabel_dot_api_dot_data_dot_v1_dot_data__set__service__pb2.ListDataSetsResponse.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/entity_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xe2\x01\n\nEntityType\x12B\n\x04name\x18\x01 \x01(\tB4\xe0A\x05\xe0A\x02\x92A+J\x15"entityTypes/company"\xca>\x11\xfa\x02\x0eentityTypeName\x12&\n\x0cdisplay_name\x18\x02 \x01(\tB\x10\x92A\rJ\x0b"Companies"\x12,\n\x0bdescription\x18\x03 \x01(\tB\x17\x92A\x14J\x12"Public companies"\x12\x16\n\tread_only\x18\x04 \x01(\x08B\x03\xe0A\x03\x12"\n\x0eis_associative\x18\x05 \x01(\x08B\n\x92A\x07J\x05false"\xa1\x01\n\x06Entity\x12\'\n\x04name\x18\x01 \x01(\tB\x19\xe0A\x05\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nentityName\x12\x14\n\x0cdisplay_name\x18\x02 \x01(\t\x12\x13\n\x0bdescription\x18\x03 \x01(\t\x12\x16\n\tread_only\x18\x04 \x01(\x08B\x03\xe0A\x03\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.StructBG\n\x16com.exabel.api.data.v1B\x13EntityMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/entity_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xe2\x01\n\nEntityType\x12B\n\x04name\x18\x01 \x01(\tB4\xe0A\x05\xe0A\x02\x92A+J\x15"entityTypes/company"\xca>\x11\xfa\x02\x0eentityTypeName\x12&\n\x0cdisplay_name\x18\x02 \x01(\tB\x10\x92A\rJ\x0b"Companies"\x12,\n\x0bdescription\x18\x03 \x01(\tB\x17\x92A\x14J\x12"Public companies"\x12\x16\n\tread_only\x18\x04 \x01(\x08B\x03\xe0A\x03\x12"\n\x0eis_associative\x18\x05 \x01(\x08B\n\x92A\x07J\x05false"\xf7\x01\n\x06Entity\x12@\n\x04name\x18\x01 \x01(\tB2\xe0A\x05\xe0A\x02\x92A)J\x17"entities/ns.my_entity"\xca>\r\xfa\x02\nentityName\x12&\n\x0cdisplay_name\x18\x02 \x01(\tB\x10\x92A\rJ\x0b"My Entity"\x12>\n\x0bdescription\x18\x03 \x01(\tB)\x92A&J$"This is a description of My Entity"\x12\x16\n\tread_only\x18\x04 \x01(\x08B\x03\xe0A\x03\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.StructBG\n\x16com.exabel.api.data.v1B\x13EntityMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.entity_messages_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x13EntityMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _ENTITYTYPE.fields_by_name['name']._options = None
     _ENTITYTYPE.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A+J\x15"entityTypes/company"\xca>\x11\xfa\x02\x0eentityTypeName'
@@ -20,14 +20,18 @@
     _ENTITYTYPE.fields_by_name['description']._options = None
     _ENTITYTYPE.fields_by_name['description']._serialized_options = b'\x92A\x14J\x12"Public companies"'
     _ENTITYTYPE.fields_by_name['read_only']._options = None
     _ENTITYTYPE.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
     _ENTITYTYPE.fields_by_name['is_associative']._options = None
     _ENTITYTYPE.fields_by_name['is_associative']._serialized_options = b'\x92A\x07J\x05false'
     _ENTITY.fields_by_name['name']._options = None
-    _ENTITY.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nentityName'
+    _ENTITY.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A)J\x17"entities/ns.my_entity"\xca>\r\xfa\x02\nentityName'
+    _ENTITY.fields_by_name['display_name']._options = None
+    _ENTITY.fields_by_name['display_name']._serialized_options = b'\x92A\rJ\x0b"My Entity"'
+    _ENTITY.fields_by_name['description']._options = None
+    _ENTITY.fields_by_name['description']._serialized_options = b'\x92A&J$"This is a description of My Entity"'
     _ENTITY.fields_by_name['read_only']._options = None
     _ENTITY.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
     _ENTITYTYPE._serialized_start = 176
     _ENTITYTYPE._serialized_end = 402
     _ENTITY._serialized_start = 405
-    _ENTITY._serialized_end = 566
+    _ENTITY._serialized_end = 652
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import grpc
 from .....exabel.api.data.v1 import entity_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2
 from .....exabel.api.data.v1 import entity_service_pb2 as exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 class EntityServiceStub(object):
     """Service for managing entity types and entities. See the User Guide for more information about
-    entity types and entities.
+    entity types and entities: https://help.exabel.com/docs/entities
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -26,15 +26,15 @@
         self.CreateEntity = channel.unary_unary('/exabel.api.data.v1.EntityService/CreateEntity', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.CreateEntityRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2.Entity.FromString)
         self.UpdateEntity = channel.unary_unary('/exabel.api.data.v1.EntityService/UpdateEntity', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.UpdateEntityRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2.Entity.FromString)
         self.DeleteEntity = channel.unary_unary('/exabel.api.data.v1.EntityService/DeleteEntity', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.DeleteEntityRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
         self.SearchEntities = channel.unary_unary('/exabel.api.data.v1.EntityService/SearchEntities', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.SearchEntitiesRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.SearchEntitiesResponse.FromString)
 
 class EntityServiceServicer(object):
     """Service for managing entity types and entities. See the User Guide for more information about
-    entity types and entities.
+    entity types and entities: https://help.exabel.com/docs/entities
     """
 
     def ListEntityTypes(self, request, context):
         """Lists all known entity types.
 
         Lists all entity types available to your customer, including those created by you, in the
         global catalog, and from data sets you are subscribed to.
@@ -48,25 +48,28 @@
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateEntityType(self, request, context):
         """Creates one entity type and returns it.
+
+        It is also possible to create an entity type set by calling `UpdateEntityType`
+        with `allow_missing` set to `true`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateEntityType(self, request, context):
         """Updates one entity type and returns it.
 
         This can also be used to create an entity type by setting `allow_missing` to `true`.
 
-        Note that that this method will update all fields unless `update_mask` is set.
+        Note that this method will update all fields unless `update_mask` is set.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteEntityType(self, request, context):
         """Deletes one entity type.
@@ -106,25 +109,28 @@
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateEntity(self, request, context):
         """Creates one entity and returns it.
+
+        It is also possible to create an entity by calling `UpdateEntity`
+        with `allow_missing` set to `true`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateEntity(self, request, context):
         """Updates one entity and returns it.
 
         This can also be used to create an entity by setting `allow_missing` to `true`.
 
-        Note that that this method will update all fields unless `update_mask` is set.
+        Note that this method will update all fields unless `update_mask` is set.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteEntity(self, request, context):
         """Deletes one entity.
@@ -169,15 +175,15 @@
 def add_EntityServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {'ListEntityTypes': grpc.unary_unary_rpc_method_handler(servicer.ListEntityTypes, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.ListEntityTypesRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.ListEntityTypesResponse.SerializeToString), 'GetEntityType': grpc.unary_unary_rpc_method_handler(servicer.GetEntityType, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.GetEntityTypeRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2.EntityType.SerializeToString), 'CreateEntityType': grpc.unary_unary_rpc_method_handler(servicer.CreateEntityType, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.CreateEntityTypeRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2.EntityType.SerializeToString), 'UpdateEntityType': grpc.unary_unary_rpc_method_handler(servicer.UpdateEntityType, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.UpdateEntityTypeRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2.EntityType.SerializeToString), 'DeleteEntityType': grpc.unary_unary_rpc_method_handler(servicer.DeleteEntityType, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.DeleteEntityTypeRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'ListEntities': grpc.unary_unary_rpc_method_handler(servicer.ListEntities, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.ListEntitiesRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.ListEntitiesResponse.SerializeToString), 'DeleteEntities': grpc.unary_unary_rpc_method_handler(servicer.DeleteEntities, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.DeleteEntitiesRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'GetEntity': grpc.unary_unary_rpc_method_handler(servicer.GetEntity, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.GetEntityRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2.Entity.SerializeToString), 'CreateEntity': grpc.unary_unary_rpc_method_handler(servicer.CreateEntity, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.CreateEntityRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2.Entity.SerializeToString), 'UpdateEntity': grpc.unary_unary_rpc_method_handler(servicer.UpdateEntity, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.UpdateEntityRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__messages__pb2.Entity.SerializeToString), 'DeleteEntity': grpc.unary_unary_rpc_method_handler(servicer.DeleteEntity, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.DeleteEntityRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'SearchEntities': grpc.unary_unary_rpc_method_handler(servicer.SearchEntities, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.SearchEntitiesRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.SearchEntitiesResponse.SerializeToString)}
     generic_handler = grpc.method_handlers_generic_handler('exabel.api.data.v1.EntityService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 class EntityService(object):
     """Service for managing entity types and entities. See the User Guide for more information about
-    entity types and entities.
+    entity types and entities: https://help.exabel.com/docs/entities
     """
 
     @staticmethod
     def ListEntityTypes(request, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
         return grpc.experimental.unary_unary(request, target, '/exabel.api.data.v1.EntityService/ListEntityTypes', exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.ListEntityTypesRequest.SerializeToString, exabel_dot_api_dot_data_dot_v1_dot_entity__service__pb2.ListEntityTypesResponse.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 _sym_db = _symbol_database.Default()
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/data/v1/relationship_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xd7\x01\n\x10RelationshipType\x12S\n\x04name\x18\x01 \x01(\tBE\xe0A\x05\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\x12\x13\n\x0bdescription\x18\x02 \x01(\t\x12\x16\n\tread_only\x18\x03 \x01(\x08B\x03\xe0A\x03\x12\x14\n\x0cis_ownership\x18\x04 \x01(\x08\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.Struct"\xd0\x02\n\x0cRelationship\x12R\n\x06parent\x18\x01 \x01(\tBB\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\x12E\n\x0bfrom_entity\x18\x02 \x01(\tB0\xe0A\x02\x92A*J("entityTypes/company/entities/F_12345-E"\x12K\n\tto_entity\x18\x03 \x01(\tB8\xe0A\x02\x92A2J0"entityTypes/ns.store/entities/ns.some_store_id"\x12\x13\n\x0bdescription\x18\x04 \x01(\t\x12\x16\n\tread_only\x18\x05 \x01(\x08B\x03\xe0A\x03\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.StructBM\n\x16com.exabel.api.data.v1B\x19RelationshipMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/data/v1/relationship_messages.proto\x12\x12exabel.api.data.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x85\x02\n\x10RelationshipType\x12S\n\x04name\x18\x01 \x01(\tBE\xe0A\x05\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\x12A\n\x0bdescription\x18\x02 \x01(\tB,\x92A)J\'"Indicates that an entity owns a store"\x12\x16\n\tread_only\x18\x03 \x01(\x08B\x03\xe0A\x03\x12\x14\n\x0cis_ownership\x18\x04 \x01(\x08\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.Struct"\xf5\x02\n\x0cRelationship\x12R\n\x06parent\x18\x01 \x01(\tBB\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName\x12E\n\x0bfrom_entity\x18\x02 \x01(\tB0\xe0A\x02\x92A*J("entityTypes/company/entities/F_12345-E"\x12K\n\tto_entity\x18\x03 \x01(\tB8\xe0A\x02\x92A2J0"entityTypes/ns.store/entities/ns.some_store_id"\x128\n\x0bdescription\x18\x04 \x01(\tB#\x92A J\x1e"F_12345-E owns some_store_id"\x12\x16\n\tread_only\x18\x05 \x01(\x08B\x03\xe0A\x03\x12+\n\nproperties\x18d \x01(\x0b2\x17.google.protobuf.StructBM\n\x16com.exabel.api.data.v1B\x19RelationshipMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.relationship_messages_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x19RelationshipMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _RELATIONSHIPTYPE.fields_by_name['name']._options = None
     _RELATIONSHIPTYPE.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName'
+    _RELATIONSHIPTYPE.fields_by_name['description']._options = None
+    _RELATIONSHIPTYPE.fields_by_name['description']._serialized_options = b'\x92A)J\'"Indicates that an entity owns a store"'
     _RELATIONSHIPTYPE.fields_by_name['read_only']._options = None
     _RELATIONSHIPTYPE.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
     _RELATIONSHIP.fields_by_name['parent']._options = None
     _RELATIONSHIP.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A<J "relationshipTypes/ns.HAS_STORE"\xca>\x17\xfa\x02\x14relationshipTypeName'
     _RELATIONSHIP.fields_by_name['from_entity']._options = None
     _RELATIONSHIP.fields_by_name['from_entity']._serialized_options = b'\xe0A\x02\x92A*J("entityTypes/company/entities/F_12345-E"'
     _RELATIONSHIP.fields_by_name['to_entity']._options = None
     _RELATIONSHIP.fields_by_name['to_entity']._serialized_options = b'\xe0A\x02\x92A2J0"entityTypes/ns.store/entities/ns.some_store_id"'
+    _RELATIONSHIP.fields_by_name['description']._options = None
+    _RELATIONSHIP.fields_by_name['description']._serialized_options = b'\x92A J\x1e"F_12345-E owns some_store_id"'
     _RELATIONSHIP.fields_by_name['read_only']._options = None
     _RELATIONSHIP.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
     _RELATIONSHIPTYPE._serialized_start = 182
-    _RELATIONSHIPTYPE._serialized_end = 397
-    _RELATIONSHIP._serialized_start = 400
-    _RELATIONSHIP._serialized_end = 736
+    _RELATIONSHIPTYPE._serialized_end = 443
+    _RELATIONSHIP._serialized_start = 446
+    _RELATIONSHIP._serialized_end = 819
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import grpc
 from .....exabel.api.data.v1 import relationship_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2
 from .....exabel.api.data.v1 import relationship_service_pb2 as exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 class RelationshipServiceStub(object):
     """Service for managing relationship types and relationships. See the User Guide for more
-    information about relationship types and relationships.
+    information about relationship types and relationships:
+    https://help.exabel.com/docs/relationships
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -24,15 +25,16 @@
         self.GetRelationship = channel.unary_unary('/exabel.api.data.v1.RelationshipService/GetRelationship', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.GetRelationshipRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2.Relationship.FromString)
         self.CreateRelationship = channel.unary_unary('/exabel.api.data.v1.RelationshipService/CreateRelationship', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.CreateRelationshipRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2.Relationship.FromString)
         self.UpdateRelationship = channel.unary_unary('/exabel.api.data.v1.RelationshipService/UpdateRelationship', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.UpdateRelationshipRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2.Relationship.FromString)
         self.DeleteRelationship = channel.unary_unary('/exabel.api.data.v1.RelationshipService/DeleteRelationship', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.DeleteRelationshipRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
 
 class RelationshipServiceServicer(object):
     """Service for managing relationship types and relationships. See the User Guide for more
-    information about relationship types and relationships.
+    information about relationship types and relationships:
+    https://help.exabel.com/docs/relationships
     """
 
     def ListRelationshipTypes(self, request, context):
         """List all relationship types from a common catalog.
 
         Lists all relationship types available to your customer, including those created by you, in
         the global catalog, and from data sets you are subscribed to.
@@ -46,14 +48,17 @@
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateRelationshipType(self, request, context):
         """Creates one relationship type and returns it.
+
+        It is also possible to create a relationship type by calling `UpdateRelationshipType`
+        with `allow_missing` set to `true`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateRelationshipType(self, request, context):
         """Updates one relationship type and returns it.
@@ -94,25 +99,28 @@
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateRelationship(self, request, context):
         """Creates one relationship and returns it.
+
+        It is also possible to create a relationship by calling `UpdateRelationship`
+        with `allow_missing` set to `true`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateRelationship(self, request, context):
         """Updates one relationship and returns it.
 
         This can also be used to create a relationship by setting `allow_missing` to `true`.
 
-        Note that that this method will update all fields unless `update_mask` is set.
+        Note that this method will update all fields unless `update_mask` is set.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteRelationship(self, request, context):
         """Deletes one relationship.
@@ -124,15 +132,16 @@
 def add_RelationshipServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {'ListRelationshipTypes': grpc.unary_unary_rpc_method_handler(servicer.ListRelationshipTypes, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.ListRelationshipTypesRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.ListRelationshipTypesResponse.SerializeToString), 'GetRelationshipType': grpc.unary_unary_rpc_method_handler(servicer.GetRelationshipType, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.GetRelationshipTypeRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2.RelationshipType.SerializeToString), 'CreateRelationshipType': grpc.unary_unary_rpc_method_handler(servicer.CreateRelationshipType, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.CreateRelationshipTypeRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2.RelationshipType.SerializeToString), 'UpdateRelationshipType': grpc.unary_unary_rpc_method_handler(servicer.UpdateRelationshipType, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.UpdateRelationshipTypeRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2.RelationshipType.SerializeToString), 'DeleteRelationshipType': grpc.unary_unary_rpc_method_handler(servicer.DeleteRelationshipType, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.DeleteRelationshipTypeRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'ListRelationships': grpc.unary_unary_rpc_method_handler(servicer.ListRelationships, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.ListRelationshipsRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.ListRelationshipsResponse.SerializeToString), 'GetRelationship': grpc.unary_unary_rpc_method_handler(servicer.GetRelationship, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.GetRelationshipRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2.Relationship.SerializeToString), 'CreateRelationship': grpc.unary_unary_rpc_method_handler(servicer.CreateRelationship, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.CreateRelationshipRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2.Relationship.SerializeToString), 'UpdateRelationship': grpc.unary_unary_rpc_method_handler(servicer.UpdateRelationship, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.UpdateRelationshipRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__messages__pb2.Relationship.SerializeToString), 'DeleteRelationship': grpc.unary_unary_rpc_method_handler(servicer.DeleteRelationship, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.DeleteRelationshipRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString)}
     generic_handler = grpc.method_handlers_generic_handler('exabel.api.data.v1.RelationshipService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 class RelationshipService(object):
     """Service for managing relationship types and relationships. See the User Guide for more
-    information about relationship types and relationships.
+    information about relationship types and relationships:
+    https://help.exabel.com/docs/relationships
     """
 
     @staticmethod
     def ListRelationshipTypes(request, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
         return grpc.experimental.unary_unary(request, target, '/exabel.api.data.v1.RelationshipService/ListRelationshipTypes', exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.ListRelationshipTypesRequest.SerializeToString, exabel_dot_api_dot_data_dot_v1_dot_relationship__service__pb2.ListRelationshipTypesResponse.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 _sym_db = _symbol_database.Default()
 from .....exabel.api.math import aggregation_pb2 as exabel_dot_api_dot_math_dot_aggregation__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/signal_messages.proto\x12\x12exabel.api.data.v1\x1a!exabel/api/math/aggregation.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xbf\x02\n\x06Signal\x12<\n\x04name\x18\x01 \x01(\tB.\xe0A\x05\xe0A\x02\x92A%J\x13"signals/ns.signal"\xca>\r\xfa\x02\nsignalName\x12\x17\n\x0bentity_type\x18\x02 \x01(\tB\x02\x18\x01\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"My signal"\x12\x13\n\x0bdescription\x18\x04 \x01(\t\x129\n\x13downsampling_method\x18\x05 \x01(\x0e2\x1c.exabel.api.math.Aggregation\x12\x16\n\tread_only\x18\x06 \x01(\x08B\x03\xe0A\x03\x12N\n\x0centity_types\x18\x07 \x03(\tB8\xe0A\x03\x92A2J0["entityTypes/ns.type1", "entityTypes/ns.type2"]BG\n\x16com.exabel.api.data.v1B\x13SignalMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(exabel/api/data/v1/signal_messages.proto\x12\x12exabel.api.data.v1\x1a!exabel/api/math/aggregation.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xdb\x02\n\x06Signal\x12<\n\x04name\x18\x01 \x01(\tB.\xe0A\x05\xe0A\x02\x92A%J\x13"signals/ns.signal"\xca>\r\xfa\x02\nsignalName\x12\x17\n\x0bentity_type\x18\x02 \x01(\tB\x02\x18\x01\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"My signal"\x12/\n\x0bdescription\x18\x04 \x01(\tB\x1a\x92A\x17J\x15"Describes my signal"\x129\n\x13downsampling_method\x18\x05 \x01(\x0e2\x1c.exabel.api.math.Aggregation\x12\x16\n\tread_only\x18\x06 \x01(\x08B\x03\xe0A\x03\x12N\n\x0centity_types\x18\x07 \x03(\tB8\xe0A\x03\x92A2J0["entityTypes/ns.type1", "entityTypes/ns.type2"]BG\n\x16com.exabel.api.data.v1B\x13SignalMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.signal_messages_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x13SignalMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _SIGNAL.fields_by_name['name']._options = None
     _SIGNAL.fields_by_name['name']._serialized_options = b'\xe0A\x05\xe0A\x02\x92A%J\x13"signals/ns.signal"\xca>\r\xfa\x02\nsignalName'
     _SIGNAL.fields_by_name['entity_type']._options = None
     _SIGNAL.fields_by_name['entity_type']._serialized_options = b'\x18\x01'
     _SIGNAL.fields_by_name['display_name']._options = None
     _SIGNAL.fields_by_name['display_name']._serialized_options = b'\x92A\rJ\x0b"My signal"'
+    _SIGNAL.fields_by_name['description']._options = None
+    _SIGNAL.fields_by_name['description']._serialized_options = b'\x92A\x17J\x15"Describes my signal"'
     _SIGNAL.fields_by_name['read_only']._options = None
     _SIGNAL.fields_by_name['read_only']._serialized_options = b'\xe0A\x03'
     _SIGNAL.fields_by_name['entity_types']._options = None
     _SIGNAL.fields_by_name['entity_types']._serialized_options = b'\xe0A\x03\x92A2J0["entityTypes/ns.type1", "entityTypes/ns.type2"]'
     _SIGNAL._serialized_start = 181
-    _SIGNAL._serialized_end = 500
+    _SIGNAL._serialized_end = 528
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import grpc
 from .....exabel.api.data.v1 import signal_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_signal__messages__pb2
 from .....exabel.api.data.v1 import signal_service_pb2 as exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 class SignalServiceStub(object):
     """Service for managing raw data signals. See the User Guide for more information about raw data
-    signals.
+    signals: https://help.exabel.com/docs/signals
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -19,15 +19,15 @@
         self.GetSignal = channel.unary_unary('/exabel.api.data.v1.SignalService/GetSignal', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.GetSignalRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_signal__messages__pb2.Signal.FromString)
         self.CreateSignal = channel.unary_unary('/exabel.api.data.v1.SignalService/CreateSignal', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.CreateSignalRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_signal__messages__pb2.Signal.FromString)
         self.UpdateSignal = channel.unary_unary('/exabel.api.data.v1.SignalService/UpdateSignal', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.UpdateSignalRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_signal__messages__pb2.Signal.FromString)
         self.DeleteSignal = channel.unary_unary('/exabel.api.data.v1.SignalService/DeleteSignal', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.DeleteSignalRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
 
 class SignalServiceServicer(object):
     """Service for managing raw data signals. See the User Guide for more information about raw data
-    signals.
+    signals: https://help.exabel.com/docs/signals
     """
 
     def ListSignals(self, request, context):
         """Lists all known signals.
 
         Lists all raw data signals available to your customer, including those created by you, in the
         global catalog, and from data sets you are subscribed to.
@@ -41,25 +41,28 @@
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateSignal(self, request, context):
         """Creates one signal and returns it.
+
+        It is also possible to create a signal by calling `UpdateSignal`
+        with `allow_missing` set to `true`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateSignal(self, request, context):
         """Updates one signal and returns it.
 
         This can also be used to create a signal by setting `allow_missing` to `true`.
 
-        Note that that this method will update all fields unless `update_mask` is set.
+        Note that this method will update all fields unless `update_mask` is set.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteSignal(self, request, context):
         """Deletes one signal. ALL time series for this signal will also be deleted.
@@ -73,15 +76,15 @@
 def add_SignalServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {'ListSignals': grpc.unary_unary_rpc_method_handler(servicer.ListSignals, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.ListSignalsRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.ListSignalsResponse.SerializeToString), 'GetSignal': grpc.unary_unary_rpc_method_handler(servicer.GetSignal, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.GetSignalRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_signal__messages__pb2.Signal.SerializeToString), 'CreateSignal': grpc.unary_unary_rpc_method_handler(servicer.CreateSignal, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.CreateSignalRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_signal__messages__pb2.Signal.SerializeToString), 'UpdateSignal': grpc.unary_unary_rpc_method_handler(servicer.UpdateSignal, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.UpdateSignalRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_signal__messages__pb2.Signal.SerializeToString), 'DeleteSignal': grpc.unary_unary_rpc_method_handler(servicer.DeleteSignal, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.DeleteSignalRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString)}
     generic_handler = grpc.method_handlers_generic_handler('exabel.api.data.v1.SignalService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 class SignalService(object):
     """Service for managing raw data signals. See the User Guide for more information about raw data
-    signals.
+    signals: https://help.exabel.com/docs/signals
     """
 
     @staticmethod
     def ListSignals(request, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
         return grpc.experimental.unary_unary(request, target, '/exabel.api.data.v1.SignalService/ListSignals', exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.ListSignalsRequest.SerializeToString, exabel_dot_api_dot_data_dot_v1_dot_signal__service__pb2.ListSignalsResponse.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 _sym_db = _symbol_database.Default()
 from .....exabel.api.data.v1 import time_series_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_time__series__messages__pb2
 from .....exabel.api.time import time_range_pb2 as exabel_dot_api_dot_time_dot_time__range__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from google.rpc import status_pb2 as google_dot_rpc_dot_status__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,exabel/api/data/v1/time_series_service.proto\x12\x12exabel.api.data.v1\x1a-exabel/api/data/v1/time_series_messages.proto\x1a exabel/api/time/time_range.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/api/visibility.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"l\n\x15ListTimeSeriesRequest\x12,\n\x06parent\x18\x01 \x01(\tB\x1c\xe0A\x02\x92A\x16\xca>\x13\xfa\x02\x10timeSeriesParent\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"z\n\x16ListTimeSeriesResponse\x123\n\x0btime_series\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.TimeSeries\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"r\n\x14GetTimeSeriesRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView"\xdb\x01\n\x17CreateTimeSeriesRequest\x128\n\x0btime_series\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.TimeSeriesB\x03\xe0A\x02\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x12\n\ncreate_tag\x18\x04 \x01(\x08"\xf2\x01\n\x17UpdateTimeSeriesRequest\x128\n\x0btime_series\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.TimeSeriesB\x03\xe0A\x02\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x15\n\rallow_missing\x18\x04 \x01(\x08\x12\x12\n\ncreate_tag\x18\x05 \x01(\x08"\xd0\x01\n\x17ImportTimeSeriesRequest\x12\x13\n\x06parent\x18\x01 \x01(\tB\x03\xe0A\x02\x123\n\x0btime_series\x18\x02 \x03(\x0b2\x1e.exabel.api.data.v1.TimeSeries\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x15\n\rallow_missing\x18\x04 \x01(\x08\x12\x12\n\ncreate_tag\x18\x05 \x01(\x08"\x1a\n\x18ImportTimeSeriesResponse"C\n\x17DeleteTimeSeriesRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName"\x7f\n"BatchDeleteTimeSeriesPointsRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\x12/\n\x0btime_ranges\x18\x02 \x03(\x0b2\x1a.exabel.api.time.TimeRange2\x80\x0e\n\x11TimeSeriesService\x12\xdb\x01\n\x0eListTimeSeries\x12).exabel.api.data.v1.ListTimeSeriesRequest\x1a*.exabel.api.data.v1.ListTimeSeriesResponse"r\x82\xd3\xe4\x93\x02W\x120/v1/{parent=entityTypes/*/entities/*}/timeSeriesZ#\x12!/v1/{parent=signals/*}/timeSeries\x92A\x12\x12\x10List time series\x12\xd5\x01\n\rGetTimeSeries\x12(.exabel.api.data.v1.GetTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"z\x82\xd3\xe4\x93\x02`\x12-/v1/{name=entityTypes/*/entities/*/signals/*}Z/\x12-/v1/{name=signals/*/entityTypes/*/entities/*}\x92A\x11\x12\x0fGet time series\x12\x92\x02\n\x10CreateTimeSeries\x12+.exabel.api.data.v1.CreateTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"\xb0\x01\x82\xd3\xe4\x93\x02\x92\x01"9/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH"9/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x92A\x14\x12\x12Create time series\x12\x92\x02\n\x10UpdateTimeSeries\x12+.exabel.api.data.v1.UpdateTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"\xb0\x01\x82\xd3\xe4\x93\x02\x92\x0129/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH29/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x92A\x14\x12\x12Update time series\x12\xf8\x01\n\x10ImportTimeSeries\x12+.exabel.api.data.v1.ImportTimeSeriesRequest\x1a,.exabel.api.data.v1.ImportTimeSeriesResponse"\x88\x01\x82\xd3\xe4\x93\x02k"7/v1/{parent=entityTypes/*/entities/*}/timeSeries:import:\x01*Z-"(/v1/{parent=signals/*}/timeSeries:import:\x01*\x92A\x14\x12\x12Import time series\x12\xd6\x01\n\x10DeleteTimeSeries\x12+.exabel.api.data.v1.DeleteTimeSeriesRequest\x1a\x16.google.protobuf.Empty"}\x82\xd3\xe4\x93\x02`*-/v1/{name=entityTypes/*/entities/*/signals/*}Z/*-/v1/{name=signals/*/entityTypes/*/entities/*}\x92A\x14\x12\x12Delete time series\x12\xb6\x02\n\x1bBatchDeleteTimeSeriesPoints\x126.exabel.api.data.v1.BatchDeleteTimeSeriesPointsRequest\x1a\x16.google.protobuf.Empty"\xc6\x01\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL\x82\xd3\xe4\x93\x02\x8c\x01"@/v1/{name=entityTypes/*/entities/*/signals/*}/points:batchDelete:\x01*ZE"@/v1/{name=signals/*/entityTypes/*/entities/*}/points:batchDelete:\x01*\x92A \x12\x1eDelete time series data pointsBJ\n\x16com.exabel.api.data.v1B\x16TimeSeriesServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,exabel/api/data/v1/time_series_service.proto\x12\x12exabel.api.data.v1\x1a-exabel/api/data/v1/time_series_messages.proto\x1a exabel/api/time/time_range.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/api/visibility.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x17google/rpc/status.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"l\n\x15ListTimeSeriesRequest\x12,\n\x06parent\x18\x01 \x01(\tB\x1c\xe0A\x02\x92A\x16\xca>\x13\xfa\x02\x10timeSeriesParent\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t"z\n\x16ListTimeSeriesResponse\x123\n\x0btime_series\x18\x01 \x03(\x0b2\x1e.exabel.api.data.v1.TimeSeries\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x12\x12\n\ntotal_size\x18\x03 \x01(\x05"r\n\x14GetTimeSeriesRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView"\xdb\x01\n\x17CreateTimeSeriesRequest\x128\n\x0btime_series\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.TimeSeriesB\x03\xe0A\x02\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x12\n\ncreate_tag\x18\x04 \x01(\x08"\xf2\x01\n\x17UpdateTimeSeriesRequest\x128\n\x0btime_series\x18\x01 \x01(\x0b2\x1e.exabel.api.data.v1.TimeSeriesB\x03\xe0A\x02\x120\n\x04view\x18\x02 \x01(\x0b2".exabel.api.data.v1.TimeSeriesView\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x15\n\rallow_missing\x18\x04 \x01(\x08\x12\x12\n\ncreate_tag\x18\x05 \x01(\x08"\xec\x01\n\x17ImportTimeSeriesRequest\x12\x13\n\x06parent\x18\x01 \x01(\tB\x03\xe0A\x02\x123\n\x0btime_series\x18\x02 \x03(\x0b2\x1e.exabel.api.data.v1.TimeSeries\x12@\n\x12default_known_time\x18\x03 \x01(\x0b2$.exabel.api.data.v1.DefaultKnownTime\x12\x15\n\rallow_missing\x18\x04 \x01(\x08\x12\x12\n\ncreate_tag\x18\x05 \x01(\x08\x12\x1a\n\x12status_in_response\x18\x06 \x01(\x08"\xa2\x02\n\x18ImportTimeSeriesResponse\x12X\n\tresponses\x18\x01 \x03(\x0b2E.exabel.api.data.v1.ImportTimeSeriesResponse.SingleTimeSeriesResponse\x1a\xab\x01\n\x18SingleTimeSeriesResponse\x12k\n\x10time_series_name\x18\x01 \x01(\tBQ\x92ANJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"\x12"\n\x06status\x18\x02 \x01(\x0b2\x12.google.rpc.Status"C\n\x17DeleteTimeSeriesRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName"\x7f\n"BatchDeleteTimeSeriesPointsRequest\x12(\n\x04name\x18\x01 \x01(\tB\x1a\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName\x12/\n\x0btime_ranges\x18\x02 \x03(\x0b2\x1a.exabel.api.time.TimeRange2\x80\x0e\n\x11TimeSeriesService\x12\xdb\x01\n\x0eListTimeSeries\x12).exabel.api.data.v1.ListTimeSeriesRequest\x1a*.exabel.api.data.v1.ListTimeSeriesResponse"r\x82\xd3\xe4\x93\x02W\x120/v1/{parent=entityTypes/*/entities/*}/timeSeriesZ#\x12!/v1/{parent=signals/*}/timeSeries\x92A\x12\x12\x10List time series\x12\xd5\x01\n\rGetTimeSeries\x12(.exabel.api.data.v1.GetTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"z\x82\xd3\xe4\x93\x02`\x12-/v1/{name=entityTypes/*/entities/*/signals/*}Z/\x12-/v1/{name=signals/*/entityTypes/*/entities/*}\x92A\x11\x12\x0fGet time series\x12\x92\x02\n\x10CreateTimeSeries\x12+.exabel.api.data.v1.CreateTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"\xb0\x01\x82\xd3\xe4\x93\x02\x92\x01"9/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH"9/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x92A\x14\x12\x12Create time series\x12\x92\x02\n\x10UpdateTimeSeries\x12+.exabel.api.data.v1.UpdateTimeSeriesRequest\x1a\x1e.exabel.api.data.v1.TimeSeries"\xb0\x01\x82\xd3\xe4\x93\x02\x92\x0129/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH29/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x92A\x14\x12\x12Update time series\x12\xf8\x01\n\x10ImportTimeSeries\x12+.exabel.api.data.v1.ImportTimeSeriesRequest\x1a,.exabel.api.data.v1.ImportTimeSeriesResponse"\x88\x01\x82\xd3\xe4\x93\x02k"7/v1/{parent=entityTypes/*/entities/*}/timeSeries:import:\x01*Z-"(/v1/{parent=signals/*}/timeSeries:import:\x01*\x92A\x14\x12\x12Import time series\x12\xd6\x01\n\x10DeleteTimeSeries\x12+.exabel.api.data.v1.DeleteTimeSeriesRequest\x1a\x16.google.protobuf.Empty"}\x82\xd3\xe4\x93\x02`*-/v1/{name=entityTypes/*/entities/*/signals/*}Z/*-/v1/{name=signals/*/entityTypes/*/entities/*}\x92A\x14\x12\x12Delete time series\x12\xb6\x02\n\x1bBatchDeleteTimeSeriesPoints\x126.exabel.api.data.v1.BatchDeleteTimeSeriesPointsRequest\x1a\x16.google.protobuf.Empty"\xc6\x01\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL\x82\xd3\xe4\x93\x02\x8c\x01"@/v1/{name=entityTypes/*/entities/*/signals/*}/points:batchDelete:\x01*ZE"@/v1/{name=signals/*/entityTypes/*/entities/*}/points:batchDelete:\x01*\x92A \x12\x1eDelete time series data pointsBJ\n\x16com.exabel.api.data.v1B\x16TimeSeriesServiceProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.time_series_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x16com.exabel.api.data.v1B\x16TimeSeriesServiceProtoP\x01Z\x16exabel.com/api/data/v1'
     _LISTTIMESERIESREQUEST.fields_by_name['parent']._options = None
     _LISTTIMESERIESREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02\x92A\x16\xca>\x13\xfa\x02\x10timeSeriesParent'
@@ -23,14 +24,16 @@
     _GETTIMESERIESREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName'
     _CREATETIMESERIESREQUEST.fields_by_name['time_series']._options = None
     _CREATETIMESERIESREQUEST.fields_by_name['time_series']._serialized_options = b'\xe0A\x02'
     _UPDATETIMESERIESREQUEST.fields_by_name['time_series']._options = None
     _UPDATETIMESERIESREQUEST.fields_by_name['time_series']._serialized_options = b'\xe0A\x02'
     _IMPORTTIMESERIESREQUEST.fields_by_name['parent']._options = None
     _IMPORTTIMESERIESREQUEST.fields_by_name['parent']._serialized_options = b'\xe0A\x02'
+    _IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE.fields_by_name['time_series_name']._options = None
+    _IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE.fields_by_name['time_series_name']._serialized_options = b'\x92ANJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"'
     _DELETETIMESERIESREQUEST.fields_by_name['name']._options = None
     _DELETETIMESERIESREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName'
     _BATCHDELETETIMESERIESPOINTSREQUEST.fields_by_name['name']._options = None
     _BATCHDELETETIMESERIESPOINTSREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x14\xca>\x11\xfa\x02\x0etimeSeriesName'
     _TIMESERIESSERVICE.methods_by_name['ListTimeSeries']._options = None
     _TIMESERIESSERVICE.methods_by_name['ListTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02W\x120/v1/{parent=entityTypes/*/entities/*}/timeSeriesZ#\x12!/v1/{parent=signals/*}/timeSeries\x92A\x12\x12\x10List time series'
     _TIMESERIESSERVICE.methods_by_name['GetTimeSeries']._options = None
@@ -41,27 +44,29 @@
     _TIMESERIESSERVICE.methods_by_name['UpdateTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02\x92\x0129/v1/{time_series.name=entityTypes/*/entities/*/signals/*}:\x0btime_seriesZH29/v1/{time_series.name=signals/*/entityTypes/*/entities/*}:\x0btime_series\x92A\x14\x12\x12Update time series'
     _TIMESERIESSERVICE.methods_by_name['ImportTimeSeries']._options = None
     _TIMESERIESSERVICE.methods_by_name['ImportTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02k"7/v1/{parent=entityTypes/*/entities/*}/timeSeries:import:\x01*Z-"(/v1/{parent=signals/*}/timeSeries:import:\x01*\x92A\x14\x12\x12Import time series'
     _TIMESERIESSERVICE.methods_by_name['DeleteTimeSeries']._options = None
     _TIMESERIESSERVICE.methods_by_name['DeleteTimeSeries']._serialized_options = b'\x82\xd3\xe4\x93\x02`*-/v1/{name=entityTypes/*/entities/*/signals/*}Z/*-/v1/{name=signals/*/entityTypes/*/entities/*}\x92A\x14\x12\x12Delete time series'
     _TIMESERIESSERVICE.methods_by_name['BatchDeleteTimeSeriesPoints']._options = None
     _TIMESERIESSERVICE.methods_by_name['BatchDeleteTimeSeriesPoints']._serialized_options = b'\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL\x82\xd3\xe4\x93\x02\x8c\x01"@/v1/{name=entityTypes/*/entities/*/signals/*}/points:batchDelete:\x01*ZE"@/v1/{name=signals/*/entityTypes/*/entities/*}/points:batchDelete:\x01*\x92A \x12\x1eDelete time series data points'
-    _LISTTIMESERIESREQUEST._serialized_start = 318
-    _LISTTIMESERIESREQUEST._serialized_end = 426
-    _LISTTIMESERIESRESPONSE._serialized_start = 428
-    _LISTTIMESERIESRESPONSE._serialized_end = 550
-    _GETTIMESERIESREQUEST._serialized_start = 552
-    _GETTIMESERIESREQUEST._serialized_end = 666
-    _CREATETIMESERIESREQUEST._serialized_start = 669
-    _CREATETIMESERIESREQUEST._serialized_end = 888
-    _UPDATETIMESERIESREQUEST._serialized_start = 891
-    _UPDATETIMESERIESREQUEST._serialized_end = 1133
-    _IMPORTTIMESERIESREQUEST._serialized_start = 1136
-    _IMPORTTIMESERIESREQUEST._serialized_end = 1344
-    _IMPORTTIMESERIESRESPONSE._serialized_start = 1346
-    _IMPORTTIMESERIESRESPONSE._serialized_end = 1372
-    _DELETETIMESERIESREQUEST._serialized_start = 1374
-    _DELETETIMESERIESREQUEST._serialized_end = 1441
-    _BATCHDELETETIMESERIESPOINTSREQUEST._serialized_start = 1443
-    _BATCHDELETETIMESERIESPOINTSREQUEST._serialized_end = 1570
-    _TIMESERIESSERVICE._serialized_start = 1573
-    _TIMESERIESSERVICE._serialized_end = 3365
+    _LISTTIMESERIESREQUEST._serialized_start = 343
+    _LISTTIMESERIESREQUEST._serialized_end = 451
+    _LISTTIMESERIESRESPONSE._serialized_start = 453
+    _LISTTIMESERIESRESPONSE._serialized_end = 575
+    _GETTIMESERIESREQUEST._serialized_start = 577
+    _GETTIMESERIESREQUEST._serialized_end = 691
+    _CREATETIMESERIESREQUEST._serialized_start = 694
+    _CREATETIMESERIESREQUEST._serialized_end = 913
+    _UPDATETIMESERIESREQUEST._serialized_start = 916
+    _UPDATETIMESERIESREQUEST._serialized_end = 1158
+    _IMPORTTIMESERIESREQUEST._serialized_start = 1161
+    _IMPORTTIMESERIESREQUEST._serialized_end = 1397
+    _IMPORTTIMESERIESRESPONSE._serialized_start = 1400
+    _IMPORTTIMESERIESRESPONSE._serialized_end = 1690
+    _IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE._serialized_start = 1519
+    _IMPORTTIMESERIESRESPONSE_SINGLETIMESERIESRESPONSE._serialized_end = 1690
+    _DELETETIMESERIESREQUEST._serialized_start = 1692
+    _DELETETIMESERIESREQUEST._serialized_end = 1759
+    _BATCHDELETETIMESERIESPOINTSREQUEST._serialized_start = 1761
+    _BATCHDELETETIMESERIESPOINTSREQUEST._serialized_end = 1888
+    _TIMESERIESSERVICE._serialized_start = 1891
+    _TIMESERIESSERVICE._serialized_end = 3683
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 from .....exabel.api.data.v1 import time_series_messages_pb2 as exabel_dot_api_dot_data_dot_v1_dot_time__series__messages__pb2
 from .....exabel.api.data.v1 import time_series_service_pb2 as exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 class TimeSeriesServiceStub(object):
-    """Service for managing time series. See the User Guide for more information about time series.
+    """Service for managing time series. See the User Guide for more information about time series:
+    https://help.exabel.com/docs/time-series
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -19,15 +20,16 @@
         self.CreateTimeSeries = channel.unary_unary('/exabel.api.data.v1.TimeSeriesService/CreateTimeSeries', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.CreateTimeSeriesRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__messages__pb2.TimeSeries.FromString)
         self.UpdateTimeSeries = channel.unary_unary('/exabel.api.data.v1.TimeSeriesService/UpdateTimeSeries', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.UpdateTimeSeriesRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__messages__pb2.TimeSeries.FromString)
         self.ImportTimeSeries = channel.unary_unary('/exabel.api.data.v1.TimeSeriesService/ImportTimeSeries', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.ImportTimeSeriesRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.ImportTimeSeriesResponse.FromString)
         self.DeleteTimeSeries = channel.unary_unary('/exabel.api.data.v1.TimeSeriesService/DeleteTimeSeries', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.DeleteTimeSeriesRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
         self.BatchDeleteTimeSeriesPoints = channel.unary_unary('/exabel.api.data.v1.TimeSeriesService/BatchDeleteTimeSeriesPoints', request_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.BatchDeleteTimeSeriesPointsRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
 
 class TimeSeriesServiceServicer(object):
-    """Service for managing time series. See the User Guide for more information about time series.
+    """Service for managing time series. See the User Guide for more information about time series:
+    https://help.exabel.com/docs/time-series
     """
 
     def ListTimeSeries(self, request, context):
         """Lists time series.
 
         Lists all time series for one entity or for one signal. Only the names are returned.
         """
@@ -49,16 +51,23 @@
 
     def CreateTimeSeries(self, request, context):
         """Creates one time series.
 
         *Note*: Exabel only supports processing time series with daily or lower resolution. Timestamps
         must be RFC 3339 timestamps, normalised to **midnight UTC**, e.g. `2020-01-01T00:00:00Z`.
 
+        The default `known_time` for a data point is insertion time, i.e. same as setting
+        `current_time` to `true`. To override the default behaviour, set one of the
+        `default_known_time` fields.
+
         The optional `view` argument lets you request for time series data points to be returned
         within a date range. If this is not set, no values are returned.
+
+        It is also possible to create a time series by calling `UpdateTimeSeries`
+        with `allow_missing` set to `true`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateTimeSeries(self, request, context):
         """Updates one time series.
@@ -76,14 +85,18 @@
         old value will continue to exist up until the new version, then cease to exist.
 
         Time series storage is optimized by discarding values which haven't changed from the previous
         versions. Note that this optimization may cause surprising behavior when updating older
         versions. When older versions are updated, it is therefore recommended to perform a full
         backload from this version on.
 
+        The default `known_time` for a data point is insertion time, i.e. same as setting
+        `current_time` to `true`. To override the default behaviour, set one of the
+        `default_known_time` fields.
+
         *Note*: Exabel only supports processing time series with daily or lower resolution. Timestamps
         must be RFC 3339 timestamps, normalised to **midnight UTC**, e.g. `2020-01-01T00:00:00Z`.
 
         The optional `view` argument lets you request for time series data points to be returned
         within a date range. If this is not set, no values are returned.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -96,14 +109,18 @@
         Import multiple time series in bulk, by creating new time series or updating existing time
         series.
 
         If you would like to import multiple time series belonging to different signals, specify `-`
         as the `signalId` path parameter. (Signal IDs are part of each time series' resource name,
         so your time series will still be assigned to their corresponding signals.)
 
+        The default `known_time` for a data point is insertion time, i.e. same as setting
+        `current_time` to `true`. To override the default behaviour, set one of the
+        `default_known_time` fields.
+
         *Note*: Exabel only supports processing time series with daily or lower resolution. Timestamps
         must be RFC 3339 timestamps, normalised to **midnight UTC**, e.g. `2020-01-01T00:00:00Z`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -131,15 +148,16 @@
 
 def add_TimeSeriesServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {'ListTimeSeries': grpc.unary_unary_rpc_method_handler(servicer.ListTimeSeries, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.ListTimeSeriesRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.ListTimeSeriesResponse.SerializeToString), 'GetTimeSeries': grpc.unary_unary_rpc_method_handler(servicer.GetTimeSeries, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.GetTimeSeriesRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__messages__pb2.TimeSeries.SerializeToString), 'CreateTimeSeries': grpc.unary_unary_rpc_method_handler(servicer.CreateTimeSeries, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.CreateTimeSeriesRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__messages__pb2.TimeSeries.SerializeToString), 'UpdateTimeSeries': grpc.unary_unary_rpc_method_handler(servicer.UpdateTimeSeries, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.UpdateTimeSeriesRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__messages__pb2.TimeSeries.SerializeToString), 'ImportTimeSeries': grpc.unary_unary_rpc_method_handler(servicer.ImportTimeSeries, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.ImportTimeSeriesRequest.FromString, response_serializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.ImportTimeSeriesResponse.SerializeToString), 'DeleteTimeSeries': grpc.unary_unary_rpc_method_handler(servicer.DeleteTimeSeries, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.DeleteTimeSeriesRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'BatchDeleteTimeSeriesPoints': grpc.unary_unary_rpc_method_handler(servicer.BatchDeleteTimeSeriesPoints, request_deserializer=exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.BatchDeleteTimeSeriesPointsRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString)}
     generic_handler = grpc.method_handlers_generic_handler('exabel.api.data.v1.TimeSeriesService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 class TimeSeriesService(object):
-    """Service for managing time series. See the User Guide for more information about time series.
+    """Service for managing time series. See the User Guide for more information about time series:
+    https://help.exabel.com/docs/time-series
     """
 
     @staticmethod
     def ListTimeSeries(request, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
         return grpc.experimental.unary_unary(request, target, '/exabel.api.data.v1.TimeSeriesService/ListTimeSeries', exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.ListTimeSeriesRequest.SerializeToString, exabel_dot_api_dot_data_dot_v1_dot_time__series__service__pb2.ListTimeSeriesResponse.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,35 +4,39 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 _sym_db = _symbol_database.Default()
 from .....exabel.api.management.v1 import user_messages_pb2 as exabel_dot_api_dot_management_dot_v1_dot_user__messages__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/folder_messages.proto\x12\x18exabel.api.management.v1\x1a,exabel/api/management/v1/user_messages.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xbd\x01\n\x06Folder\x120\n\x04name\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x120\n\x0cdisplay_name\x18\x02 \x01(\tB\x1a\xe0A\x02\x92A\x14J\x12"My shared folder"\x12\x12\n\x05write\x18\x03 \x01(\x08B\x03\xe0A\x03\x12;\n\x05items\x18\x04 \x03(\x0b2$.exabel.api.management.v1.FolderItemB\x06\xe0A\x06\xe0A\x03"\xf0\x02\n\nFolderItem\x122\n\x06parent\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12*\n\x04name\x18\x02 \x01(\tB\x1c\xe0A\x03\x92A\x16J\x14"derivedSignals/123"\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"my_signal"\x12\x13\n\x0bdescription\x18\t \x01(\t\x12;\n\titem_type\x18\x04 \x01(\x0e2(.exabel.api.management.v1.FolderItemType\x12/\n\x0bcreate_time\x18\x05 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\x06 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12\x12\n\nupdated_by\x18\x08 \x01(\t"O\n\x0eFolderAccessor\x12.\n\x05group\x18\x01 \x01(\x0b2\x1f.exabel.api.management.v1.Group\x12\r\n\x05write\x18\x02 \x01(\x08*\xc4\x01\n\x0eFolderItemType\x12\x1c\n\x18FOLDER_ITEM_TYPE_INVALID\x10\x00\x12\x12\n\x0eDERIVED_SIGNAL\x10\x01\x12\x14\n\x10PREDICTION_MODEL\x10\x02\x12\x16\n\x12PORTFOLIO_STRATEGY\x10\x03\x12\r\n\tDASHBOARD\x10\x04\x12\x0e\n\nDRILL_DOWN\x10\x05\x12\x07\n\x03TAG\x10\x06\x12\n\n\x06SCREEN\x10\x07\x12\x13\n\x0fFINANCIAL_MODEL\x10\x08\x12\t\n\x05CHART\x10\tBS\n\x1ccom.exabel.api.management.v1B\x13FolderMessagesProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/folder_messages.proto\x12\x18exabel.api.management.v1\x1a,exabel/api/management/v1/user_messages.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xf3\x01\n\x06Folder\x120\n\x04name\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x120\n\x0cdisplay_name\x18\x02 \x01(\tB\x1a\xe0A\x02\x92A\x14J\x12"My shared folder"\x12\x12\n\x05write\x18\x03 \x01(\x08B\x03\xe0A\x03\x12;\n\x05items\x18\x04 \x03(\x0b2$.exabel.api.management.v1.FolderItemB\x06\xe0A\x06\xe0A\x03\x124\n\x0bdescription\x18\x05 \x01(\tB\x1f\x92A\x1cJ\x1a"This is my shared folder""\xf0\x02\n\nFolderItem\x122\n\x06parent\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12*\n\x04name\x18\x02 \x01(\tB\x1c\xe0A\x03\x92A\x16J\x14"derivedSignals/123"\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"my_signal"\x12\x13\n\x0bdescription\x18\t \x01(\t\x12;\n\titem_type\x18\x04 \x01(\x0e2(.exabel.api.management.v1.FolderItemType\x12/\n\x0bcreate_time\x18\x05 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\x06 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12\x12\n\nupdated_by\x18\x08 \x01(\t"O\n\x0eFolderAccessor\x12.\n\x05group\x18\x01 \x01(\x0b2\x1f.exabel.api.management.v1.Group\x12\r\n\x05write\x18\x02 \x01(\x08"B\n\x0cSearchResult\x122\n\x04item\x18\x01 \x01(\x0b2$.exabel.api.management.v1.FolderItem*\xc4\x01\n\x0eFolderItemType\x12\x1c\n\x18FOLDER_ITEM_TYPE_INVALID\x10\x00\x12\x12\n\x0eDERIVED_SIGNAL\x10\x01\x12\x14\n\x10PREDICTION_MODEL\x10\x02\x12\x16\n\x12PORTFOLIO_STRATEGY\x10\x03\x12\r\n\tDASHBOARD\x10\x04\x12\x0e\n\nDRILL_DOWN\x10\x05\x12\x07\n\x03TAG\x10\x06\x12\n\n\x06SCREEN\x10\x07\x12\x13\n\x0fFINANCIAL_MODEL\x10\x08\x12\t\n\x05CHART\x10\tBS\n\x1ccom.exabel.api.management.v1B\x13FolderMessagesProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.folder_messages_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1ccom.exabel.api.management.v1B\x13FolderMessagesProtoP\x01Z\x1cexabel.com/api/management/v1'
     _FOLDER.fields_by_name['name']._options = None
     _FOLDER.fields_by_name['name']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _FOLDER.fields_by_name['display_name']._options = None
     _FOLDER.fields_by_name['display_name']._serialized_options = b'\xe0A\x02\x92A\x14J\x12"My shared folder"'
     _FOLDER.fields_by_name['write']._options = None
     _FOLDER.fields_by_name['write']._serialized_options = b'\xe0A\x03'
     _FOLDER.fields_by_name['items']._options = None
     _FOLDER.fields_by_name['items']._serialized_options = b'\xe0A\x06\xe0A\x03'
+    _FOLDER.fields_by_name['description']._options = None
+    _FOLDER.fields_by_name['description']._serialized_options = b'\x92A\x1cJ\x1a"This is my shared folder"'
     _FOLDERITEM.fields_by_name['parent']._options = None
     _FOLDERITEM.fields_by_name['parent']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _FOLDERITEM.fields_by_name['name']._options = None
     _FOLDERITEM.fields_by_name['name']._serialized_options = b'\xe0A\x03\x92A\x16J\x14"derivedSignals/123"'
     _FOLDERITEM.fields_by_name['display_name']._options = None
     _FOLDERITEM.fields_by_name['display_name']._serialized_options = b'\x92A\rJ\x0b"my_signal"'
-    _FOLDERITEMTYPE._serialized_start = 881
-    _FOLDERITEMTYPE._serialized_end = 1077
+    _FOLDERITEMTYPE._serialized_start = 1003
+    _FOLDERITEMTYPE._serialized_end = 1199
     _FOLDER._serialized_start = 237
-    _FOLDER._serialized_end = 426
-    _FOLDERITEM._serialized_start = 429
-    _FOLDERITEM._serialized_end = 797
-    _FOLDERACCESSOR._serialized_start = 799
-    _FOLDERACCESSOR._serialized_end = 878
+    _FOLDER._serialized_end = 480
+    _FOLDERITEM._serialized_start = 483
+    _FOLDERITEM._serialized_end = 851
+    _FOLDERACCESSOR._serialized_start = 853
+    _FOLDERACCESSOR._serialized_end = 932
+    _SEARCHRESULT._serialized_start = 934
+    _SEARCHRESULT._serialized_end = 1000
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 _sym_db = _symbol_database.Default()
 from .....exabel.api.management.v1 import folder_messages_pb2 as exabel_dot_api_dot_management_dot_v1_dot_folder__messages__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/library_service.proto\x12\x18exabel.api.management.v1\x1a.exabel/api/management/v1/folder_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x14\n\x12ListFoldersRequest"H\n\x13ListFoldersResponse\x121\n\x07folders\x18\x01 \x03(\x0b2 .exabel.api.management.v1.Folder"8\n\x10GetFolderRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName"L\n\x13CreateFolderRequest\x125\n\x06folder\x18\x01 \x01(\x0b2 .exabel.api.management.v1.FolderB\x03\xe0A\x02"\x94\x01\n\x13UpdateFolderRequest\x125\n\x06folder\x18\x01 \x01(\x0b2 .exabel.api.management.v1.FolderB\x03\xe0A\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08";\n\x13DeleteFolderRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName"\x86\x01\n\x10ListItemsRequest\x125\n\x06parent\x18\x01 \x01(\tB%\xe0A\x01\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12;\n\titem_type\x18\x02 \x01(\x0e2(.exabel.api.management.v1.FolderItemType"H\n\x11ListItemsResponse\x123\n\x05items\x18\x01 \x03(\x0b2$.exabel.api.management.v1.FolderItem"U\n\x10MoveItemsRequest\x12\x12\n\x05items\x18\x01 \x03(\tB\x03\xe0A\x02\x12-\n\rtarget_folder\x18\x02 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName"\x13\n\x11MoveItemsResponse"?\n\x1aListFolderAccessorsRequest\x12!\n\x04name\x18\x01 \x01(\tB\x13\x92A\x10\xca>\r\xfa\x02\nfolderName"a\n\x1bListFolderAccessorsResponse\x12B\n\x10folder_accessors\x18\x01 \x03(\x0b2(.exabel.api.management.v1.FolderAccessor"y\n\x12ShareFolderRequest\x122\n\x06folder\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12 \n\x05group\x18\x02 \x01(\tB\x11\x92A\x0eJ\x0c"groups/123"\x12\r\n\x05write\x18\x03 \x01(\x08"l\n\x14UnshareFolderRequest\x122\n\x06folder\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12 \n\x05group\x18\x02 \x01(\tB\x11\x92A\x0eJ\x0c"groups/123"2\xa6\x0c\n\x0eLibraryService\x12\x90\x01\n\x0bListFolders\x12,.exabel.api.management.v1.ListFoldersRequest\x1a-.exabel.api.management.v1.ListFoldersResponse"$\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/folders\x92A\x0e\x12\x0cList folders\x12\x86\x01\n\tGetFolder\x12*.exabel.api.management.v1.GetFolderRequest\x1a .exabel.api.management.v1.Folder"+\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=folders/*}\x92A\x0c\x12\nGet folder\x12\x8e\x01\n\x0cCreateFolder\x12-.exabel.api.management.v1.CreateFolderRequest\x1a .exabel.api.management.v1.Folder"-\x82\xd3\xe4\x93\x02\x15"\x0b/v1/folders:\x06folder\x92A\x0f\x12\rCreate folder\x12\x9e\x01\n\x0cUpdateFolder\x12-.exabel.api.management.v1.UpdateFolderRequest\x1a .exabel.api.management.v1.Folder"=\x82\xd3\xe4\x93\x02%2\x1b/v1/{folder.name=folders/*}:\x06folder\x92A\x0f\x12\rUpdate folder\x12\x85\x01\n\x0cDeleteFolder\x12-.exabel.api.management.v1.DeleteFolderRequest\x1a\x16.google.protobuf.Empty".\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=folders/*}\x92A\x0f\x12\rDelete folder\x12\xa0\x01\n\tListItems\x12*.exabel.api.management.v1.ListItemsRequest\x1a+.exabel.api.management.v1.ListItemsResponse":\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=folders/*}/items\x92A\x13\x12\x11List folder items\x12\xab\x01\n\tMoveItems\x12*.exabel.api.management.v1.MoveItemsRequest\x1a+.exabel.api.management.v1.MoveItemsResponse"E\x82\xd3\xe4\x93\x02)"\'/v1/{target_folder=folders/*}:moveItems\x92A\x13\x12\x11Move folder items\x12\xc4\x01\n\x13ListFolderAccessors\x124.exabel.api.management.v1.ListFolderAccessorsRequest\x1a5.exabel.api.management.v1.ListFolderAccessorsResponse"@\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=folders/*}/accessors\x92A\x17\x12\x15List folder accessors\x12\x8d\x01\n\x0bShareFolder\x12,.exabel.api.management.v1.ShareFolderRequest\x1a\x16.google.protobuf.Empty"8\x82\xd3\xe4\x93\x02!"\x1c/v1/{folder=folders/*}:share:\x01*\x92A\x0e\x12\x0cShare folder\x12\x95\x01\n\rUnshareFolder\x12..exabel.api.management.v1.UnshareFolderRequest\x1a\x16.google.protobuf.Empty"<\x82\xd3\xe4\x93\x02#"\x1e/v1/{folder=folders/*}:unshare:\x01*\x92A\x10\x12\x0eUnshare folderBS\n\x1ccom.exabel.api.management.v1B\x13LibraryServiceProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/library_service.proto\x12\x18exabel.api.management.v1\x1a.exabel/api/management/v1/folder_messages.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x14\n\x12ListFoldersRequest"H\n\x13ListFoldersResponse\x121\n\x07folders\x18\x01 \x03(\x0b2 .exabel.api.management.v1.Folder"8\n\x10GetFolderRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName"L\n\x13CreateFolderRequest\x125\n\x06folder\x18\x01 \x01(\x0b2 .exabel.api.management.v1.FolderB\x03\xe0A\x02"\x94\x01\n\x13UpdateFolderRequest\x125\n\x06folder\x18\x01 \x01(\x0b2 .exabel.api.management.v1.FolderB\x03\xe0A\x02\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b2\x1a.google.protobuf.FieldMask\x12\x15\n\rallow_missing\x18\x03 \x01(\x08";\n\x13DeleteFolderRequest\x12$\n\x04name\x18\x01 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName"\x86\x01\n\x10ListItemsRequest\x125\n\x06parent\x18\x01 \x01(\tB%\xe0A\x01\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12;\n\titem_type\x18\x02 \x01(\x0e2(.exabel.api.management.v1.FolderItemType"H\n\x11ListItemsResponse\x123\n\x05items\x18\x01 \x03(\x0b2$.exabel.api.management.v1.FolderItem"U\n\x10MoveItemsRequest\x12\x12\n\x05items\x18\x01 \x03(\tB\x03\xe0A\x02\x12-\n\rtarget_folder\x18\x02 \x01(\tB\x16\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName"\x13\n\x11MoveItemsResponse"?\n\x1aListFolderAccessorsRequest\x12!\n\x04name\x18\x01 \x01(\tB\x13\x92A\x10\xca>\r\xfa\x02\nfolderName"a\n\x1bListFolderAccessorsResponse\x12B\n\x10folder_accessors\x18\x01 \x03(\x0b2(.exabel.api.management.v1.FolderAccessor"y\n\x12ShareFolderRequest\x122\n\x06folder\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12 \n\x05group\x18\x02 \x01(\tB\x11\x92A\x0eJ\x0c"groups/123"\x12\r\n\x05write\x18\x03 \x01(\x08"l\n\x14UnshareFolderRequest\x122\n\x06folder\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12 \n\x05group\x18\x02 \x01(\tB\x11\x92A\x0eJ\x0c"groups/123""\xd0\x01\n\x12SearchItemsRequest\x12=\n\x06folder\x18\x01 \x01(\tB-\xe0A\x02\x92A\'J\x0b"folders/-"\xca>\x17\xfa\x02\x14folderNameAllFolders\x12\x12\n\x05query\x18\x02 \x01(\tB\x03\xe0A\x02\x12@\n\titem_type\x18\x03 \x01(\x0e2(.exabel.api.management.v1.FolderItemTypeB\x03\xe0A\x01\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x11\n\tpage_size\x18\x05 \x01(\x05"g\n\x13SearchItemsResponse\x127\n\x07results\x18\x01 \x03(\x0b2&.exabel.api.management.v1.SearchResult\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t2\xdc\r\n\x0eLibraryService\x12\x90\x01\n\x0bListFolders\x12,.exabel.api.management.v1.ListFoldersRequest\x1a-.exabel.api.management.v1.ListFoldersResponse"$\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/folders\x92A\x0e\x12\x0cList folders\x12\x86\x01\n\tGetFolder\x12*.exabel.api.management.v1.GetFolderRequest\x1a .exabel.api.management.v1.Folder"+\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=folders/*}\x92A\x0c\x12\nGet folder\x12\x8e\x01\n\x0cCreateFolder\x12-.exabel.api.management.v1.CreateFolderRequest\x1a .exabel.api.management.v1.Folder"-\x82\xd3\xe4\x93\x02\x15"\x0b/v1/folders:\x06folder\x92A\x0f\x12\rCreate folder\x12\x9e\x01\n\x0cUpdateFolder\x12-.exabel.api.management.v1.UpdateFolderRequest\x1a .exabel.api.management.v1.Folder"=\x82\xd3\xe4\x93\x02%2\x1b/v1/{folder.name=folders/*}:\x06folder\x92A\x0f\x12\rUpdate folder\x12\x85\x01\n\x0cDeleteFolder\x12-.exabel.api.management.v1.DeleteFolderRequest\x1a\x16.google.protobuf.Empty".\x82\xd3\xe4\x93\x02\x16*\x14/v1/{name=folders/*}\x92A\x0f\x12\rDelete folder\x12\xa0\x01\n\tListItems\x12*.exabel.api.management.v1.ListItemsRequest\x1a+.exabel.api.management.v1.ListItemsResponse":\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/{parent=folders/*}/items\x92A\x13\x12\x11List folder items\x12\xab\x01\n\tMoveItems\x12*.exabel.api.management.v1.MoveItemsRequest\x1a+.exabel.api.management.v1.MoveItemsResponse"E\x82\xd3\xe4\x93\x02)"\'/v1/{target_folder=folders/*}:moveItems\x92A\x13\x12\x11Move folder items\x12\xc4\x01\n\x13ListFolderAccessors\x124.exabel.api.management.v1.ListFolderAccessorsRequest\x1a5.exabel.api.management.v1.ListFolderAccessorsResponse"@\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=folders/*}/accessors\x92A\x17\x12\x15List folder accessors\x12\x8d\x01\n\x0bShareFolder\x12,.exabel.api.management.v1.ShareFolderRequest\x1a\x16.google.protobuf.Empty"8\x82\xd3\xe4\x93\x02!"\x1c/v1/{folder=folders/*}:share:\x01*\x92A\x0e\x12\x0cShare folder\x12\x95\x01\n\rUnshareFolder\x12..exabel.api.management.v1.UnshareFolderRequest\x1a\x16.google.protobuf.Empty"<\x82\xd3\xe4\x93\x02#"\x1e/v1/{folder=folders/*}:unshare:\x01*\x92A\x10\x12\x0eUnshare folder\x12\xb3\x01\n\x0bSearchItems\x12,.exabel.api.management.v1.SearchItemsRequest\x1a-.exabel.api.management.v1.SearchItemsResponse"G\x82\xd3\xe4\x93\x02%\x12#/v1/{folder=folders/*}/items:search\x92A\x19\x12\x17Search for folder itemsBS\n\x1ccom.exabel.api.management.v1B\x13LibraryServiceProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.library_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1ccom.exabel.api.management.v1B\x13LibraryServiceProtoP\x01Z\x1cexabel.com/api/management/v1'
     _GETFOLDERREQUEST.fields_by_name['name']._options = None
     _GETFOLDERREQUEST.fields_by_name['name']._serialized_options = b'\xe0A\x02\x92A\x10\xca>\r\xfa\x02\nfolderName'
@@ -36,14 +36,20 @@
     _SHAREFOLDERREQUEST.fields_by_name['folder']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _SHAREFOLDERREQUEST.fields_by_name['group']._options = None
     _SHAREFOLDERREQUEST.fields_by_name['group']._serialized_options = b'\x92A\x0eJ\x0c"groups/123"'
     _UNSHAREFOLDERREQUEST.fields_by_name['folder']._options = None
     _UNSHAREFOLDERREQUEST.fields_by_name['folder']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _UNSHAREFOLDERREQUEST.fields_by_name['group']._options = None
     _UNSHAREFOLDERREQUEST.fields_by_name['group']._serialized_options = b'\x92A\x0eJ\x0c"groups/123"'
+    _SEARCHITEMSREQUEST.fields_by_name['folder']._options = None
+    _SEARCHITEMSREQUEST.fields_by_name['folder']._serialized_options = b'\xe0A\x02\x92A\'J\x0b"folders/-"\xca>\x17\xfa\x02\x14folderNameAllFolders'
+    _SEARCHITEMSREQUEST.fields_by_name['query']._options = None
+    _SEARCHITEMSREQUEST.fields_by_name['query']._serialized_options = b'\xe0A\x02'
+    _SEARCHITEMSREQUEST.fields_by_name['item_type']._options = None
+    _SEARCHITEMSREQUEST.fields_by_name['item_type']._serialized_options = b'\xe0A\x01'
     _LIBRARYSERVICE.methods_by_name['ListFolders']._options = None
     _LIBRARYSERVICE.methods_by_name['ListFolders']._serialized_options = b'\x82\xd3\xe4\x93\x02\r\x12\x0b/v1/folders\x92A\x0e\x12\x0cList folders'
     _LIBRARYSERVICE.methods_by_name['GetFolder']._options = None
     _LIBRARYSERVICE.methods_by_name['GetFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/{name=folders/*}\x92A\x0c\x12\nGet folder'
     _LIBRARYSERVICE.methods_by_name['CreateFolder']._options = None
     _LIBRARYSERVICE.methods_by_name['CreateFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02\x15"\x0b/v1/folders:\x06folder\x92A\x0f\x12\rCreate folder'
     _LIBRARYSERVICE.methods_by_name['UpdateFolder']._options = None
@@ -56,14 +62,16 @@
     _LIBRARYSERVICE.methods_by_name['MoveItems']._serialized_options = b'\x82\xd3\xe4\x93\x02)"\'/v1/{target_folder=folders/*}:moveItems\x92A\x13\x12\x11Move folder items'
     _LIBRARYSERVICE.methods_by_name['ListFolderAccessors']._options = None
     _LIBRARYSERVICE.methods_by_name['ListFolderAccessors']._serialized_options = b'\x82\xd3\xe4\x93\x02 \x12\x1e/v1/{name=folders/*}/accessors\x92A\x17\x12\x15List folder accessors'
     _LIBRARYSERVICE.methods_by_name['ShareFolder']._options = None
     _LIBRARYSERVICE.methods_by_name['ShareFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02!"\x1c/v1/{folder=folders/*}:share:\x01*\x92A\x0e\x12\x0cShare folder'
     _LIBRARYSERVICE.methods_by_name['UnshareFolder']._options = None
     _LIBRARYSERVICE.methods_by_name['UnshareFolder']._serialized_options = b'\x82\xd3\xe4\x93\x02#"\x1e/v1/{folder=folders/*}:unshare:\x01*\x92A\x10\x12\x0eUnshare folder'
+    _LIBRARYSERVICE.methods_by_name['SearchItems']._options = None
+    _LIBRARYSERVICE.methods_by_name['SearchItems']._serialized_options = b'\x82\xd3\xe4\x93\x02%\x12#/v1/{folder=folders/*}/items:search\x92A\x19\x12\x17Search for folder items'
     _LISTFOLDERSREQUEST._serialized_start = 298
     _LISTFOLDERSREQUEST._serialized_end = 318
     _LISTFOLDERSRESPONSE._serialized_start = 320
     _LISTFOLDERSRESPONSE._serialized_end = 392
     _GETFOLDERREQUEST._serialized_start = 394
     _GETFOLDERREQUEST._serialized_end = 450
     _CREATEFOLDERREQUEST._serialized_start = 452
@@ -84,9 +92,13 @@
     _LISTFOLDERACCESSORSREQUEST._serialized_end = 1124
     _LISTFOLDERACCESSORSRESPONSE._serialized_start = 1126
     _LISTFOLDERACCESSORSRESPONSE._serialized_end = 1223
     _SHAREFOLDERREQUEST._serialized_start = 1225
     _SHAREFOLDERREQUEST._serialized_end = 1346
     _UNSHAREFOLDERREQUEST._serialized_start = 1348
     _UNSHAREFOLDERREQUEST._serialized_end = 1456
-    _LIBRARYSERVICE._serialized_start = 1459
-    _LIBRARYSERVICE._serialized_end = 3033
+    _SEARCHITEMSREQUEST._serialized_start = 1459
+    _SEARCHITEMSREQUEST._serialized_end = 1667
+    _SEARCHITEMSRESPONSE._serialized_start = 1669
+    _SEARCHITEMSRESPONSE._serialized_end = 1772
+    _LIBRARYSERVICE._serialized_start = 1775
+    _LIBRARYSERVICE._serialized_end = 3531
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         self.UpdateFolder = channel.unary_unary('/exabel.api.management.v1.LibraryService/UpdateFolder', request_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.UpdateFolderRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_management_dot_v1_dot_folder__messages__pb2.Folder.FromString)
         self.DeleteFolder = channel.unary_unary('/exabel.api.management.v1.LibraryService/DeleteFolder', request_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.DeleteFolderRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
         self.ListItems = channel.unary_unary('/exabel.api.management.v1.LibraryService/ListItems', request_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListItemsRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListItemsResponse.FromString)
         self.MoveItems = channel.unary_unary('/exabel.api.management.v1.LibraryService/MoveItems', request_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.MoveItemsRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.MoveItemsResponse.FromString)
         self.ListFolderAccessors = channel.unary_unary('/exabel.api.management.v1.LibraryService/ListFolderAccessors', request_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFolderAccessorsRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFolderAccessorsResponse.FromString)
         self.ShareFolder = channel.unary_unary('/exabel.api.management.v1.LibraryService/ShareFolder', request_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ShareFolderRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
         self.UnshareFolder = channel.unary_unary('/exabel.api.management.v1.LibraryService/UnshareFolder', request_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.UnshareFolderRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
+        self.SearchItems = channel.unary_unary('/exabel.api.management.v1.LibraryService/SearchItems', request_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.SearchItemsRequest.SerializeToString, response_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.SearchItemsResponse.FromString)
 
 class LibraryServiceServicer(object):
     """Service to manage library items.
 
     Requests to the LibraryService are executed in the context of the customer's service account (SA).
     The SA is a special user that is a member of the customer user group, giving it access to all
     folders that are shared with this user group, but not to private folders.
@@ -55,31 +56,36 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateFolder(self, request, context):
         """Creates a folder.
 
-        Only the display name can be set. Items must be added to the new folder subsequently with the
-        "Move folder items" method.
+        Only the display name and description can be set. Items must be added to the new folder
+        subsequently with the "Move folder items" method.
 
         The folder will be created as private to the service account user. To let other users access
         this folder, you must also share it with the "Share folder" method.
+
+        It is also possible to create a folder type by calling `UpdateFolder`
+        with `allow_missing` set to `true`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateFolder(self, request, context):
         """Updates a folder.
 
-        Only the display name can be updated. Items must be added to a folder with the "Move folder
-        items" method.
+        Only the display name and description can be updated. Items must be added to a folder with the
+        "Move folder items" method.
+
+        This can also be used to create an entity by setting `allow_missing` to `true`.
 
-        Note that this method update all fields unless `update_mask` is set.
+        Note that this method will update all fields unless `update_mask` is set.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteFolder(self, request, context):
         """Deletes a folder.
@@ -137,16 +143,25 @@
         This revokes both read and write access. To revoke only write access, use the "Share folder"
         method with the `write` flag set to `false`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SearchItems(self, request, context):
+        """Search for folder items.
+
+        Search for all folder items or items of a specific type (e.g. derived signal, dashboard) across all folders.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 def add_LibraryServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {'ListFolders': grpc.unary_unary_rpc_method_handler(servicer.ListFolders, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFoldersRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFoldersResponse.SerializeToString), 'GetFolder': grpc.unary_unary_rpc_method_handler(servicer.GetFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.GetFolderRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_folder__messages__pb2.Folder.SerializeToString), 'CreateFolder': grpc.unary_unary_rpc_method_handler(servicer.CreateFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.CreateFolderRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_folder__messages__pb2.Folder.SerializeToString), 'UpdateFolder': grpc.unary_unary_rpc_method_handler(servicer.UpdateFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.UpdateFolderRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_folder__messages__pb2.Folder.SerializeToString), 'DeleteFolder': grpc.unary_unary_rpc_method_handler(servicer.DeleteFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.DeleteFolderRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'ListItems': grpc.unary_unary_rpc_method_handler(servicer.ListItems, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListItemsRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListItemsResponse.SerializeToString), 'MoveItems': grpc.unary_unary_rpc_method_handler(servicer.MoveItems, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.MoveItemsRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.MoveItemsResponse.SerializeToString), 'ListFolderAccessors': grpc.unary_unary_rpc_method_handler(servicer.ListFolderAccessors, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFolderAccessorsRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFolderAccessorsResponse.SerializeToString), 'ShareFolder': grpc.unary_unary_rpc_method_handler(servicer.ShareFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ShareFolderRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'UnshareFolder': grpc.unary_unary_rpc_method_handler(servicer.UnshareFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.UnshareFolderRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString)}
+    rpc_method_handlers = {'ListFolders': grpc.unary_unary_rpc_method_handler(servicer.ListFolders, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFoldersRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFoldersResponse.SerializeToString), 'GetFolder': grpc.unary_unary_rpc_method_handler(servicer.GetFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.GetFolderRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_folder__messages__pb2.Folder.SerializeToString), 'CreateFolder': grpc.unary_unary_rpc_method_handler(servicer.CreateFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.CreateFolderRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_folder__messages__pb2.Folder.SerializeToString), 'UpdateFolder': grpc.unary_unary_rpc_method_handler(servicer.UpdateFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.UpdateFolderRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_folder__messages__pb2.Folder.SerializeToString), 'DeleteFolder': grpc.unary_unary_rpc_method_handler(servicer.DeleteFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.DeleteFolderRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'ListItems': grpc.unary_unary_rpc_method_handler(servicer.ListItems, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListItemsRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListItemsResponse.SerializeToString), 'MoveItems': grpc.unary_unary_rpc_method_handler(servicer.MoveItems, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.MoveItemsRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.MoveItemsResponse.SerializeToString), 'ListFolderAccessors': grpc.unary_unary_rpc_method_handler(servicer.ListFolderAccessors, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFolderAccessorsRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ListFolderAccessorsResponse.SerializeToString), 'ShareFolder': grpc.unary_unary_rpc_method_handler(servicer.ShareFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ShareFolderRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'UnshareFolder': grpc.unary_unary_rpc_method_handler(servicer.UnshareFolder, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.UnshareFolderRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString), 'SearchItems': grpc.unary_unary_rpc_method_handler(servicer.SearchItems, request_deserializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.SearchItemsRequest.FromString, response_serializer=exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.SearchItemsResponse.SerializeToString)}
     generic_handler = grpc.method_handlers_generic_handler('exabel.api.management.v1.LibraryService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 class LibraryService(object):
     """Service to manage library items.
 
     Requests to the LibraryService are executed in the context of the customer's service account (SA).
@@ -188,8 +203,12 @@
 
     @staticmethod
     def ShareFolder(request, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
         return grpc.experimental.unary_unary(request, target, '/exabel.api.management.v1.LibraryService/ShareFolder', exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.ShareFolderRequest.SerializeToString, google_dot_protobuf_dot_empty__pb2.Empty.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def UnshareFolder(request, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/exabel.api.management.v1.LibraryService/UnshareFolder', exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.UnshareFolderRequest.SerializeToString, google_dot_protobuf_dot_empty__pb2.Empty.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+        return grpc.experimental.unary_unary(request, target, '/exabel.api.management.v1.LibraryService/UnshareFolder', exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.UnshareFolderRequest.SerializeToString, google_dot_protobuf_dot_empty__pb2.Empty.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SearchItems(request, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/exabel.api.management.v1.LibraryService/SearchItems', exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.SearchItemsRequest.SerializeToString, exabel_dot_api_dot_management_dot_v1_dot_library__service__pb2.SearchItemsResponse.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/mock_entity_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_entity_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/mock_resource_store.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_resource_store.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/mock_signal_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_entity_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_entity_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_error_handler.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_export_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_export_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_namespace_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_namespace_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_pagable_resource.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 from typing import Iterator, Optional, Sequence
 
 from exabel_data_sdk.client.api.data_classes.paging_result import PagingResult
-from exabel_data_sdk.client.api.pagable_resource import PagableResourceMixin
+from exabel_data_sdk.client.api.pageable_resource import PageableResourceMixin
 
 
-class _PagableApiMock(PagableResourceMixin):
+class _PageableApiMock(PageableResourceMixin):
     def __init__(self, resources: Sequence[str]):
         self.resources = resources
 
     def get_resource_page(self, page_token: Optional[str] = None) -> PagingResult[str]:
         """Return a page of resources."""
         page_idx = int(page_token) if page_token else 0
         return PagingResult(
@@ -19,12 +19,12 @@
         )
 
     def get_resource_iterator(self) -> Iterator[str]:
         """Return an iterator with all resources."""
         return self._get_resource_iterator(self.get_resource_page)
 
 
-class TestPagableResourceMixin(unittest.TestCase):
+class TestPageableResourceMixin(unittest.TestCase):
     def test_get_resource_iterator(self):
         resources = ["a", "b", "c"]
-        api = _PagableApiMock(resources)
+        api = _PageableApiMock(resources)
         self.assertListEqual(list(api.get_resource_iterator()), resources)
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_relationship_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_relationship_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,12 +122,12 @@
             AssertionError("Should not be called"),
         ]
         relationships = list(relationship_api.get_relationships_iterator("relationship_type"))
         self.assertEqual(3, len(relationships))
         self.assertSequenceEqual([relationship_1, relationship_2, relationship_3], relationships)
         relationship_api.list_relationships.assert_has_calls(
             [
-                mock.call(relationship_type="relationship_type", page_token=None),
-                mock.call(relationship_type="relationship_type", page_token="1"),
-                mock.call(relationship_type="relationship_type", page_token="2"),
+                mock.call(relationship_type="relationship_type", page_token=None, page_size=1000),
+                mock.call(relationship_type="relationship_type", page_token="1", page_size=1000),
+                mock.call(relationship_type="relationship_type", page_token="2", page_size=1000),
             ]
         )
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_signal_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/api/test_time_series_api.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_time_series_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/exabel_mock_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/exabel_mock_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/query/test_query.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/query/test_query.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/test_client_config.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_client_config.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/test_exabel_client.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_exabel_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/client/test_user_login.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_user_login.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/decorators.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/common_utils.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/common_utils.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_actions.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_actions.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_command_line_script.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_command_line_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_export_data.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_export_data.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_scripts.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_scripts.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_reader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_csv_writer.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_excel_writer.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_excel_writer.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_file_loading_result.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_loading_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/services/test_file_writer_provider.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_writer_provider.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/test_decorators.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_batcher.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_batcher.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_parse_property_columns.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_parse_property_columns.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/tests/util/test_type_converter.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_type_converter.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/util/case_insensitive_column.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/util/case_insensitive_column.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/util/deprecate_arguments.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/util/deprecate_arguments.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/util/handle_missing_imports.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/util/handle_missing_imports.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/util/import_.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/util/import_.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/util/parse_property_columns.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/util/parse_property_columns.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/util/resource_name_normalization.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/util/resource_name_normalization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import re
 import warnings
-from collections import deque
+from collections import defaultdict, deque
 from dataclasses import dataclass
 from typing import Iterator, Mapping, MutableMapping, MutableSequence, Optional, Sequence, Tuple
 
 import pandas as pd
 
 from exabel_data_sdk.client.api.data_classes.entity_type import EntityType
 from exabel_data_sdk.client.api.entity_api import EntityApi
@@ -116,14 +116,23 @@
     """
 
     names: pd.Series
     warnings: Sequence[EntitySearchResultWarning]
     mapping: Mapping[str, str]
     identifier_type: str
 
+    def get_duplicates(self) -> Mapping[str, Sequence[str]]:
+        """
+        Return the entities for which there where multiple different identifiers in the file.
+        """
+        result = defaultdict(list)
+        for key, value in self.mapping.items():
+            result[value].append(key)
+        return {key: values for key, values in result.items() if len(values) > 1}
+
 
 def get_namespace_from_resource_identifier(resource_identifier: str) -> Optional[str]:
     """Get the namespace from a resource identifier."""
     resource_identifier_parts = resource_identifier.split(".")
     if len(resource_identifier_parts) == 1:
         return None
     if len(resource_identifier_parts) == 2:
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk/util/type_converter.py` & `exabel-data-sdk-4.2.0/exabel_data_sdk/util/type_converter.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk.egg-info/PKG-INFO` & `exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabel-data-sdk
-Version: 4.1.0
+Version: 4.2.0
 Summary: Python SDK for the Exabel Data API
 Home-page: https://github.com/Exabel/python-sdk
 Author: Exabel
 Author-email: support@exabel.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `exabel-data-sdk-4.1.0/exabel_data_sdk.egg-info/SOURCES.txt` & `exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 exabel_data_sdk/client/api/data_set_api.py
 exabel_data_sdk/client/api/derived_signal_api.py
 exabel_data_sdk/client/api/entity_api.py
 exabel_data_sdk/client/api/error_handler.py
 exabel_data_sdk/client/api/export_api.py
 exabel_data_sdk/client/api/library_api.py
 exabel_data_sdk/client/api/namespace_api.py
-exabel_data_sdk/client/api/pagable_resource.py
+exabel_data_sdk/client/api/pageable_resource.py
 exabel_data_sdk/client/api/prediction_model_api.py
 exabel_data_sdk/client/api/proto_utils.py
 exabel_data_sdk/client/api/relationship_api.py
 exabel_data_sdk/client/api/resource_creation_result.py
 exabel_data_sdk/client/api/search_service.py
 exabel_data_sdk/client/api/signal_api.py
 exabel_data_sdk/client/api/tag_api.py
@@ -209,14 +209,16 @@
 exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2_grpc.py
 exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py
 exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py
 exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py
 exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2_grpc.py
 exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py
 exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py
+exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py
+exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py
 exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py
 exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py
 exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py
 exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2_grpc.py
 exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py
 exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2_grpc.py
 exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py
@@ -279,15 +281,15 @@
 exabel_data_sdk/tests/client/api/mock_resource_store.py
 exabel_data_sdk/tests/client/api/mock_signal_api.py
 exabel_data_sdk/tests/client/api/test_bulk_insert_import.py
 exabel_data_sdk/tests/client/api/test_entity_api.py
 exabel_data_sdk/tests/client/api/test_error_handler.py
 exabel_data_sdk/tests/client/api/test_export_api.py
 exabel_data_sdk/tests/client/api/test_namespace_api.py
-exabel_data_sdk/tests/client/api/test_pagable_resource.py
+exabel_data_sdk/tests/client/api/test_pageable_resource.py
 exabel_data_sdk/tests/client/api/test_proto_utils.py
 exabel_data_sdk/tests/client/api/test_relationship_api.py
 exabel_data_sdk/tests/client/api/test_resource_creation_result.py
 exabel_data_sdk/tests/client/api/test_signal_api.py
 exabel_data_sdk/tests/client/api/test_time_series_api.py
 exabel_data_sdk/tests/client/api/api_client/__init__.py
 exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py
```

### Comparing `exabel-data-sdk-4.1.0/pyproject.toml` & `exabel-data-sdk-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.1.0/setup.py` & `exabel-data-sdk-4.2.0/setup.py`

 * *Files identical despite different names*

