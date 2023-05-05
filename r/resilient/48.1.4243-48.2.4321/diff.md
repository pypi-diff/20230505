# Comparing `tmp/resilient-48.1.4243.tar.gz` & `tmp/resilient-48.2.4321.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient-48.1.4243.tar", last modified: Thu Apr 20 19:34:54 2023, max compression
+gzip compressed data, was "resilient-48.2.4321.tar", last modified: Fri May  5 12:33:55 2023, max compression
```

## Comparing `resilient-48.1.4243.tar` & `resilient-48.2.4321.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8037 2023-04-20 19:34:29.000000 resilient-48.1.4243/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-04-20 19:34:54.035501 resilient-48.1.4243/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2023-04-20 19:34:29.000000 resilient-48.1.4243/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.031501 resilient-48.1.4243/co3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      377 2023-04-20 19:34:29.000000 resilient-48.1.4243/co3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-04-20 19:34:29.000000 resilient-48.1.4243/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.031501 resilient-48.1.4243/resilient/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/resilient/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/bin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/bin/finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/bin/gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/bin/res_keyring.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36857 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14360 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/co3argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36941 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1577 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      854 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/definitions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12719 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/resilient_rest_mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/resilient.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1425 2023-04-20 19:34:54.000000 resilient-48.1.4243/resilient.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1854 2023-04-20 19:34:54.035501 resilient-48.1.4243/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-04-20 19:34:29.000000 resilient-48.1.4243/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4241 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/shared_mock_data/mock_responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_responses/session.JSON
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/.jwk/
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/API_KEY
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/EMAIL
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/EMPTY
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/PASSWORD
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/URL
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/template_test.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2951 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_co3_ii.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9003 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/xtest_gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/xtest_patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/xtest_res_keyring.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2023-04-20 19:34:29.000000 resilient-48.1.4243/tools/res_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      885 2023-04-20 19:34:29.000000 resilient-48.1.4243/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8135 2023-05-05 12:33:36.000000 resilient-48.2.4321/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-05-05 12:33:55.543470 resilient-48.2.4321/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2023-05-05 12:33:36.000000 resilient-48.2.4321/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.539470 resilient-48.2.4321/co3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      377 2023-05-05 12:33:36.000000 resilient-48.2.4321/co3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 12:33:36.000000 resilient-48.2.4321/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.539470 resilient-48.2.4321/resilient/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/resilient/bin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/bin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/bin/finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/bin/gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/bin/res_keyring.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36857 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14360 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/co3argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36941 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1577 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      854 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/definitions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12719 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2023-05-05 12:33:36.000000 resilient-48.2.4321/resilient/resilient_rest_mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/resilient.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1425 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      350 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-05-05 12:33:55.000000 resilient-48.2.4321/resilient.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1854 2023-05-05 12:33:55.547470 resilient-48.2.4321/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-05-05 12:33:36.000000 resilient-48.2.4321/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4241 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/shared_mock_data/mock_responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_responses/session.JSON
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/.jwk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/API_KEY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/EMAIL
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/EMPTY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/PASSWORD
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/shared_mock_data/mock_secrets/URL
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/template_test.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2812 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_co3_ii.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17968 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9003 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/xtest_gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/xtest_patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2023-05-05 12:33:36.000000 resilient-48.2.4321/tests/xtest_res_keyring.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:55.543470 resilient-48.2.4321/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2023-05-05 12:33:36.000000 resilient-48.2.4321/tools/res_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      885 2023-05-05 12:33:36.000000 resilient-48.2.4321/tox.ini
```

### Comparing `resilient-48.1.4243/CHANGES` & `resilient-48.2.4321/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2023-05: version 48.2**
+
+* Update version of requests-toolbelt to v1.0 to support urllib3 v2.0
+
 **2023-04: version 48.1**
 
 * REST client updated to use ``include_permissions=false`` by default when authenticating to ``/rest/session`` endpoint.
   This will give improved performance for SOAR instances with large organizations.
 
 **2023-02: version 48.0**
```

### Comparing `resilient-48.1.4243/PKG-INFO` & `resilient-48.2.4321/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 48.1.4243
+Version: 48.2.4321
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-48.1.4243/README.md` & `resilient-48.2.4321/README.md`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/LICENSE` & `resilient-48.2.4321/resilient/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/__init__.py` & `resilient-48.2.4321/resilient/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/bin/finfo.py` & `resilient-48.2.4321/resilient/bin/finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/bin/gadget.py` & `resilient-48.2.4321/resilient/bin/gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/bin/res_keyring.py` & `resilient-48.2.4321/resilient/bin/res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/co3.py` & `resilient-48.2.4321/resilient/co3.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/co3argparse.py` & `resilient-48.2.4321/resilient/co3argparse.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/co3base.py` & `resilient-48.2.4321/resilient/co3base.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/co3sslutil.py` & `resilient-48.2.4321/resilient/co3sslutil.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/constants.py` & `resilient-48.2.4321/resilient/constants.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/definitions.py` & `resilient-48.2.4321/resilient/definitions.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/helpers.py` & `resilient-48.2.4321/resilient/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/patch.py` & `resilient-48.2.4321/resilient/patch.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient/resilient_rest_mock.py` & `resilient-48.2.4321/resilient/resilient_rest_mock.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/resilient.egg-info/PKG-INFO` & `resilient-48.2.4321/resilient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 48.1.4243
+Version: 48.2.4321
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-48.1.4243/resilient.egg-info/SOURCES.txt` & `resilient-48.2.4321/resilient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/setup.cfg` & `resilient-48.2.4321/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
 	retry2            ~= 0.9
 	requests          ~= 2.27
-	requests-toolbelt ~= 0.9
+	requests-toolbelt ~= 1.0
 	six               ~= 1.16
 	
 	jwcrypto          ~= 1.4.0;  python_version >= "3.6"
 	
 	keyring           ~= 23.5;   python_version  > "3.6"
 	cachetools        ~= 5.0;    python_version  > "3.6"
 	setuptools        ~= 65.5.1; python_version > "3.6"
```

### Comparing `resilient-48.1.4243/tests/conftest.py` & `resilient-48.2.4321/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tests/helpers.py` & `resilient-48.2.4321/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tests/shared_mock_data/mock_responses/session.JSON` & `resilient-48.2.4321/tests/shared_mock_data/mock_responses/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tests/test_co3.py` & `resilient-48.2.4321/tests/test_co3.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,30 +31,27 @@
     res_client = resilient.get_client(mock_opts)
 
     assert res_client.base_url == "https://example.com:8080"
     assert res_client.cert == mock_cert
     assert res_client.actions_enabled == False
 
 def test_client_put(fx_simple_client):
-    def headers_callback(request, context):
-        context.status_code = 200
-        context.headers = request.headers
-        return json.dumps({ "content-type": request.headers["content-type"]})
 
     base_client = fx_simple_client[0]
     requests_adapter = fx_simple_client[1]
 
     test_headers = {"content-type": "application/octet-stream"}
 
     mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)    
 
     requests_adapter.register_uri('PUT',
                                   mock_uri,
+                                  status_code=200,
                                   request_headers=test_headers,
-                                  text=headers_callback)
+                                  text=json.dumps(test_headers))
 
     uri = "/playbooks/imports"
 
     r = base_client.put(
         uri,
         "payload",
         headers=test_headers
```

### Comparing `resilient-48.1.4243/tests/test_co3_ii.py` & `resilient-48.2.4321/tests/test_co3_ii.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tests/test_co3base.py` & `resilient-48.2.4321/tests/test_co3base.py`

 * *Files 4% similar despite different names*

```diff
@@ -339,177 +339,159 @@
         bytes_handle=bytes_handle
     )
 
     assert r.get("result") == "attached"
 
 
 def test_put_with_headers(fx_base_client):
-    def headers_callback(request, context):
-        context.status_code = 200
-        context.headers = request.headers
-        return json.dumps({ "content-type": request.headers["content-type"]})
 
     base_client = fx_base_client[0]
     requests_adapter = fx_base_client[1]
 
     test_headers = {"content-type": "application/octet-stream"}
 
     mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)    
 
     requests_adapter.register_uri('PUT',
                                   mock_uri,
+                                  status_code=200,
                                   request_headers=test_headers,
-                                  text=headers_callback)
+                                  text=json.dumps(test_headers))
 
     uri = "/playbooks/imports"
 
     r = base_client.put(
         uri,
         "payload",
         headers=test_headers
     )
 
     assert r['content-type'] == test_headers['content-type']
 
 
 def test_put_with_text_payload(fx_base_client):
-    def text_payload_callback(request, context):
-        context.status_code = 200
-        context.headers = request.headers
-        return json.dumps({ "content": request.text})
 
     base_client = fx_base_client[0]
     requests_adapter = fx_base_client[1]
 
     test_content = 'abc'
 
     mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)    
 
     requests_adapter.register_uri('PUT',
                                   mock_uri,
-                                  text=text_payload_callback)
+                                  status_code=200,
+                                  text=json.dumps({ "content": test_content}))
 
     uri = "/playbooks/imports"
 
     r = base_client.put(
         uri,
         test_content        
     )
 
     assert r['content'] == test_content
 
 
 def test_put_with_json_payload(fx_base_client):
-    def json_payload_callback(request, context):
-        context.status_code = 200
-        context.headers = request.headers
-        return json.dumps({ "content": request.text})
 
     base_client = fx_base_client[0]
     requests_adapter = fx_base_client[1]
 
     test_content = {"something": "else"}
 
     mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)
 
     requests_adapter.register_uri('PUT',
                                   mock_uri,
-                                  text=json_payload_callback)
+                                  status_code=200,
+                                  text=json.dumps({"content": test_content}))
 
     uri = "/playbooks/imports"
 
     r = base_client.put(
         uri,
-        test_content        
+        test_content
     )
 
-    assert json.loads(r['content']) == test_content
+    assert r['content'] == test_content
 
 #----
 def test_post_with_headers(fx_base_client):
-    def headers_callback(request, context):
-        context.status_code = 200
-        context.headers = request.headers
-        return json.dumps({ "content-type": request.headers["content-type"]})
 
     base_client = fx_base_client[0]
     requests_adapter = fx_base_client[1]
 
     test_headers = {"content-type": "application/octet-stream"}
 
     mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)    
 
     requests_adapter.register_uri('POST',
                                   mock_uri,
+                                  status_code=200,
                                   request_headers=test_headers,
-                                  text=headers_callback)
+                                  text=json.dumps(test_headers))
 
     uri = "/playbooks/imports"
 
     r = base_client.post(
         uri,
         "payload",
         headers=test_headers
     )
 
     assert r['content-type'] == test_headers['content-type']
 
 
 def test_post_with_text_payload(fx_base_client):
-    def text_payload_callback(request, context):
-        context.status_code = 200
-        context.headers = request.headers
-        return json.dumps({ "content": request.text})
 
     base_client = fx_base_client[0]
     requests_adapter = fx_base_client[1]
 
     test_content = 'abc'
 
     mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)    
 
     requests_adapter.register_uri('POST',
                                   mock_uri,
-                                  text=text_payload_callback)
+                                  status_code=200,
+                                  text=json.dumps({"content": test_content}))
 
     uri = "/playbooks/imports"
 
     r = base_client.post(
         uri,
         test_content        
     )
 
     assert r['content'] == test_content
 
 
 def test_post_with_json_payload(fx_base_client):
-    def json_payload_callback(request, context):
-        context.status_code = 200
-        context.headers = request.headers
-        return json.dumps({ "content": request.text})
 
     base_client = fx_base_client[0]
     requests_adapter = fx_base_client[1]
 
     test_content = {"something": "else"}
 
     mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)
 
     requests_adapter.register_uri('POST',
                                   mock_uri,
-                                  text=json_payload_callback)
+                                  status_code=200,
+                                  text=json.dumps({ "content": test_content}))
 
     uri = "/playbooks/imports"
 
     r = base_client.post(
         uri,
         test_content        
     )
 
-    assert json.loads(r['content']) == test_content
+    assert r['content'] == test_content
 
     
 def test_post_attachment_bytes_handle_retry(fx_base_client, caplog):
 
     incident_id = 1001
     base_client = fx_base_client[0]
     requests_adapter = fx_base_client[1]
```

### Comparing `resilient-48.1.4243/tests/test_finfo.py` & `resilient-48.2.4321/tests/test_finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tests/test_helpers.py` & `resilient-48.2.4321/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tests/xtest_gadget.py` & `resilient-48.2.4321/tests/xtest_gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tests/xtest_patch.py` & `resilient-48.2.4321/tests/xtest_patch.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tests/xtest_res_keyring.py` & `resilient-48.2.4321/tests/xtest_res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tools/res_utils.py` & `resilient-48.2.4321/tools/res_utils.py`

 * *Files identical despite different names*

### Comparing `resilient-48.1.4243/tox.ini` & `resilient-48.2.4321/tox.ini`

 * *Files identical despite different names*

