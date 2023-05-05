# Comparing `tmp/scikit-base-0.4.2.tar.gz` & `tmp/scikit-base-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-base-0.4.2.tar", last modified: Tue May  2 20:54:45 2023, max compression
+gzip compressed data, was "scikit-base-0.4.3.tar", last modified: Fri May  5 00:38:57 2023, max compression
```

## Comparing `scikit-base-0.4.2.tar` & `scikit-base-0.4.3.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:45.114337 scikit-base-0.4.2/
--rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     6614 2023-05-02 20:54:45.115336 scikit-base-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2023-05-02 05:32:01.000000 scikit-base-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.232086 scikit-base-0.4.2/docs/
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.568015 scikit-base-0.4.2/docs/source/
--rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 scikit-base-0.4.2/docs/source/conf.py
--rw-rw-rw-   0        0        0     3468 2023-05-02 20:54:07.000000 scikit-base-0.4.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.662365 scikit-base-0.4.2/scikit_base.egg-info/
--rw-rw-rw-   0        0        0     6614 2023-05-02 20:54:44.000000 scikit-base-0.4.2/scikit_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1802 2023-05-02 20:54:44.000000 scikit-base-0.4.2/scikit_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 20:54:44.000000 scikit-base-0.4.2/scikit_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      517 2023-05-02 20:54:44.000000 scikit-base-0.4.2/scikit_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2023-05-02 20:54:44.000000 scikit-base-0.4.2/scikit_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.4.2/scikit_base.egg-info/zip-safe
--rw-rw-rw-   0        0        0      368 2023-05-02 20:54:45.125028 scikit-base-0.4.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.662365 scikit-base-0.4.2/skbase/
--rw-rw-rw-   0        0        0      468 2023-04-25 09:18:44.000000 scikit-base-0.4.2/skbase/__init__.py
--rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.4.2/skbase/_exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.709237 scikit-base-0.4.2/skbase/base/
--rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/base/__init__.py
--rw-rw-rw-   0        0        0    44811 2023-05-02 00:24:16.000000 scikit-base-0.4.2/skbase/base/_base.py
--rw-rw-rw-   0        0        0    36497 2023-04-26 13:58:57.000000 scikit-base-0.4.2/skbase/base/_meta.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.756782 scikit-base-0.4.2/skbase/base/_pretty_printing/
--rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/base/_pretty_printing/__init__.py
--rw-rw-rw-   0        0        0    11931 2023-04-26 13:58:57.000000 scikit-base-0.4.2/skbase/base/_pretty_printing/_object_html_repr.py
--rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 scikit-base-0.4.2/skbase/base/_pretty_printing/_pprint.py
--rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/base/_tagmanager.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.772435 scikit-base-0.4.2/skbase/lookup/
--rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.4.2/skbase/lookup/__init__.py
--rw-rw-rw-   0        0        0    39934 2023-05-01 22:18:40.000000 scikit-base-0.4.2/skbase/lookup/_lookup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.803686 scikit-base-0.4.2/skbase/lookup/tests/
--rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.4.2/skbase/lookup/tests/__init__.py
--rw-rw-rw-   0        0        0    37915 2023-04-26 14:48:09.000000 scikit-base-0.4.2/skbase/lookup/tests/test_lookup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.819233 scikit-base-0.4.2/skbase/testing/
--rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.4.2/skbase/testing/__init__.py
--rw-rw-rw-   0        0        0    37306 2023-05-02 00:24:16.000000 scikit-base-0.4.2/skbase/testing/test_all_objects.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.851007 scikit-base-0.4.2/skbase/testing/utils/
--rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.4.2/skbase/testing/utils/__init__.py
--rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/testing/utils/_conditional_fixtures.py
--rw-rw-rw-   0        0        0    10612 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/testing/utils/_dependencies.py
--rw-rw-rw-   0        0        0    11410 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/testing/utils/deep_equals.py
--rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.4.2/skbase/testing/utils/inspect.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.866546 scikit-base-0.4.2/skbase/testing/utils/tests/
--rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.4.2/skbase/testing/utils/tests/__init__.py
--rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.4.2/skbase/testing/utils/tests/test_check_dependencies.py
--rw-rw-rw-   0        0        0     1779 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/testing/utils/tests/test_deep_equals.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.953799 scikit-base-0.4.2/skbase/tests/
--rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.4.2/skbase/tests/__init__.py
--rw-rw-rw-   0        0        0     8017 2023-05-01 22:18:40.000000 scikit-base-0.4.2/skbase/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:44.984035 scikit-base-0.4.2/skbase/tests/mock_package/
--rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.4.2/skbase/tests/mock_package/__init__.py
--rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.4.2/skbase/tests/mock_package/test_mock_package.py
--rw-rw-rw-   0        0        0    42855 2023-05-02 00:24:16.000000 scikit-base-0.4.2/skbase/tests/test_base.py
--rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/tests/test_baseestimator.py
--rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.4.2/skbase/tests/test_exceptions.py
--rw-rw-rw-   0        0        0     4567 2023-05-02 00:24:16.000000 scikit-base-0.4.2/skbase/tests/test_meta.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:45.062543 scikit-base-0.4.2/skbase/utils/
--rw-rw-rw-   0        0        0      584 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/_check.py
--rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/_iter.py
--rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/_nested_iter.py
--rw-rw-rw-   0        0        0     3225 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:45.084067 scikit-base-0.4.2/skbase/utils/tests/
--rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/tests/__init__.py
--rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/tests/test_check.py
--rw-rw-rw-   0        0        0     5045 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/tests/test_iter.py
--rw-rw-rw-   0        0        0     2314 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/tests/test_nested_iter.py
--rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/utils/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:45.108373 scikit-base-0.4.2/skbase/validate/
--rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/validate/__init__.py
--rw-rw-rw-   0        0        0    15180 2023-05-01 22:18:40.000000 scikit-base-0.4.2/skbase/validate/_named_objects.py
--rw-rw-rw-   0        0        0    12468 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/validate/_types.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:54:45.113350 scikit-base-0.4.2/skbase/validate/tests/
--rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/validate/tests/__init__.py
--rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/validate/tests/test_iterable_named_objects.py
--rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 scikit-base-0.4.2/skbase/validate/tests/test_type_validations.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.679311 scikit-base-0.4.3/
+-rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     6614 2023-05-05 00:38:57.680364 scikit-base-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2023-05-05 00:37:15.000000 scikit-base-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.371288 scikit-base-0.4.3/docs/
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.753497 scikit-base-0.4.3/docs/source/
+-rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 scikit-base-0.4.3/docs/source/conf.py
+-rw-rw-rw-   0        0        0     3468 2023-05-05 00:38:42.000000 scikit-base-0.4.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.851061 scikit-base-0.4.3/scikit_base.egg-info/
+-rw-rw-rw-   0        0        0     6614 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1828 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      517 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.4.3/scikit_base.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      368 2023-05-05 00:38:57.707373 scikit-base-0.4.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.878875 scikit-base-0.4.3/skbase/
+-rw-rw-rw-   0        0        0      468 2023-04-25 09:18:44.000000 scikit-base-0.4.3/skbase/__init__.py
+-rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.4.3/skbase/_exceptions.py
+-rw-rw-rw-   0        0        0      989 2023-05-05 00:37:09.000000 scikit-base-0.4.3/skbase/_nopytest_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.941985 scikit-base-0.4.3/skbase/base/
+-rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/base/__init__.py
+-rw-rw-rw-   0        0        0    44812 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/base/_base.py
+-rw-rw-rw-   0        0        0    36497 2023-04-26 13:58:57.000000 scikit-base-0.4.3/skbase/base/_meta.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.991531 scikit-base-0.4.3/skbase/base/_pretty_printing/
+-rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/base/_pretty_printing/__init__.py
+-rw-rw-rw-   0        0        0    11931 2023-04-26 13:58:57.000000 scikit-base-0.4.3/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 scikit-base-0.4.3/skbase/base/_pretty_printing/_pprint.py
+-rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/base/_tagmanager.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.021323 scikit-base-0.4.3/skbase/lookup/
+-rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.4.3/skbase/lookup/__init__.py
+-rw-rw-rw-   0        0        0    39934 2023-05-01 22:18:40.000000 scikit-base-0.4.3/skbase/lookup/_lookup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.058675 scikit-base-0.4.3/skbase/lookup/tests/
+-rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/lookup/tests/__init__.py
+-rw-rw-rw-   0        0        0    37915 2023-04-26 14:48:09.000000 scikit-base-0.4.3/skbase/lookup/tests/test_lookup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.088424 scikit-base-0.4.3/skbase/testing/
+-rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.4.3/skbase/testing/__init__.py
+-rw-rw-rw-   0        0        0    37306 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/testing/test_all_objects.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.201146 scikit-base-0.4.3/skbase/testing/utils/
+-rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/testing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/testing/utils/_conditional_fixtures.py
+-rw-rw-rw-   0        0        0    10612 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/testing/utils/_dependencies.py
+-rw-rw-rw-   0        0        0    11410 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/testing/utils/deep_equals.py
+-rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.4.3/skbase/testing/utils/inspect.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.261374 scikit-base-0.4.3/skbase/testing/utils/tests/
+-rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.4.3/skbase/testing/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.4.3/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-rw-rw-   0        0        0     1779 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/testing/utils/tests/test_deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.373755 scikit-base-0.4.3/skbase/tests/
+-rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.4.3/skbase/tests/__init__.py
+-rw-rw-rw-   0        0        0     8048 2023-05-05 00:37:09.000000 scikit-base-0.4.3/skbase/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.406154 scikit-base-0.4.3/skbase/tests/mock_package/
+-rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/tests/mock_package/__init__.py
+-rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/tests/mock_package/test_mock_package.py
+-rw-rw-rw-   0        0        0    43013 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/tests/test_base.py
+-rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/tests/test_baseestimator.py
+-rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0     4567 2023-05-02 00:24:16.000000 scikit-base-0.4.3/skbase/tests/test_meta.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.487029 scikit-base-0.4.3/skbase/utils/
+-rw-rw-rw-   0        0        0      584 2023-05-04 16:33:39.000000 scikit-base-0.4.3/skbase/utils/__init__.py
+-rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/_check.py
+-rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/_iter.py
+-rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/_nested_iter.py
+-rw-rw-rw-   0        0        0     3225 2023-05-04 17:40:43.000000 scikit-base-0.4.3/skbase/utils/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.588296 scikit-base-0.4.3/skbase/utils/tests/
+-rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/tests/test_check.py
+-rw-rw-rw-   0        0        0     5045 2023-05-04 17:40:43.000000 scikit-base-0.4.3/skbase/utils/tests/test_iter.py
+-rw-rw-rw-   0        0        0     2314 2023-05-04 17:40:43.000000 scikit-base-0.4.3/skbase/utils/tests/test_nested_iter.py
+-rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.624895 scikit-base-0.4.3/skbase/validate/
+-rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/validate/__init__.py
+-rw-rw-rw-   0        0        0    15180 2023-05-01 22:18:40.000000 scikit-base-0.4.3/skbase/validate/_named_objects.py
+-rw-rw-rw-   0        0        0    12466 2023-05-02 20:58:49.000000 scikit-base-0.4.3/skbase/validate/_types.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.678275 scikit-base-0.4.3/skbase/validate/tests/
+-rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/validate/tests/__init__.py
+-rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/validate/tests/test_iterable_named_objects.py
+-rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/validate/tests/test_type_validations.py
```

### Comparing `scikit-base-0.4.2/LICENSE` & `scikit-base-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/PKG-INFO` & `scikit-base-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
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

### Comparing `scikit-base-0.4.2/README.md` & `scikit-base-0.4.3/README.md`

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

### Comparing `scikit-base-0.4.2/docs/source/conf.py` & `scikit-base-0.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/pyproject.toml` & `scikit-base-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-base"
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

### Comparing `scikit-base-0.4.2/scikit_base.egg-info/PKG-INFO` & `scikit-base-0.4.3/scikit_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
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

### Comparing `scikit-base-0.4.2/scikit_base.egg-info/SOURCES.txt` & `scikit-base-0.4.3/scikit_base.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 scikit_base.egg-info/SOURCES.txt
 scikit_base.egg-info/dependency_links.txt
 scikit_base.egg-info/requires.txt
 scikit_base.egg-info/top_level.txt
 scikit_base.egg-info/zip-safe
 skbase/__init__.py
 skbase/_exceptions.py
+skbase/_nopytest_tests.py
 skbase/base/__init__.py
 skbase/base/_base.py
 skbase/base/_meta.py
 skbase/base/_tagmanager.py
 skbase/base/_pretty_printing/__init__.py
 skbase/base/_pretty_printing/_object_html_repr.py
 skbase/base/_pretty_printing/_pprint.py
```

### Comparing `scikit-base-0.4.2/scikit_base.egg-info/requires.txt` & `scikit-base-0.4.3/scikit_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/_exceptions.py` & `scikit-base-0.4.3/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/base/__init__.py` & `scikit-base-0.4.3/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/base/_base.py` & `scikit-base-0.4.3/skbase/base/_base.py`

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

### Comparing `scikit-base-0.4.2/skbase/base/_meta.py` & `scikit-base-0.4.3/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/base/_pretty_printing/_object_html_repr.py` & `scikit-base-0.4.3/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/base/_pretty_printing/_pprint.py` & `scikit-base-0.4.3/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/base/_tagmanager.py` & `scikit-base-0.4.3/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/lookup/__init__.py` & `scikit-base-0.4.3/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/lookup/_lookup.py` & `scikit-base-0.4.3/skbase/lookup/_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/lookup/tests/test_lookup.py` & `scikit-base-0.4.3/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/testing/test_all_objects.py` & `scikit-base-0.4.3/skbase/testing/test_all_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/testing/utils/_conditional_fixtures.py` & `scikit-base-0.4.3/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/testing/utils/_dependencies.py` & `scikit-base-0.4.3/skbase/testing/utils/_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/testing/utils/deep_equals.py` & `scikit-base-0.4.3/skbase/testing/utils/deep_equals.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/testing/utils/inspect.py` & `scikit-base-0.4.3/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/testing/utils/tests/test_check_dependencies.py` & `scikit-base-0.4.3/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/testing/utils/tests/test_deep_equals.py` & `scikit-base-0.4.3/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/tests/conftest.py` & `scikit-base-0.4.3/skbase/tests/conftest.py`

 * *Files 0% similar despite different names*

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

### Comparing `scikit-base-0.4.2/skbase/tests/mock_package/test_mock_package.py` & `scikit-base-0.4.3/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/tests/test_base.py` & `scikit-base-0.4.3/skbase/tests/test_base.py`

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

### Comparing `scikit-base-0.4.2/skbase/tests/test_baseestimator.py` & `scikit-base-0.4.3/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/tests/test_exceptions.py` & `scikit-base-0.4.3/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/tests/test_meta.py` & `scikit-base-0.4.3/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/utils/__init__.py` & `scikit-base-0.4.3/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/utils/_check.py` & `scikit-base-0.4.3/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/utils/_iter.py` & `scikit-base-0.4.3/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/utils/_nested_iter.py` & `scikit-base-0.4.3/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/utils/_utils.py` & `scikit-base-0.4.3/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/utils/tests/test_check.py` & `scikit-base-0.4.3/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/utils/tests/test_iter.py` & `scikit-base-0.4.3/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/utils/tests/test_nested_iter.py` & `scikit-base-0.4.3/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/utils/tests/test_utils.py` & `scikit-base-0.4.3/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/validate/__init__.py` & `scikit-base-0.4.3/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/validate/_named_objects.py` & `scikit-base-0.4.3/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/validate/_types.py` & `scikit-base-0.4.3/skbase/validate/_types.py`

 * *Files 1% similar despite different names*

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

### Comparing `scikit-base-0.4.2/skbase/validate/tests/test_iterable_named_objects.py` & `scikit-base-0.4.3/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.2/skbase/validate/tests/test_type_validations.py` & `scikit-base-0.4.3/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

