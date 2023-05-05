# Comparing `tmp/dev-gpt-0.18.37.dev51.tar.gz` & `tmp/dev-gpt-0.18.37.dev52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.37.dev51.tar", last modified: Fri May  5 01:03:28 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.37.dev52.tar", last modified: Fri May  5 01:25:23 2023, max compression
```

## Comparing `dev-gpt-0.18.37.dev51.tar` & `dev-gpt-0.18.37.dev52.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/templates_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/dev_gpt/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/dev_gpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/unit/test_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20256 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 01:25:22.000000 dev-gpt-0.18.37.dev52/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/templates_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/unit/test_strings.py
```

### Comparing `dev-gpt-0.18.37.dev51/LICENSE` & `dev-gpt-0.18.37.dev52/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/PKG-INFO` & `dev-gpt-0.18.37.dev52/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.37.dev51
+Version: 0.18.37.dev52
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -69,32 +69,32 @@
     <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
 </a>
 
 </p>
 
 Welcome to Dev GPT, where we bring your ideas to life with the power of advanced artificial intelligence! Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
 
-[//]: # ([![Watch the video]&#40;res/thumbnail.png&#41;]&#40;https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4&#41;)
-
-
-
-
 ## Quickstart
-### Requirements
-- OpenAI key with access to GPT-3.5 or GPT-4 
 
-### Installation
 ```bash
 pip install dev-gpt
+dev-gpt generate
+```
+
+### Requirements
+- OpenAI key with access to GPT-3.5 or GPT-4
+```bash
 dev-gpt configure --key <your openai api key>
 ```
+
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
+## Docs
 ### Generate Microservice
 ```bash
 dev-gpt generate \
 --description "<description of the microservice>" \
 --model <gpt-3.5 or gpt-4> \
 --path </path/to/local/folder>
 ```
@@ -112,24 +112,22 @@
 ### Run Microservice
 Run the microservice locally in docker. In case docker is not running on your machine, it will try to run it without docker.
 With this command a playground opens in your browser where you can test the microservice.
 ```bash
 dev-gpt run --path <path to microservice>
 ```
 
-
 ### Deploy Microservice
 If you want to deploy your microservice to the cloud a [Jina account](https://cloud.jina.ai/) is required.
 When creating a Jina account, you get some free credits, which you can use to deploy your microservice ($0.025/hour).
 If you run out of credits, you can purchase more.
 ```bash
 dev-gpt deploy --microservice_path <path to microservice>
 ```
 
-
 ### Delete Microservice
 To save credits you can delete your microservice via the following commands:
 ```bash
 jc list # get the microservice id
 jc delete <microservice id>
 ```
 
@@ -140,15 +138,14 @@
 ```bash
 dev-gpt generate \
 --description "The user writes something and gets a related deep compliment." \
 --model gpt-4
 ```
 <img src="res/compliment_example.png" alt="Compliment Generator" width="400" />
 
-
 ### Extract and summarize news articles given a URL
 ```bash
 dev-gpt generate \
 --description "Extract text from a news article URL using Newspaper3k library and generate a summary using gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-pot-guns-and-drones/" \
 --model gpt-4
 ```
 <img src="res/news_article_example.png" alt="News Article Example" width="400" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev51 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev52 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -17,23 +17,21 @@
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
                      platforms] [Downloads] [Discord_Chat]
 Welcome to Dev GPT, where we bring your ideas to life with the power of
 advanced artificial intelligence! Our automated development team is designed to
 create microservices tailored to your specific needs, making your software
 development process seamless and efficient. Comprised of a virtual Product
 Manager, Developer, and DevOps, our AI team ensures that every aspect of your
-project is covered, from concept to deployment. [//]: # ([![Watch the video]
-(res/thumbnail.png)](https://user-images.githubusercontent.com/11627845/
-231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4)) ## Quickstart ###
-Requirements - OpenAI key with access to GPT-3.5 or GPT-4 ### Installation
-```bash pip install dev-gpt dev-gpt configure --key  ``` If you set the
+project is covered, from concept to deployment. ## Quickstart ```bash pip
+install dev-gpt dev-gpt generate ``` ### Requirements - OpenAI key with access
+to GPT-3.5 or GPT-4 ```bash dev-gpt configure --key  ``` If you set the
 environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. We are working on a
-way to use gpt-3.5-turbo as well. ### Generate Microservice ```bash dev-gpt
-generate \ --description "" \ --model
+way to use gpt-3.5-turbo as well. ## Docs ### Generate Microservice ```bash
+dev-gpt generate \ --description "" \ --model
 5 or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x
 cheaper, but will not be able to generate as complex microservices. (default:
 largest you have access to) - A `path` on the local drive where the
 microservice will be generated. (default: ./microservice) The creation process
```

### Comparing `dev-gpt-0.18.37.dev51/README.md` & `dev-gpt-0.18.37.dev52/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,32 +49,32 @@
     <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
 </a>
 
 </p>
 
 Welcome to Dev GPT, where we bring your ideas to life with the power of advanced artificial intelligence! Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
 
-[//]: # ([![Watch the video]&#40;res/thumbnail.png&#41;]&#40;https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4&#41;)
-
-
-
-
 ## Quickstart
-### Requirements
-- OpenAI key with access to GPT-3.5 or GPT-4 
 
-### Installation
 ```bash
 pip install dev-gpt
+dev-gpt generate
+```
+
+### Requirements
+- OpenAI key with access to GPT-3.5 or GPT-4
+```bash
 dev-gpt configure --key <your openai api key>
 ```
+
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
+## Docs
 ### Generate Microservice
 ```bash
 dev-gpt generate \
 --description "<description of the microservice>" \
 --model <gpt-3.5 or gpt-4> \
 --path </path/to/local/folder>
 ```
@@ -92,24 +92,22 @@
 ### Run Microservice
 Run the microservice locally in docker. In case docker is not running on your machine, it will try to run it without docker.
 With this command a playground opens in your browser where you can test the microservice.
 ```bash
 dev-gpt run --path <path to microservice>
 ```
 
-
 ### Deploy Microservice
 If you want to deploy your microservice to the cloud a [Jina account](https://cloud.jina.ai/) is required.
 When creating a Jina account, you get some free credits, which you can use to deploy your microservice ($0.025/hour).
 If you run out of credits, you can purchase more.
 ```bash
 dev-gpt deploy --microservice_path <path to microservice>
 ```
 
-
 ### Delete Microservice
 To save credits you can delete your microservice via the following commands:
 ```bash
 jc list # get the microservice id
 jc delete <microservice id>
 ```
 
@@ -120,15 +118,14 @@
 ```bash
 dev-gpt generate \
 --description "The user writes something and gets a related deep compliment." \
 --model gpt-4
 ```
 <img src="res/compliment_example.png" alt="Compliment Generator" width="400" />
 
-
 ### Extract and summarize news articles given a URL
 ```bash
 dev-gpt generate \
 --description "Extract text from a news article URL using Newspaper3k library and generate a summary using gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-pot-guns-and-drones/" \
 --model gpt-4
 ```
 <img src="res/news_article_example.png" alt="News Article Example" width="400" />
```

#### html2text {}

```diff
@@ -6,23 +6,21 @@
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
                      platforms] [Downloads] [Discord_Chat]
 Welcome to Dev GPT, where we bring your ideas to life with the power of
 advanced artificial intelligence! Our automated development team is designed to
 create microservices tailored to your specific needs, making your software
 development process seamless and efficient. Comprised of a virtual Product
 Manager, Developer, and DevOps, our AI team ensures that every aspect of your
-project is covered, from concept to deployment. [//]: # ([![Watch the video]
-(res/thumbnail.png)](https://user-images.githubusercontent.com/11627845/
-231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4)) ## Quickstart ###
-Requirements - OpenAI key with access to GPT-3.5 or GPT-4 ### Installation
-```bash pip install dev-gpt dev-gpt configure --key  ``` If you set the
+project is covered, from concept to deployment. ## Quickstart ```bash pip
+install dev-gpt dev-gpt generate ``` ### Requirements - OpenAI key with access
+to GPT-3.5 or GPT-4 ```bash dev-gpt configure --key  ``` If you set the
 environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. We are working on a
-way to use gpt-3.5-turbo as well. ### Generate Microservice ```bash dev-gpt
-generate \ --description "" \ --model
+way to use gpt-3.5-turbo as well. ## Docs ### Generate Microservice ```bash
+dev-gpt generate \ --description "" \ --model
 5 or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x
 cheaper, but will not be able to generate as complex microservices. (default:
 largest you have access to) - A `path` on the local drive where the
 microservice will be generated. (default: ./microservice) The creation process
```

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/apis/gpt.py` & `dev-gpt-0.18.37.dev52/dev_gpt/apis/gpt.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/apis/jina_cloud.py` & `dev-gpt-0.18.37.dev52/dev_gpt/apis/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/apis/pypi.py` & `dev-gpt-0.18.37.dev52/dev_gpt/apis/pypi.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/cli.py` & `dev-gpt-0.18.37.dev52/dev_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/constants.py` & `dev-gpt-0.18.37.dev52/dev_gpt/constants.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/options/__init__.py` & `dev-gpt-0.18.37.dev52/dev_gpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/options/configure/key_handling.py` & `dev-gpt-0.18.37.dev52/dev_gpt/options/configure/key_handling.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/generator.py` & `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/apis.py` & `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/apis.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/templates_system.py` & `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/templates_system.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/templates_user.py` & `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/templates_user.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/ui.py` & `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/utils/io.py` & `dev-gpt-0.18.37.dev52/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt/utils/string_tools.py` & `dev-gpt-0.18.37.dev52/dev_gpt/utils/string_tools.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.37.dev52/dev_gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.37.dev51
+Version: 0.18.37.dev52
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -69,32 +69,32 @@
     <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
 </a>
 
 </p>
 
 Welcome to Dev GPT, where we bring your ideas to life with the power of advanced artificial intelligence! Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
 
-[//]: # ([![Watch the video]&#40;res/thumbnail.png&#41;]&#40;https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4&#41;)
-
-
-
-
 ## Quickstart
-### Requirements
-- OpenAI key with access to GPT-3.5 or GPT-4 
 
-### Installation
 ```bash
 pip install dev-gpt
+dev-gpt generate
+```
+
+### Requirements
+- OpenAI key with access to GPT-3.5 or GPT-4
+```bash
 dev-gpt configure --key <your openai api key>
 ```
+
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
+## Docs
 ### Generate Microservice
 ```bash
 dev-gpt generate \
 --description "<description of the microservice>" \
 --model <gpt-3.5 or gpt-4> \
 --path </path/to/local/folder>
 ```
@@ -112,24 +112,22 @@
 ### Run Microservice
 Run the microservice locally in docker. In case docker is not running on your machine, it will try to run it without docker.
 With this command a playground opens in your browser where you can test the microservice.
 ```bash
 dev-gpt run --path <path to microservice>
 ```
 
-
 ### Deploy Microservice
 If you want to deploy your microservice to the cloud a [Jina account](https://cloud.jina.ai/) is required.
 When creating a Jina account, you get some free credits, which you can use to deploy your microservice ($0.025/hour).
 If you run out of credits, you can purchase more.
 ```bash
 dev-gpt deploy --microservice_path <path to microservice>
 ```
 
-
 ### Delete Microservice
 To save credits you can delete your microservice via the following commands:
 ```bash
 jc list # get the microservice id
 jc delete <microservice id>
 ```
 
@@ -140,15 +138,14 @@
 ```bash
 dev-gpt generate \
 --description "The user writes something and gets a related deep compliment." \
 --model gpt-4
 ```
 <img src="res/compliment_example.png" alt="Compliment Generator" width="400" />
 
-
 ### Extract and summarize news articles given a URL
 ```bash
 dev-gpt generate \
 --description "Extract text from a news article URL using Newspaper3k library and generate a summary using gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-pot-guns-and-drones/" \
 --model gpt-4
 ```
 <img src="res/news_article_example.png" alt="News Article Example" width="400" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev51 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev52 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -17,23 +17,21 @@
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
                      platforms] [Downloads] [Discord_Chat]
 Welcome to Dev GPT, where we bring your ideas to life with the power of
 advanced artificial intelligence! Our automated development team is designed to
 create microservices tailored to your specific needs, making your software
 development process seamless and efficient. Comprised of a virtual Product
 Manager, Developer, and DevOps, our AI team ensures that every aspect of your
-project is covered, from concept to deployment. [//]: # ([![Watch the video]
-(res/thumbnail.png)](https://user-images.githubusercontent.com/11627845/
-231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4)) ## Quickstart ###
-Requirements - OpenAI key with access to GPT-3.5 or GPT-4 ### Installation
-```bash pip install dev-gpt dev-gpt configure --key  ``` If you set the
+project is covered, from concept to deployment. ## Quickstart ```bash pip
+install dev-gpt dev-gpt generate ``` ### Requirements - OpenAI key with access
+to GPT-3.5 or GPT-4 ```bash dev-gpt configure --key  ``` If you set the
 environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. We are working on a
-way to use gpt-3.5-turbo as well. ### Generate Microservice ```bash dev-gpt
-generate \ --description "" \ --model
+way to use gpt-3.5-turbo as well. ## Docs ### Generate Microservice ```bash
+dev-gpt generate \ --description "" \ --model
 5 or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x
 cheaper, but will not be able to generate as complex microservices. (default:
 largest you have access to) - A `path` on the local drive where the
 microservice will be generated. (default: ./microservice) The creation process
```

### Comparing `dev-gpt-0.18.37.dev51/dev_gpt.egg-info/SOURCES.txt` & `dev-gpt-0.18.37.dev52/dev_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/setup.py` & `dev-gpt-0.18.37.dev52/setup.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/test/integration/test_generator.py` & `dev-gpt-0.18.37.dev52/test/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/test/unit/test_api.py` & `dev-gpt-0.18.37.dev52/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev51/test/unit/test_response_parsing.py` & `dev-gpt-0.18.37.dev52/test/unit/test_response_parsing.py`

 * *Files identical despite different names*

