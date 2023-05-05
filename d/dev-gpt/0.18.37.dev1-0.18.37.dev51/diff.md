# Comparing `tmp/dev-gpt-0.18.37.dev1.tar.gz` & `tmp/dev-gpt-0.18.37.dev51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.37.dev1.tar", last modified: Thu May  4 19:20:58 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.37.dev51.tar", last modified: Fri May  5 01:03:28 2023, max compression
```

## Comparing `dev-gpt-0.18.37.dev1.tar` & `dev-gpt-0.18.37.dev51.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.176944 dev-gpt-0.18.37.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21185 2023-05-04 19:20:58.176944 dev-gpt-0.18.37.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.160944 dev-gpt-0.18.37.dev1/dev_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 19:20:57.000000 dev-gpt-0.18.37.dev1/dev_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.164944 dev-gpt-0.18.37.dev1/dev_gpt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.164944 dev-gpt-0.18.37.dev1/dev_gpt/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.164944 dev-gpt-0.18.37.dev1/dev_gpt/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.164944 dev-gpt-0.18.37.dev1/dev_gpt/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.168944 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.156944 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.168944 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.168944 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.172944 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/microservice/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/templates_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.172944 dev-gpt-0.18.37.dev1/dev_gpt/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.172944 dev-gpt-0.18.37.dev1/dev_gpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/dev_gpt/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.164944 dev-gpt-0.18.37.dev1/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21185 2023-05-04 19:20:58.000000 dev-gpt-0.18.37.dev1/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-04 19:20:58.000000 dev-gpt-0.18.37.dev1/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:20:58.000000 dev-gpt-0.18.37.dev1/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 19:20:58.000000 dev-gpt-0.18.37.dev1/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 19:20:58.000000 dev-gpt-0.18.37.dev1/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 19:20:58.000000 dev-gpt-0.18.37.dev1/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 19:20:58.176944 dev-gpt-0.18.37.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.172944 dev-gpt-0.18.37.dev1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.172944 dev-gpt-0.18.37.dev1/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:58.172944 dev-gpt-0.18.37.dev1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 19:20:52.000000 dev-gpt-0.18.37.dev1/test/unit/test_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/templates_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.475715 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 01:03:28.000000 dev-gpt-0.18.37.dev51/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:28.479715 dev-gpt-0.18.37.dev51/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-05 01:03:23.000000 dev-gpt-0.18.37.dev51/test/unit/test_strings.py
```

### Comparing `dev-gpt-0.18.37.dev1/LICENSE` & `dev-gpt-0.18.37.dev51/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/PKG-INFO` & `dev-gpt-0.18.37.dev51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.37.dev1
+Version: 0.18.37.dev51
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev1 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev51 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dev-gpt-0.18.37.dev1/README.md` & `dev-gpt-0.18.37.dev51/README.md`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/apis/gpt.py` & `dev-gpt-0.18.37.dev51/dev_gpt/apis/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,13 @@
         if os.environ['VERBOSE'].lower() == 'true':
             print()
         self.cost_callback(sum([len(m.content) for m in self.messages]), len(response.content), self.print_costs)
         self.messages.append(response)
         return response.content
 
     @staticmethod
-    def _create_system_message(task_description, test_description, system_definition_examples: List[str] = []) -> SystemMessage:
-        if system_definition_examples is None:
-            return None
-
+    def _create_system_message(task_description, test_description) -> SystemMessage:
         system_message = PromptTemplate.from_template(template_system_message_base).format(
             task_description=task_description,
             test_description=test_description,
         )
         return SystemMessage(content=system_message)
```

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/apis/jina_cloud.py` & `dev-gpt-0.18.37.dev51/dev_gpt/apis/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/apis/pypi.py` & `dev-gpt-0.18.37.dev51/dev_gpt/apis/pypi.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/cli.py` & `dev-gpt-0.18.37.dev51/dev_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/constants.py` & `dev-gpt-0.18.37.dev51/dev_gpt/constants.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/options/__init__.py` & `dev-gpt-0.18.37.dev51/dev_gpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/options/configure/key_handling.py` & `dev-gpt-0.18.37.dev51/dev_gpt/options/configure/key_handling.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/options/generate/generator.py` & `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,38 +90,37 @@
     def generate_and_persist_file(
             self,
             section_title: str,
             template: PromptTemplate,
             destination_folder: str,
             file_name_s: List[str] = None,
             parse_result_fn: Callable = None,
-            system_definition_examples: List[str] = [],
             **template_kwargs
     ):
         """This function generates file(s) using the given template and persists it/them in the given destination folder.
         It also returns the generated content as a dictionary mapping file_name to its content.
 
         Args:
             section_title (str): The title of the section to be printed in the console.
             template (PromptTemplate): The template to be used for generating the file(s).
             destination_folder (str): The destination folder where the generated file(s) should be persisted.
             file_name_s (List[str], optional): The name of the file(s) to be generated. Defaults to None.
             parse_result_fn (Callable, optional): A function that parses the generated content and returns a dictionary
                 mapping file_name to its content. If no content could be extract, it returns an empty dictionary.
                 Defaults to None. If None, default parsing is used which uses the file_name to extract from the generated content.
-            system_definition_examples (List[str], optional): The system definition examples to be used for the conversation. Defaults to [].
             **template_kwargs: The keyword arguments to be passed to the template.
         """
         if parse_result_fn is None:
             parse_result_fn = self.get_default_parse_result_fn(file_name_s)
 
         print_colored('', f'\n\n############# {section_title} #############', 'blue')
-        system_introduction_message = _GPTConversation._create_system_message(self.microservice_specification.task,
-                                                                              self.microservice_specification.test,
-                                                                              system_definition_examples)
+        system_introduction_message = _GPTConversation._create_system_message(
+            self.microservice_specification.task,
+            self.microservice_specification.test
+        )
         conversation = self.gpt_session.get_conversation(messages=[system_introduction_message])
         template_kwargs = {k: v for k, v in template_kwargs.items() if k in template.input_variables}
         if 'file_name' in template.input_variables and len(file_name_s) == 1:
             template_kwargs['file_name'] = file_name_s[0]
         content_raw = conversation.chat(
             template.format(
                 **template_kwargs
@@ -341,15 +340,14 @@
         if is_apt_get_dependency_issue:
             self.generate_and_persist_file(
                 section_title='Debugging apt-get dependency issue',
                 template=template_solve_apt_get_dependency_issue,
                 destination_folder=next_microservice_path,
                 file_name_s=['apt-get-packages.json'],
                 parse_result_fn=self.parse_result_fn_dockerfile,
-                system_definition_examples=[],
                 summarized_error=summarized_error,
                 all_files_string=dock_req_string,
             )
             print('Dockerfile updated')
         else:
             is_pip_dependency_issue = self.is_dependency_issue(summarized_error, dock_req_string, 'PIP')
             if is_pip_dependency_issue:
@@ -413,15 +411,14 @@
     def get_possible_packages(self):
         print_colored('', '\n\n############# What packages to use? #############', 'blue')
         packages_json_string = self.generate_and_persist_file(
             section_title='Generate possible packages',
             template=template_generate_possible_packages,
             destination_folder=self.microservice_root_path,
             file_name_s=['strategies.json'],
-            system_definition_examples=[],
             description=self.microservice_specification.task
         )['strategies.json']
         packages_list = [[pkg.strip().lower() for pkg in packages] for packages in json.loads(packages_json_string)]
         packages_list = [[self.replace_with_gpt_3_5_turbo_if_possible(pkg) for pkg in packages] for packages in
                          packages_list]
 
         packages_list = self.filter_packages_list(packages_list)
```

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/options/generate/static_files/microservice/apis.py` & `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/static_files/microservice/apis.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/options/generate/templates_system.py` & `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/templates_system.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/options/generate/templates_user.py` & `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/templates_user.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/options/generate/ui.py` & `dev-gpt-0.18.37.dev51/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/utils/io.py` & `dev-gpt-0.18.37.dev51/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt/utils/string_tools.py` & `dev-gpt-0.18.37.dev51/dev_gpt/utils/string_tools.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.37.dev51/dev_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.37.dev1
+Version: 0.18.37.dev51
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev1 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev51 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dev-gpt-0.18.37.dev1/dev_gpt.egg-info/SOURCES.txt` & `dev-gpt-0.18.37.dev51/dev_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/setup.py` & `dev-gpt-0.18.37.dev51/setup.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/test/integration/test_generator.py` & `dev-gpt-0.18.37.dev51/test/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/test/unit/test_api.py` & `dev-gpt-0.18.37.dev51/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev1/test/unit/test_response_parsing.py` & `dev-gpt-0.18.37.dev51/test/unit/test_response_parsing.py`

 * *Files identical despite different names*

