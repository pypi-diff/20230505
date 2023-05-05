# Comparing `tmp/django-minio-storage-0.5.0.tar.gz` & `tmp/django-minio-storage-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-minio-storage-0.5.0.tar", last modified: Sun Apr 23 11:01:30 2023, max compression
+gzip compressed data, was "django-minio-storage-0.5.1.tar", last modified: Fri May  5 15:11:34 2023, max compression
```

## Comparing `django-minio-storage-0.5.0.tar` & `django-minio-storage-0.5.1.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.flake8rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.934837 django-minio-storage-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.938837 django-minio-storage-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.938837 django-minio-storage-0.5.0/django_minio_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/django_minio_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/contributors.md
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/licences.md
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/minio_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/minio_storage/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/minio_storage/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/management/commands/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/minio_storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 11:01:30.000000 django-minio-storage-0.5.0/minio_storage/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.942837 django-minio-storage-0.5.0/tests/django_minio_storage_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/django_minio_storage_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/django_minio_storage_tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/django_minio_storage_tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/django_minio_storage_tests/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:30.946837 django-minio-storage-0.5.0/tests/test_app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/bucket_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/custom_storage_class_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/managementcommand_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/retrieve_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/upload_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/test_app/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tests/watermelon-cat.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-23 11:01:14.000000 django-minio-storage-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.291364 django-minio-storage-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.flake8rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.267364 django-minio-storage-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.279364 django-minio-storage-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-05 15:11:34.291364 django-minio-storage-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.279364 django-minio-storage-0.5.1/django_minio_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.279364 django-minio-storage-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/licences.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.283364 django-minio-storage-0.5.1/minio_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.283364 django-minio-storage-0.5.1/minio_storage/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.283364 django-minio-storage-0.5.1/minio_storage/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/management/commands/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/minio_storage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:11:34.291364 django-minio-storage-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.287364 django-minio-storage-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.287364 django-minio-storage-0.5.1/tests/django_minio_storage_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/django_minio_storage_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/django_minio_storage_tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/django_minio_storage_tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/django_minio_storage_tests/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.287364 django-minio-storage-0.5.1/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.291364 django-minio-storage-0.5.1/tests/test_app/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/bucket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/custom_storage_class_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/managementcommand_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/retrieve_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/upload_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/watermelon-cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tox.ini
```

### Comparing `django-minio-storage-0.5.0/.github/workflows/release.yml` & `django-minio-storage-0.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/.github/workflows/tox.yml` & `django-minio-storage-0.5.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/CHANGELOG.md` & `django-minio-storage-0.5.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.5.1
+
+Fix type hints
+
 ## 0.5.0
 
 Switched the minio-py client library version from `<7` to `>=7`.
 
 Minimum Django version is now 3.2
 
 Minimum Python version is now 3.8
```

### Comparing `django-minio-storage-0.5.0/LICENSE-APACHE` & `django-minio-storage-0.5.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/LICENSE-MIT` & `django-minio-storage-0.5.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/PKG-INFO` & `django-minio-storage-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.0
+Version: 0.5.1
 Summary: Django file storage using the minio python client
 Home-page: https://github.com/py-pa/django-minio-storage
 Author: Tom Houlé
 Author-email: tom@kafunsho.be
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -17,16 +17,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 
 [![PyPI version](https://badge.fury.io/py/django-minio-storage.svg)](https://badge.fury.io/py/django-minio-storage)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-minio-storage)](https://pypistats.org/packages/django-minio-storage)
 [![Documentation Status](http://readthedocs.org/projects/django-minio-storage/badge/?version=latest)](http://django-minio-storage.readthedocs.io/en/latest/?badge=latest)
 
+
 # django-minio-storage
 
 Use [minio](https://minio.io) for django static and media file storage.
 
 Minio is accessed through the Amazon S3 API, so existing django file storage
 adapters for S3 should work, but in practice they are hard to configure. This
 project uses the minio python client instead. Inspiration has been drawn from
```

### Comparing `django-minio-storage-0.5.0/README.md` & `django-minio-storage-0.5.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 [![PyPI version](https://badge.fury.io/py/django-minio-storage.svg)](https://badge.fury.io/py/django-minio-storage)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-minio-storage)](https://pypistats.org/packages/django-minio-storage)
 [![Documentation Status](http://readthedocs.org/projects/django-minio-storage/badge/?version=latest)](http://django-minio-storage.readthedocs.io/en/latest/?badge=latest)
 
+
 # django-minio-storage
 
 Use [minio](https://minio.io) for django static and media file storage.
 
 Minio is accessed through the Amazon S3 API, so existing django file storage
 adapters for S3 should work, but in practice they are hard to configure. This
 project uses the minio python client instead. Inspiration has been drawn from
```

### Comparing `django-minio-storage-0.5.0/django_minio_storage.egg-info/PKG-INFO` & `django-minio-storage-0.5.1/django_minio_storage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.0
+Version: 0.5.1
 Summary: Django file storage using the minio python client
 Home-page: https://github.com/py-pa/django-minio-storage
 Author: Tom Houlé
 Author-email: tom@kafunsho.be
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -17,16 +17,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 
 [![PyPI version](https://badge.fury.io/py/django-minio-storage.svg)](https://badge.fury.io/py/django-minio-storage)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-minio-storage)](https://pypistats.org/packages/django-minio-storage)
 [![Documentation Status](http://readthedocs.org/projects/django-minio-storage/badge/?version=latest)](http://django-minio-storage.readthedocs.io/en/latest/?badge=latest)
 
+
 # django-minio-storage
 
 Use [minio](https://minio.io) for django static and media file storage.
 
 Minio is accessed through the Amazon S3 API, so existing django file storage
 adapters for S3 should work, but in practice they are hard to configure. This
 project uses the minio python client instead. Inspiration has been drawn from
```

### Comparing `django-minio-storage-0.5.0/django_minio_storage.egg-info/SOURCES.txt` & `django-minio-storage-0.5.1/django_minio_storage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 LICENSE-MIT
 README.md
 dev-requirements.txt
 docker-compose.yml
 docs-requirements.txt
 mkdocs.yml
 pyproject.toml
+pyrightconfig.json
 setup.py
 tox.ini
 .github/workflows/release.yml
 .github/workflows/tox.yml
 django_minio_storage.egg-info/PKG-INFO
 django_minio_storage.egg-info/SOURCES.txt
 django_minio_storage.egg-info/dependency_links.txt
```

### Comparing `django-minio-storage-0.5.0/docs/development.md` & `django-minio-storage-0.5.1/docs/development.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/docs/index.md` & `django-minio-storage-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/docs/licences.md` & `django-minio-storage-0.5.1/docs/licences.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/docs/usage.md` & `django-minio-storage-0.5.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/minio_storage/files.py` & `django-minio-storage-0.5.1/minio_storage/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,15 @@
         self._mode: str = mode
         self._file = None
 
 
 class ReadOnlyMinioObjectFile(MinioStorageFile, ReadOnlyMixin, NonSeekableMixin):
     """A django File class which directly exposes the underlying minio object. This
     means the the instance doesnt support functions like .seek() and is required to
-    be closed to be able to reuse minio connections.
-
-    Note: This file class is not tested yet"""
+    be closed to be able to reuse minio connections."""
 
     def __init__(
         self,
         name: str,
         mode: str,
         storage: "Storage",
         max_memory_size: T.Optional[int] = None,
```

### Comparing `django-minio-storage-0.5.0/minio_storage/management/commands/minio.py` & `django-minio-storage-0.5.1/minio_storage/management/commands/minio.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/minio_storage/policy.py` & `django-minio-storage-0.5.1/minio_storage/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,33 +22,33 @@
         }
         pol = policies[self](bucket_name)
         if json_encode:
             return json.dumps(pol)
         return pol
 
 
-def _none(bucket_name: str) -> T.Dict:
+def _none(bucket_name: str) -> T.Dict[str, T.Any]:
     return {"Version": "2012-10-17", "Statement": []}
 
 
-def _get(bucket_name: str) -> T.Dict:
+def _get(bucket_name: str) -> T.Dict[str, T.Any]:
     return {
         "Version": "2012-10-17",
         "Statement": [
             {
                 "Effect": "Allow",
                 "Principal": {"AWS": ["*"]},
                 "Action": ["s3:GetObject"],
                 "Resource": [f"arn:aws:s3:::{bucket_name}/*"],
             }
         ],
     }
 
 
-def _read(bucket_name: str) -> T.Dict:
+def _read(bucket_name: str) -> T.Dict[str, T.Any]:
     return {
         "Version": "2012-10-17",
         "Statement": [
             {
                 "Effect": "Allow",
                 "Principal": {"AWS": ["*"]},
                 "Action": ["s3:GetBucketLocation"],
@@ -66,15 +66,15 @@
                 "Action": ["s3:GetObject"],
                 "Resource": [f"arn:aws:s3:::{bucket_name}/*"],
             },
         ],
     }
 
 
-def _write(bucket_name: str) -> T.Dict:
+def _write(bucket_name: str) -> T.Dict[str, T.Any]:
     return {
         "Version": "2012-10-17",
         "Statement": [
             {
                 "Effect": "Allow",
                 "Principal": {"AWS": ["*"]},
                 "Action": ["s3:GetBucketLocation"],
@@ -97,15 +97,15 @@
                 ],
                 "Resource": [f"arn:aws:s3:::{bucket_name}/*"],
             },
         ],
     }
 
 
-def _read_write(bucket_name: str) -> T.Dict:
+def _read_write(bucket_name: str) -> T.Dict[str, T.Any]:
     return {
         "Version": "2012-10-17",
         "Statement": [
             {
                 "Effect": "Allow",
                 "Principal": {"AWS": ["*"]},
                 "Action": ["s3:GetBucketLocation"],
```

### Comparing `django-minio-storage-0.5.0/minio_storage/storage.py` & `django-minio-storage-0.5.1/minio_storage/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
 import mimetypes
 import posixpath
 import typing as T
-import urllib
 from logging import getLogger
-from urllib.parse import urlsplit, urlunsplit
+from urllib.parse import quote, urlsplit, urlunsplit
 
 import minio
 import minio.error as merr
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files.storage import Storage
 from django.utils import timezone
@@ -115,18 +114,14 @@
             session_token=credentials.session_token,
             secure=base_url_parts.scheme == "https",
             # The bucket region may be auto-detected by client (via an HTTP
             # request), so don't just use client._region
             region=client._get_region(bucket_name, None),
             http_client=client._http,
         )
-        if hasattr(client, "_credentials"):
-            # Client credentials do not exist prior to minio-py 5.0.7, but
-            # they should be reused if possible
-            base_url_client._credentials = client._credentials
 
         return base_url_client
 
     def _sanitize_path(self, name):
         v = posixpath.normpath(name).replace("\\", "/")
         if v == ".":
             v = ""
@@ -150,15 +145,15 @@
     def _open(self, name, mode="rb"):
         try:
             f = self.file_class(self._sanitize_path(name), mode, self)
         except merr.MinioException as e:
             raise minio_error(f"File {name} could not be saved: {str(e)}", e)
         return f
 
-    def _save(self, name: str, content: bytes) -> str:
+    def _save(self, name: str, content: T.BinaryIO) -> str:
         try:
             if hasattr(content, "seek") and callable(content.seek):
                 content.seek(0)
             content_size, content_type, sane_name = self._examine_file(name, content)
             self.client.put_object(
                 self.bucket_name,
                 sane_name,
@@ -208,24 +203,23 @@
 
     def exists(self, name: str) -> bool:
         try:
             self.client.stat_object(self.bucket_name, self._sanitize_path(name))
             return True
         except merr.InvalidResponseError as error:
             # TODO - deprecate
-            if error.code == "NoSuchKey":
+            if error._code == "NoSuchKey":
                 return False
             else:
                 raise minio_error(f"Could not stat file {name}", error)
         except merr.S3Error:
             return False
-        except merr.S3Error:
-            raise
         except Exception as error:
             logger.error(error)
+        return False
 
     def listdir(self, path: str) -> T.Tuple[T.List, T.List]:
         #  [None, "", "."] is supported to mean the configured root among various
         #  implementations of Storage implementations so we copy that behaviour even if
         #  maybe None should raise an exception instead.
         #
         #  If the path prefix does not match anything full prefix that does exist this
@@ -259,15 +253,15 @@
             info = self.client.stat_object(self.bucket_name, name)
             return info.size
         except merr.InvalidResponseError as error:
             raise minio_error(f"Could not access file size for {name}", error)
 
     def _presigned_url(
         self, name: str, max_age: T.Optional[datetime.timedelta] = None
-    ) -> str:
+    ) -> T.Optional[str]:
         kwargs = {}
         if max_age is not None:
             kwargs["expires"] = max_age
 
         client = self.client if self.base_url is None else self.base_url_client
         url = client.presigned_get_object(self.bucket_name, name, **kwargs)
 
@@ -289,19 +283,22 @@
                     url_parts.scheme,
                     url_parts.netloc,
                     new_url_path,
                     url_parts.query,
                     url_parts.fragment,
                 )
             )
-        return url
+        if url:
+            return str(url)
+        return None
 
     def url(
         self, name: str, *args, max_age: T.Optional[datetime.timedelta] = None
-    ) -> str:
+    ) -> T.Optional[str]:
+        url = ""
         if self.presign_urls:
             url = self._presigned_url(name, max_age=max_age)
         else:
 
             def strip_beg(path):
                 while path.startswith("/"):
                     path = path[1:]
@@ -309,22 +306,20 @@
 
             def strip_end(path):
                 while path.endswith("/"):
                     path = path[:-1]
                 return path
 
             if self.base_url is not None:
-                url = "{}/{}".format(
-                    strip_end(self.base_url), urllib.parse.quote(strip_beg(name))
-                )
+                url = "{}/{}".format(strip_end(self.base_url), quote(strip_beg(name)))
             else:
                 url = "{}/{}/{}".format(
                     strip_end(self.endpoint_url),
                     self.bucket_name,
-                    urllib.parse.quote(strip_beg(name)),
+                    quote(strip_beg(name)),
                 )
         return url
 
     @property
     def endpoint_url(self):
         return self.client._base_url._url.geturl()
 
@@ -349,15 +344,15 @@
                 f"Could not access modification time for file {name}", error
             )
 
 
 _NoValue = object()
 
 
-def get_setting(name, default=_NoValue):
+def get_setting(name: str, default=_NoValue) -> T.Any:
     result = getattr(settings, name, default)
     if result is _NoValue:
         # print("Attr {} : {}".format(name, getattr(settings, name, default)))
         raise ImproperlyConfigured
     else:
         return result
```

### Comparing `django-minio-storage-0.5.0/setup.py` & `django-minio-storage-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/tests/django_minio_storage_tests/settings.py` & `django-minio-storage-0.5.1/tests/django_minio_storage_tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/tests/django_minio_storage_tests/urls.py` & `django-minio-storage-0.5.1/tests/django_minio_storage_tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/tests/test_app/tests/bucket_tests.py` & `django-minio-storage-0.5.1/tests/test_app/tests/bucket_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         MINIO_STORAGE_STATIC_BUCKET_NAME="inexistent",
         MINIO_STORAGE_AUTO_CREATE_STATIC_BUCKET=False,
     )
     def test_static_storage_cannot_be_initialized_without_bucket(self):
         with self.assertRaises(OSError):
             MinioStaticStorage()
 
-    def test_get_setting_throws_early(self):
+    def test_get_setting_raises_exception(self):
         with self.assertRaises(ImproperlyConfigured):
             get_setting("INEXISTENT_SETTING")
 
     @override_settings(
         MINIO_STORAGE_MEDIA_BUCKET_NAME="inexistent",
         MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET=False,
         MINIO_STORAGE_ASSUME_MEDIA_BUCKET_EXISTS=True,
```

### Comparing `django-minio-storage-0.5.0/tests/test_app/tests/custom_storage_class_tests.py` & `django-minio-storage-0.5.1/tests/test_app/tests/custom_storage_class_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 )
 
 from .utils import BaseTestMixin
 from .utils import bucket_name as create_test_bucket_name
 
 
 @deconstructible
-class SecretStorage(MinioStorage):
-    """The SecretStorage MinioStorage subclass can be used directly, as a storage in
+class PrivateStorage(MinioStorage):
+    """The PrivateStorage MinioStorage subclass can be used directly, as a storage in
     settings.DEFAULT_FILE_STORAGE or after instantiated used individually on any django
     FileField:
 
     from django.db import models
 
-    ss = SecretStorage(bucket_name='invoices')
+    private_storage = PrivateStorage(bucket_name='invoices')
 
     class Invoice(models.Model):
         ...
-        pdf = models.FileField(storage=ss)
+        pdf = models.FileField(storage=private_storage)
 
     """
 
     # We can set a new default File class implementation that will be used here because
     # we want to stream the data directly from minio. Imagine that we need to process
     # large files where we don't want to waste time/ram/disk space on  writing the file
     # to disk two times before processing it.
@@ -47,15 +47,15 @@
         # extra args.
         #
         client = create_minio_client_from_settings(minio_kwargs={"region": "us-east-1"})
 
         # or use our own Django setting
         #
         if bucket_name is None:
-            bucket_name = get_setting("SECRET_BUCKET_NAME")
+            bucket_name = get_setting("PRIVATE_BUCKET_NAME")
 
         # Run the super constructor and make a choice to only use presigned urls with
         # this bucket so that we can keep files more private here than how media files
         # usually are public readable.
         #
         super().__init__(
             client,
@@ -63,20 +63,20 @@
             auto_create_bucket=True,
             auto_create_policy=False,
             presign_urls=True,
         )
 
 
 class CustomStorageTests(BaseTestMixin, TestCase):
-    @override_settings(SECRET_BUCKET_NAME=create_test_bucket_name("my-secret-bucket"))
+    @override_settings(PRIVATE_BUCKET_NAME=create_test_bucket_name("my-private-bucket"))
     def test_custom_storage(self):
         # Instansiate a storage class and put a file in it so that we have something to
         # work with.
         #
-        storage = SecretStorage()
+        storage = PrivateStorage()
         storage_filename = storage.save("secret.txt", ContentFile(b"abcd"))
 
         # Create a temporary workspace directory.
         #
         # It's importat that this directory is deleted after we are done so we use the
         # with statement here.
         #
```

### Comparing `django-minio-storage-0.5.0/tests/test_app/tests/delete_tests.py` & `django-minio-storage-0.5.1/tests/test_app/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/tests/test_app/tests/managementcommand_tests.py` & `django-minio-storage-0.5.1/tests/test_app/tests/managementcommand_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/tests/test_app/tests/retrieve_tests.py` & `django-minio-storage-0.5.1/tests/test_app/tests/retrieve_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import datetime
 import io
 import os
-import unittest
 
 import requests
 from django.core.files.base import ContentFile
 from django.test import TestCase, override_settings
 from freezegun import freeze_time
 from minio.error import S3Error
 
-from minio_storage.errors import MinIOError
 from minio_storage.storage import MinioMediaStorage
 
 from .utils import BaseTestMixin
 
 
 @override_settings(
     MINIO_STORAGE_MEDIA_USE_PRESIGNED=True, MINIO_STORAGE_STATIC_USE_PRESIGNED=True
@@ -37,15 +35,15 @@
     def test_url_of_non_existent_object(self):
         self.media_storage.url("this does not exist")
 
     def test_file_size(self):
         test_file = self.media_storage.save("sizetest.txt", ContentFile(b"1234"))
         self.assertEqual(4, self.media_storage.size(test_file))
 
-    def test_size_of_non_existent_throws(self):
+    def test_size_of_non_existent_raises_exception(self):
         test_file = self.media_storage.save("sizetest.txt", ContentFile(b"1234"))
         self.media_storage.delete(test_file)
         with self.assertRaises(S3Error):
             self.media_storage.size(test_file)
 
     def test_modified_time(self):
         self.assertIsInstance(
@@ -58,15 +56,15 @@
         )
 
     def test_created_time(self):
         self.assertIsInstance(
             self.media_storage.created_time(self.new_file), datetime.datetime
         )
 
-    def test_modified_time_of_non_existent_throws(self):
+    def test_modified_time_of_non_existent_raises_exception(self):
         with self.assertRaises(S3Error):
             self.media_storage.modified_time("nonexistent.jpg")
 
     def _listdir_root(self, root):
         self.media_storage.save("dir1/file2.txt", ContentFile(b"meh"))
         test_dir = self.media_storage.listdir(root)
         (dirs, files) = test_dir
@@ -112,27 +110,18 @@
     def test_file_exists(self):
         existent = self.media_storage.save("existent.txt", ContentFile(b"meh"))
         self.assertTrue(self.media_storage.exists(existent))
 
     def test_file_exists_failure(self):
         self.assertFalse(self.media_storage.exists("nonexistent.txt"))
 
-    @unittest.skip("Skipping this test because undecided if it should raise exception")
-    def test_opening_non_existing_file_raises_oserror(self):
-        with self.assertRaises(OSError):
-            self.media_storage.open("this does not exist")
-
-    @unittest.skip("Skipping this test because undecided if it should raise exception")
-    def test_opening_non_existing_file_raises_minioerror(self):
-        with self.assertRaises(MinIOError):
-            self.media_storage.open("this does not exist")
-        try:
-            self.media_storage.open("this does not exist")
-        except MinIOError as e:
-            assert e.cause.__class__ == S3Error
+    def test_reading_non_existing_file_raises_exception(self):
+        with self.assertRaises(Exception):
+            f = self.media_storage.open("this does not exist")
+            f.read()
 
     def test_file_names_are_properly_sanitized(self):
         self.media_storage.save("./meh22222.txt", io.BytesIO(b"stuff"))
 
     def test_url_max_age(self):
         url = self.media_storage.url(
             "test-file", max_age=datetime.timedelta(seconds=10)
```

### Comparing `django-minio-storage-0.5.0/tests/test_app/tests/upload_tests.py` & `django-minio-storage-0.5.1/tests/test_app/tests/upload_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,23 +62,14 @@
         f = self.media_storage.open("read_seek_test.txt", mode="br")
         f.seek(4)
         f.seek(0)
 
     def test_upload_and_get_back_file_with_funky_name(self):
         self.media_storage.save("áčďěščřžýŽŇůúť.txt", ContentFile(b"12345"))
 
-    def test_uploaded_and_downloaded_file_sizes_match(self):
-        pass
-
-    def test_uploaded_files_end_up_in_the_right_bucket(self):
-        pass
-
-    def test_static_files_end_up_in_the_right_bucket(self):
-        pass
-
     def test_upload_file_beggining_with_dot(self):
         self.media_storage.save(
             ".hidden_file", ContentFile(b"Not really, but whatever")
         )
         self.assertTrue(self.media_storage.exists(".hidden_file"))
         self.media_storage.delete(".hidden_file")
         self.assertFalse(self.media_storage.exists(".hidden_file"))
```

### Comparing `django-minio-storage-0.5.0/tests/test_app/tests/utils.py` & `django-minio-storage-0.5.1/tests/test_app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/tests/watermelon-cat.jpg` & `django-minio-storage-0.5.1/tests/watermelon-cat.jpg`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.0/tox.ini` & `django-minio-storage-0.5.1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-[pytest]
-pythonpath = . tests
-DJANGO_SETTINGS_MODULE = django_minio_storage_tests.settings
-addopts=--tb=short
-python_files = tests.py test_*.py *_tests.py
-django_find_project = false
+[tox]
+envlist =
+       {py38,py39,py310,py311}-django42-minioknown
+       py311-django{32,42}-minioknown
+       py311-django42-minio
+       lint
+       docs
+       pyright
 
 [gh-actions]
 python =
        3.8: py38
        3.9: py39
        3.10: py310
-       3.11: py311, lint, docs
+       3.11: py311, lint, docs, pyright
 
+[pytest]
+pythonpath = . tests
+DJANGO_SETTINGS_MODULE = django_minio_storage_tests.settings
+addopts=--tb=short
+python_files = tests.py test_*.py *_tests.py
+django_find_project = false
 
 [testenv]
 commands = pytest {posargs}
 setenv =
         PYTHONDONTWRITEBYTECODE=1
         MINIO_STORAGE_ENDPOINT={env:MINIO_STORAGE_ENDPOINT:localhost:9153}
         MINIO_STORAGE_ACCESS_KEY={env:MINIO_STORAGE_ACCESS_KEY:weak_access_key}
@@ -24,14 +32,35 @@
 deps =
         django32: Django==3.2.*
         django42: Django==4.2.*
         minio: minio
         minioknown: minio==7.1.12
         -rdev-requirements.txt
 
+[testenv:py311-django42-minioknown]
+commands = pytest --cov --cov-append --cov-report=term-missing {posargs}
+
+[testenv:coverage-report]
+basepython = python3.11
+deps = coverage[toml]
+skip_install = true
+commands =
+    coverage report
+    coverage html
+depends=py311-django42-minioknown
+
+[testenv:pyright]
+basepython = python3
+deps =
+        pyright
+        -rdev-requirements.txt
+commands =
+    pyright --skipunannotated --level WARNING
+
+
 [testenv:lint]
 setenv=
     PYTHONWARNINGS=ignore
 basepython = python3
 deps =
         flake8==4.0.1
         isort==5.10.1
@@ -56,14 +85,7 @@
         black .
 
 [testenv:docs]
 basepython = python3
 deps = mkdocs
 commands = mkdocs build
 
-[tox]
-envlist =
-       {py38,py39,py310,py311}-django42-minioknown
-       py311-django{32,42}-minioknown
-       py311-django42-minio
-       lint
-       docs
```

