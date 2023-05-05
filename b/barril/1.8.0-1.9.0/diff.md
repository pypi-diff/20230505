# Comparing `tmp/barril-1.8.0.tar.gz` & `tmp/barril-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barril-1.8.0.tar", last modified: Mon Jan 13 12:56:31 2020, max compression
+gzip compressed data, was "dist/barril-1.9.0.tar", last modified: Thu Feb 20 20:19:26 2020, max compression
```

## Comparing `barril-1.8.0.tar` & `barril-1.9.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/docs/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)       27 2020-01-13 12:54:37.000000 barril-1.8.0/docs/readme.rst
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)       67 2020-01-13 12:54:37.000000 barril-1.8.0/docs/usage.rst
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1090 2020-01-13 12:54:37.000000 barril-1.8.0/docs/installation.rst
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)       55 2020-01-13 12:54:37.000000 barril-1.8.0/docs/changelog.rst
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/docs/img/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    36930 2020-01-13 12:54:37.000000 barril-1.8.0/docs/img/barrel-png-26.png
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)       67 2020-01-13 12:54:37.000000 barril-1.8.0/docs/units.rst
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      299 2020-01-13 12:54:37.000000 barril-1.8.0/docs/index.rst
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/docs/_extension/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1366 2020-01-13 12:54:37.000000 barril-1.8.0/docs/_extension/list_all_units.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)       33 2020-01-13 12:54:37.000000 barril-1.8.0/docs/contributing.rst
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     4966 2020-01-13 12:54:37.000000 barril-1.8.0/docs/conf.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      419 2020-01-13 12:54:37.000000 barril-1.8.0/docs/api.rst
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      237 2020-01-13 12:54:37.000000 barril-1.8.0/environment.devenv.yml
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3245 2020-01-13 12:54:37.000000 barril-1.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)       31 2020-01-13 12:54:37.000000 barril-1.8.0/pyproject.toml
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      134 2020-01-13 12:54:37.000000 barril-1.8.0/.readthedocs.yml
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1280 2020-01-13 12:54:37.000000 barril-1.8.0/.gitignore
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/.github/
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/.github/workflows/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1838 2020-01-13 12:56:20.000000 barril-1.8.0/.github/workflows/main.yml
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      317 2020-01-13 12:54:37.000000 barril-1.8.0/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      137 2020-01-13 12:56:31.000000 barril-1.8.0/setup.cfg
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      547 2020-01-13 12:54:37.000000 barril-1.8.0/tox.ini
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      431 2020-01-13 12:54:37.000000 barril-1.8.0/.pydevproject
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1041 2020-01-13 12:54:37.000000 barril-1.8.0/.gitattributes
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      380 2020-01-13 12:54:37.000000 barril-1.8.0/.codecov.yml
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      360 2020-01-13 12:54:37.000000 barril-1.8.0/.project
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      292 2020-01-13 12:54:37.000000 barril-1.8.0/.editorconfig
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      261 2020-01-13 12:54:37.000000 barril-1.8.0/HOWTORELEASE.rst
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1432 2020-01-13 12:54:37.000000 barril-1.8.0/setup.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      588 2020-01-13 12:54:37.000000 barril-1.8.0/.pre-commit-config.yaml
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1062 2020-01-13 12:54:37.000000 barril-1.8.0/LICENSE
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril.egg-info/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      169 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril.egg-info/requires.txt
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)        1 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril.egg-info/dependency_links.txt
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)        7 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril.egg-info/top_level.txt
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)        1 2020-01-13 12:55:47.000000 barril-1.8.0/src/barril.egg-info/not-zip-safe
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3038 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril.egg-info/SOURCES.txt
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     7407 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril.egg-info/PKG-INFO
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     8141 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/conftest.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/units/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     7232 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/interfaces.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    30288 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/unit_rich_text_representations.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      797 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/exceptions.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      178 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_scalar_factory.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     5333 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/__init__.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    31609 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_quantity.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      388 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_unit_constants.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    51714 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/unit_database.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3374 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/unit_system_interface.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     9897 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_abstractvaluewithquantity.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)   522578 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/posc.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     2572 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/unit_system.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    11118 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_scalar.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    19400 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/unit_system_manager.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     8391 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_fraction_scalar.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    10877 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_array.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/units/_tests/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3349 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_operations.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     6280 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_scalar_and_quantity.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    19741 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_scalar.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     5597 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_derived_quantities.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1910 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_posc2.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    17024 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_unit_database.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      337 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_empty_scalar.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3269 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_legacy_unit.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    13016 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_posc_additional_units.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3046 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_quantity.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     2465 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_scalar_refactor.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     5551 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_fraction_scalar.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     2476 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_unit_system.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    10400 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_array.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1974 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_unit_rich_text_representations.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    16184 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_posc.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     6728 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_unit_system_manager.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     5849 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_fixedarray.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1127 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_tests/test_read_only_quantity.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     6148 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_fixedarray.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/units/scalar_validation/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1810 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/scalar_validation/scalar_min_max_validator.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/scalar_validation/__init__.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/units/scalar_validation/_tests/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     2787 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/scalar_validation/_tests/test_scalar_min_max_validator.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     2129 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/units/_value_generator.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)       88 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/__init__.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/curve/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/curve/__init__.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3836 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/curve/curve.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      866 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/curve/curve_interface.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/curve/_tests/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     2939 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/curve/_tests/test_curve.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/basic/
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/basic/format_float/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3473 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/basic/format_float/__init__.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/basic/format_float/_tests/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1005 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/basic/format_float/_tests/test_format_float.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/basic/__init__.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/basic/fraction/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)    15754 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/basic/fraction/_fraction_value.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)       91 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/basic/fraction/__init__.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/basic/fraction/_tests/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3768 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/basic/fraction/_tests/test_fraction_value.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     2449 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/basic/fraction/_tests/test_fraction.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     6742 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/basic/fraction/_fraction.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/_util/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     3131 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/_util/types_.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/_util/__init__.py
-drwxrwxr-x   0 osboxes   (1000) osboxes   (1000)        0 2020-01-13 12:56:31.000000 barril-1.8.0/src/barril/_util/_tests/
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     1623 2020-01-13 12:54:37.000000 barril-1.8.0/src/barril/_util/_tests/test_types.py
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     2926 2020-01-13 12:54:37.000000 barril-1.8.0/README.rst
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     7407 2020-01-13 12:56:31.000000 barril-1.8.0/PKG-INFO
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)      919 2020-01-13 12:54:37.000000 barril-1.8.0/.isort.cfg
--rw-rw-r--   0 osboxes   (1000) osboxes   (1000)     2350 2020-01-13 12:54:37.000000 barril-1.8.0/CHANGELOG.rst
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/.github/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      317 2019-10-08 20:48:02.000000 barril-1.9.0/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/.github/workflows/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1859 2020-02-20 20:12:53.000000 barril-1.9.0/.github/workflows/main.yml
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      360 2019-10-08 20:48:02.000000 barril-1.9.0/.project
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      431 2019-10-08 20:48:02.000000 barril-1.9.0/.pydevproject
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      261 2019-10-08 20:48:02.000000 barril-1.9.0/HOWTORELEASE.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      588 2020-02-20 20:12:53.000000 barril-1.9.0/.pre-commit-config.yaml
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      237 2019-10-08 20:48:02.000000 barril-1.9.0/environment.devenv.yml
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3245 2020-02-20 20:12:53.000000 barril-1.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1041 2019-10-08 20:48:02.000000 barril-1.9.0/.gitattributes
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     2535 2020-02-20 20:12:53.000000 barril-1.9.0/CHANGELOG.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      380 2019-10-08 20:48:02.000000 barril-1.9.0/.codecov.yml
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      547 2019-10-08 20:48:02.000000 barril-1.9.0/tox.ini
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     2926 2020-02-20 20:12:53.000000 barril-1.9.0/README.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1432 2019-10-08 20:48:02.000000 barril-1.9.0/setup.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     7648 2020-02-20 20:19:26.000000 barril-1.9.0/PKG-INFO
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/docs/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)       33 2019-10-08 20:48:02.000000 barril-1.9.0/docs/contributing.rst
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/docs/img/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    36930 2019-10-08 20:48:02.000000 barril-1.9.0/docs/img/barrel-png-26.png
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      299 2020-02-20 20:12:53.000000 barril-1.9.0/docs/index.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)       27 2019-10-08 20:48:02.000000 barril-1.9.0/docs/readme.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     4966 2020-02-20 20:12:53.000000 barril-1.9.0/docs/conf.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/docs/_extension/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1366 2020-02-20 20:12:53.000000 barril-1.9.0/docs/_extension/list_all_units.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)       55 2019-10-08 20:48:02.000000 barril-1.9.0/docs/changelog.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)       67 2019-10-08 20:48:02.000000 barril-1.9.0/docs/usage.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)       67 2020-02-20 20:12:53.000000 barril-1.9.0/docs/units.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      419 2019-10-08 20:48:02.000000 barril-1.9.0/docs/api.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1090 2019-10-08 20:48:02.000000 barril-1.9.0/docs/installation.rst
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      137 2020-02-20 20:19:26.000000 barril-1.9.0/setup.cfg
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1280 2019-10-08 20:48:02.000000 barril-1.9.0/.gitignore
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      134 2019-10-08 20:48:02.000000 barril-1.9.0/.readthedocs.yml
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1062 2019-10-08 20:48:02.000000 barril-1.9.0/LICENSE
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      919 2019-10-08 20:48:02.000000 barril-1.9.0/.isort.cfg
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/units/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    30288 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/unit_rich_text_representations.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     2129 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/_value_generator.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    11118 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_scalar.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      388 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/_unit_constants.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    19400 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/unit_system_manager.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      178 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/_scalar_factory.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)   522908 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/posc.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     6148 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_fixedarray.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    12671 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_array.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/units/scalar_validation/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1810 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/scalar_validation/scalar_min_max_validator.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)        0 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/scalar_validation/__init__.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/units/scalar_validation/_tests/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     2787 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/scalar_validation/_tests/test_scalar_min_max_validator.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     8391 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_fraction_scalar.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     2572 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/unit_system.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     9897 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_abstractvaluewithquantity.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3374 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/unit_system_interface.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     7232 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/interfaces.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     5333 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/__init__.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    51714 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/unit_database.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      797 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/exceptions.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/units/_tests/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      337 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/_tests/test_empty_scalar.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    13128 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_posc_additional_units.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     5551 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_fraction_scalar.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1127 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/_tests/test_read_only_quantity.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     6728 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_unit_system_manager.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    11931 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_array.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    16184 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_posc.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1974 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_unit_rich_text_representations.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     6280 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_scalar_and_quantity.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     2465 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/_tests/test_scalar_refactor.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    19741 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_scalar.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    17024 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_unit_database.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     2476 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/units/_tests/test_unit_system.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3349 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_operations.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3269 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_legacy_unit.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1910 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_posc2.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     5849 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_fixedarray.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     5597 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_derived_quantities.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3046 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_tests/test_quantity.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    31609 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/units/_quantity.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/curve/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      866 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/curve/curve_interface.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3836 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/curve/curve.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)        0 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/curve/__init__.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/curve/_tests/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     2939 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/curve/_tests/test_curve.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/basic/
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/basic/fraction/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     6742 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/basic/fraction/_fraction.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)       91 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/basic/fraction/__init__.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)    15754 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/basic/fraction/_fraction_value.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/basic/fraction/_tests/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3768 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/basic/fraction/_tests/test_fraction_value.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     2449 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/basic/fraction/_tests/test_fraction.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/basic/format_float/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3473 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/basic/format_float/__init__.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/basic/format_float/_tests/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1005 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/basic/format_float/_tests/test_format_float.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)        0 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/basic/__init__.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     8141 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/conftest.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)       88 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/__init__.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/_util/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)        0 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/_util/__init__.py
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3131 2019-10-08 20:48:02.000000 barril-1.9.0/src/barril/_util/types_.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril/_util/_tests/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     1623 2020-02-20 20:12:53.000000 barril-1.9.0/src/barril/_util/_tests/test_types.py
+drwxrwxr-x   0 rosenbach  (1000) rosenbach  (1000)        0 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril.egg-info/
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)        1 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     7648 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril.egg-info/PKG-INFO
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)        1 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril.egg-info/not-zip-safe
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)        7 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril.egg-info/top_level.txt
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)     3038 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      169 2020-02-20 20:19:26.000000 barril-1.9.0/src/barril.egg-info/requires.txt
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)      292 2019-10-08 20:48:02.000000 barril-1.9.0/.editorconfig
+-rw-rw-r--   0 rosenbach  (1000) rosenbach  (1000)       31 2020-02-20 20:12:53.000000 barril-1.9.0/pyproject.toml
```

### Comparing `barril-1.8.0/docs/installation.rst` & `barril-1.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/docs/img/barrel-png-26.png` & `barril-1.9.0/docs/img/barrel-png-26.png`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/docs/_extension/list_all_units.py` & `barril-1.9.0/docs/_extension/list_all_units.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/docs/conf.py` & `barril-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/CONTRIBUTING.rst` & `barril-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/.gitignore` & `barril-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/.github/workflows/main.yml` & `barril-1.9.0/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 name: build
 
 on:
   push:
     branches:
       - master
       - rb-*
+    tags:
+      - v*
 
   pull_request:
   schedule:
   - cron: 0 2 * * *
 
 jobs:
   build:
```

### Comparing `barril-1.8.0/tox.ini` & `barril-1.9.0/tox.ini`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/.gitattributes` & `barril-1.9.0/.gitattributes`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/setup.py` & `barril-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/.pre-commit-config.yaml` & `barril-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/LICENSE` & `barril-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril.egg-info/SOURCES.txt` & `barril-1.9.0/src/barril.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril.egg-info/PKG-INFO` & `barril-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barril
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python package to manage units for physical quantities
 Home-page: https://github.com/ESSS/barril
 Author: ESSS
 Author-email: foss@esss.co
 License: MIT license
 Description: ======
         Barril
@@ -116,14 +116,21 @@
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         .. _`GitHub page` :                   https://github.com/ESSS/barril
         .. _Cookiecutter:                     https://github.com/audreyr/cookiecutter
         .. _pytest:                           https://github.com/pytest-dev/pytest
         .. _tox:                              https://github.com/tox-dev/tox
         
         
+        1.9.0 (2020-02-20)
+        ------------------
+        
+        * New ``classmethod`` ``Array.FromScalars`` that creates an ``Array`` from a ``List[Scalar]``.
+        * Add new unit: "barrel per second" (``bbl/s``).
+        
+        
         1.8.0 (2020-01-10)
         ------------------
         
         * Add new category: "standard volume per standard volume"
         * Move unit ``sm3/sm3`` from "volume per volume" to "standard volume per standard volume"
         
         1.7.2 (2019-10-16)
@@ -204,9 +211,9 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
-Provides-Extra: docs
 Provides-Extra: testing
+Provides-Extra: docs
```

### Comparing `barril-1.8.0/src/barril/conftest.py` & `barril-1.9.0/src/barril/conftest.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/interfaces.py` & `barril-1.9.0/src/barril/units/interfaces.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/unit_rich_text_representations.py` & `barril-1.9.0/src/barril/units/unit_rich_text_representations.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/exceptions.py` & `barril-1.9.0/src/barril/units/exceptions.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/__init__.py` & `barril-1.9.0/src/barril/units/__init__.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_quantity.py` & `barril-1.9.0/src/barril/units/_quantity.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/unit_database.py` & `barril-1.9.0/src/barril/units/unit_database.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/unit_system_interface.py` & `barril-1.9.0/src/barril/units/unit_system_interface.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_abstractvaluewithquantity.py` & `barril-1.9.0/src/barril/units/_abstractvaluewithquantity.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/posc.py` & `barril-1.9.0/src/barril/units/posc.py`

 * *Files 0% similar despite different names*

```diff
@@ -930,14 +930,24 @@
         "specific productivity index",
         "barrels/centiPoise day psi",
         "bbl/cP.d.psi",
         f_base_to_unit,
         f_unit_to_base,
         default_category=None,
     )
+    f_unit_to_base = MakeCustomaryToBase(0.0, 0.1589873, 1.0, 0.0)
+    f_base_to_unit = MakeBaseToCustomary(0.0, 0.1589873, 1.0, 0.0)
+    db.AddUnit(
+        "volume flow rate",
+        "barrel/second",
+        "bbl/s",
+        f_base_to_unit,
+        f_unit_to_base,
+        default_category=None,
+    )
     f_unit_to_base = MakeCustomaryToBase(0.0, 0.1589873, 86400, 0.0)
     f_base_to_unit = MakeBaseToCustomary(0.0, 0.1589873, 86400, 0.0)
     db.AddUnit(
         "volume flow rate",
         "barrel/day",
         "bbl/d",
         f_base_to_unit,
@@ -14171,14 +14181,15 @@
             "volume flow rate",
             override=override_categories,
             valid_units=[
                 "m3/s",
                 "Mcf/d",
                 "Mm3/d",
                 "Mm3/h",
+                "bbl/s",
                 "bbl/d",
                 "bbl/hr",
                 "bbl/min",
                 "cm3/30min",
                 "cm3/h",
                 "cm3/min",
                 "cm3/s",
```

### Comparing `barril-1.8.0/src/barril/units/unit_system.py` & `barril-1.9.0/src/barril/units/unit_system.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_scalar.py` & `barril-1.9.0/src/barril/units/_scalar.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/unit_system_manager.py` & `barril-1.9.0/src/barril/units/unit_system_manager.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_fraction_scalar.py` & `barril-1.9.0/src/barril/units/_fraction_scalar.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_array.py` & `barril-1.9.0/src/barril/units/_array.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from typing import Optional, Iterable
+
 from barril._util.types_ import IsNumber
 from barril.basic.format_float import FormatFloat
 from barril.units.unit_database import UnitDatabase
 from oop_ext.interface._interface import ImplementsInterface
 
 from ._abstractvaluewithquantity import AbstractValueWithQuantityObject
 from ._quantity import Quantity
 from .interfaces import IArray
+from ._scalar import Scalar
 
 __all__ = ["Array"]
 
 
 @ImplementsInterface(IArray)
 class Array(AbstractValueWithQuantityObject):
     """
@@ -175,14 +178,59 @@
                             CheckValue(min_value)
                             CheckValue(max_value)
 
                             # Break the outer 'for' used just to get the min/max
                             break
 
     @classmethod
+    def FromScalars(
+        cls,
+        scalars: Iterable[Scalar],
+        *,
+        unit: Optional[str] = None,
+        category: Optional[str] = None
+    ):
+        """
+        Create an Array from a sequence of Scalars.
+
+        When not defined, the unit and category assumed will be from the first Scalar on the sequence.
+
+        :param values:
+            A sequence of Scalars. When the values parameter is an empty sequence and
+            the unit is not provided an Array with an empty quantity will be returned.
+
+        :param unit:
+            A string representing the unit, if not defined
+            the unit from the first Scalar on the sequence will be used.
+
+        :param category:
+            A string representing the category, if not defined
+            the category from the first Scalar on the sequence will be used.
+        """
+        scalars = iter(scalars)
+        try:
+            first_scalar = next(scalars)
+        except StopIteration:
+            if unit is None and category is None:
+                return cls.CreateEmptyArray()
+            elif category is None:
+                category = UnitDatabase.GetSingleton().GetDefaultCategory(unit)
+                return cls(values=[], unit=unit, category=category)
+            else:
+                assert unit is None
+                return cls(
+                    values=[], unit=unit, category=category
+                )  # This actually will raise an exception
+
+        unit = unit or first_scalar.unit
+        category = category or first_scalar.category
+        values = [first_scalar.GetValue(unit)] + [scalar.GetValue(unit) for scalar in scalars]
+        return cls(values=values, unit=unit, category=category)
+
+    @classmethod
     def CreateEmptyArray(cls, values=None):
         """
             Allows the creation of a array that does not have any associated
             category nor unit.
 
             :rtype: Array
         """
```

### Comparing `barril-1.8.0/src/barril/units/_tests/test_operations.py` & `barril-1.9.0/src/barril/units/_tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_scalar_and_quantity.py` & `barril-1.9.0/src/barril/units/_tests/test_scalar_and_quantity.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_scalar.py` & `barril-1.9.0/src/barril/units/_tests/test_scalar.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_derived_quantities.py` & `barril-1.9.0/src/barril/units/_tests/test_derived_quantities.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_posc2.py` & `barril-1.9.0/src/barril/units/_tests/test_posc2.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_unit_database.py` & `barril-1.9.0/src/barril/units/_tests/test_unit_database.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_legacy_unit.py` & `barril-1.9.0/src/barril/units/_tests/test_legacy_unit.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_posc_additional_units.py` & `barril-1.9.0/src/barril/units/_tests/test_posc_additional_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,18 @@
     assert approx(DoConversion("eq.cp", "lbf.s^n/100ft2", 250.0)) == 0.5250109
 
 
 def testBblPerMeters(db):
     assert approx(db.Convert("volume per length", "bbl/ft", "bbl/m", 1)) == 1 / 0.3048
 
 
+def testBblPerSecond(db):
+    assert approx(db.Convert("volume flow rate", "bbl/hr", "bbl/s", 1)) == 1 / 3600
+
+
 def testConcentration(db):
     assert approx(db.Convert("concentration", "g/L", "mg/L", 1)) == 1000.0
 
 
 def testVolumeFractionPerTemperature(db):
     expected_result = db.Convert("volumetric thermal expansion", "1/degC", "1/degF", 1)
     obtained_result = db.Convert(
```

### Comparing `barril-1.8.0/src/barril/units/_tests/test_quantity.py` & `barril-1.9.0/src/barril/units/_tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_scalar_refactor.py` & `barril-1.9.0/src/barril/units/_tests/test_scalar_refactor.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_fraction_scalar.py` & `barril-1.9.0/src/barril/units/_tests/test_fraction_scalar.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_unit_system.py` & `barril-1.9.0/src/barril/units/_tests/test_unit_system.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_array.py` & `barril-1.9.0/src/barril/units/_tests/test_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from collections import OrderedDict
 from barril import units
 from barril.units import Array, InvalidUnitError, ObtainQuantity, Quantity
 from pytest import approx
+from barril.units import Scalar
 
 
 def testEmptyArray():
     arr = Array.CreateEmptyArray()
     assert not arr.HasCategory()
 
     arr = arr.CreateCopy(category="temperature", unit="degC")
@@ -324,7 +325,41 @@
     assert array.values == []
 
     array = Array(ObtainQuantity("m"))
     assert array.values == []
 
     with pytest.raises(AssertionError):
         Array(ObtainQuantity("m"), unit="m")
+
+
+class TestFromScalar:
+    def test_create_array_informing_category(self):
+        array_molar_fraction = Array.FromScalars(
+            scalars=[Scalar(1, "-"), Scalar(2, "-")], category="percentage"
+        )
+        assert array_molar_fraction.values == [1, 2]
+        assert array_molar_fraction.unit == "-"
+        assert array_molar_fraction.category == "percentage"
+
+    def test_create_array_informing_unit(self):
+        array_in_cm = Array.FromScalars(scalars=[Scalar(1, "m"), Scalar(2, "m")], unit="cm")
+        assert array_in_cm.values == [100.0, 200.0]
+        assert array_in_cm.unit == "cm"
+        assert array_in_cm.category == "length"
+
+    def test_create_array_from_list_of_scalar(self):
+        array_in_m = Array.FromScalars(scalars=iter([Scalar(1, "m"), Scalar(2, "m")]))
+        assert array_in_m.values == [1, 2]
+        assert array_in_m.unit == "m"
+        assert array_in_m.category == "length"
+
+    def test_check_empty_array(self):
+        assert Array.FromScalars(scalars=[]) == Array.CreateEmptyArray()
+        assert Array.FromScalars(scalars=[], unit="m") == Array([], "m")
+
+        expected_msg = "If category and value are given, the unit must be specified too."
+        with pytest.raises(AssertionError, match=expected_msg):
+            Array.FromScalars(scalars=[], category="length")
+
+    def test_check_array_with_different_units(self):
+        with pytest.raises(InvalidUnitError):
+            Array.FromScalars(scalars=[Scalar(1, "m"), Scalar(1, "kg")])
```

### Comparing `barril-1.8.0/src/barril/units/_tests/test_unit_rich_text_representations.py` & `barril-1.9.0/src/barril/units/_tests/test_unit_rich_text_representations.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_posc.py` & `barril-1.9.0/src/barril/units/_tests/test_posc.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_unit_system_manager.py` & `barril-1.9.0/src/barril/units/_tests/test_unit_system_manager.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_fixedarray.py` & `barril-1.9.0/src/barril/units/_tests/test_fixedarray.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_tests/test_read_only_quantity.py` & `barril-1.9.0/src/barril/units/_tests/test_read_only_quantity.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_fixedarray.py` & `barril-1.9.0/src/barril/units/_fixedarray.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/scalar_validation/scalar_min_max_validator.py` & `barril-1.9.0/src/barril/units/scalar_validation/scalar_min_max_validator.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/scalar_validation/_tests/test_scalar_min_max_validator.py` & `barril-1.9.0/src/barril/units/scalar_validation/_tests/test_scalar_min_max_validator.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/units/_value_generator.py` & `barril-1.9.0/src/barril/units/_value_generator.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/curve/curve.py` & `barril-1.9.0/src/barril/curve/curve.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/curve/curve_interface.py` & `barril-1.9.0/src/barril/curve/curve_interface.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/curve/_tests/test_curve.py` & `barril-1.9.0/src/barril/curve/_tests/test_curve.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/basic/format_float/__init__.py` & `barril-1.9.0/src/barril/basic/format_float/__init__.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/basic/format_float/_tests/test_format_float.py` & `barril-1.9.0/src/barril/basic/format_float/_tests/test_format_float.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/basic/fraction/_fraction_value.py` & `barril-1.9.0/src/barril/basic/fraction/_fraction_value.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/basic/fraction/_tests/test_fraction_value.py` & `barril-1.9.0/src/barril/basic/fraction/_tests/test_fraction_value.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/basic/fraction/_tests/test_fraction.py` & `barril-1.9.0/src/barril/basic/fraction/_tests/test_fraction.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/basic/fraction/_fraction.py` & `barril-1.9.0/src/barril/basic/fraction/_fraction.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/_util/types_.py` & `barril-1.9.0/src/barril/_util/types_.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/src/barril/_util/_tests/test_types.py` & `barril-1.9.0/src/barril/_util/_tests/test_types.py`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/README.rst` & `barril-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/PKG-INFO` & `barril-1.9.0/src/barril.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barril
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python package to manage units for physical quantities
 Home-page: https://github.com/ESSS/barril
 Author: ESSS
 Author-email: foss@esss.co
 License: MIT license
 Description: ======
         Barril
@@ -116,14 +116,21 @@
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         .. _`GitHub page` :                   https://github.com/ESSS/barril
         .. _Cookiecutter:                     https://github.com/audreyr/cookiecutter
         .. _pytest:                           https://github.com/pytest-dev/pytest
         .. _tox:                              https://github.com/tox-dev/tox
         
         
+        1.9.0 (2020-02-20)
+        ------------------
+        
+        * New ``classmethod`` ``Array.FromScalars`` that creates an ``Array`` from a ``List[Scalar]``.
+        * Add new unit: "barrel per second" (``bbl/s``).
+        
+        
         1.8.0 (2020-01-10)
         ------------------
         
         * Add new category: "standard volume per standard volume"
         * Move unit ``sm3/sm3`` from "volume per volume" to "standard volume per standard volume"
         
         1.7.2 (2019-10-16)
@@ -204,9 +211,9 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
-Provides-Extra: docs
 Provides-Extra: testing
+Provides-Extra: docs
```

### Comparing `barril-1.8.0/.isort.cfg` & `barril-1.9.0/.isort.cfg`

 * *Files identical despite different names*

### Comparing `barril-1.8.0/CHANGELOG.rst` & `barril-1.9.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+1.9.0 (2020-02-20)
+------------------
+
+* New ``classmethod`` ``Array.FromScalars`` that creates an ``Array`` from a ``List[Scalar]``.
+* Add new unit: "barrel per second" (``bbl/s``).
+
+
 1.8.0 (2020-01-10)
 ------------------
 
 * Add new category: "standard volume per standard volume"
 * Move unit ``sm3/sm3`` from "volume per volume" to "standard volume per standard volume"
 
 1.7.2 (2019-10-16)
```

