# Comparing `tmp/cornflow-1.0.4.tar.gz` & `tmp/cornflow-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornflow-1.0.4.tar", last modified: Mon Apr 24 08:04:26 2023, max compression
+gzip compressed data, was "cornflow-1.0.5.tar", last modified: Fri May  5 08:12:33 2023, max compression
```

## Comparing `cornflow-1.0.4.tar` & `cornflow-1.0.5.tar`

### file list

```diff
@@ -1,166 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.489382 cornflow-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 08:04:22.000000 cornflow-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-04-24 08:04:26.489382 cornflow-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-04-24 08:04:22.000000 cornflow-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.477382 cornflow-1.0.4/airflow_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/airflow_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.477382 cornflow-1.0.4/airflow_config/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.477382 cornflow-1.0.4/airflow_config/plugins/XCom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/airflow_config/plugins/XCom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-24 08:04:22.000000 cornflow-1.0.4/airflow_config/plugins/XCom/gce_xcom_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/airflow_config/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-24 08:04:22.000000 cornflow-1.0.4/airflow_config/webserver_ldap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.477382 cornflow-1.0.4/cornflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.477382 cornflow-1.0.4/cornflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/cli/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.477382 cornflow-1.0.4/cornflow/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/commands/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.481382 cornflow-1.0.4/cornflow/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/apiview.py
--rw-r--r--   0 runner    (1001) docker     (123)    18747 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/case.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/data_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/example_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/signup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/endpoints/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/gunicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.481382 cornflow-1.0.4/cornflow/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/README
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.481382 cornflow-1.0.4/cornflow/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/00757b557b02_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/1af47a419bbd_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/4aac5e0c6e66_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/7c3ea5ab5501_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/a472b5ad50b7_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/c2db9409cb5f_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/c8a6c762e818_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/ca449af8034c_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/d0e0700dcd8e_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/d1b5be1f0549_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/e1a50dae1ac9_.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/e937a5234ce4_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/ebdd955fcc5e_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/migrations/versions/f3bee20314a2_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.485382 cornflow-1.0.4/cornflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/base_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/dag_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/models/user_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.485382 cornflow-1.0.4/cornflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/case.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/example_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/model_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/solution_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/schemas/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.485382 cornflow-1.0.4/cornflow/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/shared/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/shared/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/shared/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/shared/log_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/shared/query_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/shared/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/shared/utils_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.485382 cornflow-1.0.4/cornflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/custom_liveServer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24778 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/custom_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.485382 cornflow-1.0.4/cornflow/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/integration/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    20646 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/integration/test_cornflowclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.485382 cornflow-1.0.4/cornflow/tests/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/ldap/test_ldap_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.489382 cornflow-1.0.4/cornflow/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_apiview.py
--rw-r--r--   0 runner    (1001) docker     (123)    23985 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_dags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_data_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_example_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13339 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_health.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_instances_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_log_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-24 08:04:22.000000 cornflow-1.0.4/cornflow/tests/unit/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:04:26.477382 cornflow-1.0.4/cornflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-04-24 08:04:25.000000 cornflow-1.0.4/cornflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-24 08:04:26.000000 cornflow-1.0.4/cornflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:04:25.000000 cornflow-1.0.4/cornflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 08:04:25.000000 cornflow-1.0.4/cornflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 08:04:25.000000 cornflow-1.0.4/cornflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 08:04:25.000000 cornflow-1.0.4/cornflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:04:26.489382 cornflow-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-24 08:04:22.000000 cornflow-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.270341 cornflow-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 08:12:29.000000 cornflow-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-05-05 08:12:33.266341 cornflow-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-05 08:12:29.000000 cornflow-1.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.250341 cornflow-1.0.5/airflow_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:29.000000 cornflow-1.0.5/airflow_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.250341 cornflow-1.0.5/airflow_config/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.250341 cornflow-1.0.5/airflow_config/plugins/XCom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:29.000000 cornflow-1.0.5/airflow_config/plugins/XCom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-05 08:12:29.000000 cornflow-1.0.5/airflow_config/plugins/XCom/gce_xcom_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:29.000000 cornflow-1.0.5/airflow_config/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-05 08:12:29.000000 cornflow-1.0.5/airflow_config/webserver_ldap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.250341 cornflow-1.0.5/cornflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.250341 cornflow-1.0.5/cornflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.254341 cornflow-1.0.5/cornflow/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/tools/api_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/tools/endpoint_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/tools/models_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/tools/schema_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/tools/schemas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/tools/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/cli/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.254341 cornflow-1.0.5/cornflow/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/commands/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.258341 cornflow-1.0.5/cornflow/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/apiview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18670 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28043 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/meta_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/signup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/endpoints/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/gunicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.258341 cornflow-1.0.5/cornflow/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.258341 cornflow-1.0.5/cornflow/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/00757b557b02_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/1af47a419bbd_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/4aac5e0c6e66_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/7c3ea5ab5501_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/a472b5ad50b7_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/c2db9409cb5f_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/c8a6c762e818_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/ca449af8034c_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/d0e0700dcd8e_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/d1b5be1f0549_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/e1a50dae1ac9_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/e937a5234ce4_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/ebdd955fcc5e_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/migrations/versions/f3bee20314a2_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.258341 cornflow-1.0.5/cornflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/base_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/dag_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/meta_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/models/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.262341 cornflow-1.0.5/cornflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/model_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/solution_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/schemas/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.262341 cornflow-1.0.5/cornflow/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.262341 cornflow-1.0.5/cornflow/shared/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/authentication/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/authentication/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/query_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/utils_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/shared/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.266341 cornflow-1.0.5/cornflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/custom_liveServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/custom_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.266341 cornflow-1.0.5/cornflow/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/integration/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20646 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/integration/test_cornflowclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.266341 cornflow-1.0.5/cornflow/tests/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/ldap/test_ldap_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.266341 cornflow-1.0.5/cornflow/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_apiview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23985 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9034 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_dags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_data_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13339 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_generate_from_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_instances_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_log_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_schema_from_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-05 08:12:29.000000 cornflow-1.0.5/cornflow/tests/unit/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:33.250341 cornflow-1.0.5/cornflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-05-05 08:12:33.000000 cornflow-1.0.5/cornflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-05 08:12:33.000000 cornflow-1.0.5/cornflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:12:33.000000 cornflow-1.0.5/cornflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 08:12:33.000000 cornflow-1.0.5/cornflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-05 08:12:33.000000 cornflow-1.0.5/cornflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 08:12:33.000000 cornflow-1.0.5/cornflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:12:33.270341 cornflow-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-05 08:12:30.000000 cornflow-1.0.5/setup.py
```

### Comparing `cornflow-1.0.4/PKG-INFO` & `cornflow-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cornflow
-Version: 1.0.4
+Version: 1.0.5
 Summary: Cornflow is an open source multi-solver optimization server with a REST API built using flask.
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: cornflow@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow
         =========
```

### Comparing `cornflow-1.0.4/README.rst` & `cornflow-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/airflow_config/plugins/XCom/gce_xcom_backend.py` & `cornflow-1.0.5/airflow_config/plugins/XCom/gce_xcom_backend.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/airflow_config/webserver_ldap.py` & `cornflow-1.0.5/airflow_config/webserver_ldap.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/app.py` & `cornflow-1.0.5/cornflow/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     register_deployed_dags_command,
     register_dag_permissions_command,
 )
 from cornflow.config import app_config
 from cornflow.endpoints import resources, alarms_resources
 from cornflow.endpoints.login import LoginEndpoint, LoginOpenAuthEndpoint
 from cornflow.endpoints.signup import SignUpEndpoint
+from cornflow.shared import db, bcrypt
+from cornflow.shared.compress import init_compress
 from cornflow.shared.const import AUTH_DB, AUTH_LDAP, AUTH_OID
+from cornflow.shared.exceptions import initialize_errorhandlers
 from cornflow.shared.log_config import log_config
-from cornflow_core.compress import init_compress
-from cornflow_core.exceptions import initialize_errorhandlers
-from cornflow_core.shared import db, bcrypt
 
 
 def create_app(env_name="development", dataconn=None):
     """
 
     :param str env_name: 'testing' or 'development' or 'production'
     :param str dataconn: string to connect to the database
```

### Comparing `cornflow-1.0.4/cornflow/cli/__init__.py` & `cornflow-1.0.5/cornflow/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import click
 from cornflow.cli.actions import actions
 from cornflow.cli.config import config
 from cornflow.cli.migrations import migrations
 from cornflow.cli.permissions import permissions
 from cornflow.cli.roles import roles
+from cornflow.cli.schemas import schemas
 from cornflow.cli.service import service
 from cornflow.cli.users import users
 from cornflow.cli.views import views
 
 
 @click.group(name="cornflow", help="Commands in the cornflow cli")
 def cli():
@@ -19,10 +20,11 @@
 
 
 cli.add_command(actions)
 cli.add_command(config)
 cli.add_command(migrations)
 cli.add_command(permissions)
 cli.add_command(roles)
+cli.add_command(schemas)
 cli.add_command(service)
 cli.add_command(users)
 cli.add_command(views)
```

### Comparing `cornflow-1.0.4/cornflow/cli/arguments.py` & `cornflow-1.0.5/cornflow/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/cli/config.py` & `cornflow-1.0.5/cornflow/cli/config.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/cli/migrations.py` & `cornflow-1.0.5/cornflow/cli/migrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
 
 
 import click
-from cornflow_core.shared import db
+from cornflow.shared import db
 from flask_migrate import Migrate, migrate, upgrade, init
 
 from .utils import get_app
 
 
 @click.group(name="migrations", help="Commands to manage the migrations")
 def migrations():
```

### Comparing `cornflow-1.0.4/cornflow/cli/permissions.py` & `cornflow-1.0.5/cornflow/cli/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/cli/service.py` & `cornflow-1.0.5/cornflow/cli/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     access_init_command,
     create_user_with_role,
     register_deployed_dags_command,
     register_dag_permissions_command,
     update_schemas_command,
 )
 from cornflow.shared.const import AUTH_DB, ADMIN_ROLE, SERVICE_ROLE
-from cornflow_core.shared import db
+from cornflow.shared import db
 from cryptography.fernet import Fernet
 from flask_migrate import Migrate, upgrade
 
 
 @click.group(name="service", help="Commands to run the cornflow service")
 def service():
     pass
```

### Comparing `cornflow-1.0.4/cornflow/cli/users.py` & `cornflow-1.0.5/cornflow/cli/users.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/cli/utils.py` & `cornflow-1.0.5/cornflow/cli/utils.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/cli/views.py` & `cornflow-1.0.5/cornflow/cli/views.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/commands/__init__.py` & `cornflow-1.0.5/cornflow/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/commands/access.py` & `cornflow-1.0.5/cornflow/commands/access.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/commands/actions.py` & `cornflow-1.0.5/cornflow/commands/actions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 def register_actions_command(verbose: bool = True):
     from flask import current_app
     from sqlalchemy.exc import DBAPIError, IntegrityError
 
-    from cornflow_core.models import ActionBaseModel
+    from cornflow.models import ActionModel
     from cornflow.shared.const import ACTIONS_MAP
-    from cornflow_core.shared import db
+    from cornflow.shared import db
 
-    actions_registered = [ac.name for ac in ActionBaseModel.get_all_objects()]
+    actions_registered = [ac.name for ac in ActionModel.get_all_objects()]
 
     actions_to_register = [
-        ActionBaseModel(id=key, name=value)
+        ActionModel(id=key, name=value)
         for key, value in ACTIONS_MAP.items()
         if value not in actions_registered
     ]
 
     if len(actions_to_register) > 0:
         db.session.bulk_save_objects(actions_to_register)
```

### Comparing `cornflow-1.0.4/cornflow/commands/dag.py` & `cornflow-1.0.5/cornflow/commands/dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     # Partial imports
     from sqlalchemy.exc import DBAPIError, IntegrityError
     from flask import current_app
 
     # Internal modules imports
     from cornflow_client.airflow.api import Airflow
     from cornflow.models import DeployedDAG
-    from cornflow_core.shared import db
+    from cornflow.shared import db
 
     af_client = Airflow(url, user, pwd)
     max_attempts = 20
     attempts = 0
     while not af_client.is_alive() and attempts < max_attempts:
         attempts += 1
         if verbose:
```

### Comparing `cornflow-1.0.4/cornflow/commands/permissions.py` & `cornflow-1.0.5/cornflow/commands/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 from importlib import import_module
 
 from cornflow.shared.const import (
     BASE_PERMISSION_ASSIGNATION,
     EXTRA_PERMISSION_ASSIGNATION,
 )
-from cornflow_core.models import ViewBaseModel, PermissionViewRoleBaseModel
-from cornflow_core.shared import db
+from cornflow.models import ViewModel, PermissionViewRoleModel
+from cornflow.shared import db
 from flask import current_app
 from sqlalchemy.exc import DBAPIError, IntegrityError
 
 
 def register_base_permissions_command(external_app: str = None, verbose: bool = False):
     if external_app is None:
         from cornflow.endpoints import resources, alarms_resources
@@ -21,35 +21,35 @@
         sys.path.append("./")
         external_module = import_module(external_app)
         resources_to_register = external_module.endpoints.resources
     else:
         resources_to_register = []
         exit()
 
-    views_in_db = {view.name: view.id for view in ViewBaseModel.get_all_objects()}
-    permissions_in_db = [perm for perm in PermissionViewRoleBaseModel.get_all_objects()]
+    views_in_db = {view.name: view.id for view in ViewModel.get_all_objects()}
+    permissions_in_db = [perm for perm in PermissionViewRoleModel.get_all_objects()]
     permissions_in_db_keys = [
         (perm.role_id, perm.action_id, perm.api_view_id) for perm in permissions_in_db
     ]
     resources_names = [resource["endpoint"] for resource in resources_to_register]
 
     # Create base permissions
     permissions_in_app = [
-        PermissionViewRoleBaseModel(
+        PermissionViewRoleModel(
             {
                 "role_id": role,
                 "action_id": action,
                 "api_view_id": views_in_db[view["endpoint"]],
             }
         )
         for role, action in BASE_PERMISSION_ASSIGNATION
         for view in resources_to_register
         if role in view["resource"].ROLES_WITH_ACCESS
     ] + [
-        PermissionViewRoleBaseModel(
+        PermissionViewRoleModel(
             {
                 "role_id": role,
                 "action_id": action,
                 "api_view_id": views_in_db[endpoint],
             }
         )
         for role, action, endpoint in EXTRA_PERMISSION_ASSIGNATION
@@ -125,15 +125,15 @@
     open_deployment: int = None, verbose: bool = False
 ):
 
     from flask import current_app
     from sqlalchemy.exc import DBAPIError, IntegrityError
 
     from cornflow.models import DeployedDAG, PermissionsDAG, UserModel
-    from cornflow_core.shared import db
+    from cornflow.shared import db
 
     if open_deployment is None:
         open_deployment = int(current_app.config["OPEN_DEPLOYMENT"])
 
     existing_permissions = [
         (permission.dag_id, permission.user_id)
         for permission in PermissionsDAG.get_all_objects()
```

### Comparing `cornflow-1.0.4/cornflow/commands/roles.py` & `cornflow-1.0.5/cornflow/commands/roles.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 def register_roles_command(verbose: bool = True):
 
     from sqlalchemy.exc import DBAPIError, IntegrityError
     from flask import current_app
 
-    from cornflow_core.models import RoleBaseModel
+    from cornflow.models import RoleModel
     from cornflow.shared.const import ROLES_MAP
-    from cornflow_core.shared import db
+    from cornflow.shared import db
 
-    roles_registered = [role.name for role in RoleBaseModel.get_all_objects()]
+    roles_registered = [role.name for role in RoleModel.get_all_objects()]
 
     roles_to_register = [
-        RoleBaseModel({"id": key, "name": value})
+        RoleModel({"id": key, "name": value})
         for key, value in ROLES_MAP.items()
         if value not in roles_registered
     ]
 
     if len(roles_to_register) > 0:
         db.session.bulk_save_objects(roles_to_register)
```

### Comparing `cornflow-1.0.4/cornflow/commands/schemas.py` & `cornflow-1.0.5/cornflow/commands/schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/commands/users.py` & `cornflow-1.0.5/cornflow/commands/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 def create_user_with_role(
     username, email, password, role_name, role, verbose: bool = False
 ):
-    from cornflow.models import UserModel, UserRoleModel
-    from cornflow_core.models import RoleBaseModel
+    from cornflow.models import UserModel, UserRoleModel, RoleModel
     from flask import current_app
 
     user = UserModel.get_one_user_by_username(username)
 
     if user is None:
         data = dict(username=username, email=email, password=password)
         user = UserModel(data=data)
@@ -19,15 +18,15 @@
             )
         return True
 
     user_roles = UserRoleModel.get_all_objects(user_id=user.id)
     user_actual_roles = [ur.role for ur in user_roles]
     if (
         user_roles is not None
-        and RoleBaseModel.get_one_object(role) in user_actual_roles
+        and RoleModel.get_one_object(role) in user_actual_roles
     ):
         if verbose:
             current_app.logger.info(
                 f"User {username} exists and already has {role_name} role assigned"
             )
         return True
```

### Comparing `cornflow-1.0.4/cornflow/commands/views.py` & `cornflow-1.0.5/cornflow/commands/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-import sys
-from importlib import import_module
 
-from cornflow_core.models import ViewBaseModel
-from cornflow_core.shared import db
+# Imports from external libraries
 from flask import current_app
+from importlib import import_module
 from sqlalchemy.exc import DBAPIError, IntegrityError
+import sys
+
+# Imports from internal libraries
+from cornflow.models import ViewModel
+from cornflow.shared import db
 
 
 def register_views_command(external_app: str = None, verbose: bool = False):
 
     if external_app is None:
         from cornflow.endpoints import resources, alarms_resources
         resources_to_register = resources
@@ -18,18 +21,18 @@
         sys.path.append("./")
         external_module = import_module(external_app)
         resources_to_register = external_module.endpoints.resources
     else:
         resources_to_register = []
         exit()
 
-    views_registered = [view.name for view in ViewBaseModel.get_all_objects()]
+    views_registered = [view.name for view in ViewModel.get_all_objects()]
 
     views_to_register = [
-        ViewBaseModel(
+        ViewModel(
             {
                 "name": view["endpoint"],
                 "url_rule": view["urls"],
                 "description": view["resource"].DESCRIPTION,
             }
         )
         for view in resources_to_register
```

### Comparing `cornflow-1.0.4/cornflow/config.py` & `cornflow-1.0.5/cornflow/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,20 +73,24 @@
     SERVICE_EMAIL_PORT = os.getenv("SERVICE_EMAIL_PORT", None)
 
     # Alarms endpoints
     ALARMS_ENDPOINTS = os.getenv("CF_ALARMS_ENDPOINT", 0)
 
 
 class Development(DefaultConfig):
+
     """ """
 
+    ENV = "development"
+
 
 class Testing(DefaultConfig):
     """ """
 
+    ENV = "testing"
     SQLALCHEMY_TRACK_MODIFICATIONS = False
     DEBUG = False
     TESTING = True
     PROPAGATE_EXCEPTIONS = True
     SECRET_KEY = "TESTINGSECRETKEY"
     SQLALCHEMY_DATABASE_URI = os.getenv("DATABASE_URL", "sqlite:///cornflow_test.db")
     AIRFLOW_URL = os.getenv("AIRFLOW_URL", "http://localhost:8080")
@@ -96,14 +100,15 @@
     OPEN_DEPLOYMENT = 1
     LOG_LEVEL = int(os.getenv("LOG_LEVEL", 10))
 
 
 class Production(DefaultConfig):
     """ """
 
+    ENV = "production"
     SQLALCHEMY_TRACK_MODIFICATIONS = False
     DEBUG = False
     TESTING = False
     # needs to be on to avoid getting only 500 codes:
     # and https://medium.com/@johanesriandy/flask-error-handler-not-working-on-production-mode-3adca4c7385c
     PROPAGATE_EXCEPTIONS = True
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/__init__.py` & `cornflow-1.0.5/cornflow/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/endpoints/action.py` & `cornflow-1.0.5/cornflow/endpoints/action.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """
 
 """
-
-from cornflow_core.authentication import authenticate
-from cornflow_core.resources import BaseMetaResource
-from cornflow_core.schemas import ActionsResponse
+# Imports from external libraries
 from flask_apispec import marshal_with, doc
 from flask import current_app
 
 # Import from internal modules
-from cornflow_core.models import ActionBaseModel
-from cornflow.shared.authentication import Auth
+from cornflow.endpoints.meta_resource import BaseMetaResource
+from cornflow.models import ActionModel
+from cornflow.schemas.action import ActionsResponse
+from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import ADMIN_ROLE
 
 
 class ActionListEndpoint(BaseMetaResource):
     ROLES_WITH_ACCESS = [ADMIN_ROLE]
     DESCRIPTION = "Endpoint which allows to get the actions defined in the application"
 
     def __init__(self):
         super().__init__()
-        self.data_model = ActionBaseModel
+        self.data_model = ActionModel
 
     @doc(description="Get all the actions", tags=["Actions"])
     @authenticate(auth_class=Auth())
     @marshal_with(ActionsResponse(many=True))
     def get(self):
         """
         API method to get the actions defined in the application.
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/alarms.py` & `cornflow-1.0.5/cornflow/endpoints/alarms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Imports from libraries
 from flask_apispec import doc, marshal_with, use_kwargs
-from cornflow_core.authentication import authenticate
-from cornflow_core.resources import BaseMetaResource
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import AlarmsModel
 from cornflow.schemas.alarms import (
     AlarmsResponse,
     AlarmsPostRequest,
     QueryFiltersAlarms
 )
-from cornflow.shared.authentication import Auth
+from cornflow.shared.authentication import Auth, authenticate
 
 
 class AlarmsEndpoint(BaseMetaResource):
     """
     Endpoint used to manage the table alarms.
     Available methods: [get, post]
     """
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/apiview.py` & `cornflow-1.0.5/cornflow/endpoints/apiview.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 """
 
 """
-from cornflow_core.authentication import authenticate
-
 # Import from internal modules
-from cornflow_core.models import ViewBaseModel
-from cornflow_core.resources import BaseMetaResource
-from cornflow_core.schemas import ViewResponse
+from cornflow.endpoints.meta_resource import BaseMetaResource
+from cornflow.models import ViewModel
+from cornflow.schemas.view import ViewResponse
+from cornflow.shared.authentication import Auth, authenticate
+from cornflow.shared.const import ADMIN_ROLE
 
-# Import from libraries
+# Import from external libraries
 from flask_apispec import marshal_with, doc
 from flask import current_app
 
-from cornflow.shared.authentication import Auth
-from cornflow.shared.const import ADMIN_ROLE
-
 
 class ApiViewListEndpoint(BaseMetaResource):
     ROLES_WITH_ACCESS = [ADMIN_ROLE]
     DESCRIPTION = (
         "Endpoint to get the list of all the endpoints defined in cornflow and its url"
     )
 
     def __init__(self):
         super().__init__()
-        self.data_model = ViewBaseModel
+        self.data_model = ViewModel
 
     @doc(description="Get all the api views", tags=["ApiViews"])
     @authenticate(auth_class=Auth())
     @marshal_with(ViewResponse(many=True))
     def get(self):
         """
         API method to get the api views defined in cornflow.
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/case.py` & `cornflow-1.0.5/cornflow/endpoints/case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 """
 External endpoints to manage the cases: create new cases from raw data, from an existing instance or execution
 or from an existing case, update the case info, patch its data, get all of them or one, move them and delete them.
 These endpoints have different access url, but manage the same data entities
 """
 # Import from libraries
+from cornflow_client.constants import (
+    INSTANCE_SCHEMA,
+    SOLUTION_SCHEMA
+)
 from flask import current_app
 from flask_apispec import marshal_with, use_kwargs, doc
 from flask_inflate import inflate
 import jsonpatch
 
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import CaseModel, ExecutionModel, DeployedDAG, InstanceModel
-
+from cornflow.shared.authentication import Auth, authenticate
+from cornflow.shared.compress import compressed
+from cornflow.shared.const import VIEWER_ROLE, PLANNER_ROLE, ADMIN_ROLE
+from cornflow.shared.exceptions import InvalidData, ObjectDoesNotExist
+from cornflow.shared.validators import json_schema_validate_as_string
 from cornflow.schemas.case import (
     CaseBase,
     CaseFromInstanceExecution,
     CaseRawRequest,
     CaseListResponse,
     CaseToInstanceResponse,
     CaseEditRequest,
     QueryFiltersCase,
     QueryCaseCompare,
     CaseCompareResponse,
     CaseListAllWithIndicators,
 )
 
-from cornflow.schemas.model_json import DataSchema
-from cornflow.shared.authentication import Auth
-from cornflow.shared.const import VIEWER_ROLE, PLANNER_ROLE, ADMIN_ROLE
-
-from cornflow_client.constants import (
-    INSTANCE_SCHEMA,
-    SOLUTION_SCHEMA
-)
-
-from cornflow_core.authentication import authenticate
-from cornflow_core.compress import compressed
-from cornflow_core.exceptions import InvalidData, ObjectDoesNotExist
-from cornflow_core.resources import BaseMetaResource
-from cornflow_core.shared import json_schema_validate_as_string
-
-
 
 class CaseEndpoint(BaseMetaResource):
     """
     Endpoint used to create a new case or get all the cases and their related information
     """
     ROLES_WITH_ACCESS = [VIEWER_ROLE, PLANNER_ROLE, ADMIN_ROLE]
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/dag.py` & `cornflow-1.0.5/cornflow/endpoints/dag.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,43 +4,37 @@
 """
 # Import from libraries
 from cornflow_client.constants import SOLUTION_SCHEMA
 from flask import current_app
 from flask_apispec import use_kwargs, doc, marshal_with
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import DeployedDAG, ExecutionModel, InstanceModel, CaseModel
 from cornflow.schemas import DeployedDAGSchema, DeployedDAGEditSchema
 from cornflow.schemas.case import CaseCheckRequest
 from cornflow.schemas.instance import InstanceCheckRequest
 from cornflow.schemas.execution import (
     ExecutionDagPostRequest,
     ExecutionDagRequest,
     ExecutionDetailsEndpointResponse,
     ExecutionSchema,
 )
 
-from cornflow.schemas.model_json import DataSchema
-from cornflow.shared.authentication import Auth
+from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import (
     ADMIN_ROLE,
     EXEC_STATE_CORRECT,
     EXEC_STATE_MANUAL,
     EXECUTION_STATE_MESSAGE_DICT,
     SERVICE_ROLE,
     PLANNER_ROLE,
 )
-
-from cornflow_core.exceptions import ObjectDoesNotExist, InvalidData
-from cornflow_core.authentication import authenticate
-from cornflow_core.resources import BaseMetaResource
-from cornflow_core.shared import json_schema_validate_as_string
-
-
-execution_schema = ExecutionSchema()
+from cornflow.shared.exceptions import ObjectDoesNotExist, InvalidData
+from cornflow.shared.validators import json_schema_validate_as_string
 
 
 class DAGDetailEndpoint(BaseMetaResource):
     """
     Endpoint used for the DAG endpoint
     """
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/data_check.py` & `cornflow-1.0.5/cornflow/endpoints/data_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """
 External endpoints to launch the solution check on an execution
 """
 
 # Import from libraries
 from cornflow_client.airflow.api import Airflow
 from cornflow_client.constants import INSTANCE_SCHEMA, SOLUTION_SCHEMA
-from cornflow_core.authentication import authenticate
-from cornflow_core.exceptions import AirflowError, ObjectDoesNotExist, InvalidUsage, InvalidData
-from cornflow_core.resources import BaseMetaResource
-from cornflow_core.shared import json_schema_validate_as_string
 from flask import request, current_app
 from flask_apispec import marshal_with, doc
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import InstanceModel, ExecutionModel, CaseModel, DeployedDAG
 from cornflow.schemas.execution import ExecutionDetailsEndpointResponse
-from cornflow.shared.authentication import Auth
-
+from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import (
     EXEC_STATE_QUEUED,
     EXEC_STATE_ERROR,
     EXEC_STATE_ERROR_START,
     EXEC_STATE_NOT_RUN,
     EXECUTION_STATE_MESSAGE_DICT, VIEWER_ROLE, PLANNER_ROLE, ADMIN_ROLE,
 )
-
+from cornflow.shared.exceptions import (
+    AirflowError,
+    ObjectDoesNotExist,
+    InvalidUsage,
+    InvalidData
+)
+from cornflow.shared.validators import json_schema_validate_as_string
 
 
 class DataCheckExecutionEndpoint(BaseMetaResource):
     """
     Endpoint used to execute the instance and solution checks on an execution
     """
     ROLES_WITH_ACCESS = [PLANNER_ROLE, ADMIN_ROLE]
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/example_data.py` & `cornflow-1.0.5/cornflow/endpoints/example_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 Endpoints to get the example data from a DAG
 """
 
 # Import from libraries
 from cornflow_client.airflow.api import Airflow
 from flask import current_app, request
 from flask_apispec import marshal_with, doc
-from cornflow_core.authentication import authenticate
 import json
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import PermissionsDAG
-from cornflow.shared.authentication import Auth
-from cornflow_core.exceptions import AirflowError, NoPermission
 from cornflow.schemas.example_data import ExampleData
-from cornflow_core.resources import BaseMetaResource
-
+from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import VIEWER_ROLE, PLANNER_ROLE, ADMIN_ROLE
+from cornflow.shared.exceptions import AirflowError, NoPermission
 
 
 class ExampleDataDetailsEndpoint(BaseMetaResource):
     """
     Endpoint used to obtain schemas for one app
     """
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/execution.py` & `cornflow-1.0.5/cornflow/endpoints/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,53 +2,48 @@
 External endpoints to manage the executions: create new ones, list all of them, get one in particular
 or check the status of an ongoing one
 These endpoints hve different access url, but manage the same data entities
 """
 
 # Import from libraries
 from cornflow_client.airflow.api import Airflow
-from cornflow_core.resources import BaseMetaResource
-from cornflow_core.shared import (
-    json_schema_validate_as_string,
-)
 from cornflow_client.constants import INSTANCE_SCHEMA, CONFIG_SCHEMA, SOLUTION_SCHEMA
 from flask import request, current_app
 from flask_apispec import marshal_with, use_kwargs, doc
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import InstanceModel, DeployedDAG, ExecutionModel
 from cornflow.schemas.execution import (
     ExecutionDetailsEndpointResponse,
     ExecutionDetailsEndpointWithIndicatorsResponse,
     ExecutionDataEndpointResponse,
     ExecutionLogEndpointResponse,
     ExecutionStatusEndpointResponse,
     ExecutionStatusEndpointUpdate,
     ExecutionRequest,
     ExecutionEditRequest,
     QueryFiltersExecution,
     ReLaunchExecutionRequest,
 )
-
-from cornflow.shared.authentication import Auth
+from cornflow.shared.authentication import Auth, authenticate
+from cornflow.shared.compress import compressed
 from cornflow.shared.const import (
     EXEC_STATE_RUNNING,
     EXEC_STATE_ERROR,
     EXEC_STATE_ERROR_START,
     EXEC_STATE_NOT_RUN,
     EXEC_STATE_UNKNOWN,
     EXECUTION_STATE_MESSAGE_DICT,
     AIRFLOW_TO_STATE_MAP,
     EXEC_STATE_STOPPED,
     EXEC_STATE_QUEUED,
 )
-from cornflow_core.authentication import authenticate
-from cornflow_core.exceptions import AirflowError, ObjectDoesNotExist, InvalidData
-from cornflow_core.compress import compressed
-
+from cornflow.shared.exceptions import AirflowError, ObjectDoesNotExist, InvalidData
+from cornflow.shared.validators import json_schema_validate_as_string
 
 class ExecutionEndpoint(BaseMetaResource):
     """
     Endpoint used to create a new execution or get all the executions and their information back
     """
 
     def __init__(self):
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/health.py` & `cornflow-1.0.5/cornflow/endpoints/health.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 # Import from libraries
 from cornflow_client.airflow.api import Airflow
 from flask import current_app
 from flask_apispec import marshal_with, doc
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
+from cornflow.models import UserModel
 from cornflow.schemas.health import HealthResponse
 from cornflow.shared.const import STATUS_HEALTHY, STATUS_UNHEALTHY
-from cornflow_core.resources import BaseMetaResource
-from cornflow.models import UserModel
 
 
 class HealthEndpoint(BaseMetaResource):
     @doc(description="Health check", tags=["Health"])
     @marshal_with(HealthResponse)
     def get(self):
         """
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/instance.py` & `cornflow-1.0.5/cornflow/endpoints/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
 External endpoints to manage the instances: create new ones, or get all the instances created by the user,
 or get only one.
 These endpoints have different access url, but manage the same data entities
 """
 
 # Import from libraries
-from cornflow_core.resources import BaseMetaResource
-from cornflow_core.shared import json_schema_validate_as_string
+from cornflow_client.constants import INSTANCE_SCHEMA
 from flask import request, current_app
 from flask_apispec import marshal_with, use_kwargs, doc
 from flask_inflate import inflate
 from marshmallow.exceptions import ValidationError
 import os
 import pulp
 from werkzeug.utils import secure_filename
-from cornflow_core.authentication import authenticate
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import InstanceModel, DeployedDAG
 from cornflow.schemas.instance import (
     InstanceSchema,
     InstanceEndpointResponse,
     InstanceDetailsEndpointResponse,
     InstanceDataEndpointResponse,
     InstanceRequest,
     InstanceEditRequest,
     InstanceFileRequest,
     QueryFiltersInstance,
 )
 
-from cornflow.shared.authentication import Auth
-from cornflow_core.compress import compressed
-from cornflow_core.exceptions import InvalidUsage, InvalidData
-from cornflow_client.constants import INSTANCE_SCHEMA
+from cornflow.shared.authentication import Auth, authenticate
+from cornflow.shared.compress import compressed
+from cornflow.shared.exceptions import InvalidUsage, InvalidData
+from cornflow.shared.validators import json_schema_validate_as_string
+
 
 
 # Initialize the schema that all endpoints are going to use
 ALLOWED_EXTENSIONS = {"mps", "lp"}
 
 
 class InstanceEndpoint(BaseMetaResource):
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/licenses.py` & `cornflow-1.0.5/cornflow/endpoints/licenses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Imports from libraries
-from cornflow_core.authentication import authenticate
-from cornflow_core.resources import BaseMetaResource
 from flask_apispec import doc
+
+# Imports from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
+from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import VIEWER_ROLE, PLANNER_ROLE, ADMIN_ROLE
 from cornflow.shared.licenses import get_licenses_summary
-from cornflow.shared.authentication import Auth
 
 
 class LicensesEndpoint(BaseMetaResource):
     """
     Endpoint used to obtain data about library licenses.
 
     Available methods: [get]
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/login.py` & `cornflow-1.0.5/cornflow/endpoints/tables.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,82 @@
-"""
-External endpoint for the user to login to the cornflow webserver
-"""
-
-# Full import from libraries
-from cornflow_core.resources import LoginBaseEndpoint
-
-# Partial imports
+# Import from libraries
+from flask_apispec import doc, use_kwargs
 from flask import current_app
-from flask_apispec import use_kwargs, doc
 
 # Import from internal modules
-from cornflow.models import PermissionsDAG, UserModel, UserRoleModel
-from cornflow_core.schemas import LoginEndpointRequest, LoginOpenAuthRequest
-from cornflow.shared.authentication import Auth
+from cornflow.endpoints.meta_resource import BaseMetaResource
+from cornflow.schemas.common import QueryFilters
+from cornflow.shared.authentication import Auth, authenticate
+from cornflow.shared.const import SERVICE_ROLE
+from cornflow.shared.exceptions import InvalidUsage, ObjectDoesNotExist
+from cornflow.shared.utils_tables import get_all_tables, item_as_dict, items_as_dict_list
 
 
-class LoginEndpoint(LoginBaseEndpoint):
-    """
-    Endpoint used to do the login to the cornflow webserver
-    """
+class TablesEndpoint(BaseMetaResource):
+    ROLES_WITH_ACCESS = [SERVICE_ROLE]
 
     def __init__(self):
         super().__init__()
-        self.data_model = UserModel
-        self.auth_class = Auth
-        self.user_role_association = UserRoleModel
-
-    @doc(description="Log in", tags=["Users"])
-    @use_kwargs(LoginEndpointRequest, location="json")
-    def post(self, **kwargs):
+        self.data_model = None
+        self.tables = get_all_tables()
+
+    @doc(description="Get all rows of a table", tags=["Tables"])
+    @authenticate(auth_class=Auth())
+    @use_kwargs(QueryFilters, location="query")
+    def get(self, table_name, **kwargs):
         """
-        API (POST) method to log in in to the web server.
+        API (GET) method to get all directory structure of cases for the user
+        It requires authentication to be passed in the form of a token that has to be linked to
+        an existing session (login) made by a user
 
-        :return: A dictionary with a message (either an error during login or the generated token for the user session)
-          and an integer with the HTTP status code
+        :return: a dictionary with a tree structure of the cases and an integer with the HTTP status code
         :rtype: Tuple(dict, integer)
         """
-
-        content, status = self.log_in(**kwargs)
-        if int(current_app.config["OPEN_DEPLOYMENT"]) == 1:
-            PermissionsDAG.delete_all_permissions_from_user(content["id"])
-            PermissionsDAG.add_all_permissions_to_user(content["id"])
-        return content, status
+        self.data_model = self.tables[table_name]["model"]
+        current_app.logger.info(
+            f"User {self.get_user()} gets all rows of table {table_name}."
+        )
+        res = self.get_list(user=self.get_user(), **kwargs)
+        return items_as_dict_list(res), 200
 
 
-class LoginOpenAuthEndpoint(LoginBaseEndpoint):
-    """ """
+class TablesDetailsEndpoint(BaseMetaResource):
+    ROLES_WITH_ACCESS = [SERVICE_ROLE]
 
     def __init__(self):
         super().__init__()
-        self.data_model = UserModel
-        self.auth_class = Auth
-        self.user_role_association = UserRoleModel
-
-    @doc(description="Log in", tags=["Users"])
-    @use_kwargs(LoginOpenAuthRequest, location="json")
-    def post(self, **kwargs):
-        """ """
-
-        content, status = self.log_in(**kwargs)
-        if int(current_app.config["OPEN_DEPLOYMENT"]) == 1:
-            PermissionsDAG.delete_all_permissions_from_user(content["id"])
-            PermissionsDAG.add_all_permissions_to_user(content["id"])
-        return content, status
+        self.data_model = None
+        self.tables = get_all_tables()
+
+    @doc(description="Get a row", tags=["Tables"])
+    @authenticate(auth_class=Auth())
+    @BaseMetaResource.get_data_or_404
+    def get(self, table_name, idx):
+        """
+        :param table_name: Name of the table to get data from
+        :param idx: id of the row.
+        :return:
+        :rtype: Tuple(dict, integer)
+        """
+        model_info = self.tables[table_name]
+        self.data_model = model_info["model"]
+        conv_idx = idx
+        if model_info["convert_id"]:
+            try:
+                conv_idx = int(idx)
+            except (ValueError, TypeError):
+                raise InvalidUsage(
+                    "Invalid identifier.",
+                    log_txt=f"Error while user {self.get_user()} tries to access row {idx} of table {table_name}. "
+                    f"Identifier is not valid.",
+                )
+
+        current_app.logger.info(
+            f"User {self.get_user()} gets row {idx} of table {table_name}."
+        )
+        res = self.get_detail(idx=conv_idx)
+        if res is None:
+            raise ObjectDoesNotExist(
+                log_txt=f"Error while user {self.get_user()} tries to access row {idx} of table {table_name}. "
+                "The object does not exist."
+            )
+        return item_as_dict(res), 200
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/main_alarms.py` & `cornflow-1.0.5/cornflow/endpoints/main_alarms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Imports from libraries
 from flask_apispec import doc, marshal_with, use_kwargs
-from cornflow_core.authentication import authenticate
-from cornflow_core.resources import BaseMetaResource
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import MainAlarmsModel
 from cornflow.schemas.main_alarms import (
     MainAlarmsResponse,
     MainAlarmsPostRequest,
     QueryFiltersMainAlarms
 )
-from cornflow.shared.authentication import Auth
+from cornflow.shared.authentication import Auth, authenticate
 
 
 class MainAlarmsEndpoint(BaseMetaResource):
     """
     Endpoint used to manage the table main_alarms.
     Available methods: [get, post]
     """
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/permission.py` & `cornflow-1.0.5/cornflow/endpoints/permission.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 """
 
 """
-
-# Import from internal modules
-from cornflow_core.authentication import authenticate
-from cornflow_core.compress import compressed
-from cornflow_core.exceptions import ObjectAlreadyExists
-from cornflow_core.models import PermissionViewRoleBaseModel
-from cornflow_core.resources import BaseMetaResource
-from cornflow_core.schemas import (
-    PermissionViewRoleBaseEditRequest,
-    PermissionViewRoleBaseRequest,
-    PermissionViewRoleBaseResponse,
-)
-
 # Import from libraries
 from flask_apispec import doc, marshal_with, use_kwargs
 from flask import current_app
 
-from cornflow.shared.authentication import Auth
+# Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
+from cornflow.models import PermissionViewRoleModel
+from cornflow.schemas.permissions import (
+    PermissionViewRoleEditRequest,
+    PermissionViewRoleRequest,
+    PermissionViewRoleResponse,
+)
+from cornflow.shared.authentication import Auth, authenticate
+from cornflow.shared.compress import compressed
 from cornflow.shared.const import ADMIN_ROLE
+from cornflow.shared.exceptions import ObjectAlreadyExists
 
 
 class PermissionsViewRoleEndpoint(BaseMetaResource):
     ROLES_WITH_ACCESS = [ADMIN_ROLE]
 
     def __init__(self):
         super().__init__()
-        self.data_model = PermissionViewRoleBaseModel
+        self.data_model = PermissionViewRoleModel
 
     @doc(
         description="Get all the permissions assigned to the roles",
         tags=["PermissionViewRole"],
     )
     @authenticate(auth_class=Auth())
-    @marshal_with(PermissionViewRoleBaseResponse(many=True))
+    @marshal_with(PermissionViewRoleResponse(many=True))
     @compressed
     def get(self):
         current_app.logger.info(
             f"User {self.get_user()} gets all permissions assigned to the roles"
         )
         return self.get_list()
 
     @doc(description="Create a new permission", tags=["PermissionViewRole"])
     @authenticate(auth_class=Auth())
-    @use_kwargs(PermissionViewRoleBaseRequest, location="json")
-    @marshal_with(PermissionViewRoleBaseResponse)
+    @use_kwargs(PermissionViewRoleRequest, location="json")
+    @marshal_with(PermissionViewRoleResponse)
     def post(self, **kwargs):
-        if PermissionViewRoleBaseModel.get_permission(
+        if PermissionViewRoleModel.get_permission(
             role_id=kwargs.get("role_id"),
             api_view_id=kwargs.get("api_view_id"),
             action_id=kwargs.get("action_id"),
         ):
             raise ObjectAlreadyExists(
                 log_txt=f"Error while user {self.get_user()} tries to create a new permission. "
                 f"The permission already exists."
@@ -62,19 +59,19 @@
 
 
 class PermissionsViewRoleDetailEndpoint(BaseMetaResource):
     ROLES_WITH_ACCESS = [ADMIN_ROLE]
 
     def __init__(self):
         super().__init__()
-        self.data_model = PermissionViewRoleBaseModel
+        self.data_model = PermissionViewRoleModel
 
     @doc(description="Get one permission", tags=["PermissionViewRole"])
     @authenticate(auth_class=Auth())
-    @marshal_with(PermissionViewRoleBaseResponse)
+    @marshal_with(PermissionViewRoleResponse)
     @BaseMetaResource.get_data_or_404
     def get(self, idx):
         """
         API method to get one specific permission of the application
         It requires authentication to be passed in the form of a token that has to be linked to
         an existing session (login) made by a user.
 
@@ -86,15 +83,15 @@
         current_app.logger.info(
             f"User {self.get_user()} gets details of permission {idx}"
         )
         return self.get_detail(idx=idx)
 
     @doc(description="Edit a permission", tags=["PermissionViewRole"])
     @authenticate(auth_class=Auth())
-    @use_kwargs(PermissionViewRoleBaseEditRequest, location="json")
+    @use_kwargs(PermissionViewRoleEditRequest, location="json")
     def put(self, idx, **kwargs):
         response = self.put_detail(kwargs, idx=idx, track_user=False)
         current_app.logger.info(f"User {self.get_user()} edits permission {idx}")
         return response
 
     @doc(description="Delete a permission", tags=["PermissionViewRole"])
     @authenticate(auth_class=Auth())
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/roles.py` & `cornflow-1.0.5/cornflow/endpoints/roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 """
 Endpoints to manage the roles of the application and the assignation fo roles to users.
 Some of this endpoints are disable in case that the authentication is not performed over AUTH DB
 """
-
-from cornflow_core.authentication import authenticate
-from cornflow_core.exceptions import EndpointNotImplemented
-from cornflow_core.resources import BaseMetaResource
-
 # Import from libraries
 from flask import current_app
 from flask_apispec import doc, marshal_with, use_kwargs
 
 # Import from internal modules
-from cornflow_core.models import RoleBaseModel
-from cornflow_core.schemas import (
+from cornflow.endpoints.meta_resource import BaseMetaResource
+from cornflow.models import RoleModel
+from cornflow.schemas.role import (
     RolesRequest,
     RolesResponse,
 )
-from cornflow.shared.authentication import Auth
+from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import ADMIN_ROLE, AUTH_LDAP
+from cornflow.shared.exceptions import EndpointNotImplemented
 
 
 class RolesListEndpoint(BaseMetaResource):
     ROLES_WITH_ACCESS = [ADMIN_ROLE]
     DESCRIPTION = "Endpoint to get or create the current roles in the application"
 
     def __init__(self):
         super().__init__()
-        self.data_model = RoleBaseModel
+        self.data_model = RoleModel
 
     @doc(description="Gets all the roles", tags=["Roles"])
     @authenticate(auth_class=Auth())
     @marshal_with(RolesResponse(many=True))
     def get(self):
         """
         API method to get the roles defined in the application.
@@ -75,15 +72,15 @@
 
 class RoleDetailEndpoint(BaseMetaResource):
     ROLES_WITH_ACCESS = [ADMIN_ROLE]
     DESCRIPTION = "Endpoint to get, modify or delete a specific role of the application"
 
     def __init__(self):
         super().__init__()
-        self.data_model = RoleBaseModel
+        self.data_model = RoleModel
 
     @doc(description="Gets one role", tags=["Roles"])
     @authenticate(auth_class=Auth())
     @marshal_with(RolesResponse)
     @BaseMetaResource.get_data_or_404
     def get(self, idx):
         """
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/schemas.py` & `cornflow-1.0.5/cornflow/endpoints/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Endpoints to get the schemas
 """
 
 # Import from libraries
-from cornflow_core.authentication import authenticate
-from cornflow_core.exceptions import NoPermission
-from cornflow_core.resources import BaseMetaResource
 from flask import current_app, request
 from flask_apispec import marshal_with, doc
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import PermissionsDAG, DeployedDAG
 from cornflow.schemas.schemas import SchemaOneApp, SchemaListApp
-from cornflow.shared.authentication import Auth
+from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import ALL_DEFAULT_ROLES
+from cornflow.shared.exceptions import NoPermission
 
 
 class SchemaEndpoint(BaseMetaResource):
     """
     Endpoint used to obtain names of available apps
     """
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/signup.py` & `cornflow-1.0.5/cornflow/endpoints/token.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-"""
-External endpoint for the user to signup
-"""
 # Import from libraries
-from cornflow_core.resources import SignupBaseEndpoint
-from flask import current_app
-from flask_apispec import use_kwargs, doc
+from flask import request
+from flask_apispec import marshal_with, doc
 
 # Import from internal modules
-from cornflow.models import PermissionsDAG, UserRoleModel, UserModel
-from cornflow_core.schemas import SignupRequest
+from cornflow.endpoints.meta_resource import BaseMetaResource
+from cornflow.schemas.user import TokenEndpointResponse
 from cornflow.shared.authentication import Auth
+from cornflow.shared.const import ALL_DEFAULT_ROLES
+from cornflow.shared.exceptions import InvalidCredentials, ObjectDoesNotExist
 
 
-class SignUpEndpoint(SignupBaseEndpoint):
-    """
-    Endpoint used to sign up to the cornflow web server.
-    """
+class TokenEndpoint(BaseMetaResource):
+    ROLES_WITH_ACCESS = ALL_DEFAULT_ROLES
 
     def __init__(self):
         super().__init__()
-        self.data_model = UserModel
-        self.auth_class = Auth
-        self.user_role_association = UserRoleModel
-
-    @doc(description="Sign up", tags=["Users"])
-    @use_kwargs(SignupRequest, location="json")
-    def post(self, **kwargs):
+        self.auth_class = Auth()
+
+    @doc(description="Check token", tags=["Users"])
+    @marshal_with(TokenEndpointResponse)
+    def get(self):
         """
-        API (POST) method to sign up to the cornflow webserver
+        API method to check if a token is valid.
 
-        :return: A dictionary with a message (either an error during signup or the generated token for the user session)
-          and an integer with the HTTP status code
+        :return: A dictionary (containing the token and a boolean 'valid') and an integer with the HTTP status code.
         :rtype: Tuple(dict, integer)
         """
-        content, status = self.sign_up(**kwargs)
-
-        if int(current_app.config["OPEN_DEPLOYMENT"]) == 1:
-            PermissionsDAG.add_all_permissions_to_user(content["id"])
-
-        return content, status
+        token = Auth().get_token_from_header(request.headers)
+        try:
+            self.get_user()
+        except (InvalidCredentials, ObjectDoesNotExist):
+            return {"token": token, "valid": 0}, 200
+        return {"token": token, "valid": 1}, 200
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/user.py` & `cornflow-1.0.5/cornflow/endpoints/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 """
 Endpoints for the user profiles
 """
-# Full imports
-
-from cornflow_core.authentication import authenticate
-from cornflow_core.exceptions import (
-    EndpointNotImplemented,
-    InvalidCredentials,
-    InvalidUsage,
-    NoPermission,
-    ObjectDoesNotExist,
-)
-
-# Partial imports from libraries
-from cornflow_core.resources import BaseMetaResource
-from cornflow_core.resources.recover_password import RecoverPasswordBaseEndpoint
-from cornflow_core.shared import check_email_pattern, check_password_pattern
-from cornflow_core.shared import db
+# Imports from external libraries
 from flask import current_app
 from flask_apispec import marshal_with, use_kwargs, doc
 from sqlalchemy.exc import DBAPIError, IntegrityError
 
-# Import from internal modules
+# Imports from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import UserModel, UserRoleModel
 from cornflow.schemas.user import (
     RecoverPasswordRequest,
     UserDetailsEndpointResponse,
     UserEditRequest,
     UserEndpointResponse,
     UserSchema,
 )
-from cornflow.shared.authentication import Auth
+from cornflow.shared import db
+from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import ADMIN_ROLE, AUTH_LDAP, ALL_DEFAULT_ROLES, AUTH_OID
+from cornflow.shared.exceptions import (
+    ConfigurationError,
+    EndpointNotImplemented,
+    InvalidCredentials,
+    InvalidUsage,
+    NoPermission,
+    ObjectDoesNotExist,
+)
+from cornflow.shared.email import get_password_recover_email, send_email_to
+from cornflow.shared.validators import check_email_pattern, check_password_pattern
 
 
 class UserEndpoint(BaseMetaResource):
     """
     Endpoint with a get method which gives back all the info related to the users.
     Including their instances and executions
     """
@@ -236,15 +233,15 @@
                 current_app.logger.error(f"Integrity error on privileges: {e}")
             except DBAPIError as e:
                 db.session.rollback()
                 current_app.logger.error(f"Unknown error on privileges: {e}")
         return user_obj, 200
 
 
-class RecoverPassword(RecoverPasswordBaseEndpoint):
+class RecoverPassword(BaseMetaResource):
     """
     Endpoint to recover the password
     """
 
     def __init__(self):
         super().__init__()
         self.data_model = UserModel
@@ -257,13 +254,51 @@
         Sends a temporary password and updates the database.
         :param kwargs: a dictionary containing the email address
         :return: A dictionary with a message (error if the email address is not in the database) and an integer with
             the HTTP status code.
         :rtype: Tuple(dict, integer)
         """
 
-        response, status = self.recover_password(kwargs.get("email"))
+        sender = current_app.config["SERVICE_EMAIL_ADDRESS"]
+        password = current_app.config["SERVICE_EMAIL_PASSWORD"]
+        smtp_server = current_app.config["SERVICE_EMAIL_SERVER"]
+        port = current_app.config["SERVICE_EMAIL_PORT"]
+        service_name = current_app.config["SERVICE_NAME"]
+        receiver = kwargs.get("email")
+
+        if sender is None or password is None or smtp_server is None or port is None:
+            raise ConfigurationError(
+                "This functionality is not available. Check that cornflow's email is correctly configured"
+            )
+
+        message = "The password recovery process has started. Check the email inbox."
+
+        user_obj = self.data_model({"email": receiver})
+        if not user_obj.check_email_in_use():
+            return {"message": message}, 200
+
+        new_password = self.data_model.generate_random_password()
+
+        text_email = get_password_recover_email(
+            temp_password=new_password,
+            service_name=service_name,
+            sender=sender,
+            receiver=receiver,
+        )
+
+        send_email_to(
+            email=text_email,
+            smtp_server=smtp_server,
+            port=port,
+            sender=sender,
+            password=password,
+            receiver=receiver,
+        )
+
+        data = {"password": new_password}
+        user_obj = self.data_model.get_one_user_by_email(receiver)
+        user_obj.update(data)
 
         current_app.logger.info(
-            f"User with email {kwargs.get('email')} has requested a new password"
+            f"User with email {receiver} has requested a new password"
         )
-        return response, status
+        return {"message": message}, 200
```

### Comparing `cornflow-1.0.4/cornflow/endpoints/user_role.py` & `cornflow-1.0.5/cornflow/endpoints/user_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """
 Endpoints to manage the roles of the application and the assignation fo roles to users.
-Some of this endpoints are disable in case that the authentication is not performed over AUTH DB
+Some of this endpoints are disabled in case that the authentication is not performed over AUTH DB
 """
 
-from cornflow_core.authentication import authenticate
-from cornflow_core.exceptions import EndpointNotImplemented, ObjectAlreadyExists
-from cornflow_core.resources import BaseMetaResource
-
 # Import from libraries
 from flask import current_app
 from flask_apispec import doc, marshal_with, use_kwargs
 
 # Import from internal modules
+from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import UserRoleModel
-from cornflow_core.schemas import (
-    UserRoleRequest,
-    UserRoleResponse,
-)
-from cornflow.shared.authentication import Auth
+from cornflow.schemas.user_role import UserRoleRequest, UserRoleResponse
+from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import ADMIN_ROLE, AUTH_LDAP
+from cornflow.shared.exceptions import EndpointNotImplemented, ObjectAlreadyExists
 
 
 class UserRoleListEndpoint(BaseMetaResource):
     ROLES_WITH_ACCESS = [ADMIN_ROLE]
     DESCRIPTION = (
         "Endpoint to get the list of roles assigned to users and create new assignments"
     )
```

### Comparing `cornflow-1.0.4/cornflow/migrations/alembic.ini` & `cornflow-1.0.5/cornflow/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/env.py` & `cornflow-1.0.5/cornflow/migrations/env.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/00757b557b02_.py` & `cornflow-1.0.5/cornflow/migrations/versions/00757b557b02_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/1af47a419bbd_.py` & `cornflow-1.0.5/cornflow/migrations/versions/1af47a419bbd_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/4aac5e0c6e66_.py` & `cornflow-1.0.5/cornflow/migrations/versions/4aac5e0c6e66_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/7c3ea5ab5501_.py` & `cornflow-1.0.5/cornflow/migrations/versions/7c3ea5ab5501_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/a472b5ad50b7_.py` & `cornflow-1.0.5/cornflow/migrations/versions/a472b5ad50b7_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/c2db9409cb5f_.py` & `cornflow-1.0.5/cornflow/migrations/versions/c2db9409cb5f_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/c8a6c762e818_.py` & `cornflow-1.0.5/cornflow/migrations/versions/c8a6c762e818_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/ca449af8034c_.py` & `cornflow-1.0.5/cornflow/migrations/versions/ca449af8034c_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/d0e0700dcd8e_.py` & `cornflow-1.0.5/cornflow/migrations/versions/d0e0700dcd8e_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/d1b5be1f0549_.py` & `cornflow-1.0.5/cornflow/migrations/versions/d1b5be1f0549_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/e1a50dae1ac9_.py` & `cornflow-1.0.5/cornflow/migrations/versions/e1a50dae1ac9_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/e937a5234ce4_.py` & `cornflow-1.0.5/cornflow/migrations/versions/e937a5234ce4_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/ebdd955fcc5e_.py` & `cornflow-1.0.5/cornflow/migrations/versions/ebdd955fcc5e_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/migrations/versions/f3bee20314a2_.py` & `cornflow-1.0.5/cornflow/migrations/versions/f3bee20314a2_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/models/alarms.py` & `cornflow-1.0.5/cornflow/models/alarms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Model for the alarms """
 
 # Import from internal modules
-from cornflow_core.shared import db
-from cornflow_core.models import TraceAttributesModel
+from cornflow.shared import db
+from cornflow.models.meta_models import TraceAttributesModel
 
 # Imports from external libraries
 from sqlalchemy.dialects.postgresql import TEXT
 
 
 class AlarmsModel(TraceAttributesModel):
     """
```

### Comparing `cornflow-1.0.4/cornflow/models/base_data_model.py` & `cornflow-1.0.5/cornflow/models/base_data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 
 """
 # Import from libraries
-from cornflow_core.models import TraceAttributesModel
-
-# Import from internal modules
-from cornflow_core.shared import db
 from flask import current_app
 from sqlalchemy import desc
 from sqlalchemy.dialects.postgresql import JSON
 from sqlalchemy.dialects.postgresql import TEXT
 from sqlalchemy.ext.declarative import declared_attr
 
+# Import from internal modules
+from cornflow.models.meta_models import TraceAttributesModel
+from cornflow.shared import db
 from cornflow.shared.utils import hash_json_256
 
 
 class BaseDataModel(TraceAttributesModel):
     """ """
 
     __abstract__ = True
```

### Comparing `cornflow-1.0.4/cornflow/models/case.py` & `cornflow-1.0.5/cornflow/models/case.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # Import from libraries
 import jsonpatch
 from flask import current_app
 from sqlalchemy.dialects.postgresql import JSON
 from sqlalchemy.exc import DBAPIError, IntegrityError
 
 # Import from internal modules
-from .base_data_model import BaseDataModel
-from cornflow_core.exceptions import InvalidPatch, ObjectDoesNotExist, InvalidData
-from cornflow_core.shared import db
+from cornflow.models.base_data_model import BaseDataModel
+from cornflow.shared import db
+from cornflow.shared.exceptions import InvalidPatch, ObjectDoesNotExist, InvalidData
 from cornflow.shared.utils import hash_json_256
 
 
 # Originally inspired by this:
 # https://docs.sqlalchemy.org/en/13/_modules/examples/materialized_paths/materialized_paths.html
 # An alternative implementation with fixed width strings and no separator
 # https://stackoverflow.com/questions/7276119/querying-sqlite-tree-structure
```

### Comparing `cornflow-1.0.4/cornflow/models/dag.py` & `cornflow-1.0.5/cornflow/models/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 
 """
 # Import from libraries
-from sqlalchemy.dialects.postgresql import TEXT, JSON
-
-# Import from internal modules
-from cornflow_core.models import TraceAttributesModel
-from cornflow_core.shared import db
 from cornflow_client.airflow.api import Airflow
 from cornflow_client.constants import (
     INSTANCE_SCHEMA,
     SOLUTION_SCHEMA,
     INSTANCE_CHECKS_SCHEMA,
     SOLUTION_CHECKS_SCHEMA
 )
-from cornflow_core.exceptions import ObjectDoesNotExist
+from sqlalchemy.dialects.postgresql import TEXT, JSON
+
+# Import from internal modules
+from cornflow.models.meta_models import TraceAttributesModel
+from cornflow.shared import db
+from cornflow.shared.exceptions import ObjectDoesNotExist
 
 
 class DeployedDAG(TraceAttributesModel):
     """
     This model contains the registry of the DAGs that are deployed on the corresponding Airflow server
     """
```

### Comparing `cornflow-1.0.4/cornflow/models/dag_permissions.py` & `cornflow-1.0.5/cornflow/models/dag_permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from cornflow_core.models import TraceAttributesModel
-from cornflow_core.shared import db
-
-# from .meta_model import TraceAttributes
-from .dag import DeployedDAG
+from cornflow.models.dag import DeployedDAG
+from cornflow.models.meta_models import TraceAttributesModel
+from cornflow.shared import db
 
 
 class PermissionsDAG(TraceAttributesModel):
     __tablename__ = "permission_dag"
     __table_args__ = (db.UniqueConstraint("dag_id", "user_id"),)
 
     id = db.Column(db.Integer, primary_key=True, autoincrement=True)
```

### Comparing `cornflow-1.0.4/cornflow/models/execution.py` & `cornflow-1.0.5/cornflow/models/execution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 Model for the executions
 """
 
 # Import from libraries
 import hashlib
-
-# Imports from sqlalchemy
-from sqlalchemy.dialects.postgresql import JSON
-from sqlalchemy.dialects.postgresql import TEXT
+from sqlalchemy.dialects.postgresql import JSON, TEXT
 
 # Imports from internal modules
-from cornflow_core.shared import db
-from .base_data_model import BaseDataModel
+from cornflow.models.base_data_model import BaseDataModel
+from cornflow.shared import db
 from cornflow.shared.const import DEFAULT_EXECUTION_CODE, EXECUTION_STATE_MESSAGE_DICT
 
 
 class ExecutionModel(BaseDataModel):
     """
     Model class for the Executions.
     It inherits from :class:`BaseDataModel` to have the trace fields and user field
```

### Comparing `cornflow-1.0.4/cornflow/models/instance.py` & `cornflow-1.0.5/cornflow/models/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Model for the instances"""
 
 # Import from libraries
 import hashlib
 
 # Imported from internal models
-from .base_data_model import BaseDataModel
-from cornflow_core.shared import db
+from cornflow.models.base_data_model import BaseDataModel
+from cornflow.shared import db
 
 
 class InstanceModel(BaseDataModel):
     """
     Model class for the Instances
     It inherits from :class:`BaseDataModel` to have the trace fields and user field
```

### Comparing `cornflow-1.0.4/cornflow/models/main_alarms.py` & `cornflow-1.0.5/cornflow/models/main_alarms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Model for the alarms """
 
 # Import from internal modules
-from cornflow_core.shared import db
-from cornflow_core.models import TraceAttributesModel
+from cornflow.shared import db
+from cornflow.models.meta_models import TraceAttributesModel
 
 
 # Imports from external libraries
 from sqlalchemy.dialects.postgresql import TEXT
 
 
 class MainAlarmsModel(TraceAttributesModel):
```

### Comparing `cornflow-1.0.4/cornflow/models/user.py` & `cornflow-1.0.5/cornflow/models/role.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,58 @@
-from cornflow_core.models import UserBaseModel
-from cornflow_core.shared import db
+"""
+This file contains the RoleModel
+"""
+# Imports from internal modules
+from cornflow.models.meta_models import TraceAttributesModel
+from cornflow.shared import db
 
-from .user_role import UserRoleModel
 
-
-class UserModel(UserBaseModel):
+class RoleModel(TraceAttributesModel):
     """
-    Model class for the Users.
-    It inherits from :class:`TraceAttributes` to have trace fields.
+    This model has the roles that are defined on the REST API
+    It inherits from :class:`TraceAttributesModel` to have trace fields
 
-    The class :class:`UserModel` has the following fields:
+    The :class:`RoleModel` has the following fields:
 
-    - **id**: int, the user id, primary key for the users.
-    - **first_name**: str, the name of the user.
-    - **last_name**: str, the name of the user.
-    - **username**: str, the username of the user used for the login.
-    - **email**: str, the email of the user.
-    - **password**: str, the hashed password of the user.
-    - **created_at**: datetime, the datetime when the execution was created (in UTC).
+    - **id**: int, the primary key of the table, an integer value that is auto incremented
+    - **name**: str, the name of the role
+    - **created_at**: datetime, the datetime when the user was created (in UTC).
       This datetime is generated automatically, the user does not need to provide it.
-    - **updated_at**: datetime, the datetime when the execution was last updated (in UTC).
+    - **updated_at**: datetime, the datetime when the user was last updated (in UTC).
       This datetime is generated automatically, the user does not need to provide it.
-    - **deleted_at**: datetime, the datetime when the execution was deleted (in UTC). Even though it is deleted,
-      actually, it is not deleted from the database, in order to have a command that cleans up deleted data
-      after a certain time of its deletion.
+    - **deleted_at**: datetime, the datetime when the user was deleted (in UTC).
+      This field is used only if we deactivate instead of deleting the record.
       This datetime is generated automatically, the user does not need to provide it.
-
-    :param dict data: the parsed json got from and endpoint that contains all the required information to
-      create a new user.
     """
 
-    __tablename__ = "users"
-    __table_args__ = {"extend_existing": True}
-
-    instances = db.relationship(
-        "InstanceModel",
-        backref="users",
+    __tablename__ = "roles"
+    id = db.Column(db.Integer, primary_key=True, autoincrement=True)
+    name = db.Column(db.String(128), nullable=False)
+
+    user_roles = db.relationship(
+        "UserRoleModel",
+        backref="roles",
         lazy=True,
-        primaryjoin="and_(UserModel.id==InstanceModel.user_id, "
-        "InstanceModel.deleted_at==None)",
+        primaryjoin="and_(RoleModel.id==UserRoleModel.role_id, "
+        "UserRoleModel.deleted_at==None)",
         cascade="all,delete",
     )
 
-    cases = db.relationship(
-        "CaseModel",
-        backref="users",
+    permissions = db.relationship(
+        "PermissionViewRoleModel",
+        backref="roles",
         lazy=True,
-        primaryjoin="and_(UserModel.id==CaseModel.user_id, CaseModel.deleted_at==None)",
+        primaryjoin="and_(RoleModel.id==PermissionViewRoleModel.role_id, "
+        "PermissionViewRoleModel.deleted_at==None)",
         cascade="all,delete",
     )
 
-    dag_permissions = db.relationship(
-        "PermissionsDAG",
-        cascade="all,delete",
-        backref="users",
-        primaryjoin="and_(UserModel.id==PermissionsDAG.user_id)",
-    )
+    def __init__(self, data):
+        super().__init__()
+        self.id = data.get("id")
+        self.name = data.get("name")
+
+    def __repr__(self):
+        return f"<Role {self.name}>"
 
-    def is_admin(self):
-        """
-        Returns a boolean if a user is an admin or not
-        """
-        return UserRoleModel.is_admin(self.id)
-
-    def is_service_user(self):
-        """
-        Returns a boolean if a user is a service user or not
-        """
-        return UserRoleModel.is_service_user(self.id)
+    def __str__(self):
+        return self.__repr__()
```

### Comparing `cornflow-1.0.4/cornflow/schemas/alarms.py` & `cornflow-1.0.5/cornflow/schemas/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/schemas/case.py` & `cornflow-1.0.5/cornflow/schemas/case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 This file contains the schemas used to validate the incoming data to the different cases endpoints
 and to serialize the response data given by the same endpoints.
 """
 
-from cornflow_core.schemas import BasePatchOperation
-
 # Imports from marshmallow library
 from marshmallow import fields, Schema
 
 # Import from internal modules
 from .common import BaseDataEndpointResponse, QueryFilters
+from .patch import BasePatchOperation
 
 
 class CaseRawRequest(Schema):
 
     name = fields.Str(required=True)
     description = fields.Str()
     schema = fields.Str(required=True)
```

### Comparing `cornflow-1.0.4/cornflow/schemas/dag.py` & `cornflow-1.0.5/cornflow/schemas/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/schemas/execution.py` & `cornflow-1.0.5/cornflow/schemas/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+# Imports from libraries
 from marshmallow import fields, Schema, validate
-from .solution_log import LogSchema
+
+# Imports from internal modules
 from cornflow.shared.const import MIN_EXECUTION_STATUS_CODE, MAX_EXECUTION_STATUS_CODE
 from .common import QueryFilters, BaseDataEndpointResponse
+from .solution_log import LogSchema
 
 
 class QueryFiltersExecution(QueryFilters):
     pass
     # status = fields.Int(required=False)
```

### Comparing `cornflow-1.0.4/cornflow/schemas/instance.py` & `cornflow-1.0.5/cornflow/schemas/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/schemas/main_alarms.py` & `cornflow-1.0.5/cornflow/schemas/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/schemas/solution_log.py` & `cornflow-1.0.5/cornflow/schemas/solution_log.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/shared/const.py` & `cornflow-1.0.5/cornflow/shared/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,10 @@
 """
 In this files we import the values for different constants on cornflow server
-This constants can be inherited from cornflow-core or can be overridden here
 """
-from cornflow_core.constants import (
-    AUTH_DB,
-    AUTH_LDAP,
-    AUTH_OID,
-    AUTH_OAUTH,
-    OID_NONE,
-    OID_AZURE,
-    OID_GOOGLE,
-    VIEWER_ROLE,
-    PLANNER_ROLE,
-    ADMIN_ROLE,
-    SERVICE_ROLE,
-    ALL_DEFAULT_ROLES,
-    ROLES_MAP,
-)
 
 # endpoints responses for health check
 STATUS_HEALTHY = "healthy"
 STATUS_UNHEALTHY = "unhealthy"
 
 # execution states for executions table
 EXEC_STATE_CORRECT = 1
@@ -57,23 +41,23 @@
     running=EXEC_STATE_RUNNING,
     failed=EXEC_STATE_ERROR,
     queued=EXEC_STATE_QUEUED,
 )
 
 # These codes and names are inherited from flask app builder in order to have the same names and values
 # as this library that is the base of airflow
-AUTH_DB = AUTH_DB
-AUTH_LDAP = AUTH_LDAP
-AUTH_OAUTH = AUTH_OAUTH
-AUTH_OID = AUTH_OID
+AUTH_DB = 1
+AUTH_LDAP = 2
+AUTH_OAUTH = 4
+AUTH_OID = 0
 
 # Providers of open ID:
-OID_NONE = OID_NONE
-OID_AZURE = OID_AZURE
-OID_GOOGLE = OID_GOOGLE
+OID_NONE = 0
+OID_AZURE = 1
+OID_GOOGLE = 2
 
 # AZURE OPEN ID URLS
 OID_AZURE_DISCOVERY_COMMON_URL = (
     "https://login.microsoftonline.com/common/.well-known/openid-configuration"
 )
 OID_AZURE_DISCOVERY_TENANT_URL = (
     "https://login.microsoftonline.com/{tenant_id}/.well-known/openid-configuration"
@@ -83,20 +67,20 @@
 PATCH_ACTION = 2
 POST_ACTION = 3
 PUT_ACTION = 4
 DELETE_ACTION = 5
 
 ALL_DEFAULT_ACTIONS = [GET_ACTION, PATCH_ACTION, POST_ACTION, PUT_ACTION, DELETE_ACTION]
 
-VIEWER_ROLE = VIEWER_ROLE
-PLANNER_ROLE = PLANNER_ROLE
-ADMIN_ROLE = ADMIN_ROLE
-SERVICE_ROLE = SERVICE_ROLE
+VIEWER_ROLE = 1
+PLANNER_ROLE = 2
+ADMIN_ROLE = 3
+SERVICE_ROLE = 4
 
-ALL_DEFAULT_ROLES = ALL_DEFAULT_ROLES
+ALL_DEFAULT_ROLES = [VIEWER_ROLE, PLANNER_ROLE, ADMIN_ROLE, SERVICE_ROLE]
 
 ACTIONS_MAP = {
     GET_ACTION: "can_get",
     PATCH_ACTION: "can_patch",
     POST_ACTION: "can_post",
     PUT_ACTION: "can_put",
     DELETE_ACTION: "can_delete",
@@ -106,15 +90,20 @@
     "GET": GET_ACTION,
     "PATCH": PATCH_ACTION,
     "POST": POST_ACTION,
     "PUT": PUT_ACTION,
     "DELETE": DELETE_ACTION,
 }
 
-ROLES_MAP = ROLES_MAP
+ROLES_MAP = {
+    PLANNER_ROLE: "planner",
+    VIEWER_ROLE: "viewer",
+    ADMIN_ROLE: "admin",
+    SERVICE_ROLE: "service",
+}
 
 BASE_PERMISSION_ASSIGNATION = [
     (VIEWER_ROLE, GET_ACTION),
     (PLANNER_ROLE, GET_ACTION),
     (PLANNER_ROLE, PATCH_ACTION),
     (PLANNER_ROLE, POST_ACTION),
     (PLANNER_ROLE, PUT_ACTION),
```

### Comparing `cornflow-1.0.4/cornflow/shared/licenses.py` & `cornflow-1.0.5/cornflow/shared/licenses.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/shared/log_config.py` & `cornflow-1.0.5/cornflow/shared/log_config.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/shared/query_tools.py` & `cornflow-1.0.5/cornflow/shared/query_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/shared/utils_tables.py` & `cornflow-1.0.5/cornflow/shared/utils_tables.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from importlib import import_module
-import sys
-import os
+# Imports from external libraries
 import inspect
+import os
+import sys
+
+from importlib import import_module
 from sqlalchemy.dialects.postgresql import TEXT
-from cornflow_core.models import EmptyBaseModel
-from cornflow_core.shared import db
 from sqlalchemy.sql.sqltypes import Integer
+
+# Imports from internal modules
 from cornflow.models import *
+from cornflow.models.meta_models import EmptyBaseModel
+from cornflow.shared import db
 
 
 def _import_file(filename):
     return import_module(filename)
 
 
 def import_models():
```

### Comparing `cornflow-1.0.4/cornflow/tests/const.py` & `cornflow-1.0.5/cornflow/tests/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/custom_liveServer.py` & `cornflow-1.0.5/cornflow/tests/custom_liveServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Full imports
 import os
 
 import cornflow_client as cf
-from cornflow_core.shared import db
+from cornflow.shared import db
 
 # External libraries
 from flask import current_app
 from flask_testing import LiveServerTestCase
 
 # Internal modules
 from cornflow.app import create_app
```

### Comparing `cornflow-1.0.4/cornflow/tests/custom_test_case.py` & `cornflow-1.0.5/cornflow/tests/custom_test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from cornflow.app import create_app
 from cornflow.models import UserRoleModel
 from cornflow.commands.access import access_init_command
 from cornflow.commands.dag import register_deployed_dags_command_test
 from cornflow.commands.permissions import register_dag_permissions_command
 from cornflow.shared.authentication import Auth
 from cornflow.shared.const import ADMIN_ROLE, PLANNER_ROLE, SERVICE_ROLE
-from cornflow_core.shared import db
+from cornflow.shared import db
 from cornflow.tests.const import (
     LOGIN_URL,
     SIGNUP_URL,
     USER_URL,
     USER_ROLE_URL,
     TOKEN_URL,
 )
```

### Comparing `cornflow-1.0.4/cornflow/tests/integration/test_commands.py` & `cornflow-1.0.5/cornflow/tests/integration/test_commands.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/integration/test_cornflowclient.py` & `cornflow-1.0.5/cornflow/tests/integration/test_cornflowclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
     def test_status_solving_timer(self):
         execution = self.create_timer_instance_and_execution(10)
         status = self.client.get_status(execution["id"])
         self.assertEqual(status["state"], EXEC_STATE_QUEUED)
         time.sleep(5)
         status = self.client.get_status(execution["id"])
         self.assertEqual(status["state"], EXEC_STATE_RUNNING)
-        time.sleep(10)
+        time.sleep(12)
         status = self.client.get_status(execution["id"])
         self.assertEqual(status["state"], EXEC_STATE_CORRECT)
 
     def test_manual_execution(self):
 
         instance_payload = load_file(INSTANCE_PATH)
         one_instance = self.create_new_instance_payload(instance_payload)
```

### Comparing `cornflow-1.0.4/cornflow/tests/ldap/test_ldap_authentication.py` & `cornflow-1.0.5/cornflow/tests/ldap/test_ldap_authentication.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_actions.py` & `cornflow-1.0.5/cornflow/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_alarms.py` & `cornflow-1.0.5/cornflow/tests/unit/test_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_apiview.py` & `cornflow-1.0.5/cornflow/tests/unit/test_apiview.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_cases.py` & `cornflow-1.0.5/cornflow/tests/unit/test_cases.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_cli.py` & `cornflow-1.0.5/cornflow/tests/unit/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import configparser
 import os
 
 from click.testing import CliRunner
 from cornflow.app import create_app
 from cornflow.cli import cli
 from cornflow.models import UserModel
-from cornflow_core.models import (
-    ActionBaseModel,
-    RoleBaseModel,
-    ViewBaseModel,
-    PermissionViewRoleBaseModel,
+from cornflow.models import (
+    ActionModel,
+    RoleModel,
+    ViewModel,
+    PermissionViewRoleModel,
 )
-from cornflow_core.shared import db
+from cornflow.shared import db
 from flask_testing import TestCase
 
 
 class CLITests(TestCase):
     def setUp(self):
         db.create_all()
 
@@ -58,15 +58,15 @@
         self.assertIn("init", result.output)
         self.assertIn("Initialize the actions", result.output)
 
     def test_actions(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["actions", "init", "-v"])
         self.assertEqual(result.exit_code, 0)
-        actions = ActionBaseModel.get_all_objects().all()
+        actions = ActionModel.get_all_objects().all()
         self.assertEqual(len(actions), 5)
 
     def test_config_entrypoint(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["config", "--help"])
         self.assertEqual(result.exit_code, 0)
         self.assertIn("Commands to manage the configuration variables", result.output)
@@ -109,30 +109,30 @@
         self.assertIn("init", result.output)
         self.assertIn("Initializes the roles with the default roles", result.output)
 
     def test_roles_init_command(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["roles", "init", "-v"])
         self.assertEqual(result.exit_code, 0)
-        roles = RoleBaseModel.get_all_objects().all()
+        roles = RoleModel.get_all_objects().all()
         self.assertEqual(len(roles), 4)
 
     def test_views_entrypoint(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["views", "--help"])
         self.assertEqual(result.exit_code, 0)
         self.assertIn("Commands to manage the views", result.output)
         self.assertIn("init", result.output)
         self.assertIn("Initialize the views", result.output)
 
     def test_views_init_command(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["views", "init", "-v"])
         self.assertEqual(result.exit_code, 0)
-        views = ViewBaseModel.get_all_objects().all()
+        views = ViewModel.get_all_objects().all()
         self.assertEqual(len(views), 48)
 
     def test_permissions_entrypoint(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["permissions", "--help"])
         self.assertEqual(result.exit_code, 0)
         self.assertIn("Commands to manage the permissions", result.output)
@@ -143,34 +143,34 @@
         self.assertIn("base", result.output)
         self.assertIn("Initialize the base permissions", result.output)
 
     def test_permissions_init(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["permissions", "init", "-v"])
         self.assertEqual(result.exit_code, 0)
-        actions = ActionBaseModel.get_all_objects().all()
-        roles = RoleBaseModel.get_all_objects().all()
-        views = ViewBaseModel.get_all_objects().all()
-        permissions = PermissionViewRoleBaseModel.get_all_objects().all()
+        actions = ActionModel.get_all_objects().all()
+        roles = RoleModel.get_all_objects().all()
+        views = ViewModel.get_all_objects().all()
+        permissions = PermissionViewRoleModel.get_all_objects().all()
         self.assertEqual(len(actions), 5)
         self.assertEqual(len(roles), 4)
         self.assertEqual(len(views), 48)
         self.assertEqual(len(permissions), 530)
 
     def test_permissions_base_command(self):
         runner = CliRunner()
         runner.invoke(cli, ["actions", "init", "-v"])
         runner.invoke(cli, ["roles", "init", "-v"])
         runner.invoke(cli, ["views", "init", "-v"])
         result = runner.invoke(cli, ["permissions", "base", "-v"])
         self.assertEqual(result.exit_code, 0)
-        actions = ActionBaseModel.get_all_objects().all()
-        roles = RoleBaseModel.get_all_objects().all()
-        views = ViewBaseModel.get_all_objects().all()
-        permissions = PermissionViewRoleBaseModel.get_all_objects().all()
+        actions = ActionModel.get_all_objects().all()
+        roles = RoleModel.get_all_objects().all()
+        views = ViewModel.get_all_objects().all()
+        permissions = PermissionViewRoleModel.get_all_objects().all()
         self.assertEqual(len(actions), 5)
         self.assertEqual(len(roles), 4)
         self.assertEqual(len(views), 48)
         self.assertEqual(len(permissions), 530)
 
     def test_service_entrypoint(self):
         runner = CliRunner()
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_commands.py` & `cornflow-1.0.5/cornflow/tests/unit/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 import json
 
-from cornflow.tests.const import LOGIN_URL, INSTANCE_URL, INSTANCE_PATH
-from cornflow.tests.integration.test_cornflowclient import load_file
-from cornflow_core.models import (
-    ActionBaseModel,
-    PermissionViewRoleBaseModel,
-    RoleBaseModel,
-    ViewBaseModel,
-)
-
-from cornflow_core.shared import db
 from flask_testing import TestCase
 
 from cornflow.app import (
     access_init,
     create_admin_user,
     create_app,
     create_base_user,
     create_service_user,
     register_actions,
     register_dag_permissions,
     register_roles,
     register_views,
 )
-
-
 from cornflow.commands.dag import register_deployed_dags_command_test
 from cornflow.endpoints import resources, alarms_resources
-
+from cornflow.models import (
+    ActionModel,
+    PermissionViewRoleModel,
+    RoleModel,
+    ViewModel,
+)
 from cornflow.models import (
     DeployedDAG,
     PermissionsDAG,
     UserModel,
 )
-
+from cornflow.shared import db
 from cornflow.shared.const import (
     ACTIONS_MAP,
     ROLES_MAP,
     BASE_PERMISSION_ASSIGNATION,
 )
+from cornflow.tests.const import LOGIN_URL, INSTANCE_URL, INSTANCE_PATH
+from cornflow.tests.integration.test_cornflowclient import load_file
 
 
 class TestCommands(TestCase):
     def create_app(self):
         app = create_app("testing")
         app.config["OPEN_DEPLOYMENT"] = 1
         return app
@@ -146,45 +141,44 @@
 
     def test_base_user_command(self):
         return self.user_command(create_base_user, "base", "base@test.org")
 
     def test_register_actions(self):
         self.runner.invoke(register_actions)
 
-        actions = ActionBaseModel.query.all()
+        actions = ActionModel.query.all()
 
         for a in actions:
             self.assertEqual(ACTIONS_MAP[a.id], a.name)
 
     def test_register_views(self):
         self.runner.invoke(register_views)
 
-        views = ViewBaseModel.query.all()
+        views = ViewModel.query.all()
         views_list = [v.name for v in views]
         resources_list = [
             self.resources[i]["endpoint"] for i in range(len(self.resources))
         ]
 
         self.assertCountEqual(views_list, resources_list)
 
     def test_register_roles(self):
-        roles = RoleBaseModel.query.all()
+        roles = RoleModel.query.all()
         for r in roles:
             self.assertEqual(ROLES_MAP[r.id], r.name)
 
     def test_base_permissions_assignation(self):
         self.runner.invoke(access_init)
 
         for base in BASE_PERMISSION_ASSIGNATION:
             for view in self.resources:
                 if base[0] in view["resource"].ROLES_WITH_ACCESS:
-
-                    permission = PermissionViewRoleBaseModel.get_permission(
+                    permission = PermissionViewRoleModel.get_permission(
                         role_id=base[0],
-                        api_view_id=ViewBaseModel.query.filter_by(name=view["endpoint"])
+                        api_view_id=ViewModel.query.filter_by(name=view["endpoint"])
                         .first()
                         .id,
                         action_id=base[1],
                     )
 
                     self.assertEqual(True, permission)
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_dags.py` & `cornflow-1.0.5/cornflow/tests/unit/test_dags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from cornflow.app import create_app
 from cornflow.commands.access import access_init_command
 from cornflow.commands.dag import register_deployed_dags_command_test
 from cornflow.commands.permissions import register_dag_permissions_command
 from cornflow.shared.const import ADMIN_ROLE, SERVICE_ROLE
 from cornflow.models import DeployedDAG, PermissionsDAG, UserModel, UserRoleModel
 from cornflow.shared.const import EXEC_STATE_CORRECT, EXEC_STATE_MANUAL
-from cornflow_core.shared import db
+from cornflow.shared import db
 from cornflow.tests.const import (
     CASE_PATH,
     DAG_URL,
     DEPLOYED_DAG_URL,
     EXECUTION_URL_NORUN,
     INSTANCE_URL,
     LOGIN_URL,
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_data_checks.py` & `cornflow-1.0.5/cornflow/tests/unit/test_data_checks.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_example_data.py` & `cornflow-1.0.5/cornflow/tests/unit/test_example_data.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_executions.py` & `cornflow-1.0.5/cornflow/tests/unit/test_executions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_health.py` & `cornflow-1.0.5/cornflow/tests/unit/test_health.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from cornflow_core.shared import db
+from cornflow.shared import db
 
 from cornflow.app import create_app
 from cornflow.commands import access_init_command
 from cornflow.shared.const import STATUS_HEALTHY
 from cornflow.tests.const import HEALTH_URL
 from cornflow.tests.custom_test_case import CustomTestCase
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_instances.py` & `cornflow-1.0.5/cornflow/tests/unit/test_instances.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_instances_file.py` & `cornflow-1.0.5/cornflow/tests/unit/test_instances_file.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_log_in.py` & `cornflow-1.0.5/cornflow/tests/unit/test_log_in.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # Import from libraries
 from flask import current_app
 
 # Import from internal modules
 from cornflow.models import UserModel
-from cornflow_core.shared import db
+from cornflow.shared import db
 from cornflow.tests.custom_test_case import LoginTestCases
 
 
 class TestLogIn(LoginTestCases.LoginEndpoint):
     def setUp(self):
         super().setUp()
         db.create_all()
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_main_alarms.py` & `cornflow-1.0.5/cornflow/tests/unit/test_main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_permissions.py` & `cornflow-1.0.5/cornflow/tests/unit/test_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Unit test for the permissions table
 """
 
 # Import from libraries
 import json
 
-from cornflow_core.models import (
-    ActionBaseModel,
-    PermissionViewRoleBaseModel,
-    RoleBaseModel,
-    ViewBaseModel,
+from cornflow.models import (
+    ActionModel,
+    PermissionViewRoleModel,
+    RoleModel,
+    ViewModel,
 )
 
 # Import from internal modules
 from cornflow.app import create_app
 from cornflow.endpoints import (
     PermissionsViewRoleEndpoint,
     PermissionsViewRoleDetailEndpoint,
@@ -23,15 +23,15 @@
 from cornflow.tests.const import INSTANCE_PATH, INSTANCE_URL, PERMISSION_URL
 from cornflow.tests.custom_test_case import CustomTestCase
 
 
 class TestPermissionsViewRoleEndpoint(CustomTestCase):
     def setUp(self):
         super().setUp()
-        self.model = PermissionViewRoleBaseModel
+        self.model = PermissionViewRoleModel
         self.roles_with_access = PermissionsViewRoleEndpoint.ROLES_WITH_ACCESS
         self.payload = {"role_id": 1, "permission_id": 1, "api_view_id": 1}
 
     def tearDown(self):
         super().tearDown()
 
     def test_get_permissions_view_role(self):
@@ -84,15 +84,15 @@
                     check_payload=False,
                 )
 
 
 class TestPermissionViewRolesDetailEndpoint(CustomTestCase):
     def setUp(self):
         super().setUp()
-        self.model = PermissionViewRoleBaseModel
+        self.model = PermissionViewRoleModel
         self.roles_with_access = PermissionsViewRoleDetailEndpoint.ROLES_WITH_ACCESS
         self.payload = {"role_id": 1, "action_id": 3, "api_view_id": 1}
         self.items_to_check = []
 
     def test_modify_permission_authorized_user(self):
         authorized_user = self.roles_with_access[0]
         self.token = self.create_user_with_role(authorized_user)
@@ -219,26 +219,26 @@
 
 
 class TestPermissionsViewModel(CustomTestCase):
     def setUp(self):
         super().setUp()
 
     def test_permission_role_cascade_deletion(self):
-        before_permissions = PermissionViewRoleBaseModel.get_all_objects()
-        role = RoleBaseModel.get_one_object(VIEWER_ROLE)
+        before_permissions = PermissionViewRoleModel.get_all_objects()
+        role = RoleModel.get_one_object(VIEWER_ROLE)
         role.delete()
-        after_permissions = PermissionViewRoleBaseModel.get_all_objects()
+        after_permissions = PermissionViewRoleModel.get_all_objects()
         self.assertNotEqual(before_permissions, after_permissions)
 
     def test_permission_action_cascade_deletion(self):
-        before_permissions = PermissionViewRoleBaseModel.get_all_objects()
-        action = ActionBaseModel.get_one_object(GET_ACTION)
+        before_permissions = PermissionViewRoleModel.get_all_objects()
+        action = ActionModel.get_one_object(GET_ACTION)
         action.delete()
-        after_permissions = PermissionViewRoleBaseModel.get_all_objects()
+        after_permissions = PermissionViewRoleModel.get_all_objects()
         self.assertNotEqual(before_permissions, after_permissions)
 
     def test_permission_api_view_cascade_deletion(self):
-        before_permissions = PermissionViewRoleBaseModel.get_all_objects()
-        api_view = ViewBaseModel.get_one_by_name("instance")
+        before_permissions = PermissionViewRoleModel.get_all_objects()
+        api_view = ViewModel.get_one_by_name("instance")
         api_view.delete()
-        after_permissions = PermissionViewRoleBaseModel.get_all_objects()
+        after_permissions = PermissionViewRoleModel.get_all_objects()
         self.assertNotEqual(before_permissions, after_permissions)
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_roles.py` & `cornflow-1.0.5/cornflow/tests/unit/test_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Unit test for the role endpoints
 """
 import json
 import logging as log
-from cornflow_core.models import PermissionViewRoleBaseModel, RoleBaseModel
+from cornflow.models import PermissionViewRoleModel, RoleModel
 
 # Import from internal modules
 from cornflow.endpoints import (
     RoleDetailEndpoint,
     RolesListEndpoint,
     UserRoleListEndpoint,
     UserRoleDetailEndpoint,
@@ -28,15 +28,15 @@
 
 class TestRolesListEndpoint(CustomTestCase):
     def setUp(self):
         super().setUp()
         self.payload = {"name": "new_role"}
         self.payloads = [{"id": key, "name": value} for key, value in ROLES_MAP.items()]
         self.url = ROLES_URL
-        self.model = RoleBaseModel
+        self.model = RoleModel
         self.items_to_check = ["name"]
         self.roles_with_access = RolesListEndpoint.ROLES_WITH_ACCESS
 
     def tearDown(self):
         super().tearDown()
 
     def test_get_roles_authorized_user(self):
@@ -111,15 +111,15 @@
                 )
 
 
 class TestRolesDetailEndpoint(CustomTestCase):
     def setUp(self):
         super().setUp()
         self.url = ROLES_URL
-        self.model = RoleBaseModel
+        self.model = RoleModel
         self.items_to_check = ["id", "name"]
         self.roles_with_access = RoleDetailEndpoint.ROLES_WITH_ACCESS
 
     def test_get_one_role_authorized_user(self):
         for role in self.roles_with_access:
             token = self.create_user_with_role(role)
 
@@ -423,15 +423,15 @@
         self.assertEqual(all_roles, [])
 
 
 class TestRolesModelMethods(CustomTestCase):
     def setUp(self):
         super().setUp()
         self.url = ROLES_URL
-        self.model = RoleBaseModel
+        self.model = RoleModel
         self.payload = {"name": "test_role"}
 
     def test_user_role_delete_cascade(self):
         payload = {"user_id": self.user}
         self.token = self.create_user_with_role(ADMIN_ROLE)
         self.cascade_delete(
             self.url,
@@ -443,26 +443,26 @@
             "role_id",
         )
 
     def test_permission_delete_cascade(self):
         self.token = self.create_user_with_role(ADMIN_ROLE)
         idx = self.create_new_row(self.url, self.model, self.payload)
         payload = {"action_id": 1, "api_view_id": 1, "role_id": idx}
-        PermissionViewRoleBaseModel(payload).save()
+        PermissionViewRoleModel(payload).save()
 
         role = self.model.query.get(idx)
-        permission = PermissionViewRoleBaseModel.query.filter_by(role_id=idx).first()
+        permission = PermissionViewRoleModel.query.filter_by(role_id=idx).first()
 
         self.assertIsNotNone(role)
         self.assertIsNotNone(permission)
 
         role.delete()
 
         role = self.model.query.get(idx)
-        permission = PermissionViewRoleBaseModel.query.filter_by(role_id=idx).first()
+        permission = PermissionViewRoleModel.query.filter_by(role_id=idx).first()
 
         self.assertIsNone(role)
         self.assertIsNone(permission)
 
     def test_repr_method(self):
         self.token = self.create_user_with_role(ADMIN_ROLE)
         idx = self.create_new_row(self.url, self.model, self.payload)
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_schemas.py` & `cornflow-1.0.5/cornflow/tests/unit/test_schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_sign_up.py` & `cornflow-1.0.5/cornflow/tests/unit/test_sign_up.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from flask_testing import TestCase
 import json
 
 # Import from internal modules
 from cornflow.app import create_app
 from cornflow.models import UserModel, UserRoleModel
 from cornflow.shared.const import PLANNER_ROLE
-from cornflow_core.shared import db
+from cornflow.shared import db
 from cornflow.tests.const import SIGNUP_URL
 
 
 class TestSignUp(TestCase):
     def create_app(self):
         app = create_app("testing")
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_tables.py` & `cornflow-1.0.5/cornflow/tests/unit/test_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # Import from libraries
 import json
 from flask_testing import TestCase
 
 # Import from internal modules
 from cornflow.app import create_app
 from cornflow.commands.access import access_init_command
+from cornflow.models import UserRoleModel
+from cornflow.shared import db
 from cornflow.shared.const import ADMIN_ROLE, SERVICE_ROLE
-from cornflow.models import UserModel, UserRoleModel
-from cornflow_core.shared import db
 from cornflow.tests.const import LOGIN_URL, SIGNUP_URL, TABLES_URL
 
 
 class TestTablesListEndpoint(TestCase):
     def create_app(self):
         app = create_app("testing")
         return app
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_token.py` & `cornflow-1.0.5/cornflow/tests/unit/test_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Import from libraries
 from flask import current_app
 import json
 
 # Import from internal modules
 from cornflow.models import UserModel
-from cornflow_core.shared import db
+from cornflow.shared import db
 from cornflow.tests.custom_test_case import CheckTokenTestCase
 from cornflow.tests.const import LOGIN_URL
 
 
 class TestCheckToken(CheckTokenTestCase.TokenEndpoint):
     def setUp(self):
         super().setUp()
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/test_users.py` & `cornflow-1.0.5/cornflow/tests/unit/test_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     InstanceModel,
     PermissionsDAG,
     UserModel,
     UserRoleModel,
 )
 
 from cornflow.shared.const import ADMIN_ROLE, PLANNER_ROLE, SERVICE_ROLE, VIEWER_ROLE
-from cornflow_core.shared import db
+from cornflow.shared import db
 from cornflow.tests.const import (
     CASE_PATH,
     CASE_URL,
     EXECUTION_PATH,
     EXECUTION_URL_NORUN,
     INSTANCE_PATH,
     INSTANCE_URL,
```

### Comparing `cornflow-1.0.4/cornflow/tests/unit/tools.py` & `cornflow-1.0.5/cornflow/tests/unit/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.4/cornflow.egg-info/PKG-INFO` & `cornflow-1.0.5/cornflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cornflow
-Version: 1.0.4
+Version: 1.0.5
 Summary: Cornflow is an open source multi-solver optimization server with a REST API built using flask.
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: cornflow@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow
         =========
```

### Comparing `cornflow-1.0.4/cornflow.egg-info/SOURCES.txt` & `cornflow-1.0.5/cornflow.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,18 +19,26 @@
 cornflow/cli/__init__.py
 cornflow/cli/actions.py
 cornflow/cli/arguments.py
 cornflow/cli/config.py
 cornflow/cli/migrations.py
 cornflow/cli/permissions.py
 cornflow/cli/roles.py
+cornflow/cli/schemas.py
 cornflow/cli/service.py
 cornflow/cli/users.py
 cornflow/cli/utils.py
 cornflow/cli/views.py
+cornflow/cli/tools/__init__.py
+cornflow/cli/tools/api_generator.py
+cornflow/cli/tools/endpoint_tools.py
+cornflow/cli/tools/models_tools.py
+cornflow/cli/tools/schema_generator.py
+cornflow/cli/tools/schemas_tools.py
+cornflow/cli/tools/tools.py
 cornflow/commands/__init__.py
 cornflow/commands/access.py
 cornflow/commands/actions.py
 cornflow/commands/cleanup.py
 cornflow/commands/dag.py
 cornflow/commands/permissions.py
 cornflow/commands/roles.py
@@ -47,14 +55,15 @@
 cornflow/endpoints/example_data.py
 cornflow/endpoints/execution.py
 cornflow/endpoints/health.py
 cornflow/endpoints/instance.py
 cornflow/endpoints/licenses.py
 cornflow/endpoints/login.py
 cornflow/endpoints/main_alarms.py
+cornflow/endpoints/meta_resource.py
 cornflow/endpoints/permission.py
 cornflow/endpoints/roles.py
 cornflow/endpoints/schemas.py
 cornflow/endpoints/signup.py
 cornflow/endpoints/tables.py
 cornflow/endpoints/token.py
 cornflow/endpoints/user.py
@@ -74,47 +83,66 @@
 cornflow/migrations/versions/d0e0700dcd8e_.py
 cornflow/migrations/versions/d1b5be1f0549_.py
 cornflow/migrations/versions/e1a50dae1ac9_.py
 cornflow/migrations/versions/e937a5234ce4_.py
 cornflow/migrations/versions/ebdd955fcc5e_.py
 cornflow/migrations/versions/f3bee20314a2_.py
 cornflow/models/__init__.py
+cornflow/models/action.py
 cornflow/models/alarms.py
 cornflow/models/base_data_model.py
 cornflow/models/case.py
 cornflow/models/dag.py
 cornflow/models/dag_permissions.py
 cornflow/models/execution.py
 cornflow/models/instance.py
 cornflow/models/main_alarms.py
+cornflow/models/meta_models.py
+cornflow/models/permissions.py
+cornflow/models/role.py
 cornflow/models/user.py
 cornflow/models/user_role.py
+cornflow/models/view.py
 cornflow/schemas/__init__.py
+cornflow/schemas/action.py
 cornflow/schemas/alarms.py
 cornflow/schemas/case.py
 cornflow/schemas/common.py
 cornflow/schemas/dag.py
 cornflow/schemas/example_data.py
 cornflow/schemas/execution.py
 cornflow/schemas/health.py
 cornflow/schemas/instance.py
 cornflow/schemas/main_alarms.py
 cornflow/schemas/model_json.py
+cornflow/schemas/patch.py
+cornflow/schemas/permissions.py
+cornflow/schemas/query.py
+cornflow/schemas/role.py
 cornflow/schemas/schemas.py
 cornflow/schemas/solution_log.py
 cornflow/schemas/tables.py
 cornflow/schemas/user.py
+cornflow/schemas/user_role.py
+cornflow/schemas/view.py
 cornflow/shared/__init__.py
-cornflow/shared/authentication.py
+cornflow/shared/compress.py
 cornflow/shared/const.py
+cornflow/shared/email.py
+cornflow/shared/exceptions.py
 cornflow/shared/licenses.py
 cornflow/shared/log_config.py
 cornflow/shared/query_tools.py
 cornflow/shared/utils.py
 cornflow/shared/utils_tables.py
+cornflow/shared/validators.py
+cornflow/shared/authentication/__init__.py
+cornflow/shared/authentication/auth.py
+cornflow/shared/authentication/decorators.py
+cornflow/shared/authentication/ldap.py
 cornflow/tests/__init__.py
 cornflow/tests/const.py
 cornflow/tests/custom_liveServer.py
 cornflow/tests/custom_test_case.py
 cornflow/tests/integration/__init__.py
 cornflow/tests/integration/test_commands.py
 cornflow/tests/integration/test_cornflowclient.py
@@ -127,20 +155,22 @@
 cornflow/tests/unit/test_cases.py
 cornflow/tests/unit/test_cli.py
 cornflow/tests/unit/test_commands.py
 cornflow/tests/unit/test_dags.py
 cornflow/tests/unit/test_data_checks.py
 cornflow/tests/unit/test_example_data.py
 cornflow/tests/unit/test_executions.py
+cornflow/tests/unit/test_generate_from_schema.py
 cornflow/tests/unit/test_health.py
 cornflow/tests/unit/test_instances.py
 cornflow/tests/unit/test_instances_file.py
 cornflow/tests/unit/test_log_in.py
 cornflow/tests/unit/test_main_alarms.py
 cornflow/tests/unit/test_permissions.py
 cornflow/tests/unit/test_roles.py
+cornflow/tests/unit/test_schema_from_models.py
 cornflow/tests/unit/test_schemas.py
 cornflow/tests/unit/test_sign_up.py
 cornflow/tests/unit/test_tables.py
 cornflow/tests/unit/test_token.py
 cornflow/tests/unit/test_users.py
 cornflow/tests/unit/tools.py
```

### Comparing `cornflow-1.0.4/setup.py` & `cornflow-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 required = []
 with open("requirements.txt", "r") as fh:
     required.append(fh.read().splitlines())
 
 setuptools.setup(
     name="cornflow",
-    version="1.0.4",
+    version="1.0.5",
     author="baobab soluciones",
     author_email="cornflow@baobabsoluciones.es",
     description="Cornflow is an open source multi-solver optimization server with a REST API built using flask.",
     long_description=long_description,
     url="https://github.com/baobabsoluciones/cornflow",
     packages=setuptools.find_packages(),
     install_requires=required,
```

