# Comparing `tmp/flytekit-1.6.0b1.tar.gz` & `tmp/flytekit-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.6.0b1.tar", last modified: Wed May  3 04:47:56 2023, max compression
+gzip compressed data, was "flytekit-1.6.0b2.tar", last modified: Fri May  5 17:49:35 2023, max compression
```

## Comparing `flytekit-1.6.0b1.tar` & `flytekit-1.6.0b2.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.004263 flytekit-1.6.0b1/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-03 04:47:53.000000 flytekit-1.6.0b1/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.004263 flytekit-1.6.0b1/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.004263 flytekit-1.6.0b1/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    29387 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    35938 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31110 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36193 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    75520 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/stats/taggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    82901 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44333 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.004263 flytekit-1.6.0b1/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-03 04:47:53.000000 flytekit-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-05 17:49:34.000000 flytekit-1.6.0b2/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29387 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    35938 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31110 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36193 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75520 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/stats/taggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82901 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44333 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-05 17:49:34.000000 flytekit-1.6.0b2/setup.py
```

### Comparing `flytekit-1.6.0b1/LICENSE` & `flytekit-1.6.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/MANIFEST.in` & `flytekit-1.6.0b2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/PKG-INFO` & `flytekit-1.6.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b2 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0b1/README.md` & `flytekit-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/__init__.py` & `flytekit-1.6.0b2/flytekit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.6.0b1"
+__version__ = "1.6.0b2"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.6.0b1/flytekit/bin/entrypoint.py` & `flytekit-1.6.0b2/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/auth/auth_client.py` & `flytekit-1.6.0b2/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/auth/authenticator.py` & `flytekit-1.6.0b2/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/auth/keyring.py` & `flytekit-1.6.0b2/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/auth/token_client.py` & `flytekit-1.6.0b2/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/auth_helper.py` & `flytekit-1.6.0b2/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/friendly.py` & `flytekit-1.6.0b2/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.6.0b2/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.6.0b2/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/helpers.py` & `flytekit-1.6.0b2/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clients/raw.py` & `flytekit-1.6.0b2/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/flyte_cli/main.py` & `flytekit-1.6.0b2/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/helpers.py` & `flytekit-1.6.0b2/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/run.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/configuration/__init__.py` & `flytekit-1.6.0b2/flytekit/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/configuration/default_images.py` & `flytekit-1.6.0b2/flytekit/configuration/default_images.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,19 +26,23 @@
     def default_image(cls) -> str:
         return cls.find_image_for()
 
     @classmethod
     def find_image_for(
         cls, python_version: typing.Optional[PythonVersion] = None, flytekit_version: typing.Optional[str] = None
     ) -> str:
+        if python_version is None:
+            python_version = PythonVersion((sys.version_info.major, sys.version_info.minor))
+
+        return cls._DEFAULT_IMAGE_PREFIXES[python_version] + (
+            flytekit_version.replace("v", "") if flytekit_version else cls.get_version_suffix()
+        )
+
+    @classmethod
+    def get_version_suffix(cls) -> str:
         from flytekit import __version__
 
         if not __version__ or __version__ == "0.0.0+develop":
             version_suffix = "latest"
         else:
             version_suffix = __version__
-        if python_version is None:
-            python_version = PythonVersion((sys.version_info.major, sys.version_info.minor))
-
-        return cls._DEFAULT_IMAGE_PREFIXES[python_version] + (
-            flytekit_version.replace("v", "") if flytekit_version else version_suffix
-        )
+        return version_suffix
```

### Comparing `flytekit-1.6.0b1/flytekit/configuration/feature_flags.py` & `flytekit-1.6.0b2/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/configuration/file.py` & `flytekit-1.6.0b2/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/configuration/internal.py` & `flytekit-1.6.0b2/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/annotation.py` & `flytekit-1.6.0b2/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/base_sql_task.py` & `flytekit-1.6.0b2/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/base_task.py` & `flytekit-1.6.0b2/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/checkpointer.py` & `flytekit-1.6.0b2/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/class_based_resolver.py` & `flytekit-1.6.0b2/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/condition.py` & `flytekit-1.6.0b2/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/constants.py` & `flytekit-1.6.0b2/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/container_task.py` & `flytekit-1.6.0b2/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/context_manager.py` & `flytekit-1.6.0b2/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/data_persistence.py` & `flytekit-1.6.0b2/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/docstring.py` & `flytekit-1.6.0b2/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.6.0b2/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/gate.py` & `flytekit-1.6.0b2/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/interface.py` & `flytekit-1.6.0b2/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/launch_plan.py` & `flytekit-1.6.0b2/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/local_cache.py` & `flytekit-1.6.0b2/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/map_task.py` & `flytekit-1.6.0b2/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/mock_stats.py` & `flytekit-1.6.0b2/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/node.py` & `flytekit-1.6.0b2/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/node_creation.py` & `flytekit-1.6.0b2/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/notification.py` & `flytekit-1.6.0b2/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/pod_template.py` & `flytekit-1.6.0b2/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/promise.py` & `flytekit-1.6.0b2/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/python_auto_container.py` & `flytekit-1.6.0b2/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/python_customized_container_task.py` & `flytekit-1.6.0b2/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/python_function_task.py` & `flytekit-1.6.0b2/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/reference.py` & `flytekit-1.6.0b2/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/reference_entity.py` & `flytekit-1.6.0b2/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/resources.py` & `flytekit-1.6.0b2/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/schedule.py` & `flytekit-1.6.0b2/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/shim_task.py` & `flytekit-1.6.0b2/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/task.py` & `flytekit-1.6.0b2/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/testing.py` & `flytekit-1.6.0b2/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/tracker.py` & `flytekit-1.6.0b2/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/type_engine.py` & `flytekit-1.6.0b2/flytekit/core/type_engine.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/type_helpers.py` & `flytekit-1.6.0b2/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/utils.py` & `flytekit-1.6.0b2/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/core/workflow.py` & `flytekit-1.6.0b2/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/deck/deck.py` & `flytekit-1.6.0b2/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/deck/html/template.html` & `flytekit-1.6.0b2/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/deck/renderer.py` & `flytekit-1.6.0b2/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/exceptions/scopes.py` & `flytekit-1.6.0b2/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/exceptions/system.py` & `flytekit-1.6.0b2/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/exceptions/user.py` & `flytekit-1.6.0b2/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extend/__init__.py` & `flytekit-1.6.0b2/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.6.0b2/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/pytorch/__init__.py` & `flytekit-1.6.0b2/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.6.0b2/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/pytorch/native.py` & `flytekit-1.6.0b2/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/sklearn/__init__.py` & `flytekit-1.6.0b2/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/sklearn/native.py` & `flytekit-1.6.0b2/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/sqlite3/task.py` & `flytekit-1.6.0b2/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/tasks/shell.py` & `flytekit-1.6.0b2/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.6.0b2/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/tensorflow/model.py` & `flytekit-1.6.0b2/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/extras/tensorflow/record.py` & `flytekit-1.6.0b2/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/image_spec/image_spec.py` & `flytekit-1.6.0b2/flytekit/image_spec/image_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 import hashlib
 import os
-import sys
 import typing
 from abc import abstractmethod
 from copy import copy
 from dataclasses import dataclass
 from functools import lru_cache
 from typing import List, Optional
 
@@ -23,26 +22,26 @@
 @dataclass
 class ImageSpec:
     """
     This class is used to specify the docker image that will be used to run the task.
 
     Args:
         name: name of the image.
-        python_version: python version of the image.
+        python_version: python version of the image. Use default python in the base image if None.
         builder: Type of plugin to build the image. Use envd by default.
         source_root: source root of the image.
         env: environment variables of the image.
         registry: registry of the image.
         packages: list of python packages to install.
         apt_packages: list of apt packages to install.
         base_image: base image of the image.
     """
 
     name: str = "flytekit"
-    python_version: str = f"{sys.version_info.major}.{sys.version_info.minor}"
+    python_version: str = None  # Use default python in the base image if None.
     builder: str = "envd"
     source_root: Optional[str] = None
     env: Optional[typing.Dict[str, str]] = None
     registry: Optional[str] = None
     packages: Optional[List[str]] = None
     apt_packages: Optional[List[str]] = None
     base_image: Optional[str] = None
@@ -90,14 +89,17 @@
                 container_registry = self.registry.split("/")[0]
             if container_registry == DOCKER_HUB:
                 url = f"https://hub.docker.com/v2/repositories/{self.registry}/{self.name}/tags/{tag}"
                 response = requests.get(url)
                 if response.status_code == 200:
                     return True
 
+                if response.status_code == 404:
+                    return False
+
             click.secho(f"Failed to check if the image exists with error : {e}", fg="red")
             click.secho("Flytekit assumes that the image already exists.", fg="blue")
             return True
 
     def __hash__(self):
         return hash(self.to_json())
```

### Comparing `flytekit-1.6.0b1/flytekit/interaction/parse_stdin.py` & `flytekit-1.6.0b2/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.6.0b2/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/interfaces/random.py` & `flytekit-1.6.0b2/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/interfaces/stats/client.py` & `flytekit-1.6.0b2/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/interfaces/stats/taggable.py` & `flytekit-1.6.0b2/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/loggers.py` & `flytekit-1.6.0b2/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/admin/common.py` & `flytekit-1.6.0b2/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/admin/task_execution.py` & `flytekit-1.6.0b2/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/admin/workflow.py` & `flytekit-1.6.0b2/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/annotation.py` & `flytekit-1.6.0b2/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/array_job.py` & `flytekit-1.6.0b2/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/common.py` & `flytekit-1.6.0b2/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/core/catalog.py` & `flytekit-1.6.0b2/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/core/compiler.py` & `flytekit-1.6.0b2/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/core/condition.py` & `flytekit-1.6.0b2/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/core/errors.py` & `flytekit-1.6.0b2/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/core/execution.py` & `flytekit-1.6.0b2/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/core/identifier.py` & `flytekit-1.6.0b2/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/core/types.py` & `flytekit-1.6.0b2/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/core/workflow.py` & `flytekit-1.6.0b2/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/documentation.py` & `flytekit-1.6.0b2/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/dynamic_job.py` & `flytekit-1.6.0b2/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/execution.py` & `flytekit-1.6.0b2/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/filters.py` & `flytekit-1.6.0b2/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/interface.py` & `flytekit-1.6.0b2/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/launch_plan.py` & `flytekit-1.6.0b2/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/literals.py` & `flytekit-1.6.0b2/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/matchable_resource.py` & `flytekit-1.6.0b2/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/named_entity.py` & `flytekit-1.6.0b2/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/node_execution.py` & `flytekit-1.6.0b2/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/presto.py` & `flytekit-1.6.0b2/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/project.py` & `flytekit-1.6.0b2/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/qubole.py` & `flytekit-1.6.0b2/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/schedule.py` & `flytekit-1.6.0b2/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/security.py` & `flytekit-1.6.0b2/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/task.py` & `flytekit-1.6.0b2/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/types.py` & `flytekit-1.6.0b2/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/models/workflow_closure.py` & `flytekit-1.6.0b2/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/remote/__init__.py` & `flytekit-1.6.0b2/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/remote/backfill.py` & `flytekit-1.6.0b2/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/remote/entities.py` & `flytekit-1.6.0b2/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/remote/executions.py` & `flytekit-1.6.0b2/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/remote/lazy_entity.py` & `flytekit-1.6.0b2/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/remote/remote.py` & `flytekit-1.6.0b2/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/remote/remote_callable.py` & `flytekit-1.6.0b2/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/testing/__init__.py` & `flytekit-1.6.0b2/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/tools/fast_registration.py` & `flytekit-1.6.0b2/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/tools/ignore.py` & `flytekit-1.6.0b2/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/tools/module_loader.py` & `flytekit-1.6.0b2/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/tools/repo.py` & `flytekit-1.6.0b2/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/tools/script_mode.py` & `flytekit-1.6.0b2/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/tools/serialize_helpers.py` & `flytekit-1.6.0b2/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/tools/subprocess.py` & `flytekit-1.6.0b2/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/tools/translator.py` & `flytekit-1.6.0b2/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/directory/__init__.py` & `flytekit-1.6.0b2/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/directory/types.py` & `flytekit-1.6.0b2/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/file/__init__.py` & `flytekit-1.6.0b2/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/file/file.py` & `flytekit-1.6.0b2/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/numpy/ndarray.py` & `flytekit-1.6.0b2/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/pickle/pickle.py` & `flytekit-1.6.0b2/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/schema/types.py` & `flytekit-1.6.0b2/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/schema/types_pandas.py` & `flytekit-1.6.0b2/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/structured/__init__.py` & `flytekit-1.6.0b2/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/structured/basic_dfs.py` & `flytekit-1.6.0b2/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/structured/bigquery.py` & `flytekit-1.6.0b2/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit/types/structured/structured_dataset.py` & `flytekit-1.6.0b2/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit.egg-info/PKG-INFO` & `flytekit-1.6.0b2/flytekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b2 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0b1/flytekit.egg-info/SOURCES.txt` & `flytekit-1.6.0b2/flytekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit.egg-info/requires.txt` & `flytekit-1.6.0b2/flytekit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.6.0b2/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b1/setup.py` & `flytekit-1.6.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.6.0b1"
+__version__ = "1.6.0b2"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
```

