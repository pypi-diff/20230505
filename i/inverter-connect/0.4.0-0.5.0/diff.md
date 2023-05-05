# Comparing `tmp/inverter-connect-0.4.0.tar.gz` & `tmp/inverter-connect-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.4.0.tar", last modified: Wed May  3 17:55:25 2023, max compression
+gzip compressed data, was "inverter-connect-0.5.0.tar", last modified: Fri May  5 20:06:42 2023, max compression
```

## Comparing `inverter-connect-0.4.0.tar` & `inverter-connect-0.5.0.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.4.0/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.4.0/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-03 17:50:50.000000 inverter-connect-0.4.0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.4.0/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)    13375 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)    12961 2023-05-03 17:42:44.000000 inverter-connect-0.4.0/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.4.0/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.4.0/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-03 17:43:39.000000 inverter-connect-0.4.0/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.4.0/inverter/__main__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4114 2023-04-28 11:04:08.000000 inverter-connect-0.4.0/inverter/api.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    11799 2023-05-03 17:27:43.000000 inverter-connect-0.4.0/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7864 2023-05-03 17:42:33.000000 inverter-connect-0.4.0/inverter/cli/dev.py
--rw-rw-r--   0 jens      (1000) users      (100)      276 2023-04-23 15:55:16.000000 inverter-connect-0.4.0/inverter/config.py
--rw-rw-r--   0 jens      (1000) users      (100)    10136 2023-04-28 11:07:05.000000 inverter-connect-0.4.0/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      261 2023-04-27 15:55:08.000000 inverter-connect-0.4.0/inverter/constants.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.4.0/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2784 2023-04-23 17:17:07.000000 inverter-connect-0.4.0/inverter/definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      429 2023-04-27 16:18:39.000000 inverter-connect-0.4.0/inverter/exceptions.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/test_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/test_doctests.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.4.0/inverter/mqtt4homeassistant/utilities/string_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     2460 2023-04-24 09:00:54.000000 inverter-connect-0.4.0/inverter/publish_loop.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.4.0/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3262 2023-04-24 15:18:26.000000 inverter-connect-0.4.0/inverter/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-27 15:42:06.000000 inverter-connect-0.4.0/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     1452 2023-04-23 17:17:07.000000 inverter-connect-0.4.0/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.4.0/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.4.0/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     3015 2023-05-03 17:43:47.000000 inverter-connect-0.4.0/inverter/tests/test_readme.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.4.0/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2179 2023-04-28 07:13:12.000000 inverter-connect-0.4.0/inverter/utilities/cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.4.0/inverter/utilities/credentials.py
--rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.4.0/inverter/utilities/log_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.4.0/inverter/utilities/modbus_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)    13375 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1575 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      259 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-03 17:55:25.000000 inverter-connect-0.4.0/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4774 2023-05-03 17:23:48.000000 inverter-connect-0.4.0/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    50591 2023-04-27 17:07:50.000000 inverter-connect-0.4.0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     5305 2023-04-27 17:07:31.000000 inverter-connect-0.4.0/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-03 17:55:25.379229 inverter-connect-0.4.0/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.5.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.5.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.827138 inverter-connect-0.5.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.827138 inverter-connect-0.5.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-03 17:50:50.000000 inverter-connect-0.5.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.5.0/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)    15040 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)    14626 2023-05-05 19:51:29.000000 inverter-connect-0.5.0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.5.0/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.5.0/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.827138 inverter-connect-0.5.0/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-05 20:00:24.000000 inverter-connect-0.5.0/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.5.0/inverter/__main__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4771 2023-05-05 20:00:11.000000 inverter-connect-0.5.0/inverter/api.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    13143 2023-05-05 19:50:36.000000 inverter-connect-0.5.0/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7864 2023-05-03 17:42:33.000000 inverter-connect-0.5.0/inverter/cli/dev.py
+-rw-rw-r--   0 jens      (1000) users      (100)      480 2023-05-05 17:29:20.000000 inverter-connect-0.5.0/inverter/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)    10438 2023-05-05 14:42:51.000000 inverter-connect-0.5.0/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      261 2023-04-27 15:55:08.000000 inverter-connect-0.5.0/inverter/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1963 2023-05-05 19:06:27.000000 inverter-connect-0.5.0/inverter/daily_reset.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.5.0/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2784 2023-04-23 17:17:07.000000 inverter-connect-0.5.0/inverter/definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      429 2023-04-27 16:18:39.000000 inverter-connect-0.5.0/inverter/exceptions.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/test_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/test_doctests.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/utilities/string_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2943 2023-05-05 19:48:37.000000 inverter-connect-0.5.0/inverter/publish_loop.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.5.0/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3262 2023-04-24 15:18:26.000000 inverter-connect-0.5.0/inverter/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-27 15:42:06.000000 inverter-connect-0.5.0/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5897 2023-05-05 19:10:09.000000 inverter-connect-0.5.0/inverter/tests/test_daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1452 2023-04-23 17:17:07.000000 inverter-connect-0.5.0/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.5.0/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3422 2023-05-05 19:51:25.000000 inverter-connect-0.5.0/inverter/tests/test_readme.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.5.0/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2179 2023-04-28 07:13:12.000000 inverter-connect-0.5.0/inverter/utilities/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.5.0/inverter/utilities/credentials.py
+-rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.5.0/inverter/utilities/log_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.5.0/inverter/utilities/modbus_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    15040 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1634 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      269 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4830 2023-05-05 18:27:54.000000 inverter-connect-0.5.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    50845 2023-05-05 18:28:31.000000 inverter-connect-0.5.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     5305 2023-05-05 18:28:07.000000 inverter-connect-0.5.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/setup.cfg
```

### Comparing `inverter-connect-0.4.0/.github/workflows/tests.yml` & `inverter-connect-0.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/PKG-INFO` & `inverter-connect-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.4.0
+Version: 0.5.0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -42,31 +42,58 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ debug-settings              Display (anonymized) MQTT server username and password               │
-│ print-at-commands           Print one or more AT command values from Inverter.                   │
-│ print-values                Print all known register values from Inverter, e.g.:                 │
-│ publish-loop                Publish current data via MQTT (endless loop)                         │
-│ read-register               Read register(s) from the inverter                                   │
-│ set-time                    Set current date time in the inverter device.                        │
-│ store-settings              Store MQTT server settings.                                          │
-│ test-mqtt-connection        Test connection to MQTT Server                                       │
-│ version                     Print version and exit                                               │
+│ debug-settings           Display (anonymized) MQTT server username and password                  │
+│ print-at-commands        Print one or more AT command values from Inverter.                      │
+│ print-values             Print all known register values from Inverter, e.g.:                    │
+│ publish-loop             Publish current data via MQTT for Home Assistant (endless loop)         │
+│ read-register            Read register(s) from the inverter                                      │
+│ set-time                 Set current date time in the inverter device.                           │
+│ store-settings           Store MQTT server settings.                                             │
+│ test-mqtt-connection     Test connection to MQTT Server                                          │
+│ version                  Print version and exit                                                  │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 # most important commands
 
 
+## publish-loop
+
+Help from `./cli.py print-values --help` Looks like:
+
+[comment]: <> (✂✂✂ auto generated publish-loop help start ✂✂✂)
+```
+Usage: ./cli.py publish-loop [OPTIONS] IP
+
+ Publish current data via MQTT for Home Assistant (endless loop)
+ The "Daily Production" count will be cleared in the night, by set the current date time via
+ AT-command.
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
+│                                                           [default: 48899; 1000<=x<=65535]       │
+│ --log/--no-log                                            [default: log]                         │
+│ --verbose/--no-verbose                                    [default: verbose]                     │
+│ --debug/--no-debug                                        [default: no-debug]                    │
+│ --help                                                    Show this message and exit.            │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated publish-loop help end ✂✂✂)
+
+
+----
+
+
 ## print-values
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
 Usage: ./cli.py print-values [OPTIONS] IP
```

### Comparing `inverter-connect-0.4.0/README.md` & `inverter-connect-0.5.0/inverter_connect.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: inverter-connect
+Version: 0.5.0
+Summary: Get information from Deye Microinverter
+Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
+License: GPL-3.0-or-later
+Project-URL: Documentation, https://github.com/jedie/inverter-connect
+Project-URL: Source, https://github.com/jedie/inverter-connect
+Requires-Python: <4,>=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
@@ -30,31 +42,58 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ debug-settings              Display (anonymized) MQTT server username and password               │
-│ print-at-commands           Print one or more AT command values from Inverter.                   │
-│ print-values                Print all known register values from Inverter, e.g.:                 │
-│ publish-loop                Publish current data via MQTT (endless loop)                         │
-│ read-register               Read register(s) from the inverter                                   │
-│ set-time                    Set current date time in the inverter device.                        │
-│ store-settings              Store MQTT server settings.                                          │
-│ test-mqtt-connection        Test connection to MQTT Server                                       │
-│ version                     Print version and exit                                               │
+│ debug-settings           Display (anonymized) MQTT server username and password                  │
+│ print-at-commands        Print one or more AT command values from Inverter.                      │
+│ print-values             Print all known register values from Inverter, e.g.:                    │
+│ publish-loop             Publish current data via MQTT for Home Assistant (endless loop)         │
+│ read-register            Read register(s) from the inverter                                      │
+│ set-time                 Set current date time in the inverter device.                           │
+│ store-settings           Store MQTT server settings.                                             │
+│ test-mqtt-connection     Test connection to MQTT Server                                          │
+│ version                  Print version and exit                                                  │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 # most important commands
 
 
+## publish-loop
+
+Help from `./cli.py print-values --help` Looks like:
+
+[comment]: <> (✂✂✂ auto generated publish-loop help start ✂✂✂)
+```
+Usage: ./cli.py publish-loop [OPTIONS] IP
+
+ Publish current data via MQTT for Home Assistant (endless loop)
+ The "Daily Production" count will be cleared in the night, by set the current date time via
+ AT-command.
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
+│                                                           [default: 48899; 1000<=x<=65535]       │
+│ --log/--no-log                                            [default: log]                         │
+│ --verbose/--no-verbose                                    [default: verbose]                     │
+│ --debug/--no-debug                                        [default: no-debug]                    │
+│ --help                                                    Show this message and exit.            │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated publish-loop help end ✂✂✂)
+
+
+----
+
+
 ## print-values
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
 Usage: ./cli.py print-values [OPTIONS] IP
```

### Comparing `inverter-connect-0.4.0/cli.py` & `inverter-connect-0.5.0/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/dev-cli.py` & `inverter-connect-0.5.0/dev-cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/.github/workflows/tests.yml` & `inverter-connect-0.5.0/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/api.py` & `inverter-connect-0.5.0/inverter/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 import logging
 from collections.abc import Iterable
+from datetime import datetime
 from enum import Enum
 
 from rich import print  # noqa
 
 from inverter.config import Config
 from inverter.connection import InverterSock, ModbusReadResult
 from inverter.definitions import get_parameter
@@ -125,7 +126,31 @@
         if values := compute_values(values):
             yield from values
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.inv_sock.__exit__(exc_type, exc_val, exc_tb)
         if exc_type:
             return False
+
+
+def set_current_time(inv_sock: InverterSock, address=0x16, verbose=True):
+    """
+    Set current date time in the inverter device.
+
+    Default start address is 0x16, so that this will be filled:
+        0x16 - year + month
+        0x17 - day + hour
+        0x18 - minute + second
+    """
+    now = datetime.now()
+    if verbose:
+        print(f'Send current time: {now}')
+
+    values = [
+        256 * (now.year % 100) + now.month,
+        256 * now.day + now.hour,
+        256 * now.minute + now.second,
+    ]
+    data = inv_sock.write(address=address, values=values)
+
+    if verbose:
+        print(f'Response: {data!r}')
```

### Comparing `inverter-connect-0.4.0/inverter/cli/cli_app.py` & `inverter-connect-0.5.0/inverter/cli/cli_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
     CLI for usage
 """
-import datetime
 import getpass
 import logging
 import sys
 import time
 from pathlib import Path
 
 import rich_click as click
 from bx_py_utils.path import assert_is_file
 from rich import print  # noqa
 from rich.pretty import pprint
 from rich_click import RichGroup
 
 import inverter
 from inverter import constants
-from inverter.api import Inverter, ValueType
+from inverter.api import Inverter, ValueType, set_current_time
 from inverter.config import Config
 from inverter.connection import InverterInfo, InverterSock
 from inverter.constants import ERROR_STR_NO_DATA
 from inverter.definitions import Parameter
 from inverter.mqtt4homeassistant.data_classes import MqttSettings
 from inverter.mqtt4homeassistant.mqtt import get_connected_client
 from inverter.publish_loop import publish_forever
@@ -155,27 +154,55 @@
 
     (Note: The prefix "AT+" will be added to every command)
     """
     basic_log_setup(debug=debug)
 
     if not commands:
         commands = (
-            'WANN',
-            'WEBVER',
-            'WEBU',
-            'WAP',
-            'WSSSID',
-            'WSKEY',
+            # 'KEY',  # Set/Get Device Password
+            'VER',
+            'BVER',  # bootloader version
+            'HWVER',  # hardware version
+            'WEBVER',  # web version
+            'YZVER',  # Firmware version
+            'PING',
+            # 'YZWAKEYCTL',
+            # 'YZLOG',
+            # 'YZAPP',
+            # 'YZAPSTAT',
+            # 'YZEXPFUN',
+            # 'MID',
+            #
+            # 'CFGRD',  # current system config
+            # 'SMEM',  # system memory stat
+            'TIME',
+            # 'ADDRESS', # Set/Get Device Address
+            # 'KEY',
+            'NDBGS',  # Set/Get Debug Status
+            'WIFI',  # Set/Get WIFI status: Power up: "WIFI=UP" Power down: "WIFI=DOWN"
+            'WMODE',  # Set/Get the WIFI Operation Mode (AP or STA)
+            'WEBU',  # Set/Get the Login Parameters of WEB page
+            'WAP',  # Set/Get the AP parameters
+            'WSSSID',  # Set/Get the AP's SSID of WIFI STA Mode
+            'WSKEY',  # Set/Get the Security Parameters of WIFI STA Mode
+            'WAKEY',  # Set/Get the Security Parameters of WIFI AP Mode
+            # 'TXPWR',  # Set/Get wifi rf tx power'
+            'WANN',  # Set/Get The WAN setting if in STA mode.
+            'LANN',  # Set/Get The LAN setting if in ADHOC mode.
+            'UPURL',  # Set/Get the path of remote upgrade
             'YZAPP',
-            'UPURL',
-            'WAPMXSTA',  # max. number of wifi clients
+            'WAPMXSTA',  # Set/Get the Max Number Of Sta Connected to Ap
+            # 'WSCAN',  # Get The AP site Survey (only for STA Mode).
             'NTPTM',  # NTP date time? e.g.: "1970-1-1  0:3:9  Thur"
             'NTPSER',  # set/query NTP server, e.g.: "NTPSER=192.168.1.1"
             'NTPRF',  # NTP request interval in min (?)
-            'NTPEN',  # NTP enabled?
+            'NTPEN',  # Enable/Disable NTP Server
+            'WSDNS',  # Set/Get the DNS Server address
+            'DEVICENUM',  # Set/Get Device Link Num
+            'DEVSELCTL',  # Set/Get Web Device List Info
         )
 
     config = Config(yaml_filename=None, host=ip, port=port, debug=debug)
     if debug:
         print(config)
 
     with InverterSock(config) as inv_sock:
@@ -215,23 +242,15 @@
         print(config)
 
     with InverterSock(config) as inv_sock:
         inverter_info: InverterInfo = inv_sock.inverter_info
         print(inverter_info)
         print()
 
-        now = datetime.datetime.now()
-        print(f'Send current time: {now}')
-        values = [
-            256 * (now.year % 100) + now.month,
-            256 * now.day + now.hour,
-            256 * now.minute + now.second,
-        ]
-        data = inv_sock.write(address=address, values=values)
-        print(f'Response: {data!r}')
+        set_current_time(inv_sock=inv_sock, address=address, verbose=True)
 
         print('\nRead register...')
         time.sleep(1)
         print_register(inv_sock, start_register=address, length=3)
 
         print('\nCheck time by request "AT+NTPTM"', end='...')
         time.sleep(1)
@@ -364,15 +383,18 @@
     '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
 )
 @click.option('--log/--no-log', **OPTION_ARGS_DEFAULT_TRUE)
 @click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
 @click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
 def publish_loop(ip, port, log, verbose, debug):
     """
-    Publish current data via MQTT (endless loop)
+    Publish current data via MQTT for Home Assistant (endless loop)
+
+    The "Daily Production" count will be cleared in the night,
+    by set the current date time via AT-command.
     """
     if log:
         basic_log_setup(debug=debug)
 
     config = Config(yaml_filename='deye_2mppt.yaml', host=ip, port=port, debug=debug)
 
     mqtt_settings: MqttSettings = get_mqtt_settings()
```

### Comparing `inverter-connect-0.4.0/inverter/cli/dev.py` & `inverter-connect-0.5.0/inverter/cli/dev.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/connection.py` & `inverter-connect-0.5.0/inverter/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,28 +133,33 @@
 
 def parse_response(data: bytes) -> RawModBusResponse:
     """
     >>> parse_response(b'+ok=01\x1003\x1004\x1001\x105E\x1000\x1000\x109A\x101D\x10\\r\\n\\r\\n')
     RawModBusResponse(prefix='+ok', data='010304015E00009A1D')
     """
     logger.debug(f'parse_response({data=})')
-    data = data.decode('ASCII')
-    data = data.rstrip('\r\n')
-    data = data.replace('\x10', '')  # FIXME
-    logger.debug(f'{data=}')
-
-    if data == '+ok':
-        result = RawModBusResponse(prefix=data, data='')
+    try:
+        data = data.decode('ASCII')
+    except UnicodeDecodeError as err:
+        logger.warning(f'Non ASCII: {data=} ({err})')
+        result = RawModBusResponse(prefix='', data=data)
     else:
-        try:
-            prefix, data = data.split('=', 1)
-        except ValueError as err:
-            raise ValueError(f'{data=}: {err}')
-
-        result = RawModBusResponse(prefix=prefix, data=data)
+        data = data.rstrip('\r\n')
+        data = data.replace('\x10', '')  # FIXME
+        logger.debug(f'{data=}')
+        if data == '+ok':
+            result = RawModBusResponse(prefix=data, data='')
+        else:
+            try:
+                prefix, data = data.split('=', 1)
+            except ValueError:
+                logger.warning(f'Unexpected data: {data=}')
+                result = RawModBusResponse(prefix='', data=data)
+            else:
+                result = RawModBusResponse(prefix=prefix, data=data)
     logger.debug('%s', result)
     return result
 
 
 def parse_modbus_response(data: str) -> ModbusResponse:
     logger.debug(f'parse_modbus_response({data=})')
     if data == ERROR_STR_NO_DATA:
```

### Comparing `inverter-connect-0.4.0/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.5.0/inverter/definitions/deye_2mppt.yaml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/definitions.py` & `inverter-connect-0.5.0/inverter/definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/mqtt4homeassistant/converter.py` & `inverter-connect-0.5.0/inverter/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/mqtt4homeassistant/data_classes.py` & `inverter-connect-0.5.0/inverter/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/mqtt4homeassistant/mqtt.py` & `inverter-connect-0.5.0/inverter/mqtt4homeassistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/mqtt4homeassistant/tests/test_converter.py` & `inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/tests/test_api.py` & `inverter-connect-0.5.0/inverter/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/tests/test_connect.py` & `inverter-connect-0.5.0/inverter/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/tests/test_definitions.py` & `inverter-connect-0.5.0/inverter/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/tests/test_project_setup.py` & `inverter-connect-0.5.0/inverter/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/tests/test_readme.py` & `inverter-connect-0.5.0/inverter/tests/test_readme.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,26 @@
                 'fix-code-style',
                 'tox',
                 constants.CLI_EPILOG,
             ),
         )
         assert_cli_help_in_readme(text_block=stdout, marker='dev help')
 
+    def test_publish_loop_help(self):
+        stdout = invoke_click(cli, 'publish-loop', '--help')
+        self.assert_in_content(
+            got=stdout,
+            parts=(
+                'Usage: ./cli.py publish-loop [OPTIONS] IP',
+                '--port',
+                '--debug/--no-debug',
+            ),
+        )
+        assert_cli_help_in_readme(text_block=stdout, marker='publish-loop help')
+
     def test_print_values_help(self):
         stdout = invoke_click(cli, 'print-values', '--help')
         self.assert_in_content(
             got=stdout,
             parts=(
                 'Usage: ./cli.py print-values [OPTIONS] IP',
                 '--port',
```

### Comparing `inverter-connect-0.4.0/inverter/utilities/cli.py` & `inverter-connect-0.5.0/inverter/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/utilities/credentials.py` & `inverter-connect-0.5.0/inverter/utilities/credentials.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter/utilities/modbus_converter.py` & `inverter-connect-0.5.0/inverter/utilities/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.4.0/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: inverter-connect
-Version: 0.4.0
-Summary: Get information from Deye Microinverter
-Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
-License: GPL-3.0-or-later
-Project-URL: Documentation, https://github.com/jedie/inverter-connect
-Project-URL: Source, https://github.com/jedie/inverter-connect
-Requires-Python: <4,>=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
@@ -42,31 +30,58 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ debug-settings              Display (anonymized) MQTT server username and password               │
-│ print-at-commands           Print one or more AT command values from Inverter.                   │
-│ print-values                Print all known register values from Inverter, e.g.:                 │
-│ publish-loop                Publish current data via MQTT (endless loop)                         │
-│ read-register               Read register(s) from the inverter                                   │
-│ set-time                    Set current date time in the inverter device.                        │
-│ store-settings              Store MQTT server settings.                                          │
-│ test-mqtt-connection        Test connection to MQTT Server                                       │
-│ version                     Print version and exit                                               │
+│ debug-settings           Display (anonymized) MQTT server username and password                  │
+│ print-at-commands        Print one or more AT command values from Inverter.                      │
+│ print-values             Print all known register values from Inverter, e.g.:                    │
+│ publish-loop             Publish current data via MQTT for Home Assistant (endless loop)         │
+│ read-register            Read register(s) from the inverter                                      │
+│ set-time                 Set current date time in the inverter device.                           │
+│ store-settings           Store MQTT server settings.                                             │
+│ test-mqtt-connection     Test connection to MQTT Server                                          │
+│ version                  Print version and exit                                                  │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 # most important commands
 
 
+## publish-loop
+
+Help from `./cli.py print-values --help` Looks like:
+
+[comment]: <> (✂✂✂ auto generated publish-loop help start ✂✂✂)
+```
+Usage: ./cli.py publish-loop [OPTIONS] IP
+
+ Publish current data via MQTT for Home Assistant (endless loop)
+ The "Daily Production" count will be cleared in the night, by set the current date time via
+ AT-command.
+
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
+│                                                           [default: 48899; 1000<=x<=65535]       │
+│ --log/--no-log                                            [default: log]                         │
+│ --verbose/--no-verbose                                    [default: verbose]                     │
+│ --debug/--no-debug                                        [default: no-debug]                    │
+│ --help                                                    Show this message and exit.            │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+[comment]: <> (✂✂✂ auto generated publish-loop help end ✂✂✂)
+
+
+----
+
+
 ## print-values
 
 Help from `./cli.py print-values --help` Looks like:
 
 [comment]: <> (✂✂✂ auto generated print-values help start ✂✂✂)
 ```
 Usage: ./cli.py print-values [OPTIONS] IP
```

### Comparing `inverter-connect-0.4.0/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.5.0/inverter_connect.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 inverter/.gitignore
 inverter/__init__.py
 inverter/__main__.py
 inverter/api.py
 inverter/config.py
 inverter/connection.py
 inverter/constants.py
+inverter/daily_reset.py
 inverter/definitions.py
 inverter/exceptions.py
 inverter/publish_loop.py
 inverter/.github/workflows/tests.yml
 inverter/cli/__init__.py
 inverter/cli/cli_app.py
 inverter/cli/dev.py
@@ -33,14 +34,15 @@
 inverter/mqtt4homeassistant/tests/test_converter.py
 inverter/mqtt4homeassistant/tests/test_doctests.py
 inverter/mqtt4homeassistant/utilities/__init__.py
 inverter/mqtt4homeassistant/utilities/string_utils.py
 inverter/tests/__init__.py
 inverter/tests/test_api.py
 inverter/tests/test_connect.py
+inverter/tests/test_daily_reset.py
 inverter/tests/test_definitions.py
 inverter/tests/test_doctests.py
 inverter/tests/test_project_setup.py
 inverter/tests/test_readme.py
 inverter/utilities/__init__.py
 inverter/utilities/cli.py
 inverter/utilities/credentials.py
```

### Comparing `inverter-connect-0.4.0/pyproject.toml` & `inverter-connect-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
 ]
 [project.optional-dependencies]
 dev = [
+    "freezegun",  # https://github.com/spulec/freezegun
     "manageprojects",  # https://github.com/jedie/manageprojects
     "pip-tools",  # https://github.com/jazzband/pip-tools/
     "tox",  # https://github.com/tox-dev/tox
     "coverage",  # https://github.com/nedbat/coveragepy
     "autopep8",  # https://github.com/hhatto/autopep8
     "pyupgrade",  # https://github.com/asottile/pyupgrade
     "flake8",  # https://github.com/pycqa/flake8
```

### Comparing `inverter-connect-0.4.0/requirements.dev.txt` & `inverter-connect-0.5.0/requirements.dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -237,66 +237,66 @@
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via tox
 cookiecutter==2.1.1 \
     --hash=sha256:9f3ab027cec4f70916e28f03470bdb41e637a3ad354b4d65c765d93aad160022 \
     --hash=sha256:f3982be8d9c53dac1261864013fdec7f83afd2e42ede6f6dd069c5e149c540d5
     # via manageprojects
-coverage==7.2.3 \
-    --hash=sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93 \
-    --hash=sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013 \
-    --hash=sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f \
-    --hash=sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21 \
-    --hash=sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462 \
-    --hash=sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc \
-    --hash=sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df \
-    --hash=sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1 \
-    --hash=sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235 \
-    --hash=sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934 \
-    --hash=sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9 \
-    --hash=sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1 \
-    --hash=sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48 \
-    --hash=sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4 \
-    --hash=sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe \
-    --hash=sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a \
-    --hash=sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b \
-    --hash=sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21 \
-    --hash=sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d \
-    --hash=sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa \
-    --hash=sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367 \
-    --hash=sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535 \
-    --hash=sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152 \
-    --hash=sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e \
-    --hash=sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539 \
-    --hash=sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1 \
-    --hash=sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925 \
-    --hash=sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0 \
-    --hash=sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2 \
-    --hash=sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab \
-    --hash=sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841 \
-    --hash=sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30 \
-    --hash=sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91 \
-    --hash=sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c \
-    --hash=sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257 \
-    --hash=sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9 \
-    --hash=sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040 \
-    --hash=sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911 \
-    --hash=sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623 \
-    --hash=sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259 \
-    --hash=sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c \
-    --hash=sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79 \
-    --hash=sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5 \
-    --hash=sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4 \
-    --hash=sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4 \
-    --hash=sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22 \
-    --hash=sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd \
-    --hash=sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1 \
-    --hash=sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910 \
-    --hash=sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859 \
-    --hash=sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312
+coverage==7.2.5 \
+    --hash=sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3 \
+    --hash=sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a \
+    --hash=sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813 \
+    --hash=sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0 \
+    --hash=sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a \
+    --hash=sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd \
+    --hash=sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139 \
+    --hash=sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b \
+    --hash=sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252 \
+    --hash=sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790 \
+    --hash=sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045 \
+    --hash=sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce \
+    --hash=sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200 \
+    --hash=sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718 \
+    --hash=sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b \
+    --hash=sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f \
+    --hash=sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5 \
+    --hash=sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade \
+    --hash=sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5 \
+    --hash=sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a \
+    --hash=sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8 \
+    --hash=sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33 \
+    --hash=sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e \
+    --hash=sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c \
+    --hash=sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3 \
+    --hash=sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969 \
+    --hash=sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068 \
+    --hash=sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2 \
+    --hash=sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771 \
+    --hash=sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed \
+    --hash=sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212 \
+    --hash=sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614 \
+    --hash=sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88 \
+    --hash=sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3 \
+    --hash=sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c \
+    --hash=sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84 \
+    --hash=sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11 \
+    --hash=sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1 \
+    --hash=sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1 \
+    --hash=sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e \
+    --hash=sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1 \
+    --hash=sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd \
+    --hash=sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47 \
+    --hash=sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a \
+    --hash=sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c \
+    --hash=sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31 \
+    --hash=sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5 \
+    --hash=sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6 \
+    --hash=sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303 \
+    --hash=sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5 \
+    --hash=sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47
     # via inverter-connect (pyproject.toml)
 cryptography==40.0.2 \
     --hash=sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440 \
     --hash=sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288 \
     --hash=sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b \
     --hash=sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958 \
     --hash=sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b \
@@ -345,14 +345,18 @@
     --hash=sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7 \
     --hash=sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181
     # via inverter-connect (pyproject.toml)
 flynt==0.77 \
     --hash=sha256:2863ac8ec19d6ec8d29e760546e6ced644baf6dff3c7cdc77e03abbd29b80f14 \
     --hash=sha256:2bd1b37043ad88a3f3c3c34a76fc0b64d24e5f03d36ea6b48cb69cc642bff17e
     # via darker
+freezegun==1.2.2 \
+    --hash=sha256:cd22d1ba06941384410cd967d8a99d5ae2442f57dfafeff2fda5de8dc5c05446 \
+    --hash=sha256:ea1b963b993cb9ea195adbd893a48d573fda951b0da64f60883d7e988b606c9f
+    # via inverter-connect (pyproject.toml)
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
 importlib-metadata==6.6.0 \
     --hash=sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed \
     --hash=sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705
@@ -559,15 +563,17 @@
 pyproject-hooks==1.0.0 \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
     # via build
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
-    # via arrow
+    # via
+    #   arrow
+    #   freezegun
 python-slugify==8.0.1 \
     --hash=sha256:70ca6ea68fe63ecc8fa4fcf00ae651fc8a5d02d93dcd12ae6d4fc7ca46c4d395 \
     --hash=sha256:ce0d46ddb668b3be82f4ed5e503dbc33dd815d83e2eb6824211310d3fb172a27
     # via cookiecutter
 pyupgrade==3.3.2 \
     --hash=sha256:bcfed63d38811809f179fd269dec246680b0aaa5bbe662b535826e5fa2275219 \
     --hash=sha256:c05b82c911934b3a638b29f48f48dc6e0ef6c57c55ec36f2b41ae9dbf6711b4b
@@ -616,25 +622,25 @@
     # via
     #   cookiecutter
     #   inverter-connect (pyproject.toml)
 readme-renderer==37.3 \
     --hash=sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273 \
     --hash=sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343
     # via twine
-requests==2.29.0 \
-    --hash=sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b \
-    --hash=sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059
+requests==2.30.0 \
+    --hash=sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294 \
+    --hash=sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4
     # via
     #   cookiecutter
     #   requests-toolbelt
     #   safety
     #   twine
-requests-toolbelt==0.10.1 \
-    --hash=sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7 \
-    --hash=sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d
+requests-toolbelt==1.0.0 \
+    --hash=sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6 \
+    --hash=sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06
     # via twine
 rfc3986==2.0.0 \
     --hash=sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd \
     --hash=sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c
     # via twine
 rich==13.3.5 \
     --hash=sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c \
@@ -646,17 +652,17 @@
     #   twine
 rich-click==1.6.1 \
     --hash=sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95 \
     --hash=sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e
     # via
     #   inverter-connect (pyproject.toml)
     #   manageprojects
-ruamel-yaml==0.17.21 \
-    --hash=sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7 \
-    --hash=sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af
+ruamel-yaml==0.17.23 \
+    --hash=sha256:40e549c264e799d8e4cd9e54e869ffa60c9436e1ef497500b08fbda3b92a1517 \
+    --hash=sha256:605510839d5af3ae730f3ed6408b7004c83f97aa2b732f6f366da7c2fc2f0d9c
     # via safety
 ruamel-yaml-clib==0.2.7 \
     --hash=sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e \
     --hash=sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3 \
     --hash=sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5 \
     --hash=sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497 \
     --hash=sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f \
@@ -745,23 +751,23 @@
     --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
     --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
     # via inverter-connect (pyproject.toml)
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via mypy
-urllib3==1.26.15 \
-    --hash=sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305 \
-    --hash=sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42
+urllib3==2.0.2 \
+    --hash=sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc \
+    --hash=sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e
     # via
     #   requests
     #   twine
-virtualenv==20.22.0 \
-    --hash=sha256:278753c47aaef1a0f14e6db8a4c5e1e040e90aea654d0fc1dc7e0d8a42616cc3 \
-    --hash=sha256:48fd3b907b5149c5aab7c23d9790bea4cac6bc6b150af8635febc4cfeab1275a
+virtualenv==20.23.0 \
+    --hash=sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e \
+    --hash=sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924
     # via tox
 webencodings==0.5.1 \
     --hash=sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78 \
     --hash=sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923
     # via bleach
 wheel==0.40.0 \
     --hash=sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873 \
```

### Comparing `inverter-connect-0.4.0/requirements.txt` & `inverter-connect-0.5.0/requirements.txt`

 * *Files identical despite different names*

