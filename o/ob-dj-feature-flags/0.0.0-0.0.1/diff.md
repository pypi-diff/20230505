# Comparing `tmp/ob-dj-feature-flags-0.0.0.tar.gz` & `tmp/ob-dj-feature-flags-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-dj-feature-flags-0.0.0.tar", last modified: Fri May  5 18:18:03 2023, max compression
+gzip compressed data, was "ob-dj-feature-flags-0.0.1.tar", last modified: Fri May  5 18:21:51 2023, max compression
```

## Comparing `ob-dj-feature-flags-0.0.0.tar` & `ob-dj-feature-flags-0.0.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.648577 ob-dj-feature-flags-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.644577 ob-dj-feature-flags-0.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.644577 ob-dj-feature-flags-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/.github/workflows/pre-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/.github/workflows/test-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-05 18:18:03.648577 ob-dj-feature-flags-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    94545 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.644577 ob-dj-feature-flags-0.0.0/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/config/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/config/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/config/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/docker-compose.env
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1036 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.644577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.644577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.644577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/flags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/flags/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      288 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/flags/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/flags/urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/flags/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.648577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/todos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/todos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/todos/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/todos/urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/todos/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.648577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.648577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/admin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      286 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.648577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/migrations/0002_auto_20230503_2339.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.648577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/todos/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/todos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/todos/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.648577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/todos/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/todos/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/todos/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/todos/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.648577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/utils/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:18:03.644577 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-05 18:18:03.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-05 18:18:03.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:18:03.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 18:18:03.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 18:18:03.000000 ob-dj-feature-flags-0.0.0/ob_dj_feature_flags.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-05 18:18:03.652577 ob-dj-feature-flags-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 18:17:50.000000 ob-dj-feature-flags-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.999993 ob-dj-feature-flags-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.983993 ob-dj-feature-flags-0.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.987993 ob-dj-feature-flags-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/.github/workflows/pre-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/.github/workflows/test-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-05 18:21:50.999993 ob-dj-feature-flags-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    94545 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.987993 ob-dj-feature-flags-0.0.1/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/config/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/config/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/config/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/docker-compose.env
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1036 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.987993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.991993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.991993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/flags/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      288 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/flags/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/flags/urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/flags/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.991993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/todos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/todos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/todos/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/todos/urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/todos/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.991993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.995993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/admin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      286 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.995993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/migrations/0002_auto_20230503_2339.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.999993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/todos/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/todos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/todos/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.999993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/todos/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/todos/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/todos/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/todos/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.999993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/utils/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:21:50.991993 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-05 18:21:50.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-05 18:21:50.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:21:50.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 18:21:50.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 18:21:50.000000 ob-dj-feature-flags-0.0.1/ob_dj_feature_flags.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-05 18:21:50.999993 ob-dj-feature-flags-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 18:21:39.000000 ob-dj-feature-flags-0.0.1/setup.py
```

### Comparing `ob-dj-feature-flags-0.0.0/.github/workflows/pre-release.yml` & `ob-dj-feature-flags-0.0.1/.github/workflows/pre-release.yml`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/.github/workflows/release.yml` & `ob-dj-feature-flags-0.0.1/.github/workflows/release.yml`

 * *Files 6% similar despite different names*

```diff
@@ -47,24 +47,24 @@
 #          status: ${{ job.status }}
 #          author_name: Publish to PyPI
 #        env:
 #          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 #          SLACK_WEBHOOK_URL: ${{ secrets.SLACK_RELEASE_ALERTS_WEBHOOK }}
 #        if: failure()
 
-#  slack-notifications:
-#    needs: build-n-publish
-#    runs-on: ubuntu-latest
-#    steps:
-#      - name: Checkout code
-#        uses: actions/checkout@v2
-#      - name: Slackify the release body
-#        id: release_body
-#        uses: LoveToKnow/slackify-markdown-action@v1.0.0
-#        with:
-#          text: ${{ github.event.release.body }}
-#      - uses: homeday-de/slack-release-bot-action@main
-#        with:
-#          webhook_url: ${{ secrets.SLACK_RELEASE_ALERTS_WEBHOOK }}
-#          title: ${{ github.event.release.name }}
-#          body: ${{ steps.release_body.outputs.text }}
-#          context: https://pypi.org/project/ob-dj-feature-flags/
+  slack-notifications:
+    needs: build-n-publish
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v2
+      - name: Slackify the release body
+        id: release_body
+        uses: LoveToKnow/slackify-markdown-action@v1.0.0
+        with:
+          text: ${{ github.event.release.body }}
+      - uses: homeday-de/slack-release-bot-action@main
+        with:
+          webhook_url: ${{ secrets.SLACK_RELEASE_ALERTS_WEBHOOK }}
+          title: ${{ github.event.release.name }}
+          body: ${{ steps.release_body.outputs.text }}
+          context: https://pypi.org/project/ob-dj-feature-flags/
```

### Comparing `ob-dj-feature-flags-0.0.0/.github/workflows/test-build.yml` & `ob-dj-feature-flags-0.0.1/.github/workflows/test-build.yml`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/.pre-commit-config.yaml` & `ob-dj-feature-flags-0.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/Dockerfile` & `ob-dj-feature-flags-0.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/LICENSE` & `ob-dj-feature-flags-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/Makefile` & `ob-dj-feature-flags-0.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/PKG-INFO` & `ob-dj-feature-flags-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-dj-feature-flags
-Version: 0.0.0
+Version: 0.0.1
 Summary: OBytes django application for managing feature flags
 Home-page: https://www.obytes.com/
 Author: OBytes
 Author-email: hello@obytes.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `ob-dj-feature-flags-0.0.0/Pipfile` & `ob-dj-feature-flags-0.0.1/Pipfile`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/Pipfile.lock` & `ob-dj-feature-flags-0.0.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/README.md` & `ob-dj-feature-flags-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/config/settings.py` & `ob-dj-feature-flags-0.0.1/config/settings.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/config/urls.py` & `ob-dj-feature-flags-0.0.1/config/urls.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/docker-compose.yml` & `ob-dj-feature-flags-0.0.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/manage.py` & `ob-dj-feature-flags-0.0.1/manage.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/apis/todos/views.py` & `ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/apis/todos/views.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/admin.py` & `ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/admin.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/migrations/0001_initial.py` & `ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/flags/models.py` & `ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/flags/models.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/core/todos/migrations/0001_initial.py` & `ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/core/todos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/ob_dj_feature_flags/utils/decorators.py` & `ob-dj-feature-flags-0.0.1/ob_dj_feature_flags/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/ob_dj_feature_flags.egg-info/PKG-INFO` & `ob-dj-feature-flags-0.0.1/ob_dj_feature_flags.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-dj-feature-flags
-Version: 0.0.0
+Version: 0.0.1
 Summary: OBytes django application for managing feature flags
 Home-page: https://www.obytes.com/
 Author: OBytes
 Author-email: hello@obytes.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `ob-dj-feature-flags-0.0.0/ob_dj_feature_flags.egg-info/SOURCES.txt` & `ob-dj-feature-flags-0.0.1/ob_dj_feature_flags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.0/setup.cfg` & `ob-dj-feature-flags-0.0.1/setup.cfg`

 * *Files identical despite different names*

