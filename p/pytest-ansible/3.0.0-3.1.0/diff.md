# Comparing `tmp/pytest-ansible-3.0.0.tar.gz` & `tmp/pytest-ansible-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ansible-3.0.0.tar", last modified: Fri Apr 14 16:27:42 2023, max compression
+gzip compressed data, was "pytest-ansible-3.1.0.tar", last modified: Fri May  5 12:19:50 2023, max compression
```

## Comparing `pytest-ansible-3.0.0.tar` & `pytest-ansible-3.1.0.tar`

### file list

```diff
@@ -1,71 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.765158 pytest-ansible-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.741158 pytest-ansible-3.0.0/.config/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.config/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.741158 pytest-ansible-3.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.745158 pytest-ansible-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.745158 pytest-ansible-3.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-04-14 16:27:42.761157 pytest-ansible-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/inventory
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:27:42.765158 pytest-ansible-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.737158 pytest-ansible-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.749158 pytest-ansible-3.0.0/src/pytest_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/has_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.753157 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v29.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.757157 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v29.py
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/src/pytest_ansible/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.753157 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 16:27:42.000000 pytest-ansible-3.0.0/src/pytest_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:27:42.761157 pytest-ansible-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_adhoc_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_host_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_module_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_module_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-14 16:27:26.000000 pytest-ansible-3.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.306345 pytest-ansible-3.1.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.306345 pytest-ansible-3.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.310345 pytest-ansible-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.310345 pytest-ansible-3.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/inventory
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.294345 pytest-ansible-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.314345 pytest-ansible-3.1.0/src/pytest_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/has_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.322345 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v29.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.326346 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v29.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.318345 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_adhoc_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_host_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_module_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_module_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/unit/test_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tox.ini
```

### Comparing `pytest-ansible-3.0.0/.config/requirements-lock.txt` & `pytest-ansible-3.1.0/.config/requirements-lock.txt`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/.config/requirements.txt` & `pytest-ansible-3.1.0/.config/requirements.txt`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/.flake8` & `pytest-ansible-3.1.0/.flake8`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/.github/workflows/release.yml` & `pytest-ansible-3.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/.github/workflows/tox.yml` & `pytest-ansible-3.1.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/.gitignore` & `pytest-ansible-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/.pre-commit-config.yaml` & `pytest-ansible-3.1.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -10,33 +10,28 @@
   skip:
     - pip-compile
 repos:
   - repo: meta
     hooks:
       - id: check-useless-excludes
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.261"
+    rev: "v0.0.263"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         always_run: true
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        name: Sort import statements using isort
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pycqa/flake8.git
     rev: 6.0.0
```

### Comparing `pytest-ansible-3.0.0/HISTORY.md` & `pytest-ansible-3.1.0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/LICENSE` & `pytest-ansible-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/PKG-INFO` & `pytest-ansible-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.0.0
-Summary: Plugin for py.test to simplify calling ansible modules from tests or fixtures
+Version: 3.1.0
+Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
 Project-URL: changelog, https://github.com/ansible-community/pytest-ansible/releases
@@ -31,15 +31,15 @@
 # pytest-ansible
 
 [![Build Status](https://github.com/ansible-community/pytest-ansible/actions/workflows/tox.yml/badge.svg)](https://github.com/ansible-community/pytest-ansible/actions/workflows/tox.yml)
 [![Version](https://img.shields.io/pypi/v/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 [![License](https://img.shields.io/pypi/l/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 
-This repository contains a plugin for `py.test` which adds several fixtures
+This repository contains a plugin for `pytest` which adds several fixtures
 for running `ansible` modules, or inspecting `ansible_facts`. While one
 can simply call out to `ansible` using the `subprocess` module, having to
 parse stdout to determine the outcome of the operation is unpleasant and prone
 to error. With `pytest-ansible`, modules return JSON data which you can
 inspect and act on, much like with an ansible
 [playbook](http://docs.ansible.com/playbooks.html).
 
@@ -49,18 +49,18 @@
 
 ```bash
 pip install pytest-ansible
 ```
 
 ## Usage
 
-Once installed, the following `py.test` command-line parameters are available:
+Once installed, the following `pytest` command-line parameters are available:
 
 ```bash
-py.test \
+pytest \
     [--inventory <path_to_inventory>] \
     [--extra-inventory <path_to_extra_inventory>] \
     [--host-pattern <host-pattern>] \
     [--connection <plugin>] \
     [--module-path <path_to_modules] \
     [--user <username>] \
     [--become] \
@@ -86,27 +86,27 @@
 supported by ansible, which includes an [INI
 file](http://docs.ansible.com/ansible/latest/intro_inventory.html) or an
 executable script that returns [properly formatted
 JSON](http://docs.ansible.com/ansible/latest/intro_dynamic_inventory.html).
 For example,
 
 ```bash
-py.test --inventory my_inventory.ini --host-pattern all
+pytest --inventory my_inventory.ini --host-pattern all
 ```
 
 or
 
 ```bash
-py.test --inventory path/to/my/script.py --host-pattern webservers
+pytest --inventory path/to/my/script.py --host-pattern webservers
 ```
 
 or
 
 ```bash
-py.test --inventory one.example.com,two.example.com --host-pattern all
+pytest --inventory one.example.com,two.example.com --host-pattern all
 ```
 
 In the above examples, the inventory provided at runtime will be used in all
 tests that use the `ansible_adhoc` fixture. A more realistic scenario may
 involve using different inventory files (or host patterns) with different
 tests. To accomplish this, the fixture `ansible_adhoc` allows you to customize
 the inventory parameters. Read on for more detail on using the `ansible_adhoc`
@@ -117,26 +117,26 @@
 Using ansible first starts with defining your extra inventory. This feature was added in version 2.3.0, and is intended
 to allow the user to work with two different inventories. This can be done in several ways, but to start,
 we'll use the `ansible_adhoc` fixture.
 
 For example,
 
 ```bash
-py.test --inventory my_inventory.ini --extra-inventory my_second_inventory.ini --host-pattern host_in_second_inventory
+pytest --inventory my_inventory.ini --extra-inventory my_second_inventory.ini --host-pattern host_in_second_inventory
 ```
 
 ### Fixture `ansible_adhoc`
 
 The `ansible_adhoc` fixture returns a function used to initialize
 a `HostManager` object. The `ansible_adhoc` fixture will default to parameters
-supplied to the `py.test` command-line, but also allows one to provide keyword
+supplied to the `pytest` command-line, but also allows one to provide keyword
 arguments used to initialize the inventory.
 
 The example below demonstrates basic usage with options supplied at run-time to
-`py.test`.
+`pytest`.
 
 ```python
 def test_all_the_pings(ansible_adhoc):
     ansible_adhoc().all.ping()
 ```
 
 The following example demonstrates available keyword arguments when creating
@@ -206,15 +206,15 @@
     localhost.ec2(**params)
 ```
 
 ### Fixture `ansible_module`
 
 The `ansible_module` fixture allows tests and fixtures to call [ansible
 modules](http://docs.ansible.com/modules.html). Unlike the `ansible_adhoc`
-fixture, this fixture only uses the options supplied to `py.test` at run time.
+fixture, this fixture only uses the options supplied to `pytest` at run time.
 
 A very basic example demonstrating the ansible [`ping` module](http://docs.ansible.com/ping_module.html):
 
 ```python
 def test_ping(ansible_module):
     ansible_module.ping()
 ```
```

### Comparing `pytest-ansible-3.0.0/README.md` & `pytest-ansible-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pytest-ansible
 
 [![Build Status](https://github.com/ansible-community/pytest-ansible/actions/workflows/tox.yml/badge.svg)](https://github.com/ansible-community/pytest-ansible/actions/workflows/tox.yml)
 [![Version](https://img.shields.io/pypi/v/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 [![License](https://img.shields.io/pypi/l/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 
-This repository contains a plugin for `py.test` which adds several fixtures
+This repository contains a plugin for `pytest` which adds several fixtures
 for running `ansible` modules, or inspecting `ansible_facts`. While one
 can simply call out to `ansible` using the `subprocess` module, having to
 parse stdout to determine the outcome of the operation is unpleasant and prone
 to error. With `pytest-ansible`, modules return JSON data which you can
 inspect and act on, much like with an ansible
 [playbook](http://docs.ansible.com/playbooks.html).
 
@@ -19,18 +19,18 @@
 
 ```bash
 pip install pytest-ansible
 ```
 
 ## Usage
 
-Once installed, the following `py.test` command-line parameters are available:
+Once installed, the following `pytest` command-line parameters are available:
 
 ```bash
-py.test \
+pytest \
     [--inventory <path_to_inventory>] \
     [--extra-inventory <path_to_extra_inventory>] \
     [--host-pattern <host-pattern>] \
     [--connection <plugin>] \
     [--module-path <path_to_modules] \
     [--user <username>] \
     [--become] \
@@ -56,27 +56,27 @@
 supported by ansible, which includes an [INI
 file](http://docs.ansible.com/ansible/latest/intro_inventory.html) or an
 executable script that returns [properly formatted
 JSON](http://docs.ansible.com/ansible/latest/intro_dynamic_inventory.html).
 For example,
 
 ```bash
-py.test --inventory my_inventory.ini --host-pattern all
+pytest --inventory my_inventory.ini --host-pattern all
 ```
 
 or
 
 ```bash
-py.test --inventory path/to/my/script.py --host-pattern webservers
+pytest --inventory path/to/my/script.py --host-pattern webservers
 ```
 
 or
 
 ```bash
-py.test --inventory one.example.com,two.example.com --host-pattern all
+pytest --inventory one.example.com,two.example.com --host-pattern all
 ```
 
 In the above examples, the inventory provided at runtime will be used in all
 tests that use the `ansible_adhoc` fixture. A more realistic scenario may
 involve using different inventory files (or host patterns) with different
 tests. To accomplish this, the fixture `ansible_adhoc` allows you to customize
 the inventory parameters. Read on for more detail on using the `ansible_adhoc`
@@ -87,26 +87,26 @@
 Using ansible first starts with defining your extra inventory. This feature was added in version 2.3.0, and is intended
 to allow the user to work with two different inventories. This can be done in several ways, but to start,
 we'll use the `ansible_adhoc` fixture.
 
 For example,
 
 ```bash
-py.test --inventory my_inventory.ini --extra-inventory my_second_inventory.ini --host-pattern host_in_second_inventory
+pytest --inventory my_inventory.ini --extra-inventory my_second_inventory.ini --host-pattern host_in_second_inventory
 ```
 
 ### Fixture `ansible_adhoc`
 
 The `ansible_adhoc` fixture returns a function used to initialize
 a `HostManager` object. The `ansible_adhoc` fixture will default to parameters
-supplied to the `py.test` command-line, but also allows one to provide keyword
+supplied to the `pytest` command-line, but also allows one to provide keyword
 arguments used to initialize the inventory.
 
 The example below demonstrates basic usage with options supplied at run-time to
-`py.test`.
+`pytest`.
 
 ```python
 def test_all_the_pings(ansible_adhoc):
     ansible_adhoc().all.ping()
 ```
 
 The following example demonstrates available keyword arguments when creating
@@ -176,15 +176,15 @@
     localhost.ec2(**params)
 ```
 
 ### Fixture `ansible_module`
 
 The `ansible_module` fixture allows tests and fixtures to call [ansible
 modules](http://docs.ansible.com/modules.html). Unlike the `ansible_adhoc`
-fixture, this fixture only uses the options supplied to `py.test` at run time.
+fixture, this fixture only uses the options supplied to `pytest` at run time.
 
 A very basic example demonstrating the ansible [`ping` module](http://docs.ansible.com/ping_module.html):
 
 ```python
 def test_ping(ansible_module):
     ansible_module.ping()
 ```
```

### Comparing `pytest-ansible-3.0.0/inventory` & `pytest-ansible-3.1.0/inventory`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/pyproject.toml` & `pytest-ansible-3.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 # https://peps.python.org/pep-0621/#readme
 requires-python = ">=3.9"
 dynamic = ["version", "dependencies", "optional-dependencies"]
 name = "pytest-ansible"
-description = "Plugin for py.test to simplify calling ansible modules from tests or fixtures"
+description = "Plugin for pytest to simplify calling ansible modules from tests or fixtures"
 readme = "README.md"
 authors = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
 maintainers = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
 license = { text = "MIT" }
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Developers',
@@ -37,32 +37,26 @@
 
 [project.urls]
 homepage = "https://github.com/ansible-community/pytest-ansible"
 documentation = "https://github.com/ansible-community/pytest-ansible"
 repository = "https://github.com/ansible-community/pytest-ansible"
 changelog = "https://github.com/ansible-community/pytest-ansible/releases"
 
-[tool.isort]
-force_single_line = true # Force from .. import to be 1 per line, minimizing changes at time of implementation
-known_first_party = ["pytest_ansible"]
-lines_after_imports = 2 # Ensures consistency for cases when there's variable vs function/class definitions after imports
-lines_between_types = 1 # Separate import/from with 1 line
-no_lines_before = "LOCALFOLDER" # Keeps local imports bundled with first-party
-profile = "black" # Avoid conflict with black
-skip_glob = []
-
 [tool.mypy]
 python_version = 3.9
+ignore_missing_imports = true
+ignore_errors = true
 # strict = true
 color_output = true
 error_summary = true
 # Temporary disabled until we fix them:
 disallow_untyped_calls = false
 disallow_untyped_defs = false
 disallow_any_generics = false
+disable_error_code = ["var-annotated", "attr-defined"]
 
 [[tool.mypy.overrides]]
 module = ["ansible.*"]
 ignore_missing_imports = true
 ignore_errors = true
 
 [tool.pylint.MAIN]
@@ -82,26 +76,25 @@
   # https://github.com/PyCQA/pylint/issues/8453
   "preferred-module",
   # Temporarily disabled until we fix them:
   "duplicate-code",
   "fixme",
   "import-error",
   "import-outside-toplevel",
-  "invalid-name",
   "missing-function-docstring",
   "missing-module-docstring",
-  "no-member",
   "no-name-in-module",
   "protected-access",
   "redefined-outer-name",
   "too-many-branches",
   "too-many-locals",
   "too-many-statements",
   "unexpected-keyword-arg",
   "unused-argument",
+  "invalid-name",
 ]
 
 [tool.pytest]
 minversion = 6.0
 addopts = ["-v", "--tb=native"]
 markers = [
   "old",
@@ -109,24 +102,50 @@
   "ansible_v1_xfail",
   "requires_ansible_v1",
   "requires_ansible_v2",
   "requires_ansible_v24",
 ]
 
 [tool.ruff]
-select = ["PT"]
+select = ["ALL"]
 ignore = [
   "E501", # we use black
-
+  # temporary disabled until we fix them:
+  "ANN",
+  "ARG",
+  "B",
+  "C",
+  "D",
+  "EM",
+  "FBT",
+  "INP",
+  "ISC",
+  "PGH",
+  "PIE",
+  "PLC",
+  "PLR",
+  "PLW",
+  "RUF",
+  "S",
+  "SLF",
+  "T",
+  "TRY",
+  "PTH",
+  "TCH",
 ]
 target-version = "py39"
+# Same as Black.
+line-length = 88
 
 [tool.ruff.flake8-pytest-style]
 parametrize-values-type = "tuple"
 
+[tool.ruff.per-file-ignores]
+"tests/**" = ["S101"]
+
 [tool.setuptools.dynamic]
 optional-dependencies.test = { file = [".config/requirements-test.txt"] }
 optional-dependencies.lock = { file = [".config/requirements-lock.txt"] }
 dependencies = { file = [".config/requirements.in"] }
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/errors.py` & `pytest-ansible-3.1.0/src/pytest_ansible/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Defines pytest-ansible exception classes."""
 
 import ansible.errors
 
 
 class AnsibleNoHostsMatch(ansible.errors.AnsibleError):
-
     """Sub-class AnsibleError when no hosts match."""
 
 
 class AnsibleConnectionFailure(ansible.errors.AnsibleError):
-
     """Sub-class AnsibleError when connection failures occur."""
 
-    def __init__(self, msg, dark=None, contacted=None):
+    def __init__(self, msg, dark=None, contacted=None) -> None:
         """Initialize connection error class."""
         super().__init__(msg)
         self.contacted = contacted
         self.dark = dark
 
 
 class AnsibleModuleError(ansible.errors.AnsibleError):
-
     """Sub-class AnsibleError when module failures occur."""
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/fixtures.py` & `pytest-ansible-3.1.0/src/pytest_ansible/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/has_version.py` & `pytest-ansible-3.1.0/src/pytest_ansible/has_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import ansible
-
 from pkg_resources import parse_version
 
-
 has_ansible_v1 = parse_version(ansible.__version__) < parse_version("2.0.0")
 has_ansible_v2 = parse_version(ansible.__version__) >= parse_version("2.0.0")
 has_ansible_v24 = parse_version(ansible.__version__) >= parse_version("2.4.0")
 has_ansible_v28 = parse_version(ansible.__version__) >= parse_version(
-    "2.8.0.dev0"
+    "2.8.0.dev0",
 ) or parse_version(ansible.__version__) >= parse_version("2.8.0")
 has_ansible_v29 = parse_version(ansible.__version__) >= parse_version("2.9.0")
 has_ansible_v212 = parse_version(ansible.__version__) >= parse_version("2.12.0")
 has_ansible_v213 = parse_version(ansible.__version__) >= parse_version("2.13.0")
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/__init__.py` & `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Fixme."""
 
 import ansible
 
-from pytest_ansible.has_version import has_ansible_v2
-from pytest_ansible.has_version import has_ansible_v24
-from pytest_ansible.has_version import has_ansible_v28
-from pytest_ansible.has_version import has_ansible_v29
-from pytest_ansible.has_version import has_ansible_v212
-from pytest_ansible.has_version import has_ansible_v213
+from pytest_ansible.has_version import (
+    has_ansible_v2,
+    has_ansible_v24,
+    has_ansible_v28,
+    has_ansible_v29,
+    has_ansible_v212,
+    has_ansible_v213,
+)
 
 
 class BaseHostManager:
     """Fixme."""
 
     _required_kwargs = ("inventory",)
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Fixme."""
         self.options = kwargs
 
         self.check_required_kwargs(**kwargs)
 
         # Sub-classes should override this value
         self._dispatcher = self._default_dispatcher
@@ -36,15 +38,15 @@
                 extra_inventory_hosts = [
                     h.name for h in self.options["extra_inventory_manager"].list_hosts()
                 ]
             else:
                 extra_inventory_hosts = [
                     h.name
                     for h in self.options["extra_inventory_manager"].list_hosts(
-                        host_pattern
+                        host_pattern,
                     )
                 ]
         except KeyError:
             extra_inventory_hosts = []
         return extra_inventory_hosts
 
     def get_extra_inventory_groups(self):
@@ -104,43 +106,40 @@
         ]
         extra_inventory_hosts = self.get_extra_inventory_hosts()
         return inventory_hosts + extra_inventory_hosts
 
     def __iter__(self):
         """Return an iterator for hosts matching the `host_pattern`."""
         extra_hosts = self.get_extra_inventory_hosts(
-            host_pattern=self.options["host_pattern"]
+            host_pattern=self.options["host_pattern"],
         )
         all_hosts = self.options["inventory_manager"].list_hosts(
-            self.options["host_pattern"]
+            self.options["host_pattern"],
         )
         # Return only the name (ala .keys()
-        # return iter(self.options['inventory_manager'].list_hosts(self.options['host_pattern']))
         # Return a BaseHostManager instance initialized for each host in the inventory
-        # return iter([self.__class__(host_pattern=h, **self.options) for h in all_hosts])
         # Return a ModuleDispatcher representing the group
         return iter([self[h] for h in all_hosts + extra_hosts])
 
-    def __len__(self):
+    def __len__(self) -> int:
         """Return the number of inventory hosts."""
         return len(self.options["inventory_manager"].list_hosts()) + len(
-            self.get_extra_inventory_hosts()
+            self.get_extra_inventory_hosts(),
         )
 
-    def __contains__(self, item):
+    def __contains__(self, item) -> bool:
         """Return whether there is inventory matching the provided `item`."""
         return self.has_matching_inventory(item)
 
     def initialize_inventory(self):
         raise NotImplementedError("Must be implemented by sub-class")
 
 
 def get_host_manager(*args, **kwargs):
     """Initialize and return a HostManager instance."""
-
     if has_ansible_v213:
         from pytest_ansible.host_manager.v213 import HostManagerV213 as HostManager
     elif has_ansible_v212:
         from pytest_ansible.host_manager.v212 import HostManagerV212 as HostManager
     elif has_ansible_v29:
         from pytest_ansible.host_manager.v29 import HostManagerV29 as HostManager
     elif has_ansible_v28:
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v1.py` & `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from ansible.inventory import Inventory
 
 from pytest_ansible.host_manager import BaseHostManager
 from pytest_ansible.module_dispatcher.v1 import ModuleDispatcherV1
 
 
 class HostManagerV1(BaseHostManager):
-
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Fixme."""
         super().__init__(*args, **kwargs)
         self._dispatcher = ModuleDispatcherV1
 
     def keys(self):
         return list(self.options["inventory_manager"].list_hosts())
 
     def initialize_inventory(self):
         self.options["inventory_manager"] = Inventory(self.options["inventory"])
-        # self.options['inventory_manager'].subset(self.pattern)
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v2.py` & `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 from ansible.vars import VariableManager
 
 from pytest_ansible.host_manager import BaseHostManager
 from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
 
 
 class HostManagerV2(BaseHostManager):
-
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Fixme."""
         super().__init__(*args, **kwargs)
         self._dispatcher = ModuleDispatcherV2
 
     def initialize_inventory(self):
         self.options["loader"] = DataLoader()
         self.options["variable_manager"] = VariableManager()
         self.options["inventory_manager"] = Inventory(
             loader=self.options["loader"],
             variable_manager=self.options["variable_manager"],
             host_list=self.options["inventory"],
         )
         self.options["variable_manager"].set_inventory(
-            self.options["inventory_manager"]
+            self.options["inventory_manager"],
         )
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v212.py` & `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v213.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from ansible.inventory.manager import InventoryManager
 from ansible.parsing.dataloader import DataLoader
 from ansible.vars.manager import VariableManager
 
 from pytest_ansible.host_manager import BaseHostManager
-from pytest_ansible.module_dispatcher.v212 import ModuleDispatcherV212
+from pytest_ansible.module_dispatcher.v213 import ModuleDispatcherV213
 
 
-class HostManagerV212(BaseHostManager):
+class HostManagerV213(BaseHostManager):
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Fixme."""
         super().__init__(*args, **kwargs)
-        self._dispatcher = ModuleDispatcherV212
+        self._dispatcher = ModuleDispatcherV213
 
     def initialize_inventory(self):
         self.options["loader"] = DataLoader()
         self.options["inventory_manager"] = InventoryManager(
-            loader=self.options["loader"], sources=self.options["inventory"]
+            loader=self.options["loader"],
+            sources=self.options["inventory"],
         )
         self.options["variable_manager"] = VariableManager(
-            loader=self.options["loader"], inventory=self.options["inventory_manager"]
+            loader=self.options["loader"],
+            inventory=self.options["inventory_manager"],
         )
         if "extra_inventory" in self.options:
             self.options["extra_loader"] = DataLoader()
             self.options["extra_inventory_manager"] = InventoryManager(
                 loader=self.options["extra_loader"],
                 sources=self.options["extra_inventory"],
             )
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v213.py` & `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v212.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from ansible.inventory.manager import InventoryManager
 from ansible.parsing.dataloader import DataLoader
 from ansible.vars.manager import VariableManager
 
 from pytest_ansible.host_manager import BaseHostManager
-from pytest_ansible.module_dispatcher.v213 import ModuleDispatcherV213
+from pytest_ansible.module_dispatcher.v212 import ModuleDispatcherV212
 
 
-class HostManagerV213(BaseHostManager):
+class HostManagerV212(BaseHostManager):
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Fixme."""
         super().__init__(*args, **kwargs)
-        self._dispatcher = ModuleDispatcherV213
+        self._dispatcher = ModuleDispatcherV212
 
     def initialize_inventory(self):
         self.options["loader"] = DataLoader()
         self.options["inventory_manager"] = InventoryManager(
-            loader=self.options["loader"], sources=self.options["inventory"]
+            loader=self.options["loader"],
+            sources=self.options["inventory"],
         )
         self.options["variable_manager"] = VariableManager(
-            loader=self.options["loader"], inventory=self.options["inventory_manager"]
+            loader=self.options["loader"],
+            inventory=self.options["inventory_manager"],
         )
         if "extra_inventory" in self.options:
             self.options["extra_loader"] = DataLoader()
             self.options["extra_inventory_manager"] = InventoryManager(
                 loader=self.options["extra_loader"],
                 sources=self.options["extra_inventory"],
             )
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v24.py` & `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v24.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from ansible.vars.manager import VariableManager
 
 from pytest_ansible.host_manager import BaseHostManager
 from pytest_ansible.module_dispatcher.v24 import ModuleDispatcherV24
 
 
 class HostManagerV24(BaseHostManager):
-
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Fixme."""
         super().__init__(*args, **kwargs)
         self._dispatcher = ModuleDispatcherV24
 
     def initialize_inventory(self):
         self.options["loader"] = DataLoader()
         self.options["inventory_manager"] = InventoryManager(
-            loader=self.options["loader"], sources=self.options["inventory"]
+            loader=self.options["loader"],
+            sources=self.options["inventory"],
         )
         self.options["variable_manager"] = VariableManager(
-            loader=self.options["loader"], inventory=self.options["inventory_manager"]
+            loader=self.options["loader"],
+            inventory=self.options["inventory_manager"],
         )
-        # self.options['inventory_manager'].clear_caches()
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v28.py` & `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v28.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from ansible.vars.manager import VariableManager
 
 from pytest_ansible.host_manager import BaseHostManager
 from pytest_ansible.module_dispatcher.v28 import ModuleDispatcherV28
 
 
 class HostManagerV28(BaseHostManager):
-
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Fixme."""
         super().__init__(*args, **kwargs)
         self._dispatcher = ModuleDispatcherV28
 
     def initialize_inventory(self):
         self.options["loader"] = DataLoader()
         self.options["inventory_manager"] = InventoryManager(
-            loader=self.options["loader"], sources=self.options["inventory"]
+            loader=self.options["loader"],
+            sources=self.options["inventory"],
         )
         self.options["variable_manager"] = VariableManager(
-            loader=self.options["loader"], inventory=self.options["inventory_manager"]
+            loader=self.options["loader"],
+            inventory=self.options["inventory_manager"],
         )
-        # self.options['inventory_manager'].clear_caches()
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/host_manager/v29.py` & `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v29.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 from pytest_ansible.host_manager import BaseHostManager
 from pytest_ansible.module_dispatcher.v29 import ModuleDispatcherV29
 
 
 class HostManagerV29(BaseHostManager):
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Fixme."""
         super().__init__(*args, **kwargs)
         self._dispatcher = ModuleDispatcherV29
 
     def initialize_inventory(self):
         self.options["loader"] = DataLoader()
         self.options["inventory_manager"] = InventoryManager(
-            loader=self.options["loader"], sources=self.options["inventory"]
+            loader=self.options["loader"],
+            sources=self.options["inventory"],
         )
         self.options["variable_manager"] = VariableManager(
-            loader=self.options["loader"], inventory=self.options["inventory_manager"]
+            loader=self.options["loader"],
+            inventory=self.options["inventory_manager"],
         )
         if "extra_inventory" in self.options:
             self.options["extra_loader"] = DataLoader()
             self.options["extra_inventory_manager"] = InventoryManager(
                 loader=self.options["extra_loader"],
                 sources=self.options["extra_inventory"],
             )
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/__init__.py` & `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 """Define BaseModuleDispatcher class."""
 
-from typing import Sequence
+from collections.abc import Sequence
 
 from pytest_ansible.errors import AnsibleModuleError
 
 
 class BaseModuleDispatcher:
-
     """Fixme.."""
 
     required_kwargs: Sequence[str] = ("inventory",)
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         """Save provided keyword arguments and assert required values have been provided."""
         self.options = kwargs
 
         # Assert the expected kwargs were provided
         self.check_required_kwargs(**kwargs)
 
-    def __len__(self):
+    def __len__(self) -> int:
         """Return the number of hosts that match the `host_pattern`."""
         return len(
-            self.options["inventory_manager"].list_hosts(self.options["host_pattern"])
+            self.options["inventory_manager"].list_hosts(self.options["host_pattern"]),
         )
 
-    def __contains__(self, item):
+    def __contains__(self, item) -> bool:
         """Return the whether the inventory contains a host matching the provided `item`."""
         return len(self.options["inventory_manager"].list_hosts(item)) > 0
 
     def __getattr__(self, name):
         """Run the ansible module matching the provided `name`.
 
         Raise `AnsibleModuleError` when no such module exists.
         """
         if not self.has_module(name):
             # TODO: should we just raise an AttributeError, or a more
-            # raise AttributeError("'{0}' object has no attribute '{1}'".format(self.__class__.__name__, name))
             raise AnsibleModuleError(
-                f"The module {name} was not found in configured module paths."
+                f"The module {name} was not found in configured module paths.",
             )
         self.options["module_name"] = name
         return self._run
 
     def check_required_kwargs(self, **kwargs):
         """Raise a TypeError if any required kwargs are missing."""
         for kwarg in self.required_kwargs:
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v1.py` & `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import warnings
 
 import ansible
 import ansible.constants
 import ansible.errors
 import ansible.utils
-
 from ansible.runner import Runner
+from ansible.utils import module_finder
 
 from pytest_ansible.errors import AnsibleConnectionFailure
 from pytest_ansible.has_version import has_ansible_v1
 from pytest_ansible.module_dispatcher import BaseModuleDispatcher
 from pytest_ansible.results import AdHocResult
 
-
 if not has_ansible_v1:
     raise ImportError("Only supported with ansible < 2.0")
 
 
 class ModuleDispatcherV1(BaseModuleDispatcher):
-
     """Pass."""
 
     required_kwargs = ("inventory", "inventory_manager", "host_pattern")
 
     def has_module(self, name):
         # Make sure we parse module_path and pass it to the loader,
         # otherwise, only built-in modules will work.
@@ -30,15 +28,15 @@
             paths = self.options["module_path"]
             if isinstance(paths, (list, tuple, set)):
                 for path in paths:
                     ansible.utils.module_finder.add_directory(path)
             else:
                 ansible.utils.module_finder.add_directory(paths)
 
-        return ansible.utils.module_finder.has_plugin(name)
+        return module_finder.has_plugin(name)
 
     def _run(self, *module_args, **complex_args):
         """Execute an ansible adhoc command returning the results in a AdHocResult object."""
         # Assemble module argument string
         if module_args:
             complex_args.update({"_raw_params": " ".join(module_args)})
         else:
@@ -49,19 +47,19 @@
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
         self.options["inventory_manager"].subset(self.options.get("subset"))
         hosts = self.options["inventory_manager"].list_hosts(
-            self.options["host_pattern"]
+            self.options["host_pattern"],
         )
         if len(hosts) == 0 and not no_hosts:
             raise ansible.errors.AnsibleError(
-                "Specified hosts and/or --limit does not match any hosts"
+                "Specified hosts and/or --limit does not match any hosts",
             )
 
         # Build module runner object
         kwargs = {
             "inventory": self.options.get("inventory_manager"),
             "pattern": self.options.get("host_pattern"),
             "module_name": self.options.get("module_name"),
@@ -77,12 +75,14 @@
 
         # Run the module
         runner = Runner(**kwargs)
         results = runner.run()
 
         if "dark" in results and results["dark"]:
             raise AnsibleConnectionFailure(
-                "Host unreachable", dark=results["dark"], contacted=results["contacted"]
+                "Host unreachable",
+                dark=results["dark"],
+                contacted=results["contacted"],
             )
 
         # Success!
         return AdHocResult(contacted=results["contacted"])
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v2.py` & `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v24.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from __future__ import annotations
-
 import warnings
 
-from typing import Sequence
-
 import ansible.constants
 import ansible.errors
 import ansible.utils
-
-# from ansible.plugins.loader import module_loader
 from ansible.cli import CLI
 from ansible.executor.task_queue_manager import TaskQueueManager
 from ansible.playbook.play import Play
 from ansible.plugins.callback import CallbackBase
+from ansible.plugins.loader import module_loader
 
 from pytest_ansible.errors import AnsibleConnectionFailure
-from pytest_ansible.has_version import has_ansible_v2
-from pytest_ansible.module_dispatcher import BaseModuleDispatcher
+from pytest_ansible.has_version import has_ansible_v24
+from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
 from pytest_ansible.results import AdHocResult
 
+# pylint: disable=ungrouped-imports, wrong-import-position
+
+if not has_ansible_v24:
+    raise ImportError("Only supported with ansible-2.4 and newer")
+
 
-if not has_ansible_v2:
-    raise ImportError("Only supported with ansible-2.* and newer")
+# pylint: enable=ungrouped-imports
 
 
 class ResultAccumulator(CallbackBase):
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Initialize object."""
         super().__init__(*args, **kwargs)
         self.contacted = {}
         self.unreachable = {}
 
     def v2_runner_on_failed(self, result, *args, **kwargs):
         self.contacted[result._host.get_name()] = result._result
@@ -42,38 +41,37 @@
         self.unreachable[result._host.get_name()] = result._result
 
     @property
     def results(self):
         return {"contacted": self.contacted, "unreachable": self.unreachable}
 
 
-class ModuleDispatcherV2(BaseModuleDispatcher):
+class ModuleDispatcherV24(ModuleDispatcherV2):
     """Pass."""
 
-    required_kwargs: Sequence[str] = (
+    required_kwargs = (
         "inventory",
         "inventory_manager",
         "variable_manager",
         "host_pattern",
         "loader",
     )
 
     def has_module(self, name):
         # Make sure we parse module_path and pass it to the loader,
         # otherwise, only built-in modules will work.
         if "module_path" in self.options:
             paths = self.options["module_path"]
             if isinstance(paths, (list, tuple, set)):
                 for path in paths:
-                    ansible.plugins.module_loader.add_directory(path)
+                    module_loader.add_directory(path)
             else:
-                ansible.plugins.module_loader.add_directory(paths)
+                module_loader.add_directory(paths)
 
-        return ansible.plugins.module_loader.has_plugin(name)
-        # return module_loader.has_plugin(name)
+        return module_loader.has_plugin(name)
 
     def _run(self, *module_args, **complex_args):
         """Execute an ansible adhoc command returning the result in a AdhocResult object."""
         # Assemble module argument string
         if module_args:
             complex_args.update({"_raw_params": " ".join(module_args)})
 
@@ -82,21 +80,22 @@
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
         self.options["inventory_manager"].subset(self.options.get("subset"))
         hosts = self.options["inventory_manager"].list_hosts(
-            self.options["host_pattern"]
+            self.options["host_pattern"],
         )
         if len(hosts) == 0 and not no_hosts:
             raise ansible.errors.AnsibleError(
-                "Specified hosts and/or --limit does not match any hosts"
+                "Specified hosts and/or --limit does not match any hosts",
             )
 
+        # pylint: disable=no-member
         parser = CLI.base_parser(
             runas_opts=True,
             inventory_opts=True,
             async_opts=True,
             output_opts=True,
             connect_opts=True,
             check_opts=True,
@@ -113,37 +112,37 @@
         options.remote_user = self.options.get("user")
         options.become = self.options.get("become")
         options.become_method = self.options.get("become_method")
         options.become_user = self.options.get("become_user")
         options.module_path = self.options.get("module_path")
 
         # Initialize callback to capture module JSON responses
-        cb = ResultAccumulator()
+        callback = ResultAccumulator()
 
         kwargs = {
             "inventory": self.options["inventory_manager"],
             "variable_manager": self.options["variable_manager"],
             "loader": self.options["loader"],
             "options": options,
-            "stdout_callback": cb,
+            "stdout_callback": callback,
             "passwords": {"conn_pass": None, "become_pass": None},
         }
 
         # create a pseudo-play to execute the specified module via a single task
         play_ds = {
             "name": "pytest-ansible",
             "hosts": self.options["host_pattern"],
             "gather_facts": "no",
             "tasks": [
                 {
                     "action": {
                         "module": self.options["module_name"],
                         "args": complex_args,
-                    }
-                }
+                    },
+                },
             ],
         }
 
         play = Play().load(
             play_ds,
             variable_manager=self.options["variable_manager"],
             loader=self.options["loader"],
@@ -156,14 +155,16 @@
             tqm.run(play)
         finally:
             if tqm:
                 tqm.cleanup()
 
         # Raise exception if host(s) unreachable
         # FIXME - if multiple hosts were involved, should an exception be raised?
-        if cb.unreachable:
+        if callback.unreachable:
             raise AnsibleConnectionFailure(
-                "Host unreachable", dark=cb.unreachable, contacted=cb.contacted
+                "Host unreachable",
+                dark=callback.unreachable,
+                contacted=callback.contacted,
             )
 
         # Success!
-        return AdHocResult(contacted=cb.contacted)
+        return AdHocResult(contacted=callback.contacted)
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v212.py` & `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v29.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-from __future__ import annotations
-
 import sys
 import warnings
 
-from typing import Sequence
-
 import ansible.constants
 import ansible.errors
 import ansible.utils
-
 from ansible.cli.adhoc import AdHocCLI
 from ansible.executor.task_queue_manager import TaskQueueManager
 from ansible.playbook.play import Play
 from ansible.plugins.callback import CallbackBase
 from ansible.plugins.loader import module_loader
 
 from pytest_ansible.errors import AnsibleConnectionFailure
-from pytest_ansible.has_version import has_ansible_v212
+from pytest_ansible.has_version import has_ansible_v29
 from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
 from pytest_ansible.results import AdHocResult
 
-
 # pylint: disable=ungrouped-imports, wrong-import-position
-if not has_ansible_v212:
-    raise ImportError("Only supported with ansible-2.12 and newer")
+
+if not has_ansible_v29:
+    raise ImportError("Only supported with ansible-2.9 and newer")
 
 
 # pylint: enable=ungrouped-imports
 
 
 class ResultAccumulator(CallbackBase):
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Initialize object."""
         super().__init__(*args, **kwargs)
         self.contacted = {}
         self.unreachable = {}
 
     def v2_runner_on_failed(self, result, *args, **kwargs):
         result2 = {"failed": True}
@@ -50,18 +45,18 @@
         self.unreachable[result._host.get_name()] = result._result
 
     @property
     def results(self):
         return {"contacted": self.contacted, "unreachable": self.unreachable}
 
 
-class ModuleDispatcherV212(ModuleDispatcherV2):
+class ModuleDispatcherV29(ModuleDispatcherV2):
     """Pass."""
 
-    required_kwargs: Sequence[str] = (
+    required_kwargs = (
         "inventory",
         "inventory_manager",
         "variable_manager",
         "host_pattern",
         "loader",
     )
 
@@ -89,19 +84,19 @@
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
         self.options["inventory_manager"].subset(self.options.get("subset"))
         hosts = self.options["inventory_manager"].list_hosts(
-            self.options["host_pattern"]
+            self.options["host_pattern"],
         )
         if len(hosts) == 0 and not no_hosts:
             raise ansible.errors.AnsibleError(
-                "Specified hosts and/or --limit does not match any hosts"
+                "Specified hosts and/or --limit does not match any hosts",
             )
 
         # Pass along cli options
         args = ["pytest-ansible"]
         verbosity = None
         for verbosity_syntax in ("-v", "-vv", "-vvv", "-vvvv", "-vvvvv"):
             if verbosity_syntax in sys.argv:
@@ -134,34 +129,34 @@
         adhoc = AdHocCLI(args)
         adhoc.parse()
 
         # And now we'll never speak of this again
         del adhoc
 
         # Initialize callbacks to capture module JSON responses
-        cb = ResultAccumulator()
+        callback = ResultAccumulator()
 
         kwargs = {
             "inventory": self.options["inventory_manager"],
             "variable_manager": self.options["variable_manager"],
             "loader": self.options["loader"],
-            "stdout_callback": cb,
+            "stdout_callback": callback,
             "passwords": {"conn_pass": None, "become_pass": None},
         }
 
         kwargs_extra = {}
         # If we have an extra inventory, do the same that we did for the inventory
         if "extra_inventory_manager" in self.options:
-            cb_extra = ResultAccumulator()
+            callback_extra = ResultAccumulator()
 
             kwargs_extra = {
                 "inventory": self.options["extra_inventory_manager"],
                 "variable_manager": self.options["extra_variable_manager"],
                 "loader": self.options["extra_loader"],
-                "stdout_callback": cb_extra,
+                "stdout_callback": callback_extra,
                 "passwords": {"conn_pass": None, "become_pass": None},
             }
 
         # create a pseudo-play to execute the specified module via a single task
         play_ds = {
             "name": "pytest-ansible",
             "hosts": self.options["host_pattern"],
@@ -179,15 +174,14 @@
         }
 
         play = Play().load(
             play_ds,
             variable_manager=self.options["variable_manager"],
             loader=self.options["loader"],
         )
-
         play_extra = None
         if "extra_inventory_manager" in self.options:
             play_extra = Play().load(
                 play_ds,
                 variable_manager=self.options["extra_variable_manager"],
                 loader=self.options["extra_loader"],
             )
@@ -208,29 +202,28 @@
                 tqm_extra.run(play_extra)
             finally:
                 if tqm_extra:
                     tqm_extra.cleanup()
 
         # Raise exception if host(s) unreachable
         # FIXME - if multiple hosts were involved, should an exception be raised?
-        if cb.unreachable:
+        if callback.unreachable:
             raise AnsibleConnectionFailure(
                 "Host unreachable in the inventory",
-                dark=cb.unreachable,
-                contacted=cb.contacted,
+                dark=callback.unreachable,
+                contacted=callback.contacted,
+            )
+        if "extra_inventory_manager" in self.options and callback_extra.unreachable:
+            raise AnsibleConnectionFailure(
+                "Host unreachable in the extra inventory",
+                dark=callback_extra.unreachable,
+                contacted=callback_extra.contacted,
             )
-        if "extra_inventory_manager" in self.options:
-            if cb_extra.unreachable:
-                raise AnsibleConnectionFailure(
-                    "Host unreachable in the extra inventory",
-                    dark=cb_extra.unreachable,
-                    contacted=cb_extra.contacted,
-                )
 
         # Success!
         return AdHocResult(
             contacted=(
-                {**cb.contacted, **cb_extra.contacted}
+                {**callback.contacted, **callback_extra.contacted}
                 if "extra_inventory_manager" in self.options
-                else cb.contacted
-            )
+                else callback.contacted
+            ),
         )
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v213.py` & `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v213.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import sys
 import warnings
 
 import ansible.constants
 import ansible.errors
 import ansible.utils
-
 from ansible.cli.adhoc import AdHocCLI
+from ansible.constants import COLLECTIONS_PATHS
 from ansible.executor.task_queue_manager import TaskQueueManager
 from ansible.playbook.play import Play
 from ansible.plugins.callback import CallbackBase
 from ansible.plugins.loader import module_loader
 
 from pytest_ansible.errors import AnsibleConnectionFailure
 from pytest_ansible.has_version import has_ansible_v213
 from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
 from pytest_ansible.results import AdHocResult
 
-
 # pylint: disable=ungrouped-imports, wrong-import-position
 if not has_ansible_v213:
     raise ImportError("Only supported with ansible-2.13 and newer")
 
 
 HAS_CUSTOM_LOADER_SUPPORT = True
 
@@ -33,15 +32,15 @@
 except ImportError:
     HAS_CUSTOM_LOADER_SUPPORT = False
 
 
 class ResultAccumulator(CallbackBase):
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Initialize object."""
         super().__init__(*args, **kwargs)
         self.contacted = {}
         self.unreachable = {}
 
     def v2_runner_on_failed(self, result, *args, **kwargs):
         result2 = {"failed": True}
@@ -98,24 +97,24 @@
         no_hosts = False
         if len(hosts + extra_hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
         self.options["inventory_manager"].subset(self.options.get("subset"))
         hosts = self.options["inventory_manager"].list_hosts(
-            self.options["host_pattern"]
+            self.options["host_pattern"],
         )
         if "extra_inventory_manager" in self.options:
             self.options["extra_inventory_manager"].subset(self.options.get("subset"))
             extra_hosts = self.options["extra_inventory_manager"].list_hosts()
         else:
             extra_hosts = []
         if len(hosts + extra_hosts) == 0 and not no_hosts:
             raise ansible.errors.AnsibleError(
-                "Specified hosts and/or --limit does not match any hosts."
+                "Specified hosts and/or --limit does not match any hosts.",
             )
 
         # Pass along cli options
         args = ["pytest-ansible"]
         verbosity = None
         for verbosity_syntax in ("-v", "-vv", "-vvv", "-vvvv", "-vvvvv"):
             if verbosity_syntax in sys.argv:
@@ -148,34 +147,34 @@
         adhoc = AdHocCLI(args)
         adhoc.parse()
 
         # And now we'll never speak of this again
         del adhoc
 
         # Initialize callbacks to capture module JSON responses
-        cb = ResultAccumulator()
+        callback = ResultAccumulator()
 
         kwargs = {
             "inventory": self.options["inventory_manager"],
             "variable_manager": self.options["variable_manager"],
             "loader": self.options["loader"],
-            "stdout_callback": cb,
+            "stdout_callback": callback,
             "passwords": {"conn_pass": None, "become_pass": None},
         }
 
         kwargs_extra = {}
         # If we have an extra inventory, do the same that we did for the inventory
         if "extra_inventory_manager" in self.options:
-            cb_extra = ResultAccumulator()
+            callback_extra = ResultAccumulator()
 
             kwargs_extra = {
                 "inventory": self.options["extra_inventory_manager"],
                 "variable_manager": self.options["extra_variable_manager"],
                 "loader": self.options["extra_loader"],
-                "stdout_callback": cb_extra,
+                "stdout_callback": callback_extra,
                 "passwords": {"conn_pass": None, "become_pass": None},
             }
 
         # create a pseudo-play to execute the specified module via a single task
         play_ds = {
             "name": "pytest-ansible",
             "hosts": self.options["host_pattern"],
@@ -184,15 +183,15 @@
             "gather_facts": "no",
             "tasks": [
                 {
                     "action": {
                         "module": self.options["module_name"],
                         "args": complex_args,
                     },
-                }
+                },
             ],
         }
 
         play = Play().load(
             play_ds,
             variable_manager=self.options["variable_manager"],
             loader=self.options["loader"],
@@ -203,15 +202,15 @@
                 play_ds,
                 variable_manager=self.options["extra_variable_manager"],
                 loader=self.options["extra_loader"],
             )
 
         if HAS_CUSTOM_LOADER_SUPPORT:
             # Load the collection finder, unsupported, may change in future
-            init_plugin_loader(ansible.constants.COLLECTIONS_PATHS)
+            init_plugin_loader(COLLECTIONS_PATHS)
 
         # now create a task queue manager to execute the play
         tqm = None
         try:
             tqm = TaskQueueManager(**kwargs)
             tqm.run(play)
         finally:
@@ -225,29 +224,28 @@
                 tqm_extra.run(play_extra)
             finally:
                 if tqm_extra:
                     tqm_extra.cleanup()
 
         # Raise exception if host(s) unreachable
         # FIXME - if multiple hosts were involved, should an exception be raised?
-        if cb.unreachable:
+        if callback.unreachable:
             raise AnsibleConnectionFailure(
                 "Host unreachable in the inventory",
-                dark=cb.unreachable,
-                contacted=cb.contacted,
+                dark=callback.unreachable,
+                contacted=callback.contacted,
+            )
+        if "extra_inventory_manager" in self.options and callback_extra.unreachable:
+            raise AnsibleConnectionFailure(
+                "Host unreachable in the extra inventory",
+                dark=callback_extra.unreachable,
+                contacted=callback_extra.contacted,
             )
-        if "extra_inventory_manager" in self.options:
-            if cb_extra.unreachable:
-                raise AnsibleConnectionFailure(
-                    "Host unreachable in the extra inventory",
-                    dark=cb_extra.unreachable,
-                    contacted=cb_extra.contacted,
-                )
 
         # Success!
         return AdHocResult(
             contacted=(
-                {**cb.contacted, **cb_extra.contacted}
+                {**callback.contacted, **callback_extra.contacted}
                 if "extra_inventory_manager" in self.options
-                else cb.contacted
-            )
+                else callback.contacted
+            ),
         )
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v24.py` & `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,34 @@
+from __future__ import annotations
+
 import warnings
+from typing import TYPE_CHECKING
 
 import ansible.constants
 import ansible.errors
 import ansible.utils
-
 from ansible.cli import CLI
 from ansible.executor.task_queue_manager import TaskQueueManager
 from ansible.playbook.play import Play
 from ansible.plugins.callback import CallbackBase
 from ansible.plugins.loader import module_loader
 
 from pytest_ansible.errors import AnsibleConnectionFailure
-from pytest_ansible.has_version import has_ansible_v24
-from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
+from pytest_ansible.has_version import has_ansible_v2
+from pytest_ansible.module_dispatcher import BaseModuleDispatcher
 from pytest_ansible.results import AdHocResult
 
-
-# pylint: disable=ungrouped-imports, wrong-import-position
-
-if not has_ansible_v24:
-    raise ImportError("Only supported with ansible-2.4 and newer")
-
-
-# pylint: enable=ungrouped-imports
+if not has_ansible_v2:
+    raise ImportError("Only supported with ansible-2.* and newer")
 
 
 class ResultAccumulator(CallbackBase):
-
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Initialize object."""
         super().__init__(*args, **kwargs)
         self.contacted = {}
         self.unreachable = {}
 
     def v2_runner_on_failed(self, result, *args, **kwargs):
         self.contacted[result._host.get_name()] = result._result
@@ -44,19 +39,21 @@
         self.unreachable[result._host.get_name()] = result._result
 
     @property
     def results(self):
         return {"contacted": self.contacted, "unreachable": self.unreachable}
 
 
-class ModuleDispatcherV24(ModuleDispatcherV2):
-
+class ModuleDispatcherV2(BaseModuleDispatcher):
     """Pass."""
 
-    required_kwargs = (
+    if TYPE_CHECKING:
+        from collections.abc import Sequence
+
+    required_kwargs: Sequence[str] = (
         "inventory",
         "inventory_manager",
         "variable_manager",
         "host_pattern",
         "loader",
     )
 
@@ -84,21 +81,22 @@
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
         self.options["inventory_manager"].subset(self.options.get("subset"))
         hosts = self.options["inventory_manager"].list_hosts(
-            self.options["host_pattern"]
+            self.options["host_pattern"],
         )
         if len(hosts) == 0 and not no_hosts:
             raise ansible.errors.AnsibleError(
-                "Specified hosts and/or --limit does not match any hosts"
+                "Specified hosts and/or --limit does not match any hosts",
             )
 
+        # pylint: disable=no-member
         parser = CLI.base_parser(
             runas_opts=True,
             inventory_opts=True,
             async_opts=True,
             output_opts=True,
             connect_opts=True,
             check_opts=True,
@@ -115,22 +113,22 @@
         options.remote_user = self.options.get("user")
         options.become = self.options.get("become")
         options.become_method = self.options.get("become_method")
         options.become_user = self.options.get("become_user")
         options.module_path = self.options.get("module_path")
 
         # Initialize callback to capture module JSON responses
-        cb = ResultAccumulator()
+        callback = ResultAccumulator()
 
         kwargs = {
             "inventory": self.options["inventory_manager"],
             "variable_manager": self.options["variable_manager"],
             "loader": self.options["loader"],
             "options": options,
-            "stdout_callback": cb,
+            "stdout_callback": callback,
             "passwords": {"conn_pass": None, "become_pass": None},
         }
 
         # create a pseudo-play to execute the specified module via a single task
         play_ds = {
             "name": "pytest-ansible",
             "hosts": self.options["host_pattern"],
@@ -158,14 +156,16 @@
             tqm.run(play)
         finally:
             if tqm:
                 tqm.cleanup()
 
         # Raise exception if host(s) unreachable
         # FIXME - if multiple hosts were involved, should an exception be raised?
-        if cb.unreachable:
+        if callback.unreachable:
             raise AnsibleConnectionFailure(
-                "Host unreachable", dark=cb.unreachable, contacted=cb.contacted
+                "Host unreachable",
+                dark=callback.unreachable,
+                contacted=callback.contacted,
             )
 
         # Success!
-        return AdHocResult(contacted=cb.contacted)
+        return AdHocResult(contacted=callback.contacted)
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v28.py` & `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v28.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 import sys
 import warnings
 
 import ansible.constants
 import ansible.errors
 import ansible.utils
-
 from ansible.cli.adhoc import AdHocCLI
 from ansible.executor.task_queue_manager import TaskQueueManager
 from ansible.playbook.play import Play
 from ansible.plugins.callback import CallbackBase
 from ansible.plugins.loader import module_loader
 
 from pytest_ansible.errors import AnsibleConnectionFailure
 from pytest_ansible.has_version import has_ansible_v28
 from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
 from pytest_ansible.results import AdHocResult
 
-
 # pylint: disable=ungrouped-imports, wrong-import-position
 if not has_ansible_v28:
     raise ImportError("Only supported with ansible-2.8 and newer")
 
 
 # pylint: enable=ungrouped-imports
 
 
 class ResultAccumulator(CallbackBase):
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Initialize object."""
         super().__init__(*args, **kwargs)
         self.contacted = {}
         self.unreachable = {}
 
     def v2_runner_on_failed(self, result, *args, **kwargs):
         result2 = {"failed": True}
@@ -85,19 +83,19 @@
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
         self.options["inventory_manager"].subset(self.options.get("subset"))
         hosts = self.options["inventory_manager"].list_hosts(
-            self.options["host_pattern"]
+            self.options["host_pattern"],
         )
         if len(hosts) == 0 and not no_hosts:
             raise ansible.errors.AnsibleError(
-                "Specified hosts and/or --limit does not match any hosts"
+                "Specified hosts and/or --limit does not match any hosts",
             )
 
         # Pass along cli options
         args = ["pytest-ansible"]
         verbosity = None
         for verbosity_syntax in ("-v", "-vv", "-vvv", "-vvvv", "-vvvvv"):
             if verbosity_syntax in sys.argv:
@@ -130,21 +128,21 @@
         adhoc = AdHocCLI(args)
         adhoc.parse()
 
         # And now we'll never speak of this again
         del adhoc
 
         # Initialize callback to capture module JSON responses
-        cb = ResultAccumulator()
+        callback = ResultAccumulator()
 
         kwargs = {
             "inventory": self.options["inventory_manager"],
             "variable_manager": self.options["variable_manager"],
             "loader": self.options["loader"],
-            "stdout_callback": cb,
+            "stdout_callback": callback,
             "passwords": {"conn_pass": None, "become_pass": None},
         }
 
         # create a pseudo-play to execute the specified module via a single task
         play_ds = {
             "name": "pytest-ansible",
             "hosts": self.options["host_pattern"],
@@ -174,14 +172,16 @@
             tqm.run(play)
         finally:
             if tqm:
                 tqm.cleanup()
 
         # Raise exception if host(s) unreachable
         # FIXME - if multiple hosts were involved, should an exception be raised?
-        if cb.unreachable:
+        if callback.unreachable:
             raise AnsibleConnectionFailure(
-                "Host unreachable", dark=cb.unreachable, contacted=cb.contacted
+                "Host unreachable",
+                dark=callback.unreachable,
+                contacted=callback.contacted,
             )
 
         # Success!
-        return AdHocResult(contacted=cb.contacted)
+        return AdHocResult(contacted=callback.contacted)
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/module_dispatcher/v29.py` & `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v212.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
+from __future__ import annotations
+
 import sys
 import warnings
+from typing import TYPE_CHECKING
 
 import ansible.constants
 import ansible.errors
 import ansible.utils
-
 from ansible.cli.adhoc import AdHocCLI
 from ansible.executor.task_queue_manager import TaskQueueManager
 from ansible.playbook.play import Play
 from ansible.plugins.callback import CallbackBase
 from ansible.plugins.loader import module_loader
 
 from pytest_ansible.errors import AnsibleConnectionFailure
-from pytest_ansible.has_version import has_ansible_v29
+from pytest_ansible.has_version import has_ansible_v212
 from pytest_ansible.module_dispatcher.v2 import ModuleDispatcherV2
 from pytest_ansible.results import AdHocResult
 
-
 # pylint: disable=ungrouped-imports, wrong-import-position
-
-if not has_ansible_v29:
-    raise ImportError("Only supported with ansible-2.9 and newer")
+if not has_ansible_v212:
+    raise ImportError("Only supported with ansible-2.12 and newer")
 
 
 # pylint: enable=ungrouped-imports
 
 
 class ResultAccumulator(CallbackBase):
     """Fixme."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Initialize object."""
         super().__init__(*args, **kwargs)
         self.contacted = {}
         self.unreachable = {}
 
     def v2_runner_on_failed(self, result, *args, **kwargs):
         result2 = {"failed": True}
@@ -47,18 +47,21 @@
         self.unreachable[result._host.get_name()] = result._result
 
     @property
     def results(self):
         return {"contacted": self.contacted, "unreachable": self.unreachable}
 
 
-class ModuleDispatcherV29(ModuleDispatcherV2):
+class ModuleDispatcherV212(ModuleDispatcherV2):
     """Pass."""
 
-    required_kwargs = (
+    if TYPE_CHECKING:
+        from collections.abc import Sequence
+
+    required_kwargs: Sequence[str] = (
         "inventory",
         "inventory_manager",
         "variable_manager",
         "host_pattern",
         "loader",
     )
 
@@ -86,19 +89,19 @@
         no_hosts = False
         if len(hosts) == 0:
             no_hosts = True
             warnings.warn("provided hosts list is empty, only localhost is available")
 
         self.options["inventory_manager"].subset(self.options.get("subset"))
         hosts = self.options["inventory_manager"].list_hosts(
-            self.options["host_pattern"]
+            self.options["host_pattern"],
         )
         if len(hosts) == 0 and not no_hosts:
             raise ansible.errors.AnsibleError(
-                "Specified hosts and/or --limit does not match any hosts"
+                "Specified hosts and/or --limit does not match any hosts",
             )
 
         # Pass along cli options
         args = ["pytest-ansible"]
         verbosity = None
         for verbosity_syntax in ("-v", "-vv", "-vvv", "-vvvv", "-vvvvv"):
             if verbosity_syntax in sys.argv:
@@ -131,34 +134,34 @@
         adhoc = AdHocCLI(args)
         adhoc.parse()
 
         # And now we'll never speak of this again
         del adhoc
 
         # Initialize callbacks to capture module JSON responses
-        cb = ResultAccumulator()
+        callback = ResultAccumulator()
 
         kwargs = {
             "inventory": self.options["inventory_manager"],
             "variable_manager": self.options["variable_manager"],
             "loader": self.options["loader"],
-            "stdout_callback": cb,
+            "stdout_callback": callback,
             "passwords": {"conn_pass": None, "become_pass": None},
         }
 
         kwargs_extra = {}
         # If we have an extra inventory, do the same that we did for the inventory
         if "extra_inventory_manager" in self.options:
-            cb_extra = ResultAccumulator()
+            callback_extra = ResultAccumulator()
 
             kwargs_extra = {
                 "inventory": self.options["extra_inventory_manager"],
                 "variable_manager": self.options["extra_variable_manager"],
                 "loader": self.options["extra_loader"],
-                "stdout_callback": cb_extra,
+                "stdout_callback": callback_extra,
                 "passwords": {"conn_pass": None, "become_pass": None},
             }
 
         # create a pseudo-play to execute the specified module via a single task
         play_ds = {
             "name": "pytest-ansible",
             "hosts": self.options["host_pattern"],
@@ -176,14 +179,15 @@
         }
 
         play = Play().load(
             play_ds,
             variable_manager=self.options["variable_manager"],
             loader=self.options["loader"],
         )
+
         play_extra = None
         if "extra_inventory_manager" in self.options:
             play_extra = Play().load(
                 play_ds,
                 variable_manager=self.options["extra_variable_manager"],
                 loader=self.options["extra_loader"],
             )
@@ -204,29 +208,28 @@
                 tqm_extra.run(play_extra)
             finally:
                 if tqm_extra:
                     tqm_extra.cleanup()
 
         # Raise exception if host(s) unreachable
         # FIXME - if multiple hosts were involved, should an exception be raised?
-        if cb.unreachable:
+        if callback.unreachable:
             raise AnsibleConnectionFailure(
                 "Host unreachable in the inventory",
-                dark=cb.unreachable,
-                contacted=cb.contacted,
+                dark=callback.unreachable,
+                contacted=callback.contacted,
+            )
+        if "extra_inventory_manager" in self.options and callback_extra.unreachable:
+            raise AnsibleConnectionFailure(
+                "Host unreachable in the extra inventory",
+                dark=callback_extra.unreachable,
+                contacted=callback_extra.contacted,
             )
-        if "extra_inventory_manager" in self.options:
-            if cb_extra.unreachable:
-                raise AnsibleConnectionFailure(
-                    "Host unreachable in the extra inventory",
-                    dark=cb_extra.unreachable,
-                    contacted=cb_extra.contacted,
-                )
 
         # Success!
         return AdHocResult(
             contacted=(
-                {**cb.contacted, **cb_extra.contacted}
+                {**callback.contacted, **callback_extra.contacted}
                 if "extra_inventory_manager" in self.options
-                else cb.contacted
-            )
+                else callback.contacted
+            ),
         )
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/plugin.py` & `pytest-ansible-3.1.0/src/pytest_ansible/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 """PyTest Ansible Plugin."""
 
+import logging
+
 import ansible
 import ansible.constants
 import ansible.errors
 import ansible.utils
+import ansible.utils.display
 import pytest
 
-from ansible.plugins.loader import become_loader
-
-from pytest_ansible.fixtures import ansible_adhoc
-from pytest_ansible.fixtures import ansible_facts
-from pytest_ansible.fixtures import ansible_module
-from pytest_ansible.fixtures import localhost
+from pytest_ansible.fixtures import (
+    ansible_adhoc,
+    ansible_facts,
+    ansible_module,
+    localhost,
+)
 from pytest_ansible.host_manager import get_host_manager
 
+from .units import inject, inject_only
+
+logger = logging.getLogger(__name__)
 
 # Silence linters for imported fixtures
-# pylint: disable=pointless-statement
+# pylint: disable=pointless-statement, no-member
 (ansible_adhoc, ansible_module, ansible_facts, localhost)
 
-
-def become_methods():
-    """Return string list of become methods available to ansible."""
-    if become_loader:
-        return [method.name for method in become_loader.all()]
-    return ansible.constants.BECOME_METHODS
+log_map = {
+    0: logging.CRITICAL,
+    1: logging.ERROR,
+    2: logging.WARNING,
+    3: logging.INFO,
+    4: logging.DEBUG,
+}
 
 
 def pytest_addoption(parser):
     """Add options to control ansible."""
-
     group = parser.getgroup("pytest-ansible")
     group.addoption(
         "--inventory",
         "--ansible-inventory",
         action="store",
         dest="ansible_inventory",
         default=ansible.constants.DEFAULT_HOST_LIST,
@@ -111,15 +117,15 @@
     )
     group.addoption(
         "--become-method",
         "--ansible-become-method",
         action="store",
         dest="ansible_become_method",
         default=ansible.constants.DEFAULT_BECOME_METHOD,
-        help=f"privilege escalation method to use (default: %(default)s), valid choices: [ {' | '.join(become_methods())} ]",
+        help="privilege escalation method to use (default: %(default)s)",
     )
 
     group.addoption(
         "--become-user",
         "--ansible-become-user",
         action="store",
         dest="ansible_become_user",
@@ -130,102 +136,108 @@
         "--ask-become-pass",
         "--ansible-ask-become-pass",
         action="store",
         dest="ansible_ask_become_pass",
         default=ansible.constants.DEFAULT_BECOME_ASK_PASS,
         help="ask for privilege escalation password (default: %(default)s)",
     )
-
+    group.addoption(
+        "--ansible-unit-inject-only",
+        action="store_true",
+        default=False,
+        help="Enable support for ansible collection unit tests by only injecting exisiting ANSIBLE_COLLECTIONS_PATHS.",
+    )
     # Add github marker to --help
     parser.addini("ansible", "Ansible integration", "args")
 
 
 def pytest_configure(config):
     """Validate --ansible-* parameters."""
-
     config.addinivalue_line("markers", "ansible(**kwargs): Ansible integration")
 
     # Enable connection debugging
     if config.option.verbose > 0:
         if hasattr(ansible.utils, "VERBOSITY"):
             ansible.utils.VERBOSITY = int(config.option.verbose)
         else:
-            from ansible.utils.display import Display
+            ansible.utils.display.verbosity = int(config.option.verbose)
 
-            display = Display()
-            display.verbosity = int(config.option.verbose)
+    # Configure the logger.
+    level = log_map.get(config.option.verbose)
+    logging.basicConfig(level=level)
+    logging.debug("Logging initialized")
 
     assert config.pluginmanager.register(PyTestAnsiblePlugin(config), "ansible")
 
+    if config.option.ansible_unit_inject_only:
+        inject_only()
+    else:
+        start_path = config.invocation_params.dir
+        inject(start_path)
+
 
 def pytest_generate_tests(metafunc):
     """Generate tests when specific `ansible_*` fixtures are used by tests."""
-
     if "ansible_host" in metafunc.fixturenames:
         # assert required --ansible-* parameters were used
         PyTestAnsiblePlugin.assert_required_ansible_parameters(metafunc.config)
         try:
             plugin = metafunc.config.pluginmanager.getplugin("ansible")
             hosts = plugin.initialize(
                 config=plugin.config,
                 pattern=metafunc.config.getoption("ansible_host_pattern"),
             )
-        except ansible.errors.AnsibleError as e:
-            raise pytest.UsageError(e)
+        except ansible.errors.AnsibleError as exception:
+            raise pytest.UsageError(exception)
         # Return the host name as a string
-        # metafunc.parametrize("ansible_host", hosts.keys())
         # Return a HostManager instance where pattern=host (e.g. ansible_host.all.shell('date'))
         # metafunc.parametrize("ansible_host", iter(plugin.initialize(config=plugin.config, pattern=h) for h in
         #                                           hosts.keys()))
         # Return a ModuleDispatcher instance representing `host` (e.g. ansible_host.shell('date'))
-        metafunc.parametrize("ansible_host", iter(hosts[h] for h in hosts.keys()))
+        metafunc.parametrize("ansible_host", iter(hosts[h] for h in hosts))
 
     if "ansible_group" in metafunc.fixturenames:
         # assert required --ansible-* parameters were used
         PyTestAnsiblePlugin.assert_required_ansible_parameters(metafunc.config)
         try:
             plugin = metafunc.config.pluginmanager.getplugin("ansible")
             hosts = plugin.initialize(
                 config=plugin.config,
                 pattern=metafunc.config.getoption("ansible_host_pattern"),
             )
-        except ansible.errors.AnsibleError as e:
-            raise pytest.UsageError(e)
+        except ansible.errors.AnsibleError as exception:
+            raise pytest.UsageError(exception)
         # FIXME: Eeew, this shouldn't be interfacing with `hosts.options`
         groups = hosts.options["inventory_manager"].list_groups()
         extra_groups = hosts.get_extra_inventory_groups()
         # Return the group name as a string
-        # metafunc.parametrize("ansible_group", groups)
         # Return a ModuleDispatcher instance representing the group (e.g. ansible_group.shell('date'))
         metafunc.parametrize("ansible_group", iter(hosts[g] for g in groups))
         metafunc.parametrize("ansible_group", iter(hosts[g] for g in extra_groups))
 
 
 class PyTestAnsiblePlugin:
-
     """Ansible PyTest Plugin Class."""
 
-    def __init__(self, config):
+    def __init__(self, config) -> None:
         """Initialize plugin."""
         self.config = config
 
     def pytest_report_header(self, config, startdir):
         """Return the version of ansible."""
         return f"ansible: {ansible.__version__}"
 
     def pytest_collection_modifyitems(self, session, config, items):
         """Validate --ansible-* parameters."""
-
         uses_ansible_fixtures = False
         for item in items:
             if not hasattr(item, "fixturenames"):
                 continue
             if any(fixture.startswith("ansible_") for fixture in item.fixturenames):
                 # TODO - ignore if they are using a marker
-                # marker = item.get_marker('ansible')
                 # if marker and 'inventory' in marker.kwargs:
                 uses_ansible_fixtures = True
                 break
 
         if uses_ansible_fixtures:
             # assert required --ansible-* parameters were used
             self.assert_required_ansible_parameters(config)
@@ -293,22 +305,22 @@
         """Assert whether the required --ansible-* parameters were provided."""
         errors = []
 
         # Verify --ansible-host-pattern was provided
         ansible_hostname = config.getoption("ansible_host_pattern")
         if ansible_hostname is None or ansible_hostname == "":
             errors.append(
-                "Missing required parameter --ansible-host-pattern/--host-pattern"
+                "Missing required parameter --ansible-host-pattern/--host-pattern",
             )
 
         # NOTE: I don't think this will ever catch issues since ansible_inventory
         # defaults to '/etc/ansible/hosts'
         # Verify --ansible-inventory was provided
         ansible_inventory = config.getoption("ansible_inventory")
         if ansible_inventory is None or ansible_inventory == "":
             errors.append(
                 "Unable to find an inventory file, specify one with the --ansible-inventory/--inventory "
-                "parameter."
+                "parameter.",
             )
 
         if errors:
             raise pytest.UsageError(*errors)
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible/results.py` & `pytest-ansible-3.1.0/src/pytest_ansible/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 """Fixme."""
 
 
 class ModuleResult(dict):
-
     """Fixme."""
 
     def _check_key(self, key):
         # if 'results' in self:
-        #     flag = False
         #     for res in self.get('results', []):
         #         if isinstance(res, dict):
-        #             flag |= res.get(key, False)
-        #     return flag
-        # else:
         return self.get(key, False)
 
     @property
     def is_ok(self):
         return not (
             self.is_changed or self.is_unreachable or self.is_skipped or self.is_failed
         )
@@ -39,18 +34,17 @@
 
     @property
     def is_successful(self):
         return not (self.is_failed or self.is_unreachable)
 
 
 class AdHocResult:
-
     """Fixme."""
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         """Fixme."""
         required_kwargs = ("contacted",)
         for kwarg in required_kwargs:
             assert kwarg in kwargs, f"Missing required keyword argument '{kwarg}'"
             setattr(self, kwarg, kwargs.get(kwarg))
 
     def __getitem__(self, item):
@@ -61,31 +55,31 @@
 
     def __getattr__(self, attr):
         """Return a ModuleResult instance matching the provided `attr`."""
         if attr in self.contacted:
             return ModuleResult(**self.contacted[attr])
         raise AttributeError(f"type AdHocResult has no attribute '{attr}'")
 
-    def __len__(self):
+    def __len__(self) -> int:
         """Return the number of contacted hosts."""
         return len(self.contacted)
 
-    def __contains__(self, item):
+    def __contains__(self, item) -> bool:
         """Return whether the provided `item` was contacted."""
         return item in self.contacted
 
     def __iter__(self):
         """Return an iterator of the contacted inventory hosts."""
         return iter(self.contacted)
 
     def keys(self):
         """Return a list of contacted inventory hosts."""
         return self.contacted.keys()
 
     def items(self):
         """Return a list of tuples containing the inventory host key, and the ModuleResult instance."""
-        for k in self.contacted.keys():
+        for k in self.contacted:
             yield (k, getattr(self, k))
 
     def values(self):
         """Return a list of ModuleResult instances for each contacted inventory host."""
-        return [getattr(self, k) for k in self.contacted.keys()]
+        return [getattr(self, k) for k in self.contacted]
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible.egg-info/PKG-INFO` & `pytest-ansible-3.1.0/src/pytest_ansible.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.0.0
-Summary: Plugin for py.test to simplify calling ansible modules from tests or fixtures
+Version: 3.1.0
+Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
 Project-URL: changelog, https://github.com/ansible-community/pytest-ansible/releases
@@ -31,15 +31,15 @@
 # pytest-ansible
 
 [![Build Status](https://github.com/ansible-community/pytest-ansible/actions/workflows/tox.yml/badge.svg)](https://github.com/ansible-community/pytest-ansible/actions/workflows/tox.yml)
 [![Version](https://img.shields.io/pypi/v/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 [![License](https://img.shields.io/pypi/l/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pytest-ansible.svg)](https://pypi.python.org/pypi/pytest-ansible/)
 
-This repository contains a plugin for `py.test` which adds several fixtures
+This repository contains a plugin for `pytest` which adds several fixtures
 for running `ansible` modules, or inspecting `ansible_facts`. While one
 can simply call out to `ansible` using the `subprocess` module, having to
 parse stdout to determine the outcome of the operation is unpleasant and prone
 to error. With `pytest-ansible`, modules return JSON data which you can
 inspect and act on, much like with an ansible
 [playbook](http://docs.ansible.com/playbooks.html).
 
@@ -49,18 +49,18 @@
 
 ```bash
 pip install pytest-ansible
 ```
 
 ## Usage
 
-Once installed, the following `py.test` command-line parameters are available:
+Once installed, the following `pytest` command-line parameters are available:
 
 ```bash
-py.test \
+pytest \
     [--inventory <path_to_inventory>] \
     [--extra-inventory <path_to_extra_inventory>] \
     [--host-pattern <host-pattern>] \
     [--connection <plugin>] \
     [--module-path <path_to_modules] \
     [--user <username>] \
     [--become] \
@@ -86,27 +86,27 @@
 supported by ansible, which includes an [INI
 file](http://docs.ansible.com/ansible/latest/intro_inventory.html) or an
 executable script that returns [properly formatted
 JSON](http://docs.ansible.com/ansible/latest/intro_dynamic_inventory.html).
 For example,
 
 ```bash
-py.test --inventory my_inventory.ini --host-pattern all
+pytest --inventory my_inventory.ini --host-pattern all
 ```
 
 or
 
 ```bash
-py.test --inventory path/to/my/script.py --host-pattern webservers
+pytest --inventory path/to/my/script.py --host-pattern webservers
 ```
 
 or
 
 ```bash
-py.test --inventory one.example.com,two.example.com --host-pattern all
+pytest --inventory one.example.com,two.example.com --host-pattern all
 ```
 
 In the above examples, the inventory provided at runtime will be used in all
 tests that use the `ansible_adhoc` fixture. A more realistic scenario may
 involve using different inventory files (or host patterns) with different
 tests. To accomplish this, the fixture `ansible_adhoc` allows you to customize
 the inventory parameters. Read on for more detail on using the `ansible_adhoc`
@@ -117,26 +117,26 @@
 Using ansible first starts with defining your extra inventory. This feature was added in version 2.3.0, and is intended
 to allow the user to work with two different inventories. This can be done in several ways, but to start,
 we'll use the `ansible_adhoc` fixture.
 
 For example,
 
 ```bash
-py.test --inventory my_inventory.ini --extra-inventory my_second_inventory.ini --host-pattern host_in_second_inventory
+pytest --inventory my_inventory.ini --extra-inventory my_second_inventory.ini --host-pattern host_in_second_inventory
 ```
 
 ### Fixture `ansible_adhoc`
 
 The `ansible_adhoc` fixture returns a function used to initialize
 a `HostManager` object. The `ansible_adhoc` fixture will default to parameters
-supplied to the `py.test` command-line, but also allows one to provide keyword
+supplied to the `pytest` command-line, but also allows one to provide keyword
 arguments used to initialize the inventory.
 
 The example below demonstrates basic usage with options supplied at run-time to
-`py.test`.
+`pytest`.
 
 ```python
 def test_all_the_pings(ansible_adhoc):
     ansible_adhoc().all.ping()
 ```
 
 The following example demonstrates available keyword arguments when creating
@@ -206,15 +206,15 @@
     localhost.ec2(**params)
 ```
 
 ### Fixture `ansible_module`
 
 The `ansible_module` fixture allows tests and fixtures to call [ansible
 modules](http://docs.ansible.com/modules.html). Unlike the `ansible_adhoc`
-fixture, this fixture only uses the options supplied to `py.test` at run time.
+fixture, this fixture only uses the options supplied to `pytest` at run time.
 
 A very basic example demonstrating the ansible [`ping` module](http://docs.ansible.com/ping_module.html):
 
 ```python
 def test_ping(ansible_module):
     ansible_module.ping()
 ```
```

### Comparing `pytest-ansible-3.0.0/src/pytest_ansible.egg-info/SOURCES.txt` & `pytest-ansible-3.1.0/src/pytest_ansible.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,33 +3,36 @@
 .pre-commit-config.yaml
 HISTORY.md
 LICENSE
 README.md
 inventory
 pyproject.toml
 tox.ini
+.config/dictionary.txt
 .config/requirements-lock.txt
 .config/requirements.in
 .config/requirements.txt
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/dependabot.yml
 .github/release-drafter.yml
 .github/workflows/ack.yml
 .github/workflows/push.yml
 .github/workflows/release.yml
 .github/workflows/tox.yml
+.vscode/launch.json
 .vscode/settings.json
 src/pytest_ansible/__init__.py
 src/pytest_ansible/_version.py
 src/pytest_ansible/errors.py
 src/pytest_ansible/fixtures.py
 src/pytest_ansible/has_version.py
 src/pytest_ansible/plugin.py
 src/pytest_ansible/results.py
+src/pytest_ansible/units.py
 src/pytest_ansible.egg-info/PKG-INFO
 src/pytest_ansible.egg-info/SOURCES.txt
 src/pytest_ansible.egg-info/dependency_links.txt
 src/pytest_ansible.egg-info/entry_points.txt
 src/pytest_ansible.egg-info/requires.txt
 src/pytest_ansible.egg-info/top_level.txt
 src/pytest_ansible/host_manager/__init__.py
@@ -51,8 +54,10 @@
 tests/conftest.py
 tests/test_adhoc.py
 tests/test_adhoc_result.py
 tests/test_fixtures.py
 tests/test_host_manager.py
 tests/test_module_dispatcher.py
 tests/test_module_result.py
-tests/test_params.py
+tests/test_params.py
+tests/unit/__init__.py
+tests/unit/test_unit.py
```

### Comparing `pytest-ansible-3.0.0/tests/conftest.py` & `pytest-ansible-3.1.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import pytest
-
-from pytest_ansible.has_version import has_ansible_v1
-from pytest_ansible.has_version import has_ansible_v24
-
+from pytest_ansible.has_version import has_ansible_v1, has_ansible_v24
 
 try:
     from ansible.utils import context_objects as co
 except ImportError:
     # if it does not exist because of old version of ansible, we don't need it
     co = None
 
 
-pytest_plugins = ("pytester",)
+pytest_plugins = ["pytester"]
 
 
 ALL_HOSTS = ["another_host", "localhost", "yet_another_host"]
 
 POSITIVE_HOST_PATTERNS = [
     ("all", 3),
     ("*", 3),
@@ -24,15 +21,17 @@
     ("local*,&*host", 1),
     ("!localhost", 2),
     ("all[0]", 1),
     ("all[-1]", 1),
     pytest.param("*[0-1]", 1, marks=pytest.mark.requires_ansible_v1()),
     pytest.param("*[0-1]", 2, marks=pytest.mark.requires_ansible_v2()),
     pytest.param(
-        "*[0:1]", 2, marks=pytest.mark.requires_ansible_v2()
+        "*[0:1]",
+        2,
+        marks=pytest.mark.requires_ansible_v2(),
     ),  # this is confusing, but how host slicing works on v2
     pytest.param("*[0:]", 3, marks=pytest.mark.requires_ansible_v2()),
 ]
 
 NEGATIVE_HOST_PATTERNS = [
     ("none", 0),
     ("all[8:]", 0),
@@ -72,32 +71,32 @@
         # conditionally xfail
         mark = item.get_closest_marker("ansible_v1_xfail")
         if mark and has_ansible_v1:
             item.add_marker(
                 pytest.mark.xfail(
                     reason="expected failure on < ansible-2.*",
                     raises=mark.kwargs.get("raises"),
-                )
+                ),
             )
 
         mark = item.get_closest_marker("ansible_v2_xfail")
         if mark and not has_ansible_v1:
             item.add_marker(
                 pytest.xfail(
                     reason="expected failure on >= ansible-2.*",
                     raises=mark.kwargs.get("raises"),
-                )
+                ),
             )
 
 
 # pylint: disable=too-few-public-methods
 class PyTestOption:
     """Helper class that provides methods for creating and managing an inventory file."""
 
-    def __init__(self, config, testdir):
+    def __init__(self, config, testdir) -> None:
         self.config = config
 
         # Create inventory file
         self.inventory = testdir.makefile(
             ".ini",
             inventory="""
             [local]
@@ -116,15 +115,14 @@
             unreachable-host-1.example.com
             unreachable-host-2.example.com
             unreachable-host-3.example.com
         """,
         )
 
         # Create ansible.cfg file
-        # self.ansible_cfg = testdir.makefile('.cfg', ansible='''[ssh_connection]\ncontrol_path = %(directory)s/%%h-%%r''')
 
     @property
     def args(self):
         args = []
         args.append("--tb")
         args.append("native")
         return args
```

### Comparing `pytest-ansible-3.0.0/tests/test_adhoc.py` & `pytest-ansible-3.1.0/tests/test_adhoc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import pytest
 
-
 # pylint: disable=unused-import
 try:
-    from _pytest.main import EXIT_INTERRUPTED  # type: ignore[attr-defined]
-    from _pytest.main import EXIT_NOTESTSCOLLECTED  # type: ignore[attr-defined]
-    from _pytest.main import EXIT_OK  # type: ignore[attr-defined]
-    from _pytest.main import EXIT_TESTSFAILED  # type: ignore[attr-defined]
-    from _pytest.main import EXIT_USAGEERROR  # type: ignore[attr-defined]
+    from _pytest.main import (
+        EXIT_INTERRUPTED,  # type: ignore[attr-defined]
+        EXIT_NOTESTSCOLLECTED,  # type: ignore[attr-defined]
+        EXIT_OK,  # type: ignore[attr-defined]
+        EXIT_TESTSFAILED,  # type: ignore[attr-defined]
+        EXIT_USAGEERROR,  # type: ignore[attr-defined]
+    )
 except ImportError:
     from _pytest.main import ExitCode
 
     EXIT_OK = ExitCode.OK
     EXIT_TESTSFAILED = ExitCode.TESTS_FAILED
     EXIT_USAGEERROR = ExitCode.USAGE_ERROR
     EXIT_INTERRUPTED = ExitCode.INTERRUPTED
     EXIT_NOTESTSCOLLECTED = ExitCode.NO_TESTS_COLLECTED
 
 
 @pytest.mark.old()
 def test_contacted_with_params(testdir, option):
-    """FIXME"""
-
+    """FIXME."""
     src = """
         import pytest
         def test_func(ansible_module):
             contacted = ansible_module.ping()
 
             # assert contacted hosts ...
             assert contacted
@@ -33,29 +33,29 @@
             for result in contacted.values():
                 assert result.is_successful
                 assert result['ping'] == 'pong'
 
     """
     testdir.makepyfile(src)
     result = testdir.runpytest_subprocess(
-        *option.args
-        + [
+        *[
+            *option.args,
             "--ansible-inventory",
             str(option.inventory),
             "--ansible-host-pattern",
             "local",
-        ]
+        ],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 @pytest.mark.old()
 def test_contacted_with_params_and_inventory_marker(testdir, option):
-    """FIXME"""
+    """FIXME."""
     src = f"""
         import pytest
         @pytest.mark.ansible(inventory='{option.inventory}')
         def test_func(ansible_module):
             contacted = ansible_module.ping()
 
             # assert contacted hosts ...
@@ -65,23 +65,23 @@
                 assert result.is_successful
                 assert result['ping'] == 'pong'
 
         """
 
     testdir.makepyfile(src)
     result = testdir.runpytest_subprocess(
-        *option.args + ["--ansible-host-pattern", "local"]
+        *[*option.args, "--ansible-host-pattern", "local"],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 @pytest.mark.old()
 def test_contacted_with_params_and_host_pattern_marker(testdir, option):
-    """FIXME"""
+    """FIXME."""
     src = """
         import pytest
         @pytest.mark.ansible(host_pattern='local')
         def test_func(ansible_module):
             contacted = ansible_module.ping()
 
             # assert contacted hosts ...
@@ -90,29 +90,29 @@
             for result in contacted.values():
                 assert result.is_successful
                 assert result['ping'] == 'pong'
 
     """
     testdir.makepyfile(src)
     result = testdir.runpytest_subprocess(
-        *option.args
-        + [
+        *[
+            *option.args,
             "--ansible-inventory",
             str(option.inventory),
             "--ansible-host-pattern",
             "unreachable",
-        ]
+        ],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 @pytest.mark.old()
 def test_contacted_with_params_and_inventory_host_pattern_marker(testdir, option):
-    """FIXME"""
+    """FIXME."""
     src = f"""
         import pytest
         @pytest.mark.ansible(inventory='{option.inventory}', host_pattern='local')
         def test_func(ansible_module):
             contacted = ansible_module.ping()
 
             # assert contacted hosts ...
@@ -121,16 +121,21 @@
             for result in contacted.values():
                 assert result.is_successful
                 assert result['ping'] == 'pong'
         """
 
     testdir.makepyfile(src)
     result = testdir.runpytest_subprocess(
-        *option.args
-        + ["--ansible-inventory", "/dev/null", "--ansible-host-pattern", "unreachable"]
+        *[
+            *option.args,
+            "--ansible-inventory",
+            "/dev/null",
+            "--ansible-host-pattern",
+            "unreachable",
+        ],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 @pytest.mark.old()
 def test_become(testdir, option):
@@ -174,23 +179,23 @@
             "--ansible-inventory",
             str(option.inventory),
             "--ansible-host-pattern",
             "localhost",  # run against a single host
             "--ansible-become",  # Enable become support
             "--ansible-become-user",
             "asdfasdf",  # Connect as asdfasdf
-        ]
+        ],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 @pytest.mark.old()
 def test_dark_with_params(testdir, option):
-    """FIXME"""
+    """FIXME."""
     src = """
         import pytest
         from pytest_ansible.errors import (AnsibleConnectionFailure, AnsibleNoHostsMatch)
         def test_func(ansible_module):
             exc_info = pytest.raises(AnsibleConnectionFailure, ansible_module.ping)
 
             # assert no contacted hosts ...
@@ -198,31 +203,31 @@
                 % (len(exc_info.value.contacted), 0)
 
             # assert dark hosts ...
             assert exc_info.value.dark
     """
     testdir.makepyfile(src)
     result = testdir.runpytest_subprocess(
-        *option.args
-        + [
+        *[
+            *option.args,
             "--ansible-inventory",
             str(option.inventory),
             "--ansible-host-pattern",
             "unreachable",
-        ]
+        ],
     )
     print("\n".join(result.stdout.lines))
     print("\n".join(result.stderr.lines))
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 @pytest.mark.old()
 def test_dark_with_params_and_inventory_marker(testdir, option):
-    """FIXME"""
+    """FIXME."""
     src = f"""
         import pytest
         from pytest_ansible.errors import (AnsibleConnectionFailure, AnsibleNoHostsMatch)
         @pytest.mark.ansible(inventory='{option.inventory}')
         def test_func(ansible_module):
             exc_info = pytest.raises(AnsibleConnectionFailure, ansible_module.ping)
 
@@ -232,23 +237,23 @@
 
             # assert dark hosts ...
             assert exc_info.value.dark
         """
 
     testdir.makepyfile(src)
     result = testdir.runpytest_subprocess(
-        *option.args + ["--ansible-host-pattern", "unreachable"]
+        *[*option.args, "--ansible-host-pattern", "unreachable"],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 @pytest.mark.old()
 def test_dark_with_params_and_host_pattern_marker(testdir, option):
-    """FIXME"""
+    """FIXME."""
     src = """
         import pytest
         import ansible
         from pytest_ansible.errors import (AnsibleConnectionFailure, AnsibleNoHostsMatch)
         @pytest.mark.ansible(host_pattern='unreachable')
         def test_func(ansible_module):
             exc_info = pytest.raises(AnsibleConnectionFailure, ansible_module.ping)
@@ -258,21 +263,21 @@
                 % (len(exc_info.value.contacted), 0)
 
             # assert dark hosts ...
             assert exc_info.value.dark
     """
     testdir.makepyfile(src)
     result = testdir.runpytest_subprocess(
-        *option.args
-        + [
+        *[
+            *option.args,
             "--ansible-inventory",
             str(option.inventory),
             "--ansible-host-pattern",
             "local",
-        ]
+        ],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 @pytest.mark.old()
 def test_dark_with_debug_enabled(testdir, option):
@@ -281,24 +286,22 @@
         import pytest
         from pytest_ansible.errors import AnsibleConnectionFailure
         def test_func(ansible_module):
             ansible_module.ping()
     """
     testdir.makepyfile(src)
     result = testdir.runpytest_subprocess(
-        *option.args
-        + [
+        *[
+            *option.args,
             "--ansible-inventory",
             str(option.inventory),
             "--ansible-host-pattern",
             "unreachable",
             "-v",
-        ]
+        ],
     )
     assert result.ret == EXIT_TESTSFAILED
     assert result.parseoutcomes()["failed"] == 1
     # FIXME - the following doesn't work on ansible-v2
     # result.stdout.fnmatch_lines([
-    #     '*ESTABLISH CONNECTION FOR USER: *',
     #     '*REMOTE_MODULE ping',
     #     '*EXEC ssh *',
-    # ])
```

### Comparing `pytest-ansible-3.0.0/tests/test_adhoc_result.py` & `pytest-ansible-3.1.0/tests/test_adhoc_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from types import GeneratorType
 
 import pytest
-
 from conftest import ALL_HOSTS
-
 from pytest_ansible.results import ModuleResult
 
-
 invalid_hosts = ["none", "all", "*", "local*"]
 
 
 @pytest.fixture()
 def adhoc_result(hosts):
     return hosts.all.ping()
 
@@ -96,15 +93,15 @@
     assert "unknown.example.com" in exc_info.value.dark
     # Assert unreachable
     assert "failed" in exc_info.value.dark["unknown.example.com"]
     assert exc_info.value.dark["unknown.example.com"]["failed"]
     # Assert msg
     assert "msg" in exc_info.value.dark["unknown.example.com"]
     assert exc_info.value.dark["unknown.example.com"]["msg"].startswith(
-        "SSH Error: ssh: Could not resolve hostname" + " unknown.example.com:"
+        "SSH Error: ssh: Could not resolve hostname" + " unknown.example.com:",
     )
 
 
 @pytest.mark.requires_ansible_v2()
 def test_connection_failure_v2():
     from pytest_ansible.errors import AnsibleConnectionFailure
     from pytest_ansible.host_manager import get_host_manager
@@ -133,15 +130,16 @@
 
 @pytest.mark.requires_ansible_v2()
 def test_connection_failure_extra_inventory_v2():
     from pytest_ansible.errors import AnsibleConnectionFailure
     from pytest_ansible.host_manager import get_host_manager
 
     hosts = get_host_manager(
-        inventory="localhost", extra_inventory="unknown.example.extra.com,"
+        inventory="localhost",
+        extra_inventory="unknown.example.extra.com,",
     )
     with pytest.raises(AnsibleConnectionFailure) as exc_info:
         hosts.all.ping()
     # Assert message
     assert exc_info.value.message == "Host unreachable in the extra inventory"
     # Assert contacted
     assert exc_info.value.contacted == {}
```

### Comparing `pytest-ansible-3.0.0/tests/test_fixtures.py` & `pytest-ansible-3.1.0/tests/test_fixtures.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # pylint: disable=unused-import
-import pytest
 
 
 try:
     from _pytest.main import EXIT_OK  # type: ignore
 except ImportError:
     from _pytest.main import ExitCode
 
@@ -17,63 +16,63 @@
         from pytest_ansible.host_manager import BaseHostManager
         def test_func(ansible_adhoc):
             assert isinstance(ansible_adhoc, types.FunctionType)
             assert isinstance(ansible_adhoc(), BaseHostManager)
     """
     testdir.makepyfile(src)
     result = testdir.runpytest(
-        *option.args
-        + [
+        *[
+            *option.args,
             "--ansible-inventory",
             str(option.inventory),
             "--ansible-host-pattern",
             "local",
-        ]
+        ],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 def test_ansible_module(testdir, option):
     src = """
         import pytest
         from pytest_ansible.module_dispatcher import BaseModuleDispatcher
         def test_func(ansible_module):
             assert isinstance(ansible_module, BaseModuleDispatcher)
     """
     testdir.makepyfile(src)
     result = testdir.runpytest(
-        *option.args
-        + [
+        *[
+            *option.args,
             "--ansible-inventory",
             str(option.inventory),
             "--ansible-host-pattern",
             "local",
-        ]
+        ],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 def test_ansible_facts(testdir, option):
     src = """
         import pytest
         from pytest_ansible.results import AdHocResult
         def test_func(ansible_facts):
             assert isinstance(ansible_facts, AdHocResult)
     """
     testdir.makepyfile(src)
     result = testdir.runpytest(
-        *option.args
-        + [
+        *[
+            *option.args,
             "--ansible-inventory",
             str(option.inventory),
             "--ansible-host-pattern",
             "local",
-        ]
+        ],
     )
     assert result.ret == EXIT_OK
     assert result.parseoutcomes()["passed"] == 1
 
 
 def test_localhost(testdir, option):
     src = """
```

### Comparing `pytest-ansible-3.0.0/tests/test_host_manager.py` & `pytest-ansible-3.1.0/tests/test_host_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
-
 from ansible.errors import AnsibleError
-from conftest import ALL_HOSTS
-from conftest import NEGATIVE_HOST_PATTERNS
-from conftest import NEGATIVE_HOST_SLICES
-from conftest import POSITIVE_HOST_PATTERNS
-from conftest import POSITIVE_HOST_SLICES
-
+from conftest import (
+    ALL_HOSTS,
+    NEGATIVE_HOST_PATTERNS,
+    NEGATIVE_HOST_SLICES,
+    POSITIVE_HOST_PATTERNS,
+    POSITIVE_HOST_SLICES,
+)
 
 pytestmark = [
     pytest.mark.unit,
 ]
 
 
 def test_len(hosts):
@@ -74,11 +74,9 @@
 @pytest.mark.ansible_v1_xfail(raises=AnsibleError)
 def test_defaults(request):
     from ansible.constants import DEFAULT_TRANSPORT
 
     plugin = request.config.pluginmanager.getplugin("ansible")
     hosts = plugin.initialize(config=request.config, request=request)
 
-    # from pytest_ansible.host_manager import get_host_manager
-    # hosts = get_host_manager(inventory='unknown.example.com,')
     assert "connection" in hosts.options
     assert hosts.options["connection"] == DEFAULT_TRANSPORT
```

### Comparing `pytest-ansible-3.0.0/tests/test_module_dispatcher.py` & `pytest-ansible-3.1.0/tests/test_module_dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pytest
-
-from conftest import NEGATIVE_HOST_PATTERNS
-from conftest import POSITIVE_HOST_PATTERNS
+from conftest import NEGATIVE_HOST_PATTERNS, POSITIVE_HOST_PATTERNS
 
 
 def test_runtime_error():
     from pytest_ansible.module_dispatcher import BaseModuleDispatcher
 
     bmd = BaseModuleDispatcher(inventory="localhost,")
     with pytest.raises(RuntimeError):
```

### Comparing `pytest-ansible-3.0.0/tests/test_module_result.py` & `pytest-ansible-3.1.0/tests/test_module_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import pytest
-
 from pytest_ansible.results import ModuleResult
 
-
 positive_host_patterns = {
     "all": 2,
     "*": 2,
     "localhost": 1,
     "local*": 1,
     "local*:&*host": 1,
     "!localhost": 1,
@@ -29,28 +27,28 @@
     return ModuleResult(
         **{
             "invocation": {"module_name": "debug", "module_args": {"msg": "testing"}},
             "msg": "testing",
             "changed": False,
             "_ansible_verbose_always": True,
             "_ansible_no_log": False,
-        }
+        },
     )
 
 
 @pytest.fixture()
 def module_result_failed():
     return ModuleResult(
         **{
             "invocation": {"module_name": "fail", "module_args": {}},
             "failed": True,
             "changed": False,
             "_ansible_no_log": False,
             "msg": "Failed as requested from task",
-        }
+        },
     )
 
 
 @pytest.fixture()
 def module_result_changed(request):
     return ModuleResult(
         **{
@@ -73,15 +71,15 @@
                     "removes": None,
                     "warn": True,
                     "chdir": None,
                 },
             },
             "stdout_lines": ["Fri Jun 17 21:32:54 EDT 2016"],
             "warnings": [],
-        }
+        },
     )
 
 
 @pytest.fixture()
 def _module_result_skipped():
     raise NotImplementedError("Coming soon!")
```

### Comparing `pytest-ansible-3.0.0/tests/test_params.py` & `pytest-ansible-3.1.0/tests/test_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 import re
 import sys
-
 from unittest import mock
 
 import ansible
 import pytest
-
 from pkg_resources import parse_version
-
 from pytest_ansible.has_version import has_ansible_v28
 
-
 # pylint: disable=unused-import
 try:
-    from _pytest.main import EXIT_INTERRUPTED  # type: ignore[attr-defined]
-    from _pytest.main import EXIT_NOTESTSCOLLECTED  # type: ignore[attr-defined]
-    from _pytest.main import EXIT_OK  # type: ignore[attr-defined]
-    from _pytest.main import EXIT_TESTSFAILED  # type: ignore[attr-defined]
-    from _pytest.main import EXIT_USAGEERROR  # type: ignore[attr-defined]
+    from _pytest.main import (
+        EXIT_INTERRUPTED,  # type: ignore[attr-defined]
+        EXIT_NOTESTSCOLLECTED,  # type: ignore[attr-defined]
+        EXIT_OK,  # type: ignore[attr-defined]
+        EXIT_TESTSFAILED,  # type: ignore[attr-defined]
+        EXIT_USAGEERROR,  # type: ignore[attr-defined]
+    )
 except ImportError:
     from _pytest.main import ExitCode
 
     EXIT_OK = ExitCode.OK
     EXIT_TESTSFAILED = ExitCode.TESTS_FAILED
     EXIT_USAGEERROR = ExitCode.USAGE_ERROR
     EXIT_INTERRUPTED = ExitCode.INTERRUPTED
     EXIT_NOTESTSCOLLECTED = ExitCode.NO_TESTS_COLLECTED
 
 # pylint: disable=unused-import
 if sys.version_info[0] == 2:
-    import __builtin__ as builtins  # NOQA
+    import __builtin__ as builtins
 else:
     import builtins  # NOQA
 
 
 def test_plugin_help(testdir):
-    """Verifies expected output from of py.test --help"""
-
+    """Verifies expected output from of pytest --help."""
     result = testdir.runpytest("--help")
     result.stdout.fnmatch_lines(
         [
             # Check for the github args section header
             "pytest-ansible:",
             # Check for the specific args
             "  --inventory=ANSIBLE_INVENTORY, --ansible-inventory=ANSIBLE_INVENTORY",
@@ -51,40 +48,37 @@
             "  --module-path=ANSIBLE_MODULE_PATH, --ansible-module-path=ANSIBLE_MODULE_PATH",
             "  --become, --ansible-become",
             "  --become-method=ANSIBLE_BECOME_METHOD, --ansible-become-method=ANSIBLE_BECOME_METHOD",
             "  --become-user=ANSIBLE_BECOME_USER, --ansible-become-user=ANSIBLE_BECOME_USER",
             "  --ask-become-pass=ANSIBLE_ASK_BECOME_PASS, --ansible-ask-become-pass=ANSIBLE_ASK_BECOME_PASS",
             # Check for the marker in --help
             "  ansible (args)*Ansible integration",
-        ]
+        ],
     )
 
 
 def test_plugin_markers(testdir):
-    """Verifies expected output from of py.test --markers"""
-
+    """Verifies expected output from of pytest --markers."""
     result = testdir.runpytest("--markers")
     result.stdout.fnmatch_lines(
         [
             "@pytest.mark.ansible(*args): Ansible integration",
-        ]
+        ],
     )
 
 
 def test_report_header(testdir, option):
     """Verify the expected ansible version in the pytest report header."""
-
     result = testdir.runpytest(*option.args)
     assert result.ret == EXIT_NOTESTSCOLLECTED
     result.stdout.fnmatch_lines([f"ansible: {ansible.__version__}"])
 
 
 def test_params_not_required_when_not_using_fixture(testdir, option):
     """Verify the ansible parameters are not required if the fixture is not used."""
-
     src = """
         import pytest
         def test_func():
             assert True
     """
     testdir.makepyfile(src)
     result = testdir.runpytest(*option.args)
@@ -97,28 +91,27 @@
         "ansible_adhoc",
         "ansible_module",
         "ansible_facts",
     ),
 )
 def test_params_required_when_using_fixture(testdir, option, fixture_name):
     """Verify the ansible parameters are required if the fixture is used."""
-
     src = f"""
         import pytest
         def test_func({fixture_name}):
             {fixture_name}
         """
 
     testdir.makepyfile(src)
     result = testdir.runpytest(*option.args)
     assert result.ret == EXIT_USAGEERROR
     result.stderr.fnmatch_lines(
         [
             "ERROR: Missing required parameter --ansible-host-pattern/--host-pattern",
-        ]
+        ],
     )
 
 
 @pytest.mark.parametrize(
     "required_value_parameter",
     (
         "--ansible-inventory",
@@ -134,61 +127,60 @@
         "--ansible-become-user",
         "--become-user",
         "--ansible-module-path",
         "--module-path",
     ),
 )
 def test_param_requires_value(testdir, required_value_parameter):
-    """Verifies failure when not providing a value to a parameter that requires a value"""
-
+    """Verifies failure when not providing a value to a parameter that requires a value."""
     result = testdir.runpytest(*[required_value_parameter])
     assert result.ret == EXIT_USAGEERROR
     result.stderr.fnmatch_lines(
-        [f"*: error: argument *{required_value_parameter}*: expected one argument"]
+        [f"*: error: argument *{required_value_parameter}*: expected one argument"],
     )
 
 
 def test_params_required_with_inventory_without_host_pattern(testdir, option):
     """Verify that a host pattern is required when an inventory is supplied."""
     src = """
         import pytest
         def test_func(ansible_module):
             assert True
     """
     testdir.makepyfile(src)
-    result = testdir.runpytest(*option.args + ["--ansible-inventory", "local,"])
+    result = testdir.runpytest(*[*option.args, "--ansible-inventory", "local,"])
     assert result.ret == EXIT_USAGEERROR
     result.stderr.fnmatch_lines(
         [
             "ERROR: Missing required parameter --ansible-host-pattern/--host-pattern",
-        ]
+        ],
     )
 
 
 @pytest.mark.requires_ansible_v1()
 def test_params_required_with_bogus_inventory_v1(testdir, option):
     src = """
         import pytest
         def test_func(ansible_module):
             assert True
     """
     testdir.makepyfile(src)
     with mock.patch("os.path.exists", return_value=False) as mock_exists:
         result = testdir.runpytest(
-            *["--ansible-inventory", "bogus", "--ansible-host-pattern", "all"]
+            *["--ansible-inventory", "bogus", "--ansible-host-pattern", "all"],
         )
 
-    # Assert py.test exit code
+    # Assert pytest exit code
     assert result.ret == EXIT_TESTSFAILED
 
     # Assert expected error output
     result.stdout.fnmatch_lines(
         [
             "*Unable to find an inventory file, specify one with -i ?",
-        ]
+        ],
     )
 
     # Assert mock open called on provided file
     mock_exists.assert_any_call("bogus")
 
 
 @pytest.mark.skipif(
@@ -202,27 +194,28 @@
         def test_func(ansible_module):
             with pytest.warns(UserWarning, match="provided hosts list is empty, only localhost is available"):
                 ansible_module.ping()
     """
     testdir.makepyfile(src)
 
     with mock.patch(
-        "ansible.parsing.dataloader.DataLoader.path_exists", return_value=False
+        "ansible.parsing.dataloader.DataLoader.path_exists",
+        return_value=False,
     ) as mock_exists:
         result = testdir.runpytest(
             *[
                 "-vvvvvs",
                 "--ansible-inventory",
                 "bogus",
                 "--ansible-host-pattern",
                 "all",
-            ]
+            ],
         )
 
-    # Assert py.test exit code
+    # Assert pytest exit code
     assert result.ret == EXIT_OK
 
     # Assert mock open called on provided file
     mock_exists.assert_any_call("bogus")
 
 
 @pytest.mark.requires_ansible_v24()
@@ -238,64 +231,65 @@
             # Ensure the latest warning is the ansible localhost warning
             assert record[0].message.args[0] == "provided hosts list is empty, only localhost is available"
 
     """
     testdir.makepyfile(src)
 
     result = testdir.runpytest(
-        *["-vvvvvs", "--ansible-inventory", "bogus", "--ansible-host-pattern", "all"]
+        *["-vvvvvs", "--ansible-inventory", "bogus", "--ansible-host-pattern", "all"],
     )
 
-    # Assert py.test exit code
+    # Assert pytest exit code
     assert result.ret == EXIT_OK
 
     # There appear to be '\n' newline characters within the output.  Using the join on errlines flattens the string for
     # easier comparison.
     assert re.search(
-        r"Unable to parse .*/bogus as an inventory source", " ".join(result.errlines)
+        r"Unable to parse .*/bogus as an inventory source",
+        " ".join(result.errlines),
     )
 
 
 @pytest.mark.requires_ansible_v1()
 def test_params_required_without_inventory_with_host_pattern_v1(testdir, option):
     src = """
         import pytest
         def test_func(ansible_module):
             assert True
     """
     testdir.makepyfile(src)
-    result = testdir.runpytest(*option.args + ["--ansible-host-pattern", "all"])
+    result = testdir.runpytest(*[*option.args, "--ansible-host-pattern", "all"])
     assert result.ret == EXIT_TESTSFAILED
     result.stdout.fnmatch_lines(
         [
             "*Unable to find an inventory file, specify one with -i ?",
-        ]
+        ],
     )
 
 
 @pytest.mark.requires_ansible_v2()
 def test_params_required_without_inventory_with_host_pattern_v2(testdir, option):
     src = """
         import pytest
         def test_func(ansible_module):
             assert True
     """
     testdir.makepyfile(src)
-    result = testdir.runpytest(*option.args + ["--ansible-host-pattern", "all"])
+    result = testdir.runpytest(*[*option.args, "--ansible-host-pattern", "all"])
     assert result.ret == EXIT_OK
 
     # TODO - validate the following warning message
     # [WARNING]: provided hosts list is empty, only localhost is available
     # pylint: disable=using-constant-test
     if False:
         result.stderr.fnmatch_lines(
             [
                 "*[WARNING]: Host file not found: /etc/ansible/hosts*",
                 "*provided hosts list is empty, only localhost is available",
-            ]
+            ],
         )
 
 
 def test_param_override_with_marker(testdir):
     src = """
         import pytest
         @pytest.mark.ansible(inventory='local,', connection='local', host_pattern='all')
@@ -310,12 +304,12 @@
             "native",
             "--ansible-inventory",
             "garbage,",
             "--ansible-host-pattern",
             "garbage",
             "--ansible-connection",
             "garbage",
-        ]
+        ],
     )
     assert result.ret == EXIT_OK
 
     # Mock assert the correct variables are set
```

### Comparing `pytest-ansible-3.0.0/tox.ini` & `pytest-ansible-3.1.0/tox.ini`

 * *Files identical despite different names*

