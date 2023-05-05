# Comparing `tmp/skbase-0.4.2.tar.gz` & `tmp/skbase-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skbase-0.4.2.tar", last modified: Tue May  2 20:55:49 2023, max compression
+gzip compressed data, was "skbase-0.4.3.tar", last modified: Fri May  5 00:37:28 2023, max compression
```

## Comparing `skbase-0.4.2.tar` & `skbase-0.4.3.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-05-02 20:55:32.000000 skbase-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-02 20:55:49.979898 skbase-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-02 20:55:32.000000 skbase-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.971898 skbase-0.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-05-02 20:55:32.000000 skbase-0.4.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-02 20:55:32.000000 skbase-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-02 20:55:49.979898 skbase-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43633 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/base/_pretty_printing/
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_pretty_printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_pretty_printing/_object_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_pretty_printing/_pprint.py
--rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_tagmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38936 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36450 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/testing/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/tests/test_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7762 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (122)    41672 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/test_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14777 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    12123 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/validate/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/tests/test_iterable_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/tests/test_type_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.397496 skbase-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-05-05 00:37:14.000000 skbase-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-05 00:37:28.397496 skbase-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-05 00:37:14.000000 skbase-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.377496 skbase-0.4.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.381496 skbase-0.4.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-05-05 00:37:14.000000 skbase-0.4.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-05 00:37:14.000000 skbase-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-05 00:37:28.397496 skbase-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.381496 skbase-0.4.3/skbase/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/_nopytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43634 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase/base/_pretty_printing/
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_pretty_printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_pretty_printing/_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_tagmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase/lookup/
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38936 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/lookup/_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase/lookup/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/lookup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/lookup/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.389496 skbase-0.4.3/skbase/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36450 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/test_all_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.389496 skbase-0.4.3/skbase/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/_conditional_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.389496 skbase-0.4.3/skbase/testing/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/tests/test_deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.393496 skbase-0.4.3/skbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7792 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.393496 skbase-0.4.3/skbase/tests/mock_package/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/mock_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/mock_package/test_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41827 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/test_baseestimator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.393496 skbase-0.4.3/skbase/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.393496 skbase-0.4.3/skbase/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/test_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.397496 skbase-0.4.3/skbase/validate/
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14777 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12121 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.397496 skbase-0.4.3/skbase/validate/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/tests/test_iterable_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/tests/test_type_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/zip-safe
```

### Comparing `skbase-0.4.2/LICENSE` & `skbase-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/PKG-INFO` & `skbase-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.2
+Version: 0.4.3
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
@@ -69,15 +69,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.2 is now available. Checkout our
+:rocket: Version 0.4.3 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `skbase-0.4.2/README.md` & `skbase-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.2 is now available. Checkout our
+:rocket: Version 0.4.3 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `skbase-0.4.2/docs/source/conf.py` & `skbase-0.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/pyproject.toml` & `skbase-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "skbase"
-version = "0.4.2"
+version = "0.4.3"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
     {name = "Franz Király"},
     {name = "Markus Löning"},
     {name = "Ryan Kuhns"},
 ]
 maintainers = [
```

### Comparing `skbase-0.4.2/skbase/_exceptions.py` & `skbase-0.4.3/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/base/__init__.py` & `skbase-0.4.3/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/base/_base.py` & `skbase-0.4.3/skbase/base/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     Extends scikit-learn's BaseEstimator to include sktime style interface for tags.
     """
 
     _config = {
         "display": "diagram",
         "print_changed_only": True,
-        "check_clone": True,  # whether to execute validity checks in clone
+        "check_clone": False,  # whether to execute validity checks in clone
     }
 
     def __init__(self):
         """Construct BaseObject."""
         self._init_flags(flag_attr_name="_tags")
         self._init_flags(flag_attr_name="_config")
         super(BaseObject, self).__init__()
```

### Comparing `skbase-0.4.2/skbase/base/_meta.py` & `skbase-0.4.3/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/base/_pretty_printing/_object_html_repr.py` & `skbase-0.4.3/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/base/_pretty_printing/_pprint.py` & `skbase-0.4.3/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/base/_tagmanager.py` & `skbase-0.4.3/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/lookup/__init__.py` & `skbase-0.4.3/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/lookup/_lookup.py` & `skbase-0.4.3/skbase/lookup/_lookup.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/lookup/tests/test_lookup.py` & `skbase-0.4.3/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/testing/test_all_objects.py` & `skbase-0.4.3/skbase/testing/test_all_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/testing/utils/_conditional_fixtures.py` & `skbase-0.4.3/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/testing/utils/_dependencies.py` & `skbase-0.4.3/skbase/testing/utils/_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/testing/utils/deep_equals.py` & `skbase-0.4.3/skbase/testing/utils/deep_equals.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/testing/utils/inspect.py` & `skbase-0.4.3/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/testing/utils/tests/test_check_dependencies.py` & `skbase-0.4.3/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/testing/utils/tests/test_deep_equals.py` & `skbase-0.4.3/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/tests/conftest.py` & `skbase-0.4.3/skbase/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ]
 __author__: List[str] = ["fkiraly", "RNKuhns"]
 
 SKBASE_BASE_CLASSES = (BaseObject, BaseEstimator)
 SKBASE_MODULES = (
     "skbase",
     "skbase._exceptions",
+    "skbase._nopytest_tests",
     "skbase.base",
     "skbase.base._base",
     "skbase.base._meta",
     "skbase.base._pretty_printing",
     "skbase.base._pretty_printing._object_html_repr",
     "skbase.base._pretty_printing._pprint",
     "skbase.base._tagmanager",
```

### Comparing `skbase-0.4.2/skbase/tests/mock_package/test_mock_package.py` & `skbase-0.4.3/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/tests/test_base.py` & `skbase-0.4.3/skbase/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -809,27 +809,30 @@
 def test_clone_raises_error_for_nonconforming_objects(
     fixture_invalid_init: Type[InvalidInitSignatureTester],
     fixture_buggy: Type[Buggy],
     fixture_modify_param: Type[ModifyParam],
 ):
     """Test that clone raises an error on nonconforming BaseObjects."""
     buggy = fixture_buggy()
+    buggy.set_config(**{"check_clone": True})
     buggy.a = 2
     with pytest.raises(RuntimeError):
         buggy.clone()
 
     varg_obj = fixture_invalid_init(a=7)
+    varg_obj.set_config(**{"check_clone": True})
     with pytest.raises(RuntimeError):
         varg_obj.clone()
 
     # fkiraly note: I don't think this class violates the contract,
     # as equality is defined as via deepcopy
     # leaving the code here for reference and potential discussion
     #
     # obj_that_modifies = fixture_modify_param(a=[0])
+    # obj_that_modifies.set_config(**{"check_clone": True})
     # with pytest.raises(RuntimeError):
     #     obj_that_modifies.clone()
 
 
 @pytest.mark.skipif(
     not _check_soft_dependencies("sklearn", severity="none"),
     reason="skip test if sklearn is not available",
```

### Comparing `skbase-0.4.2/skbase/tests/test_baseestimator.py` & `skbase-0.4.3/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/tests/test_exceptions.py` & `skbase-0.4.3/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/tests/test_meta.py` & `skbase-0.4.3/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/utils/__init__.py` & `skbase-0.4.3/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/utils/_check.py` & `skbase-0.4.3/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/utils/_iter.py` & `skbase-0.4.3/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/utils/_nested_iter.py` & `skbase-0.4.3/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/utils/_utils.py` & `skbase-0.4.3/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/utils/tests/test_check.py` & `skbase-0.4.3/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/utils/tests/test_iter.py` & `skbase-0.4.3/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/utils/tests/test_nested_iter.py` & `skbase-0.4.3/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/utils/tests/test_utils.py` & `skbase-0.4.3/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/validate/__init__.py` & `skbase-0.4.3/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/validate/_named_objects.py` & `skbase-0.4.3/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/validate/_types.py` & `skbase-0.4.3/skbase/validate/_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     is_valid_sequence = isinstance(input_seq, sequence_type_)
 
     # Optionally verify elements have correct types
     if element_type is not None:
         element_type_ = _convert_scalar_seq_type_input_to_tuple(
             element_type, input_name="element_type"
         )
-        element_types_okay = all([isinstance(e, element_type_) for e in input_seq])
+        element_types_okay = all(isinstance(e, element_type_) for e in input_seq)
         if not element_types_okay:
             is_valid_sequence = False
 
     return is_valid_sequence
 
 
 def check_sequence(
```

### Comparing `skbase-0.4.2/skbase/validate/tests/test_iterable_named_objects.py` & `skbase-0.4.3/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase/validate/tests/test_type_validations.py` & `skbase-0.4.3/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.2/skbase.egg-info/PKG-INFO` & `skbase-0.4.3/skbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.2
+Version: 0.4.3
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
@@ -69,15 +69,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.2 is now available. Checkout our
+:rocket: Version 0.4.3 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `skbase-0.4.2/skbase.egg-info/SOURCES.txt` & `skbase-0.4.3/skbase.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 docs/source/conf.py
 skbase/__init__.py
 skbase/_exceptions.py
+skbase/_nopytest_tests.py
 skbase.egg-info/PKG-INFO
 skbase.egg-info/SOURCES.txt
 skbase.egg-info/dependency_links.txt
 skbase.egg-info/requires.txt
 skbase.egg-info/top_level.txt
 skbase.egg-info/zip-safe
 skbase/base/__init__.py
```

### Comparing `skbase-0.4.2/skbase.egg-info/requires.txt` & `skbase-0.4.3/skbase.egg-info/requires.txt`

 * *Files identical despite different names*

