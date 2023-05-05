# Comparing `tmp/resilient_lib-48.1.4243.tar.gz` & `tmp/resilient_lib-48.2.4321.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_lib-48.1.4243.tar", last modified: Thu Apr 20 19:35:10 2023, max compression
+gzip compressed data, was "resilient_lib-48.2.4321.tar", last modified: Fri May  5 12:34:56 2023, max compression
```

## Comparing `resilient_lib-48.1.4243.tar` & `resilient_lib-48.2.4321.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6221 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.635501 resilient_lib-48.1.4243/resilient_lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      871 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/resilient_lib/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/function_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      573 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/integration_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26850 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/poller_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19335 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/requests_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24255 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/resilient_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/templates_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/components/workflow_status.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/resilient_lib/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5694 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/ui/tab.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/resilient_lib/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      410 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/resilient_lib/util/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.635501 resilient_lib-48.1.4243/resilient_lib.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-04-20 19:35:10.000000 resilient_lib-48.1.4243/resilient_lib.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/data/default_template.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/data/override_template.jinja
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/shared_mock_data/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/cert.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/key.open.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)      418 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_payload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12012 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_poller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31154 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_requests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:35:10.639501 resilient_lib-48.1.4243/tests/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5394 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/test_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2323 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/test_permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tests/ui/test_tab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      933 2023-04-20 19:34:28.000000 resilient_lib-48.1.4243/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6221 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      871 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/function_result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      573 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/integration_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26850 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/poller_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19335 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/requests_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24255 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/resilient_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/templates_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/components/workflow_status.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5694 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/ui/tab.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      410 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/resilient_lib/util/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/resilient_lib.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-05-05 12:34:56.000000 resilient_lib-48.2.4321/resilient_lib.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.499470 resilient_lib-48.2.4321/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      119 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/data/default_template.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/data/override_template.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/shared_mock_data/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/cert.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/key.open.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)      418 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_payload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12012 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_poller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31154 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_requests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:34:56.503470 resilient_lib-48.2.4321/tests/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5394 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/test_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2323 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/test_permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tests/ui/test_tab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      933 2023-05-05 12:33:36.000000 resilient_lib-48.2.4321/tox.ini
```

### Comparing `resilient_lib-48.1.4243/CHANGES` & `resilient_lib-48.2.4321/CHANGES`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/PKG-INFO` & `resilient_lib-48.2.4321/resilient_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resilient_lib
-Version: 48.1.4243
+Name: resilient-lib
+Version: 48.2.4321
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-48.1.4243/README.md` & `resilient_lib-48.2.4321/README.md`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/__init__.py` & `resilient_lib-48.2.4321/resilient_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/function_metrics.py` & `resilient_lib-48.2.4321/resilient_lib/components/function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/function_result.py` & `resilient_lib-48.2.4321/resilient_lib/components/function_result.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/html2markdown.py` & `resilient_lib-48.2.4321/resilient_lib/components/html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/integration_errors.py` & `resilient_lib-48.2.4321/resilient_lib/components/integration_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/oauth2_client_credentials_session.py` & `resilient_lib-48.2.4321/resilient_lib/components/oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/poller_common.py` & `resilient_lib-48.2.4321/resilient_lib/components/poller_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/requests_common.py` & `resilient_lib-48.2.4321/resilient_lib/components/requests_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/resilient_common.py` & `resilient_lib-48.2.4321/resilient_lib/components/resilient_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/templates_common.py` & `resilient_lib-48.2.4321/resilient_lib/components/templates_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/components/workflow_status.py` & `resilient_lib-48.2.4321/resilient_lib/components/workflow_status.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/ui/common.py` & `resilient_lib-48.2.4321/resilient_lib/ui/common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/ui/conditions.py` & `resilient_lib-48.2.4321/resilient_lib/ui/conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/ui/elements.py` & `resilient_lib-48.2.4321/resilient_lib/ui/elements.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/ui/tab.py` & `resilient_lib-48.2.4321/resilient_lib/ui/tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib/util/config.py` & `resilient_lib-48.2.4321/resilient_lib/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/resilient_lib.egg-info/PKG-INFO` & `resilient_lib-48.2.4321/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resilient-lib
-Version: 48.1.4243
+Name: resilient_lib
+Version: 48.2.4321
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-48.1.4243/resilient_lib.egg-info/SOURCES.txt` & `resilient_lib-48.2.4321/resilient_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/setup.cfg` & `resilient_lib-48.2.4321/setup.cfg`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/cert.pem` & `resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/cert.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/shared_mock_data/mock_certs/key.open.pem` & `resilient_lib-48.2.4321/tests/shared_mock_data/mock_certs/key.open.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/test_common.py` & `resilient_lib-48.2.4321/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/test_function_metrics.py` & `resilient_lib-48.2.4321/tests/test_function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/test_html2markdown.py` & `resilient_lib-48.2.4321/tests/test_html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/test_oauth2_client_credentials_session.py` & `resilient_lib-48.2.4321/tests/test_oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/test_payload.py` & `resilient_lib-48.2.4321/tests/test_payload.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/test_poller.py` & `resilient_lib-48.2.4321/tests/test_poller.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/test_requests.py` & `resilient_lib-48.2.4321/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/test_templates.py` & `resilient_lib-48.2.4321/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/ui/test_common.py` & `resilient_lib-48.2.4321/tests/ui/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/ui/test_conditions.py` & `resilient_lib-48.2.4321/tests/ui/test_conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/ui/test_permissions.py` & `resilient_lib-48.2.4321/tests/ui/test_permissions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tests/ui/test_tab.py` & `resilient_lib-48.2.4321/tests/ui/test_tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-48.1.4243/tox.ini` & `resilient_lib-48.2.4321/tox.ini`

 * *Files identical despite different names*

