# Comparing `tmp/mxmake-0.1.tar.gz` & `tmp/mxmake-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxmake-0.1.tar", last modified: Thu May 19 11:20:13 2022, max compression
+gzip compressed data, was "mxmake-1.0a1.tar", last modified: Fri May  5 06:49:45 2023, max compression
```

## Comparing `mxmake-0.1.tar` & `mxmake-1.0a1.tar`

### file list

```diff
@@ -1,35 +1,90 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-05-19 11:20:13.282081 mxmake-0.1/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       75 2022-05-19 11:20:12.000000 mxmake-0.1/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1317 2022-05-19 11:20:12.000000 mxmake-0.1/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      166 2022-05-19 11:20:12.000000 mxmake-0.1/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1972 2022-05-19 11:20:13.282081 mxmake-0.1/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      723 2022-05-19 11:20:12.000000 mxmake-0.1/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       99 2022-05-19 11:20:12.000000 mxmake-0.1/TODO.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1392 2022-05-19 11:20:13.282081 mxmake-0.1/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)       39 2022-05-19 11:20:13.000000 mxmake-0.1/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-05-19 11:20:13.278081 mxmake-0.1/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-05-19 11:20:13.278081 mxmake-0.1/src/mxmake/
--rw-r--r--   0 rnix      (1000) rnix      (1000)        0 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1202 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/hook.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1646 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/main.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-05-19 11:20:13.278081 mxmake-0.1/src/mxmake/targets/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-05-19 11:20:13.282081 mxmake-0.1/src/mxmake/targets/ldap/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1970 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/targets/ldap/openldap.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1007 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/targets/ldap/python-ldap.mk
--rw-r--r--   0 rnix      (1000) rnix      (1000)      612 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/targets.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-05-19 11:20:13.282081 mxmake-0.1/src/mxmake/templates/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      338 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/templates/env.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      469 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/templates/run-coverage.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      211 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/templates/run-tests.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)      173 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/templates/script.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4424 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/templates.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15877 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      896 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake/utils.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-05-19 11:20:13.282081 mxmake-0.1/src/mxmake.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1972 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      665 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      123 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)      106 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        7 2022-05-19 11:20:13.000000 mxmake-0.1/src/mxmake.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3155 2023-05-05 06:46:53.000000 mxmake-1.0a1/CHANGES.md
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1320 2023-01-31 23:41:42.000000 mxmake-1.0a1/LICENSE.md
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      133 2023-05-05 06:46:08.000000 mxmake-1.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7066 2023-05-05 06:49:45.769435 mxmake-1.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1359 2023-01-31 23:41:42.000000 mxmake-1.0a1/README.md
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2254 2023-05-05 06:46:28.000000 mxmake-1.0a1/pyproject.toml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-05 06:49:45.769435 mxmake-1.0a1/setup.cfg
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        0 2022-05-19 08:58:33.000000 mxmake-1.0a1/src/mxmake/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2131 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/hook.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7162 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/main.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2200 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/parser.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1410 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/sphinxext.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/templates/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2057 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/templates/Makefile
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       82 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/templates/additional_sources_targets.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      521 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/templates/dependencies.md
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      389 2022-06-10 06:32:06.000000 mxmake-1.0a1/src/mxmake/templates/env.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      380 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/templates/mx.ini
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      627 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates/pytest-run-coverage.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      180 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates/pytest-run-tests.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      173 2022-05-19 09:05:03.000000 mxmake-1.0a1/src/mxmake/templates/script.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      843 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/templates/topics.md
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      677 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates/zope-testrunner-run-coverage.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      212 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates/zope-testrunner-run-tests.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12231 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/templates.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/testing/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2759 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/testing/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/tests/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      745 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/tests/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      687 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/tests/test_hook.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2619 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/tests/test_parser.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    26046 2023-05-05 06:23:39.000000 mxmake-1.0a1/src/mxmake/tests/test_templates.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11073 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/tests/test_topics.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      953 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/tests/test_utils.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake/topics/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/applications/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1083 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/applications/cookiecutter.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       76 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/topics/applications/metadata.ini
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1177 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/topics/applications/twisted.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1969 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/applications/zest-releaser.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3362 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/applications/zope.mk
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/core/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2048 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/core/base.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       62 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/core/metadata.ini
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3537 2023-05-05 06:20:53.000000 mxmake-1.0a1/src/mxmake/topics/core/mxenv.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1960 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/core/mxfiles.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1407 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/core/packages.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      994 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/core/sources.mk
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/docs/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      910 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/topics/docs/jsdoc.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       62 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/docs/metadata.ini
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1839 2023-02-06 10:48:55.000000 mxmake-1.0a1/src/mxmake/topics/docs/sphinx.mk
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/i18n/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2106 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/i18n/gettext.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1525 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/i18n/lingua.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       83 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/i18n/metadata.ini
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/js/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      763 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/js/karma.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2023-02-06 10:28:34.000000 mxmake-1.0a1/src/mxmake/topics/js/metadata.ini
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2351 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/js/npm.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      666 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/js/rollup.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1084 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/topics/js/scss.mk
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/ldap/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       63 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/ldap/metadata.ini
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2197 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/ldap/openldap.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1307 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/ldap/python-ldap.mk
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/qa/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1253 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/qa/black.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1478 2023-05-05 06:19:52.000000 mxmake-1.0a1/src/mxmake/topics/qa/coverage.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1251 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/qa/isort.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       58 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/qa/metadata.ini
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1245 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/qa/mypy.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1592 2023-03-08 21:10:45.000000 mxmake-1.0a1/src/mxmake/topics/qa/test.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1467 2023-03-06 07:31:33.000000 mxmake-1.0a1/src/mxmake/topics/qa/zpretty.mk
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.769435 mxmake-1.0a1/src/mxmake/topics/system/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      752 2023-02-06 10:28:34.000000 mxmake-1.0a1/src/mxmake/topics/system/dependencies.mk
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       65 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/topics/system/metadata.ini
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9529 2023-05-05 06:05:05.000000 mxmake-1.0a1/src/mxmake/topics.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      831 2023-01-31 23:41:42.000000 mxmake-1.0a1/src/mxmake/utils.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-05 06:49:45.765435 mxmake-1.0a1/src/mxmake.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7066 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2295 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      314 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-05-19 09:22:24.000000 mxmake-1.0a1/src/mxmake.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      128 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        7 2023-05-05 06:49:45.000000 mxmake-1.0a1/src/mxmake.egg-info/top_level.txt
```

### Comparing `mxmake-0.1/LICENSE.rst` & `mxmake-1.0a1/LICENSE.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-License
-=======
+# License
+
+Copyright (c) 2022-2023, mxstack Contributors
 
-Copyright (c) 2022, Cone Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `mxmake-0.1/src/mxmake/main.py` & `mxmake-1.0a1/src/mxmake/hook.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,65 @@
+from mxmake.templates import get_template_environment
 from mxmake.templates import template
 from mxmake.utils import list_value
+from mxmake.utils import NAMESPACE
 from mxmake.utils import ns_name
-import argparse
+
 import logging
 import mxdev
-import sys
-import typing
+import os
+
+
+logger = logging.getLogger("mxmake")
 
 
-logger = logging.getLogger('mxmake')
+ADDITIONAL_SOURCES_TARGETS = [
+    "constraints.txt",
+    "pyproject.toml",
+    "requirements.txt",
+    "setup.cfg",
+    "setup.py",
+]
 
 
-def read_configuration(tio: typing.TextIO) -> mxdev.Configuration:
-    hooks = mxdev.load_hooks()
-    configuration = mxdev.Configuration(tio=tio, hooks=hooks)
-    state = mxdev.State(configuration=configuration)
-    mxdev.read(state)
-    mxdev.read_hooks(state, hooks)
-    return configuration
+class Hook(mxdev.Hook):
+    namespace: str = NAMESPACE
 
+    def __init__(self) -> None:
+        logger.info("mxmake: hook initialized")
 
-def clean_files(configuration: mxdev.Configuration) -> None:
-    logger.info('mxmake: clean generated files')
-    templates = list_value(configuration.settings.get(ns_name('templates')))
-    if not templates:
-        logger.info('mxmake: No templates defined')
-    else:
+    def generate_templates(self, state: mxdev.State):
+        config = state.configuration
+        templates = list_value(config.settings.get(ns_name("templates")))
+        if not templates:
+            logger.info("mxmake: No templates defined")
+            return
+        environment = get_template_environment()
         for name in templates:
-            factory = template.lookup(name)
-            instance = factory(configuration)
-            if instance.remove():
-                logger.info(f'mxmake: removed "{instance.target_name}"')
-
-
-def main() -> None:
-    mxdev.setup_logger(logging.INFO)
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        '-c',
-        '--configuration',
-        help='mxdev configuration file',
-        nargs="?",
-        type=argparse.FileType('r'),
-        required=True
-    )
-    parser.add_argument(
-        '--clean',
-        action='store_true',
-        help='Remove generated files'
-    )
-    args = parser.parse_args()
-    if args.clean:
-        configuration = read_configuration(args.configuration)
-        clean_files(configuration)
-        sys.exit(0)
-    logger.info('mxmake: no action given')
-    sys.exit(1)
+            try:
+                factory = template.lookup(name, bound=True)
+            except RuntimeError as e:
+                msg = f"mxmake: {str(e)}"
+                logger.warning(msg)
+                continue
+            factory(config, environment).write()
+
+    def generate_additional_sources_targets(self, state: mxdev.State):
+        config = state.configuration
+        additional_sources_targets = []
+        sources_folder = config.settings.get("default-target", "sources")
+        for package_name in config.packages:
+            source_folder = os.path.join(sources_folder, package_name)
+            for child in os.listdir(source_folder):
+                if child in ADDITIONAL_SOURCES_TARGETS:
+                    additional_sources_targets.append(
+                        os.path.join(source_folder, child)
+                    )
+        if not additional_sources_targets:
+            return
+        environment = get_template_environment()
+        factory = template.lookup("additional_sources_targets")
+        factory(additional_sources_targets, environment).write()
+
+    def write(self, state: mxdev.State) -> None:
+        self.generate_templates(state)
+        self.generate_additional_sources_targets(state)
```

