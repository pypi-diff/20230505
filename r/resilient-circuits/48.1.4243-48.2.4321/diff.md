# Comparing `tmp/resilient_circuits-48.1.4243.tar.gz` & `tmp/resilient_circuits-48.2.4321.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_circuits-48.1.4243.tar", last modified: Thu Apr 20 19:35:25 2023, max compression
+gzip compressed data, was "resilient_circuits-48.2.4321.tar", last modified: Fri May  5 12:35:11 2023, max compression
```

## Comparing `resilient_circuits-48.1.4243.tar` & `resilient_circuits-48.2.4321.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12364 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.011501 resilient_circuits-48.1.4243/resilient_circuits/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/README
--rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15525 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/action_message.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    59349 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/actions_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/actions_test_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    10353 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11847 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/app_argument_parser.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6029 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/app_function_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7793 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/app_restartable.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/bin/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/bin/res_action_test.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    17085 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/bin/resilient_circuits_cmd.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2996 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/bin/service_wrapper.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits/cmds/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13670 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/cmds/selftest.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2755 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits/data/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3063 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/data/app.config.base
--rwxrwxr-x   0 travis    (2000) travis    (2000)    20046 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11921 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/helpers.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/keyring_arguments.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3395 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/rest_helper.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    14446 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/stomp_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/stomp_events.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/stomp_transport.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/template_functions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/util/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/util/resilient_config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/util/resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1128 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/resilient_circuits/validate_configs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/resilient_circuits.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2581 2023-04-20 19:35:25.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-04-20 19:35:24.000000 resilient_circuits-48.1.4243/resilient_circuits.egg-info/top_level.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1511 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      287 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.015501 resilient_circuits-48.1.4243/tests/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/cmds/test_selftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3803 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/tests/selftest_tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/selftest_tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/selftest_tests/mocked_fail_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/selftest_tests/mocked_success_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      282 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/selftest_tests/mocked_unimplemented_script.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_commented_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_import_definition.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      545 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_action_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_actions_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4280 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_app_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1663 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_app_restartable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7756 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7974 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_resilient_circuits_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_rest_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_stomp_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:25.019501 resilient_circuits-48.1.4243/tests/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tests/util/test_resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2023-04-20 19:34:28.000000 resilient_circuits-48.1.4243/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12364 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-05-05 12:35:11.447470 resilient_circuits-48.2.4321/PKG-INFO
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.439470 resilient_circuits-48.2.4321/resilient_circuits/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/LICENSE
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/README
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    15525 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/action_message.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    59349 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/actions_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/actions_test_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    10353 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11847 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/app_argument_parser.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6029 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/app_function_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7793 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/app_restartable.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.439470 resilient_circuits-48.2.4321/resilient_circuits/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/bin/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/bin/res_action_test.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    17085 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/bin/resilient_circuits_cmd.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2996 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/bin/service_wrapper.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.439470 resilient_circuits-48.2.4321/resilient_circuits/cmds/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13670 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/cmds/selftest.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2755 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/resilient_circuits/data/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3063 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/data/app.config.base
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    20046 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11921 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/helpers.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/keyring_arguments.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3395 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/rest_helper.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    14446 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/stomp_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/stomp_events.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/stomp_transport.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/template_functions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/resilient_circuits/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/util/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/util/resilient_config.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/util/resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1128 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/resilient_circuits/validate_configs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.439470 resilient_circuits-48.2.4321/resilient_circuits.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2581 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      176 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-05-05 12:35:11.000000 resilient_circuits-48.2.4321/resilient_circuits.egg-info/top_level.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1511 2023-05-05 12:35:11.447470 resilient_circuits-48.2.4321/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      287 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/cmds/test_selftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3803 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/selftest_tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/selftest_tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/selftest_tests/mocked_fail_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/selftest_tests/mocked_success_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      282 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/selftest_tests/mocked_unimplemented_script.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_commented_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_import_definition.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      545 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_action_message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_actions_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4280 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_app_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1663 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_app_restartable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7756 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7974 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_resilient_circuits_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_rest_helper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_stomp_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:11.443470 resilient_circuits-48.2.4321/tests/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tests/util/test_resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2023-05-05 12:33:36.000000 resilient_circuits-48.2.4321/tox.ini
```

### Comparing `resilient_circuits-48.1.4243/CHANGES` & `resilient_circuits-48.2.4321/CHANGES`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/PKG-INFO` & `resilient_circuits-48.2.4321/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_circuits
-Version: 48.1.4243
+Version: 48.2.4321
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-48.1.4243/README.md` & `resilient_circuits-48.2.4321/README.md`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/LICENSE` & `resilient_circuits-48.2.4321/resilient_circuits/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/__init__.py` & `resilient_circuits-48.2.4321/resilient_circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/action_message.py` & `resilient_circuits-48.2.4321/resilient_circuits/action_message.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/actions_component.py` & `resilient_circuits-48.2.4321/resilient_circuits/actions_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/actions_test_component.py` & `resilient_circuits-48.2.4321/resilient_circuits/actions_test_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/app.py` & `resilient_circuits-48.2.4321/resilient_circuits/app.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/app_argument_parser.py` & `resilient_circuits-48.2.4321/resilient_circuits/app_argument_parser.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/app_function_component.py` & `resilient_circuits-48.2.4321/resilient_circuits/app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/app_restartable.py` & `resilient_circuits-48.2.4321/resilient_circuits/app_restartable.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/bin/res_action_test.py` & `resilient_circuits-48.2.4321/resilient_circuits/bin/res_action_test.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/bin/resilient_circuits_cmd.py` & `resilient_circuits-48.2.4321/resilient_circuits/bin/resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/bin/service_wrapper.py` & `resilient_circuits-48.2.4321/resilient_circuits/bin/service_wrapper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/cmds/selftest.py` & `resilient_circuits-48.2.4321/resilient_circuits/cmds/selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/component_loader.py` & `resilient_circuits-48.2.4321/resilient_circuits/component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/constants.py` & `resilient_circuits-48.2.4321/resilient_circuits/constants.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/data/app.config.base` & `resilient_circuits-48.2.4321/resilient_circuits/data/app.config.base`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/decorators.py` & `resilient_circuits-48.2.4321/resilient_circuits/decorators.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/helpers.py` & `resilient_circuits-48.2.4321/resilient_circuits/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/rest_helper.py` & `resilient_circuits-48.2.4321/resilient_circuits/rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/stomp_component.py` & `resilient_circuits-48.2.4321/resilient_circuits/stomp_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/stomp_events.py` & `resilient_circuits-48.2.4321/resilient_circuits/stomp_events.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/stomp_transport.py` & `resilient_circuits-48.2.4321/resilient_circuits/stomp_transport.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/template_functions.py` & `resilient_circuits-48.2.4321/resilient_circuits/template_functions.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/util/__init__.py` & `resilient_circuits-48.2.4321/resilient_circuits/util/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/util/resilient_config.py` & `resilient_circuits-48.2.4321/resilient_circuits/util/resilient_config.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/util/resilient_customize.py` & `resilient_circuits-48.2.4321/resilient_circuits/util/resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits/validate_configs.py` & `resilient_circuits-48.2.4321/resilient_circuits/validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/resilient_circuits.egg-info/PKG-INFO` & `resilient_circuits-48.2.4321/resilient_circuits.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-circuits
-Version: 48.1.4243
+Version: 48.2.4321
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-48.1.4243/resilient_circuits.egg-info/SOURCES.txt` & `resilient_circuits-48.2.4321/resilient_circuits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/setup.cfg` & `resilient_circuits-48.2.4321/setup.cfg`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/cmds/test_selftest.py` & `resilient_circuits-48.2.4321/tests/cmds/test_selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/conftest.py` & `resilient_circuits-48.2.4321/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/helpers.py` & `resilient_circuits-48.2.4321/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_app_config` & `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_app_config`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_app_function_component.py` & `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_commented_app_config` & `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_commented_app_config`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_component.py` & `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_constants.py` & `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_constants.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_function_component.py` & `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_import_definition.txt` & `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_import_definition.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/shared_mock_data/mock_paths.py` & `resilient_circuits-48.2.4321/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_action_message.py` & `resilient_circuits-48.2.4321/tests/test_action_message.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_actions_component.py` & `resilient_circuits-48.2.4321/tests/test_actions_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_app_config.py` & `resilient_circuits-48.2.4321/tests/test_app_config.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_app_function_component.py` & `resilient_circuits-48.2.4321/tests/test_app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_app_restartable.py` & `resilient_circuits-48.2.4321/tests/test_app_restartable.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_component_loader.py` & `resilient_circuits-48.2.4321/tests/test_component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_decorators.py` & `resilient_circuits-48.2.4321/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_errors.py` & `resilient_circuits-48.2.4321/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_helpers.py` & `resilient_circuits-48.2.4321/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_resilient_circuits_cmd.py` & `resilient_circuits-48.2.4321/tests/test_resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_rest_helper.py` & `resilient_circuits-48.2.4321/tests/test_rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_stomp_component.py` & `resilient_circuits-48.2.4321/tests/test_stomp_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/test_templates.py` & `resilient_circuits-48.2.4321/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tests/util/test_resilient_customize.py` & `resilient_circuits-48.2.4321/tests/util/test_resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-48.1.4243/tox.ini` & `resilient_circuits-48.2.4321/tox.ini`

 * *Files identical despite different names*

