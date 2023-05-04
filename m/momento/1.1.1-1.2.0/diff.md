# Comparing `tmp/momento-1.1.1.tar.gz` & `tmp/momento-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento-1.1.1.tar", max compression
+gzip compressed data, was "momento-1.2.0.tar", max compression
```

## Comparing `momento-1.1.1.tar` & `momento-1.2.0.tar`

### file list

```diff
@@ -1,93 +1,104 @@
--rw-r--r--   0        0        0    11357 2023-04-13 17:47:10.922795 momento-1.1.1/LICENSE
--rw-r--r--   0        0        0     5668 2023-04-13 17:47:10.922795 momento-1.1.1/README.md
--rw-r--r--   0        0        0     3692 2023-04-13 17:47:26.679520 momento-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      619 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/__init__.py
--rw-r--r--   0        0        0       86 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/auth/__init__.py
--rw-r--r--   0        0        0     2868 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/auth/credential_provider.py
--rw-r--r--   0        0        0     2003 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/auth/momento_endpoint_resolver.py
--rw-r--r--   0        0        0    30363 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/cache_client.py
--rw-r--r--   0        0        0    30860 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/cache_client_async.py
--rw-r--r--   0        0        0      176 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/config/__init__.py
--rw-r--r--   0        0        0     3250 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/config/configuration.py
--rw-r--r--   0        0        0     4290 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/config/configurations.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/config/transport/__init__.py
--rw-r--r--   0        0        0      314 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/config/transport/grpc_configuration.py
--rw-r--r--   0        0        0     2358 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/config/transport/transport_strategy.py
--rw-r--r--   0        0        0     1503 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/errors/__init__.py
--rw-r--r--   0        0        0     3991 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/errors/error_converter.py
--rw-r--r--   0        0        0     2329 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/errors/error_details.py
--rw-r--r--   0        0        0     8799 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/errors/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/__init__.py
--rw-r--r--   0        0        0      360 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/_utilities/__init__.py
--rw-r--r--   0        0        0     3656 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/_utilities/_data_validation.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/aio/__init__.py
--rw-r--r--   0        0        0     4377 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/aio/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1856 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/aio/_retry_interceptor.py
--rw-r--r--   0        0        0     5635 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/aio/_scs_control_client.py
--rw-r--r--   0        0        0    34156 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/aio/_scs_data_client.py
--rw-r--r--   0        0        0     3163 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/aio/_scs_grpc_manager.py
--rw-r--r--   0        0        0      123 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/aio/_utilities.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/synchronous/__init__.py
--rw-r--r--   0        0        0     3714 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/synchronous/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1829 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/synchronous/_retry_interceptor.py
--rw-r--r--   0        0        0     5553 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/synchronous/_scs_control_client.py
--rw-r--r--   0        0        0    33860 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/synchronous/_scs_data_client.py
--rw-r--r--   0        0        0     2393 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/synchronous/_scs_grpc_manager.py
--rw-r--r--   0        0        0      159 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/internal/synchronous/_utilities.py
--rw-r--r--   0        0        0     2790 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/logs.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/py.typed
--rw-r--r--   0        0        0      107 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/requests/__init__.py
--rw-r--r--   0        0        0     3800 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/requests/collection_ttl.py
--rw-r--r--   0        0        0     5669 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/control/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/control/cache/__init__.py
--rw-r--r--   0        0        0     1758 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/control/cache/create.py
--rw-r--r--   0        0        0     1405 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/control/cache/delete.py
--rw-r--r--   0        0        0     2311 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/control/cache/list.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/control/signing_key/__init__.py
--rw-r--r--   0        0        0     1764 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/control/signing_key/create.py
--rw-r--r--   0        0        0     2479 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/control/signing_key/list.py
--rw-r--r--   0        0        0      979 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/control/signing_key/revoke.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/dictionary/__init__.py
--rw-r--r--   0        0        0     2047 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/dictionary/fetch.py
--rw-r--r--   0        0        0     1678 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/dictionary/get_field.py
--rw-r--r--   0        0        0     3320 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/dictionary/get_fields.py
--rw-r--r--   0        0        0     1050 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/dictionary/increment.py
--rw-r--r--   0        0        0      945 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/dictionary/remove_field.py
--rw-r--r--   0        0        0      953 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/dictionary/remove_fields.py
--rw-r--r--   0        0        0      921 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/dictionary/set_field.py
--rw-r--r--   0        0        0      929 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/dictionary/set_fields.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/__init__.py
--rw-r--r--   0        0        0     1052 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/concatenate_back.py
--rw-r--r--   0        0        0     1060 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/concatenate_front.py
--rw-r--r--   0        0        0     1402 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/fetch.py
--rw-r--r--   0        0        0     1070 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/length.py
--rw-r--r--   0        0        0     1189 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/pop_back.py
--rw-r--r--   0        0        0     1199 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/pop_front.py
--rw-r--r--   0        0        0      977 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/push_back.py
--rw-r--r--   0        0        0      985 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/push_front.py
--rw-r--r--   0        0        0      874 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/list/remove_value.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/scalar/__init__.py
--rw-r--r--   0        0        0      823 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/scalar/delete.py
--rw-r--r--   0        0        0     1155 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/scalar/get.py
--rw-r--r--   0        0        0     1141 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/scalar/increment.py
--rw-r--r--   0        0        0      799 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/scalar/set.py
--rw-r--r--   0        0        0     1056 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/scalar/set_if_not_exists.py
--rw-r--r--   0        0        0        0 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/set/__init__.py
--rw-r--r--   0        0        0      870 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/set/add_element.py
--rw-r--r--   0        0        0      880 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/set/add_elements.py
--rw-r--r--   0        0        0     1452 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/set/fetch.py
--rw-r--r--   0        0        0      896 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/set/remove_element.py
--rw-r--r--   0        0        0      906 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/data/set/remove_elements.py
--rw-r--r--   0        0        0     1460 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/mixins.py
--rw-r--r--   0        0        0     4724 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/responses/response.py
--rw-r--r--   0        0        0      423 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/retry/__init__.py
--rw-r--r--   0        0        0     2900 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/retry/default_eligibility_strategy.py
--rw-r--r--   0        0        0      216 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/retry/eligibility_strategy.py
--rw-r--r--   0        0        0     2181 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/retry/fixed_count_retry_strategy.py
--rw-r--r--   0        0        0      251 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/retry/retry_strategy.py
--rw-r--r--   0        0        0      291 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/retry/retryable_props.py
--rw-r--r--   0        0        0     1370 2023-04-13 17:47:10.926795 momento-1.1.1/src/momento/typing.py
--rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 momento-1.1.1/setup.py
--rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 momento-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-04 22:11:34.346610 momento-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5668 2023-05-04 22:11:34.346610 momento-1.2.0/README.md
+-rw-r--r--   0        0        0     3692 2023-05-04 22:11:51.755068 momento-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      619 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/__init__.py
+-rw-r--r--   0        0        0       86 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/auth/__init__.py
+-rw-r--r--   0        0        0     2868 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/auth/credential_provider.py
+-rw-r--r--   0        0        0     2003 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/auth/momento_endpoint_resolver.py
+-rw-r--r--   0        0        0    43114 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/cache_client.py
+-rw-r--r--   0        0        0    43753 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/cache_client_async.py
+-rw-r--r--   0        0        0      176 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/__init__.py
+-rw-r--r--   0        0        0     3250 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/configuration.py
+-rw-r--r--   0        0        0     4290 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/configurations.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/transport/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/transport/grpc_configuration.py
+-rw-r--r--   0        0        0     2358 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/transport/transport_strategy.py
+-rw-r--r--   0        0        0     1503 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/errors/__init__.py
+-rw-r--r--   0        0        0     3991 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/errors/error_converter.py
+-rw-r--r--   0        0        0     2329 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/errors/error_details.py
+-rw-r--r--   0        0        0     8799 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/errors/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/__init__.py
+-rw-r--r--   0        0        0      360 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/_utilities/__init__.py
+-rw-r--r--   0        0        0     4710 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/_utilities/_data_validation.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/__init__.py
+-rw-r--r--   0        0        0     4377 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1856 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_retry_interceptor.py
+-rw-r--r--   0        0        0     5635 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_scs_control_client.py
+-rw-r--r--   0        0        0    48528 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_scs_data_client.py
+-rw-r--r--   0        0        0     3163 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      123 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/__init__.py
+-rw-r--r--   0        0        0     3714 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1829 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_retry_interceptor.py
+-rw-r--r--   0        0        0     5553 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_scs_control_client.py
+-rw-r--r--   0        0        0    48148 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_scs_data_client.py
+-rw-r--r--   0        0        0     2393 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      159 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_utilities.py
+-rw-r--r--   0        0        0     2790 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/logs.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/py.typed
+-rw-r--r--   0        0        0      154 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/requests/__init__.py
+-rw-r--r--   0        0        0     3800 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/requests/collection_ttl.py
+-rw-r--r--   0        0        0       91 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/requests/sort_order.py
+-rw-r--r--   0        0        0     6715 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/cache/__init__.py
+-rw-r--r--   0        0        0     1758 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/cache/create.py
+-rw-r--r--   0        0        0     1405 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/cache/delete.py
+-rw-r--r--   0        0        0     2311 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/cache/list.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/signing_key/__init__.py
+-rw-r--r--   0        0        0     1764 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/signing_key/create.py
+-rw-r--r--   0        0        0     2479 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/signing_key/list.py
+-rw-r--r--   0        0        0      979 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/signing_key/revoke.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/__init__.py
+-rw-r--r--   0        0        0     2047 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/fetch.py
+-rw-r--r--   0        0        0     1678 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/get_field.py
+-rw-r--r--   0        0        0     3320 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/get_fields.py
+-rw-r--r--   0        0        0     1050 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/increment.py
+-rw-r--r--   0        0        0      945 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/remove_field.py
+-rw-r--r--   0        0        0      953 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/remove_fields.py
+-rw-r--r--   0        0        0      921 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/set_field.py
+-rw-r--r--   0        0        0      929 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/set_fields.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/concatenate_back.py
+-rw-r--r--   0        0        0     1060 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/concatenate_front.py
+-rw-r--r--   0        0        0     1402 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/fetch.py
+-rw-r--r--   0        0        0     1070 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/length.py
+-rw-r--r--   0        0        0     1189 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/pop_back.py
+-rw-r--r--   0        0        0     1199 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/pop_front.py
+-rw-r--r--   0        0        0      977 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/push_back.py
+-rw-r--r--   0        0        0      985 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/push_front.py
+-rw-r--r--   0        0        0      874 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/remove_value.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/delete.py
+-rw-r--r--   0        0        0     1155 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/get.py
+-rw-r--r--   0        0        0     1141 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/increment.py
+-rw-r--r--   0        0        0      799 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/set.py
+-rw-r--r--   0        0        0     1056 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/set_if_not_exists.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/add_element.py
+-rw-r--r--   0        0        0      880 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/add_elements.py
+-rw-r--r--   0        0        0     1452 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/fetch.py
+-rw-r--r--   0        0        0      896 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/remove_element.py
+-rw-r--r--   0        0        0      906 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/remove_elements.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/sorted_set/__init__.py
+-rw-r--r--   0        0        0     1616 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/sorted_set/fetch.py
+-rw-r--r--   0        0        0     1205 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/get_rank.py
+-rw-r--r--   0        0        0     1581 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/get_score.py
+-rw-r--r--   0        0        0     2323 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/get_scores.py
+-rw-r--r--   0        0        0     1046 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/increment.py
+-rw-r--r--   0        0        0      944 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/put_element.py
+-rw-r--r--   0        0        0      952 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/put_elements.py
+-rw-r--r--   0        0        0      971 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/remove_element.py
+-rw-r--r--   0        0        0      979 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/remove_elements.py
+-rw-r--r--   0        0        0     1460 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/mixins.py
+-rw-r--r--   0        0        0     4724 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/response.py
+-rw-r--r--   0        0        0      423 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/__init__.py
+-rw-r--r--   0        0        0     2900 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/default_eligibility_strategy.py
+-rw-r--r--   0        0        0      216 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/eligibility_strategy.py
+-rw-r--r--   0        0        0     2181 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/fixed_count_retry_strategy.py
+-rw-r--r--   0        0        0      251 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/retry_strategy.py
+-rw-r--r--   0        0        0      291 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/retryable_props.py
+-rw-r--r--   0        0        0     1722 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/typing.py
+-rw-r--r--   0        0        0     7119 1970-01-01 00:00:00.000000 momento-1.2.0/setup.py
+-rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 momento-1.2.0/PKG-INFO
```

### Comparing `momento-1.1.1/LICENSE` & `momento-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/README.md` & `momento-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/pyproject.toml` & `momento-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momento"
-version = "1.1.1"
+version = "1.2.0"
 
 authors = ["Momento <hello@momentohq.com>"]
 description = "SDK for Momento"
 
 license = "Apache-2.0"
 
 documentation = "https://docs.momentohq.com/"
@@ -26,15 +26,15 @@
 ]
 
 exclude = ["src/momento/internal/codegen.py"]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 
-momento-wire-types = "^0.39"
+momento-wire-types = "^0.60"
 grpcio = "^1.50.0"
 # note if you bump this presigned url test need be updated
 pyjwt = "^2.4.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
 pytest-asyncio = "^0.19.0"
```

### Comparing `momento-1.1.1/src/momento/__init__.py` & `momento-1.2.0/src/momento/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/auth/credential_provider.py` & `momento-1.2.0/src/momento/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/auth/momento_endpoint_resolver.py` & `momento-1.2.0/src/momento/auth/momento_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/config/configuration.py` & `momento-1.2.0/src/momento/config/configuration.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/config/configurations.py` & `momento-1.2.0/src/momento/config/configurations.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/config/transport/transport_strategy.py` & `momento-1.2.0/src/momento/config/transport/transport_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/errors/__init__.py` & `momento-1.2.0/src/momento/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/errors/error_converter.py` & `momento-1.2.0/src/momento/errors/error_converter.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/errors/error_details.py` & `momento-1.2.0/src/momento/errors/error_details.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/errors/exceptions.py` & `momento-1.2.0/src/momento/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/internal/_utilities/_data_validation.py` & `momento-1.2.0/src/momento/internal/_utilities/_data_validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 from momento.errors import InvalidArgumentException
 from momento.typing import (
     TDictionaryFields,
     TDictionaryItems,
     TListValuesInput,
     TSetElementsInput,
     TSetElementsInputBytes,
+    TSortedSetElements,
+    TSortedSetValues,
 )
 
 DEFAULT_BYTES_CONVERSION_ERROR = "Could not convert the given type to bytes: "
 DEFAULT_LIST_CONVERSION_ERROR = "The given type is not list[str | bytes]: "
 DEFAULT_DICTIONARY_CONVERSION_ERROR = "The given type is not a valid Mapping: "
 DEFAULT_DICTIONARY_FIELDS_CONVERSION_ERROR = "The given type is not Iterable[str | bytes]: "
 DEFAULT_SET_CONVERSION_ERROR = "The given type is not set[str | bytes]: "
+DEFAULT_SORTED_SET_CONVERSION_ERROR = "The given type is not valid for sorted set elements: "
 
 
 def _validate_name(name: str, field_name: str) -> None:
     if not isinstance(name, str):
         raise InvalidArgumentException(f"{field_name} must be a string")
     if name == "":
         raise InvalidArgumentException(f"{field_name} must not be empty")
@@ -39,14 +42,24 @@
     _validate_name(dictionary_name, "Dictionary name")
 
 
 def _validate_set_name(set_name: str) -> None:
     _validate_name(set_name, "Set name")
 
 
+def _validate_sorted_set_name(sorted_set_name: str) -> None:
+    _validate_name(sorted_set_name, "Sorted set name")
+
+
+def _validate_sorted_set_score(score: float) -> float:
+    if isinstance(score, float):
+        return score
+    raise InvalidArgumentException(f"score must be a float. Given type: {type(score)}")
+
+
 def _as_bytes(
     data: str | bytes,
     error_message: Optional[str] = DEFAULT_BYTES_CONVERSION_ERROR,
 ) -> bytes:
     if isinstance(data, str):
         return data.encode("utf-8")
     if isinstance(data, bytes):
@@ -83,14 +96,29 @@
 def _gen_set_input_as_bytes(
     elements: TSetElementsInput, error_message: str = DEFAULT_SET_CONVERSION_ERROR
 ) -> TSetElementsInputBytes:
     # NB: the set input does not need to be unique
     yield from _gen_iterable_as_bytes(elements, error_message)
 
 
+def _gen_sorted_set_elements_as_bytes(
+    elements: TSortedSetElements, error_message: str = DEFAULT_SORTED_SET_CONVERSION_ERROR
+) -> Iterable[Tuple[bytes, float]]:
+    if not isinstance(elements, collections.abc.Mapping):
+        raise InvalidArgumentException(f"{error_message}{type(elements)}")
+    for value, score in elements.items():
+        yield _as_bytes(value), score
+
+
+def _gen_sorted_set_values_as_bytes(
+    fields: TSortedSetValues, error_message: str = DEFAULT_DICTIONARY_FIELDS_CONVERSION_ERROR
+) -> Iterable[bytes]:
+    yield from _gen_iterable_as_bytes(fields, error_message)
+
+
 def _validate_timedelta_ttl(ttl: Optional[timedelta], field_name: str) -> None:
     if not isinstance(ttl, timedelta):
         raise InvalidArgumentException(f"{field_name} must be a timedelta.")
     if ttl.total_seconds() <= 0:
         raise InvalidArgumentException(f"{field_name} must be a positive amount of time.")
```

### Comparing `momento-1.1.1/src/momento/internal/aio/_add_header_client_interceptor.py` & `momento-1.2.0/src/momento/internal/aio/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/internal/aio/_retry_interceptor.py` & `momento-1.2.0/src/momento/internal/aio/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/internal/aio/_scs_control_client.py` & `momento-1.2.0/src/momento/internal/aio/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/internal/aio/_scs_data_client.py` & `momento-1.2.0/src/momento/internal/aio/_scs_data_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,22 @@
     _ListPushFrontRequest,
     _ListRemoveRequest,
     _SetDifferenceRequest,
     _SetFetchRequest,
     _SetIfNotExistsRequest,
     _SetRequest,
     _SetUnionRequest,
+    _SortedSetElement,
+    _SortedSetFetchRequest,
+    _SortedSetGetRankRequest,
+    _SortedSetGetScoreRequest,
+    _SortedSetIncrementRequest,
+    _SortedSetPutRequest,
+    _SortedSetRemoveRequest,
+    _Unbounded,
 )
 from momento_wire_types.cacheclient_pb2_grpc import ScsStub
 
 from momento import logs
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.errors import UnknownException, convert_error
@@ -44,17 +52,23 @@
     _gen_set_input_as_bytes,
     _validate_cache_name,
     _validate_dictionary_name,
     _validate_list_name,
     _validate_set_name,
     _validate_ttl,
 )
+from momento.internal._utilities._data_validation import (
+    _gen_sorted_set_elements_as_bytes,
+    _gen_sorted_set_values_as_bytes,
+    _validate_sorted_set_name,
+    _validate_sorted_set_score,
+)
 from momento.internal.aio._scs_grpc_manager import _DataGrpcManager
 from momento.internal.aio._utilities import make_metadata
-from momento.requests import CollectionTtl
+from momento.requests import CollectionTtl, SortOrder
 from momento.responses import (
     CacheDelete,
     CacheDeleteResponse,
     CacheDictionaryFetch,
     CacheDictionaryFetchResponse,
     CacheDictionaryGetField,
     CacheDictionaryGetFieldResponse,
@@ -95,38 +109,75 @@
     CacheSetFetchResponse,
     CacheSetIfNotExists,
     CacheSetIfNotExistsResponse,
     CacheSetRemoveElements,
     CacheSetRemoveElementsResponse,
     CacheSetResponse,
 )
+from momento.responses.data.sorted_set.fetch import (
+    CacheSortedSetFetch,
+    CacheSortedSetFetchResponse,
+)
+from momento.responses.data.sorted_set.get_rank import (
+    CacheSortedSetGetRank,
+    CacheSortedSetGetRankResponse,
+)
+from momento.responses.data.sorted_set.get_score import (
+    CacheSortedSetGetScore,
+    CacheSortedSetGetScoreResponse,
+)
+from momento.responses.data.sorted_set.get_scores import (
+    CacheSortedSetGetScores,
+    CacheSortedSetGetScoresResponse,
+)
+from momento.responses.data.sorted_set.increment import (
+    CacheSortedSetIncrement,
+    CacheSortedSetIncrementResponse,
+)
+from momento.responses.data.sorted_set.put_elements import (
+    CacheSortedSetPutElements,
+    CacheSortedSetPutElementsResponse,
+)
+from momento.responses.data.sorted_set.remove_elements import (
+    CacheSortedSetRemoveElements,
+    CacheSortedSetRemoveElementsResponse,
+)
 from momento.typing import (
     TCacheName,
     TDictionaryField,
     TDictionaryFields,
     TDictionaryItems,
     TDictionaryName,
     TListName,
     TListValue,
     TListValuesInput,
     TScalarKey,
     TScalarValue,
     TSetElementsInput,
     TSetName,
+    TSortedSetElements,
+    TSortedSetName,
+    TSortedSetScore,
+    TSortedSetValue,
+    TSortedSetValues,
 )
 
 
 class _ScsDataClient:
     """Internal data client."""
 
     __UNSUPPORTED_LIST_NAME_TYPE_MSG = "Unsupported type for list_name: "
     __UNSUPPORTED_LIST_VALUE_TYPE_MSG = "Unsupported type for value: "
     __UNSUPPORTED_LIST_VALUES_TYPE_MSG = "Unsupported type for values: "
     __UNSUPPORTED_SET_NAME_TYPE_MSG = "Unsupported type for set_name: "
-    __UNSUPPORTED_SET_ELEMENTS_TYPE_MSG = "Unsupported tyoe for elements: "
+    __UNSUPPORTED_SET_ELEMENTS_TYPE_MSG = "Unsupported type for elements: "
+    __UNSUPPORTED_SORTED_SET_NAME_TYPE_MSG = "Unsupported type for sorted_set_name: "
+    __UNSUPPORTED_SORTED_SET_ELEMENTS_TYPE_MSG = "Unsupported type for sorted set elements: "
+    __UNSUPPORTED_SORTED_SET_VALUE_TYPE_MSG = "Unsupported type for sorted set value: "
+    __UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG = "Unsupported type for sorted set values: "
 
     __UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG = "Unsupported type for dictionary_name: "
     __UNSUPPORTED_DICTIONARY_FIELD_TYPE_MSG = "Unsupported type for field: "
     __UNSUPPORTED_DICTIONARY_FIELDS_TYPE_MSG = "Unsupported type for fields: "
     __UNSUPPORTED_DICTIONARY_ITEMS_TYPE_MSG = "Unsupported type for items: "
 
     def __init__(self, configuration: Configuration, credential_provider: CredentialProvider, default_ttl: timedelta):
@@ -154,15 +205,15 @@
             self._log_issuing_request("Increment", {"key": str(key), "amount": str(amount)})
             _validate_cache_name(cache_name)
             item_ttl = self._default_ttl if ttl is None else ttl
             _validate_ttl(item_ttl)
 
             request = _IncrementRequest()
             request.cache_key = _as_bytes(key, "Unsupported type for key: ")
-            request.increment_by = amount
+            request.amount = amount
             request.ttl_milliseconds = int(item_ttl.total_seconds() * 1000)
 
             response = await self._build_stub().Increment(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
@@ -768,14 +819,307 @@
             )
             self._log_received_response("SetRemoveElements", {"set_name": str(request.set_name)})
             return CacheSetRemoveElements.Success()
         except Exception as e:
             self._log_request_error("set_remove_elements", e)
             return CacheSetRemoveElements.Error(convert_error(e))
 
+    async def sorted_set_put_elements(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSetName,
+        elements: TSortedSetElements,
+        ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
+    ) -> CacheSortedSetPutElementsResponse:
+        try:
+            self._log_issuing_request("SortedSetPutElements", {})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetPutRequest()
+            request.set_name = _as_bytes(sorted_set_name, self.__UNSUPPORTED_SORTED_SET_NAME_TYPE_MSG)
+            for value, score in _gen_sorted_set_elements_as_bytes(
+                elements, self.__UNSUPPORTED_SORTED_SET_ELEMENTS_TYPE_MSG
+            ):
+                _validate_sorted_set_score(score)
+                element = _SortedSetElement()
+                element.value = value
+                element.score = score
+                request.elements.append(element)
+            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
+            request.refresh_ttl = ttl.refresh_ttl
+
+            await self._build_stub().SortedSetPut(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetPutElements", {"sorted_set_name": str(request.set_name)})
+            return CacheSortedSetPutElements.Success()
+        except Exception as e:
+            self._log_request_error("sorted_set_put_elements", e)
+            return CacheSortedSetPutElements.Error(convert_error(e))
+
+    async def sorted_set_fetch_by_score(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        min_score: Optional[float],
+        max_score: Optional[float],
+        sort_order: SortOrder,
+        offset: Optional[int],
+        count: Optional[int],
+    ) -> CacheSortedSetFetchResponse:
+        try:
+            self._log_issuing_request("SortedSetFetch", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetFetchRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for set_name: ")
+            request.with_scores = True
+
+            if min_score is not None:
+                request.by_score.min_score = min_score
+            else:
+                request.by_score.unbounded_min.CopyFrom(_Unbounded())
+
+            if max_score is not None:
+                request.by_score.max_score = max_score
+            else:
+                request.by_score.unbounded_max.CopyFrom(_Unbounded())
+
+            if offset is not None:
+                request.by_score.offset = offset
+            else:
+                request.by_score.offset = 0
+
+            if count is not None:
+                request.by_score.count = count
+            else:
+                request.by_score.count = -1
+
+            # ascending = 0, descending = 1
+            if sort_order == SortOrder.ASCENDING:
+                request.order = 0
+            else:
+                request.order = 1
+
+            response = await self._build_stub().SortedSetFetch(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetFetch", {"sorted_set_name": str(request.set_name)})
+
+            type = response.WhichOneof("sorted_set")
+            if type == "missing":
+                return CacheSortedSetFetch.Miss()
+            elif type == "found":
+                return CacheSortedSetFetch.Hit(
+                    list((e.value, e.score) for e in response.found.values_with_scores.elements)
+                )
+            else:
+                raise UnknownException(f"Unknown set field in response: {type}")
+        except Exception as e:
+            self._log_request_error("sorted_set_fetch", e)
+            return CacheSortedSetFetch.Error(convert_error(e))
+
+    async def sorted_set_fetch_by_rank(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        start_rank: Optional[int],
+        end_rank: Optional[int],
+        sort_order: SortOrder,
+    ) -> CacheSortedSetFetchResponse:
+        try:
+            self._log_issuing_request("SortedSetFetch", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetFetchRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for set_name: ")
+            request.with_scores = True
+
+            if start_rank is not None:
+                request.by_index.inclusive_start_index = start_rank
+            else:
+                request.by_index.unbounded_start.CopyFrom(_Unbounded())
+
+            if end_rank is not None:
+                request.by_index.exclusive_end_index = end_rank
+            else:
+                request.by_index.unbounded_end.CopyFrom(_Unbounded())
+
+            # ascending = 0, descending = 1
+            if sort_order == SortOrder.ASCENDING:
+                request.order = 0
+            else:
+                request.order = 1
+
+            response = await self._build_stub().SortedSetFetch(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetFetch", {"sorted_set_name": str(request.set_name)})
+
+            type = response.WhichOneof("sorted_set")
+            if type == "missing":
+                return CacheSortedSetFetch.Miss()
+            elif type == "found":
+                return CacheSortedSetFetch.Hit(
+                    list((e.value, e.score) for e in response.found.values_with_scores.elements)
+                )
+            else:
+                raise UnknownException(f"Unknown set field in response: {type}")
+        except Exception as e:
+            self._log_request_error("sorted_set_fetch", e)
+            return CacheSortedSetFetch.Error(convert_error(e))
+
+    async def sorted_set_get_scores(
+        self, cache_name: TCacheName, sorted_set_name: TSortedSetName, values: TSortedSetValues
+    ) -> CacheSortedSetGetScoresResponse:
+        try:
+            self._log_issuing_request("SortedSetGetScores", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetGetScoreRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
+
+            bytes_values = list(_gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG))
+            request.values.extend(bytes_values)
+
+            response = await self._build_stub().SortedSetGetScore(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetGetScores", {"sorted_set_name": str(request.set_name)})
+
+            type = response.WhichOneof("sorted_set")
+            if type == "found":
+                get_responses: list[CacheSortedSetGetScoreResponse] = []
+                for value, get_response in zip(bytes_values, response.found.elements):
+                    if get_response.result == Miss:
+                        get_responses.append(CacheSortedSetGetScore.Miss(value))
+                    else:
+                        get_responses.append(CacheSortedSetGetScore.Hit(value, get_response.score))
+                return CacheSortedSetGetScores.Hit(get_responses)
+            elif type == "missing":
+                return CacheSortedSetGetScores.Miss()
+            else:
+                raise UnknownException(f"Unknown field in response: {type}")
+        except Exception as e:
+            self._log_request_error("sorted_set_get_scores", e)
+            return CacheSortedSetGetScores.Error(convert_error(e))
+
+    async def sorted_set_get_rank(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        value: TSortedSetValue,
+        sort_order: SortOrder,
+    ) -> CacheSortedSetGetRankResponse:
+        try:
+            self._log_issuing_request("SortedSetGetRank", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetGetRankRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
+            request.value = _as_bytes(value, self.__UNSUPPORTED_SORTED_SET_VALUE_TYPE_MSG)
+
+            # ascending = 0, descending = 1
+            if sort_order == SortOrder.ASCENDING:
+                request.order = 0
+            else:
+                request.order = 1
+
+            response = await self._build_stub().SortedSetGetRank(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetGetRank", {"sorted_set_name": str(request.set_name)})
+
+            if response.element_rank.result == Hit:
+                return CacheSortedSetGetRank.Hit(response.element_rank.rank)
+            if response.element_rank.result == Miss:
+                return CacheSortedSetGetRank.Miss()
+            else:
+                raise UnknownException(f"Unknown field in response: {type}")
+        except Exception as e:
+            self._log_request_error("sorted_set_get_rank", e)
+            return CacheSortedSetGetRank.Error(convert_error(e))
+
+    async def sorted_set_remove_elements(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        values: TSortedSetValues,
+    ) -> CacheSortedSetRemoveElementsResponse:
+        try:
+            self._log_issuing_request("SortedSetRemoveElements", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetRemoveRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
+            request.some.values.extend(
+                _gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG)
+            )
+
+            await self._build_stub().SortedSetRemove(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetRemoveElements", {"sorted_set_name": str(request.set_name)})
+
+            return CacheSortedSetRemoveElements.Success()
+        except Exception as e:
+            self._log_request_error("sorted_set_remove_elements", e)
+            return CacheSortedSetRemoveElements.Error(convert_error(e))
+
+    async def sorted_set_increment(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        value: TSortedSetValue,
+        score: TSortedSetScore,
+        ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
+    ) -> CacheSortedSetIncrementResponse:
+        try:
+            self._log_issuing_request("SortedSetIncrement", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+            _validate_sorted_set_score(score)
+
+            request = _SortedSetIncrementRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
+            request.value = _as_bytes(value)
+            request.amount = score
+            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
+            request.refresh_ttl = ttl.refresh_ttl
+
+            response = await self._build_stub().SortedSetIncrement(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetIncrement", {"sorted_set_name": str(request.set_name)})
+
+            return CacheSortedSetIncrement.Success(response.score)
+        except Exception as e:
+            self._log_request_error("sorted_set_increment", e)
+            return CacheSortedSetIncrement.Error(convert_error(e))
+
     def _log_received_response(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Received a {request_type} response for {request_args}")
 
     def _log_issuing_request(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Issuing a {request_type} request with {request_args}")
 
     def _log_request_error(self, request_type: str, e: Exception) -> None:
```

### Comparing `momento-1.1.1/src/momento/internal/aio/_scs_grpc_manager.py` & `momento-1.2.0/src/momento/internal/aio/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/internal/synchronous/_add_header_client_interceptor.py` & `momento-1.2.0/src/momento/internal/synchronous/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/internal/synchronous/_retry_interceptor.py` & `momento-1.2.0/src/momento/internal/synchronous/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/internal/synchronous/_scs_control_client.py` & `momento-1.2.0/src/momento/internal/synchronous/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/internal/synchronous/_scs_data_client.py` & `momento-1.2.0/src/momento/internal/synchronous/_scs_data_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,22 @@
     _ListPushFrontRequest,
     _ListRemoveRequest,
     _SetDifferenceRequest,
     _SetFetchRequest,
     _SetIfNotExistsRequest,
     _SetRequest,
     _SetUnionRequest,
+    _SortedSetElement,
+    _SortedSetFetchRequest,
+    _SortedSetGetRankRequest,
+    _SortedSetGetScoreRequest,
+    _SortedSetIncrementRequest,
+    _SortedSetPutRequest,
+    _SortedSetRemoveRequest,
+    _Unbounded,
 )
 from momento_wire_types.cacheclient_pb2_grpc import ScsStub
 
 from momento import logs
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.errors import UnknownException, convert_error
@@ -44,17 +52,23 @@
     _gen_set_input_as_bytes,
     _validate_cache_name,
     _validate_dictionary_name,
     _validate_list_name,
     _validate_set_name,
     _validate_ttl,
 )
+from momento.internal._utilities._data_validation import (
+    _gen_sorted_set_elements_as_bytes,
+    _gen_sorted_set_values_as_bytes,
+    _validate_sorted_set_name,
+    _validate_sorted_set_score,
+)
 from momento.internal.synchronous._scs_grpc_manager import _DataGrpcManager
 from momento.internal.synchronous._utilities import make_metadata
-from momento.requests import CollectionTtl
+from momento.requests import CollectionTtl, SortOrder
 from momento.responses import (
     CacheDelete,
     CacheDeleteResponse,
     CacheDictionaryFetch,
     CacheDictionaryFetchResponse,
     CacheDictionaryGetField,
     CacheDictionaryGetFieldResponse,
@@ -95,38 +109,75 @@
     CacheSetFetchResponse,
     CacheSetIfNotExists,
     CacheSetIfNotExistsResponse,
     CacheSetRemoveElements,
     CacheSetRemoveElementsResponse,
     CacheSetResponse,
 )
+from momento.responses.data.sorted_set.fetch import (
+    CacheSortedSetFetch,
+    CacheSortedSetFetchResponse,
+)
+from momento.responses.data.sorted_set.get_rank import (
+    CacheSortedSetGetRank,
+    CacheSortedSetGetRankResponse,
+)
+from momento.responses.data.sorted_set.get_score import (
+    CacheSortedSetGetScore,
+    CacheSortedSetGetScoreResponse,
+)
+from momento.responses.data.sorted_set.get_scores import (
+    CacheSortedSetGetScores,
+    CacheSortedSetGetScoresResponse,
+)
+from momento.responses.data.sorted_set.increment import (
+    CacheSortedSetIncrement,
+    CacheSortedSetIncrementResponse,
+)
+from momento.responses.data.sorted_set.put_elements import (
+    CacheSortedSetPutElements,
+    CacheSortedSetPutElementsResponse,
+)
+from momento.responses.data.sorted_set.remove_elements import (
+    CacheSortedSetRemoveElements,
+    CacheSortedSetRemoveElementsResponse,
+)
 from momento.typing import (
     TCacheName,
     TDictionaryField,
     TDictionaryFields,
     TDictionaryItems,
     TDictionaryName,
     TListName,
     TListValue,
     TListValuesInput,
     TScalarKey,
     TScalarValue,
     TSetElementsInput,
     TSetName,
+    TSortedSetElements,
+    TSortedSetName,
+    TSortedSetScore,
+    TSortedSetValue,
+    TSortedSetValues,
 )
 
 
 class _ScsDataClient:
     """Internal data client."""
 
     __UNSUPPORTED_LIST_NAME_TYPE_MSG = "Unsupported type for list_name: "
     __UNSUPPORTED_LIST_VALUE_TYPE_MSG = "Unsupported type for value: "
     __UNSUPPORTED_LIST_VALUES_TYPE_MSG = "Unsupported type for values: "
     __UNSUPPORTED_SET_NAME_TYPE_MSG = "Unsupported type for set_name: "
-    __UNSUPPORTED_SET_ELEMENTS_TYPE_MSG = "Unsupported tyoe for elements: "
+    __UNSUPPORTED_SET_ELEMENTS_TYPE_MSG = "Unsupported type for elements: "
+    __UNSUPPORTED_SORTED_SET_NAME_TYPE_MSG = "Unsupported type for sorted_set_name: "
+    __UNSUPPORTED_SORTED_SET_ELEMENTS_TYPE_MSG = "Unsupported type for sorted set elements: "
+    __UNSUPPORTED_SORTED_SET_VALUE_TYPE_MSG = "Unsupported type for sorted set value: "
+    __UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG = "Unsupported type for sorted set values: "
 
     __UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG = "Unsupported type for dictionary_name: "
     __UNSUPPORTED_DICTIONARY_FIELD_TYPE_MSG = "Unsupported type for field: "
     __UNSUPPORTED_DICTIONARY_FIELDS_TYPE_MSG = "Unsupported type for fields: "
     __UNSUPPORTED_DICTIONARY_ITEMS_TYPE_MSG = "Unsupported type for items: "
 
     def __init__(self, configuration: Configuration, credential_provider: CredentialProvider, default_ttl: timedelta):
@@ -154,15 +205,15 @@
             self._log_issuing_request("Increment", {"key": str(key), "amount": str(amount)})
             _validate_cache_name(cache_name)
             item_ttl = self._default_ttl if ttl is None else ttl
             _validate_ttl(item_ttl)
 
             request = _IncrementRequest()
             request.cache_key = _as_bytes(key, "Unsupported type for key: ")
-            request.increment_by = amount
+            request.amount = amount
             request.ttl_milliseconds = int(item_ttl.total_seconds() * 1000)
 
             response = self._build_stub().Increment(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
@@ -766,14 +817,307 @@
             )
             self._log_received_response("SetRemoveElements", {"set_name": str(request.set_name)})
             return CacheSetRemoveElements.Success()
         except Exception as e:
             self._log_request_error("set_remove_elements", e)
             return CacheSetRemoveElements.Error(convert_error(e))
 
+    def sorted_set_put_elements(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSetName,
+        elements: TSortedSetElements,
+        ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
+    ) -> CacheSortedSetPutElementsResponse:
+        try:
+            self._log_issuing_request("SortedSetPutElements", {})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetPutRequest()
+            request.set_name = _as_bytes(sorted_set_name, self.__UNSUPPORTED_SORTED_SET_NAME_TYPE_MSG)
+            for value, score in _gen_sorted_set_elements_as_bytes(
+                elements, self.__UNSUPPORTED_SORTED_SET_ELEMENTS_TYPE_MSG
+            ):
+                _validate_sorted_set_score(score)
+                element = _SortedSetElement()
+                element.value = value
+                element.score = score
+                request.elements.append(element)
+            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
+            request.refresh_ttl = ttl.refresh_ttl
+
+            self._build_stub().SortedSetPut(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetPutElements", {"sorted_set_name": str(request.set_name)})
+            return CacheSortedSetPutElements.Success()
+        except Exception as e:
+            self._log_request_error("sorted_set_put_elements", e)
+            return CacheSortedSetPutElements.Error(convert_error(e))
+
+    def sorted_set_fetch_by_score(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        min_score: Optional[float],
+        max_score: Optional[float],
+        sort_order: SortOrder,
+        offset: Optional[int],
+        count: Optional[int],
+    ) -> CacheSortedSetFetchResponse:
+        try:
+            self._log_issuing_request("SortedSetFetch", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetFetchRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for set_name: ")
+            request.with_scores = True
+
+            if min_score is not None:
+                request.by_score.min_score = min_score
+            else:
+                request.by_score.unbounded_min.CopyFrom(_Unbounded())
+
+            if max_score is not None:
+                request.by_score.max_score = max_score
+            else:
+                request.by_score.unbounded_max.CopyFrom(_Unbounded())
+
+            if offset is not None:
+                request.by_score.offset = offset
+            else:
+                request.by_score.offset = 0
+
+            if count is not None:
+                request.by_score.count = count
+            else:
+                request.by_score.count = -1
+
+            # ascending = 0, descending = 1
+            if sort_order == SortOrder.ASCENDING:
+                request.order = 0
+            else:
+                request.order = 1
+
+            response = self._build_stub().SortedSetFetch(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetFetch", {"sorted_set_name": str(request.set_name)})
+
+            type = response.WhichOneof("sorted_set")
+            if type == "missing":
+                return CacheSortedSetFetch.Miss()
+            elif type == "found":
+                return CacheSortedSetFetch.Hit(
+                    list((e.value, e.score) for e in response.found.values_with_scores.elements)
+                )
+            else:
+                raise UnknownException(f"Unknown set field in response: {type}")
+        except Exception as e:
+            self._log_request_error("sorted_set_fetch", e)
+            return CacheSortedSetFetch.Error(convert_error(e))
+
+    def sorted_set_fetch_by_rank(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        start_rank: Optional[int],
+        end_rank: Optional[int],
+        sort_order: SortOrder,
+    ) -> CacheSortedSetFetchResponse:
+        try:
+            self._log_issuing_request("SortedSetFetch", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetFetchRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for set_name: ")
+            request.with_scores = True
+
+            if start_rank is not None:
+                request.by_index.inclusive_start_index = start_rank
+            else:
+                request.by_index.unbounded_start.CopyFrom(_Unbounded())
+
+            if end_rank is not None:
+                request.by_index.exclusive_end_index = end_rank
+            else:
+                request.by_index.unbounded_end.CopyFrom(_Unbounded())
+
+            # ascending = 0, descending = 1
+            if sort_order == SortOrder.ASCENDING:
+                request.order = 0
+            else:
+                request.order = 1
+
+            response = self._build_stub().SortedSetFetch(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetFetch", {"sorted_set_name": str(request.set_name)})
+
+            type = response.WhichOneof("sorted_set")
+            if type == "missing":
+                return CacheSortedSetFetch.Miss()
+            elif type == "found":
+                return CacheSortedSetFetch.Hit(
+                    list((e.value, e.score) for e in response.found.values_with_scores.elements)
+                )
+            else:
+                raise UnknownException(f"Unknown set field in response: {type}")
+        except Exception as e:
+            self._log_request_error("sorted_set_fetch", e)
+            return CacheSortedSetFetch.Error(convert_error(e))
+
+    def sorted_set_get_scores(
+        self, cache_name: TCacheName, sorted_set_name: TSortedSetName, values: TSortedSetValues
+    ) -> CacheSortedSetGetScoresResponse:
+        try:
+            self._log_issuing_request("SortedSetGetScores", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetGetScoreRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
+
+            bytes_values = list(_gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG))
+            request.values.extend(bytes_values)
+
+            response = self._build_stub().SortedSetGetScore(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetGetScores", {"sorted_set_name": str(request.set_name)})
+
+            type = response.WhichOneof("sorted_set")
+            if type == "found":
+                get_responses: list[CacheSortedSetGetScoreResponse] = []
+                for value, get_response in zip(bytes_values, response.found.elements):
+                    if get_response.result == Miss:
+                        get_responses.append(CacheSortedSetGetScore.Miss(value))
+                    else:
+                        get_responses.append(CacheSortedSetGetScore.Hit(value, get_response.score))
+                return CacheSortedSetGetScores.Hit(get_responses)
+            elif type == "missing":
+                return CacheSortedSetGetScores.Miss()
+            else:
+                raise UnknownException(f"Unknown field in response: {type}")
+        except Exception as e:
+            self._log_request_error("sorted_set_get_scores", e)
+            return CacheSortedSetGetScores.Error(convert_error(e))
+
+    def sorted_set_get_rank(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        value: TSortedSetValue,
+        sort_order: SortOrder,
+    ) -> CacheSortedSetGetRankResponse:
+        try:
+            self._log_issuing_request("SortedSetGetRank", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetGetRankRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
+            request.value = _as_bytes(value, self.__UNSUPPORTED_SORTED_SET_VALUE_TYPE_MSG)
+
+            # ascending = 0, descending = 1
+            if sort_order == SortOrder.ASCENDING:
+                request.order = 0
+            else:
+                request.order = 1
+
+            response = self._build_stub().SortedSetGetRank(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetGetRank", {"sorted_set_name": str(request.set_name)})
+
+            if response.element_rank.result == Hit:
+                return CacheSortedSetGetRank.Hit(response.element_rank.rank)
+            if response.element_rank.result == Miss:
+                return CacheSortedSetGetRank.Miss()
+            else:
+                raise UnknownException(f"Unknown field in response: {type}")
+        except Exception as e:
+            self._log_request_error("sorted_set_get_rank", e)
+            return CacheSortedSetGetRank.Error(convert_error(e))
+
+    def sorted_set_remove_elements(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        values: TSortedSetValues,
+    ) -> CacheSortedSetRemoveElementsResponse:
+        try:
+            self._log_issuing_request("SortedSetRemoveElements", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+
+            request = _SortedSetRemoveRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
+            request.some.values.extend(
+                _gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG)
+            )
+
+            self._build_stub().SortedSetRemove(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetRemoveElements", {"sorted_set_name": str(request.set_name)})
+
+            return CacheSortedSetRemoveElements.Success()
+        except Exception as e:
+            self._log_request_error("sorted_set_remove_elements", e)
+            return CacheSortedSetRemoveElements.Error(convert_error(e))
+
+    def sorted_set_increment(
+        self,
+        cache_name: TCacheName,
+        sorted_set_name: TSortedSetName,
+        value: TSortedSetValue,
+        score: TSortedSetScore,
+        ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
+    ) -> CacheSortedSetIncrementResponse:
+        try:
+            self._log_issuing_request("SortedSetIncrement", {"sorted_set_name": str(sorted_set_name)})
+            _validate_cache_name(cache_name)
+            _validate_sorted_set_name(sorted_set_name)
+            _validate_sorted_set_score(score)
+
+            request = _SortedSetIncrementRequest()
+            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
+            request.value = _as_bytes(value)
+            request.amount = score
+            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
+            request.refresh_ttl = ttl.refresh_ttl
+
+            response = self._build_stub().SortedSetIncrement(
+                request,
+                metadata=make_metadata(cache_name),
+                timeout=self._default_deadline_seconds,
+            )
+            self._log_received_response("SortedSetIncrement", {"sorted_set_name": str(request.set_name)})
+
+            return CacheSortedSetIncrement.Success(response.score)
+        except Exception as e:
+            self._log_request_error("sorted_set_increment", e)
+            return CacheSortedSetIncrement.Error(convert_error(e))
+
     def _log_received_response(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Received a {request_type} response for {request_args}")
 
     def _log_issuing_request(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Issuing a {request_type} request with {request_args}")
 
     def _log_request_error(self, request_type: str, e: Exception) -> None:
```

### Comparing `momento-1.1.1/src/momento/internal/synchronous/_scs_grpc_manager.py` & `momento-1.2.0/src/momento/internal/synchronous/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/logs.py` & `momento-1.2.0/src/momento/logs.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/requests/collection_ttl.py` & `momento-1.2.0/src/momento/requests/collection_ttl.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/__init__.py` & `momento-1.2.0/src/momento/responses/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,14 +80,35 @@
     CacheSetRemoveElement,
     CacheSetRemoveElementResponse,
 )
 from .data.set.remove_elements import (
     CacheSetRemoveElements,
     CacheSetRemoveElementsResponse,
 )
+from .data.sorted_set.fetch import CacheSortedSetFetch, CacheSortedSetFetchResponse
+from .data.sorted_set.get_rank import (
+    CacheSortedSetGetRank,
+    CacheSortedSetGetRankResponse,
+)
+from .data.sorted_set.get_score import (
+    CacheSortedSetGetScore,
+    CacheSortedSetGetScoreResponse,
+)
+from .data.sorted_set.get_scores import (
+    CacheSortedSetGetScores,
+    CacheSortedSetGetScoresResponse,
+)
+from .data.sorted_set.put_element import (
+    CacheSortedSetPutElement,
+    CacheSortedSetPutElementResponse,
+)
+from .data.sorted_set.put_elements import (
+    CacheSortedSetPutElements,
+    CacheSortedSetPutElementsResponse,
+)
 from .response import CacheResponse, ControlResponse
 
 __all__ = [
     "CreateCache",
     "CreateCacheResponse",
     "DeleteCache",
     "DeleteCacheResponse",
@@ -150,10 +171,22 @@
     "CacheSetAddElementsResponse",
     "CacheSetFetch",
     "CacheSetFetchResponse",
     "CacheSetRemoveElement",
     "CacheSetRemoveElementResponse",
     "CacheSetRemoveElements",
     "CacheSetRemoveElementsResponse",
+    "CacheSortedSetPutElement",
+    "CacheSortedSetGetRank",
+    "CacheSortedSetGetRankResponse",
+    "CacheSortedSetGetScore",
+    "CacheSortedSetGetScoreResponse",
+    "CacheSortedSetGetScores",
+    "CacheSortedSetGetScoresResponse",
+    "CacheSortedSetPutElementResponse",
+    "CacheSortedSetPutElements",
+    "CacheSortedSetPutElementsResponse",
+    "CacheSortedSetFetch",
+    "CacheSortedSetFetchResponse",
     "CacheResponse",
     "ControlResponse",
 ]
```

### Comparing `momento-1.1.1/src/momento/responses/control/cache/create.py` & `momento-1.2.0/src/momento/responses/control/cache/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/control/cache/delete.py` & `momento-1.2.0/src/momento/responses/control/cache/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/control/cache/list.py` & `momento-1.2.0/src/momento/responses/control/cache/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/control/signing_key/create.py` & `momento-1.2.0/src/momento/responses/control/signing_key/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/control/signing_key/list.py` & `momento-1.2.0/src/momento/responses/control/signing_key/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/control/signing_key/revoke.py` & `momento-1.2.0/src/momento/responses/control/signing_key/revoke.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/dictionary/fetch.py` & `momento-1.2.0/src/momento/responses/data/dictionary/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/dictionary/get_field.py` & `momento-1.2.0/src/momento/responses/data/dictionary/get_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/dictionary/get_fields.py` & `momento-1.2.0/src/momento/responses/data/dictionary/get_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/dictionary/increment.py` & `momento-1.2.0/src/momento/responses/data/dictionary/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/dictionary/remove_field.py` & `momento-1.2.0/src/momento/responses/data/dictionary/remove_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/dictionary/remove_fields.py` & `momento-1.2.0/src/momento/responses/data/dictionary/remove_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/dictionary/set_field.py` & `momento-1.2.0/src/momento/responses/data/dictionary/set_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/dictionary/set_fields.py` & `momento-1.2.0/src/momento/responses/data/dictionary/set_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/list/concatenate_back.py` & `momento-1.2.0/src/momento/responses/data/list/concatenate_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/list/concatenate_front.py` & `momento-1.2.0/src/momento/responses/data/list/concatenate_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/list/fetch.py` & `momento-1.2.0/src/momento/responses/data/list/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/list/length.py` & `momento-1.2.0/src/momento/responses/data/list/length.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/list/pop_back.py` & `momento-1.2.0/src/momento/responses/data/list/pop_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/list/pop_front.py` & `momento-1.2.0/src/momento/responses/data/list/pop_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/list/push_back.py` & `momento-1.2.0/src/momento/responses/data/list/push_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/list/push_front.py` & `momento-1.2.0/src/momento/responses/data/list/push_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/list/remove_value.py` & `momento-1.2.0/src/momento/responses/data/list/remove_value.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/scalar/delete.py` & `momento-1.2.0/src/momento/responses/data/scalar/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/scalar/get.py` & `momento-1.2.0/src/momento/responses/data/scalar/get.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/scalar/increment.py` & `momento-1.2.0/src/momento/responses/data/scalar/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/scalar/set.py` & `momento-1.2.0/src/momento/responses/data/scalar/set.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/scalar/set_if_not_exists.py` & `momento-1.2.0/src/momento/responses/data/scalar/set_if_not_exists.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/set/add_element.py` & `momento-1.2.0/src/momento/responses/data/set/add_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/set/add_elements.py` & `momento-1.2.0/src/momento/responses/data/set/add_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/set/fetch.py` & `momento-1.2.0/src/momento/responses/data/set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/set/remove_element.py` & `momento-1.2.0/src/momento/responses/data/set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/data/set/remove_elements.py` & `momento-1.2.0/src/momento/responses/data/set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/mixins.py` & `momento-1.2.0/src/momento/responses/mixins.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/responses/response.py` & `momento-1.2.0/src/momento/responses/response.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/retry/default_eligibility_strategy.py` & `momento-1.2.0/src/momento/retry/default_eligibility_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/src/momento/retry/fixed_count_retry_strategy.py` & `momento-1.2.0/src/momento/retry/fixed_count_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.1.1/setup.py` & `momento-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,28 @@
  'momento.responses.control.cache',
  'momento.responses.control.signing_key',
  'momento.responses.data',
  'momento.responses.data.dictionary',
  'momento.responses.data.list',
  'momento.responses.data.scalar',
  'momento.responses.data.set',
+ 'momento.responses.data.sorted_set',
  'momento.retry']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['grpcio>=1.50.0,<2.0.0',
- 'momento-wire-types>=0.39,<0.40',
+ 'momento-wire-types>=0.60,<0.61',
  'pyjwt>=2.4.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'momento',
-    'version': '1.1.1',
+    'version': '1.2.0',
     'description': 'SDK for Momento',
     'long_description': '<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md) \n\n# Momento Python Client Library\n\n\nPython client SDK for Momento Serverless Cache: a fast, simple, pay-as-you-go caching solution without\nany of the operational overhead required by traditional caching solutions!\n\n\n\n## Getting Started :running:\n\n### Requirements\n\n- [Python 3.7](https://www.python.org/downloads/) or above is required\n- A Momento Auth Token is required, you can generate one using the [Momento CLI](https://github.com/momentohq/momento-cli)\n\n### Examples\n\nReady to dive right in? Just check out the [examples](https://github.com/momentohq/client-sdk-python/tree/main/examples) directory for complete, working examples of\nhow to use the SDK.\n\n### Installation\n\nThe [Momento SDK is available on PyPi](https://pypi.org/project/momento/). To install via pip:\n\n```bash\npip install momento\n```\n\n### Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\nif __name__ == "__main__":\n    cache_name = "default-cache"\n    with CacheClient(\n        configuration=Configurations.Laptop.v1(),\n        credential_provider=CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n        default_ttl=timedelta(seconds=60),\n    ) as cache_client:\n        create_cache_response = cache_client.create_cache(cache_name)\n        match create_cache_response:\n            case CreateCache.CacheAlreadyExists():\n                print(f"Cache with name: {cache_name} already exists.")\n            case CreateCache.Error() as error:\n                raise error.inner_exception\n\n        print("Setting Key: foo to Value: FOO")\n        set_response = cache_client.set(cache_name, "foo", "FOO")\n        match set_response:\n            case CacheSet.Error() as error:\n                raise error.inner_exception\n\n        print("Getting Key: foo")\n        get_response = cache_client.get(cache_name, "foo")\n        match get_response:\n            case CacheGet.Hit() as hit:\n                print(f"Look up resulted in a hit: {hit}")\n                print(f"Looked up Value: {hit.value_string!r}")\n            case CacheGet.Miss():\n                print("Look up resulted in a: miss. This is unexpected.")\n            case CacheGet.Error() as error:\n                raise error.inner_exception\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\nif __name__ == "__main__":\n    cache_name = \'default-cache\'\n    with CacheClient(configuration=Configurations.Laptop.v1(),\n                     credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n                     default_ttl=timedelta(seconds=60)\n                     ) as cache_client:\n        create_cache_response = cache_client.create_cache(cache_name)\n        if isinstance(create_cache_response, CreateCache.CacheAlreadyExists):\n            print(f"Cache with name: {cache_name} already exists.")\n        elif isinstance(create_cache_response, CreateCache.Error):\n            raise create_cache_response.inner_exception\n\n        print("Setting Key: foo to Value: FOO")\n        set_response = cache_client.set(cache_name, \'foo\', \'FOO\')\n        if isinstance(set_response, CacheSet.Error):\n            raise set_response.inner_exception\n\n        print("Getting Key: foo")\n        get_response = cache_client.get(cache_name, \'foo\')\n        if isinstance(get_response, CacheGet.Hit):\n            print(f"Look up resulted in a hit: {get_response.value_string}")\n            print(f"Looked up Value: {get_response.value_string}")\n        elif isinstance(get_response, CacheGet.Miss):\n            print("Look up resulted in a: miss. This is unexpected.")\n        elif isinstance(get_response, CacheGet.Error):\n            raise get_response.inner_exception\n```\n\n### Logging\n\nTo avoid cluttering DEBUG logging with per-method logs the Momento SDK adds a TRACE logging level. This will only happen\nif the TRACE level does not already exist.\n\nTo enable TRACE level logging you can call logging.basicConfig() before making any log statements:\n\n```python\nimport logging\n\nlogging.basicConfig(level=\'TRACE\')\n```\n\n### Error Handling\n\nComing Soon!\n\n### Tuning\n\nComing Soon!\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
     'author': 'Momento',
     'author_email': 'hello@momentohq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gomomento.com',
```

### Comparing `momento-1.1.1/PKG-INFO` & `momento-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momento
-Version: 1.1.1
+Version: 1.2.0
 Summary: SDK for Momento
 Home-page: https://gomomento.com
 License: Apache-2.0
 Keywords: Momento,caching,key-value store,serverless
 Author: Momento
 Author-email: hello@momentohq.com
 Requires-Python: >=3.7,<3.12
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Typing :: Typed
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
-Requires-Dist: momento-wire-types (>=0.39,<0.40)
+Requires-Dist: momento-wire-types (>=0.60,<0.61)
 Requires-Dist: pyjwt (>=2.4.0,<3.0.0)
 Project-URL: Documentation, https://docs.momentohq.com/
 Project-URL: Repository, https://github.com/momentohq/client-sdk-python
 Description-Content-Type: text/markdown
 
 <img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>
```

